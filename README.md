# Cyber Security
- [VPN DNS MAC](#VPN-DNS-MAC)
- [Monitör Mod ve Manage Mod](#Monitör-Mod-ve-Manage-Mod)
- [Çevredeki Modemleri Bulma](#Çevredeki-Modemleri-Bulma)





# VPN DNS MAC 

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

# Monitör Mod ve Manage Mod

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

# Çevredeki Modemleri Bulma

```airopdump -ng wlan0mon``` -> Çevredeki Modemleri Bulur

```CTRL + X ile işlemi sonlandırırız```

```
* pwr -> - Olarak ne kadar büyükse modem bize o kadar yakındır
* Data -> O ağa kaç cihazın bağlı olduğunu gösterir
* CH -> Hangi kanalda olduğunu gösterir
* ENC -> Şifreleme işlemi bilgisi
```
