# Bilgi Toplama
---
> # 1. Maltego
* Arama yapmak istediğimiz şeyi seçip isimini yazarak arama yapabiliriz
* Arama sonucuna göre örneğin ```wordpress``` kullanıyorsa ```wordpress exploit``` google'layarak bilinen açıkları ve nasıl kullanıcağını görebiliriz

> # 2. Netcraft (Online)
* Netcraft'ın sitesine giderek bilgi toplayabiliriz
* Webtrackerları, kullanılan teknolojileri(php,xml vs.), risk değelerini vs görebiliriz
* HTTP mi yoksa HTTPS mi öğrenebiliriz

> # 3.Yougetsignal (Online)
* Youtgetsignal aynı IP adresini kullanan websitelerini gösterir (Reverse IP)
### ```Reverse IP: Web sitesinden IP adresinde değil, IP adresinden Websitesine gidiş```
* Aynı IP adresinde çalışan başka bir websitesini hackleyerek diğer websitesinin bilgilerine erişebiliriz
* Bundan korunmak için kendimize ait bir serverimizin bulunması lazım
* ```ip:123.456.789.123 (IP adresi)``` şeklinde aratarak o websitesiyle aynı IP adresini kullanan siteleri buluruz

> # 4.Archive (Online)
* Websitelerinin eski hallerini arşivleyen sitedir

> # 5.Whoislookup (I CANN WHO IS)(Online)
* Temel bilgileri (Register bilgileri, contact numaraları vb.) görebiliriz 
* Ne zaman ve nereden alındığını görebiliriz

> # 6.Robots.txt (Dirb)
* ```dirb http(s)://<IP>/``` yazarak websitesi içine gizlenmiş dosyaları listeleriz(e.g. http://<IP>/multilliade/)
* Liste içierisinde  (e.g. http://<IP>/multilliade/robots.txt) linkini google'da aratarak robots içindekileri görürüz
* ```robots.txt``` içindeki komutları link sonuna ekleyerek istediğimiz gizli uzantılara girebiliriz(e.g. http://<IP>/mutillidae/passwords/)

> # 7.Subbrute 
* ```git clone https://github.com/TheRook/subbrute``` çalıştırıp kaydettiğimiz klasöre gidiyoruz
* ```python3 subbrute.py siteadı.com``` diyerek belirtilen sitenin subdomainlerini(alt domain) görebiliriz
* Çıkan subdomainlere giderek ```SQL enjeksiyon``` deneyebiliriz
* Çıkan subdomainlere ```nmap``` çalıştırabiliriz
