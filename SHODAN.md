# Shodan (Bilgi Toplama ve Arama Motoru)

#### 1. Google'dan ```shodan.io``` adresine giriyoruz
#### 2. ```webcams``` yazarak daha önceden taglanmiş kameraları görebiliriz 
#### 3. ```vsat``` yazarak daha önceden taglanmiş uyduları görebiliriz
#### 4. Çıkan IP'lere tıklayarak kullanılan portları görebiliriz ```(e.g. 123.456.789.123:9000) 9000 portunu kullanıyor```

# Shodan İçerisinde Filtreleme 

* ```vsat port:80```: Port 80 çalıştıran web'e çıkış veren uyduları gösterir
* ```port:22```: SSH Kullanan Servisleri Listeleriz
* ```port:22 country:"FR" city:"Paris"```: Fransa Parisdeki SSH Sunucularını Listeler
* ```os:"Windows XP"```: Windows XP kullanan PC'leri Listeler
* ```os:"Windows XP" country:"US"```: ABD'de Windows XP kullanan PC'leri Listeler
* ```vsftpd 2.3.4```: ftp 2.3.4 Kullanan Servisleri Gösterir

# Shodan'ı Terminal Üzerinden Çalıştırmak

#### 1. ```shodan```
#### 2. ```shodan init <API key>``` (IP key shodan sitesinde hesabımıza tanımlanmış key)
#### 3. ```shodan host 123.456.789.123``` (Arama yapmak istediğimiz sunucu vs. IP'si)
