# John 
#### 1.``` apt get install john``` john'u yüklüyoruz
#### 2. Zip'in bulunduğu klasöre gidiyoruz ve ```zip2john mysecretfiles.zip``` zip dosyasının hash'ini verir
#### 3. ```zip2john mysecretfiles.zip | cut -d ':' -f 2``` diyerek ```:```'ye göre ayırıp 2. kısımını (işimize yarayan kısım) alıyoruz
#### 4. ```zip2john mysecretfiles.zip | cut -d ':' -f 2 > ziphashes.txt``` hash'i ziphashes.txt dosyasına kaydeder
#### 5. ```hashcat -m 13600 myzip.txt /usr/share/wordlist/fasttrack.txt``` 
![](https://github.com/ahmetnuysal/Cyber-Security/blob/000f66c5a107ca48ba223ed0c38bdd49c361bb0b/Websitesi%20Pentesting/Pict/WhatsApp%20Image%202022-09-01%20at%2013.43.17.jpeg)
