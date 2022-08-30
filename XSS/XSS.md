# XSS Açıkları

#### XSS açıkları site içinde JS kodu çalıştırabiliyoruz demektir

> ## XSS Reflected

#### Bir link oluşturmamız gerekiyor 
#### Site içinde site ile etkileşime girebileceğimiz yer arıyoruz 
![](https://github.com/ahmetnuysal/Cyber-Security/blob/b8d58a9d2f710cb023f9ac0dbb2d83c22e457eba/Websitesi%20Pentesting/Pict/WhatsApp%20Image%202022-08-30%20at%2013.39.08.jpeg)
#### Bu kısıma ```<script>alert("ı hack you")</script>``` yazıyoruz ve submit ediyoruz
![](https://github.com/ahmetnuysal/Cyber-Security/blob/f7a0ec1433d1e05fd007503381c54e818cfce8e6/Websitesi%20Pentesting/Pict/WhatsApp%20Image%202022-08-30%20at%2013.42.12.jpeg)
#### Eğer birisine sitenin ```url```sini yollarsak yolladığımız kişininde ekranında bu bildirimi görürüz
