# Fristileaks 1
> ## 1. netdiscover ile IP öğrenme
- ```netdiscover -i eth0 192.168.123.0/24 -c 10``` ağdaki cihazların MAC adresilerini ve IP adreslerini eşleştirerek hedef cihazın IP adresini öğreniyoruz
> ## 2. nmap ile açık arıyoruz
- ```nmap -v -sS -A -T4 192.168.123.123``` 
> ## 3. IP adresinin internet sitesinde robots.txt çalıştırıyoruz
- Google'a ```192.168.123.123/robots.txt``` yazıyoruz ve sonuçlara bakıyoruz

![](https://github.com/ahmetnuysal/Cyber-Security/blob/856e6765d793278f2f29831d141e606664ce7a21/Websitesi%20Pentesting/Pict/WhatsApp%20Image%202022-09-06%20at%2014.48.06%20(1).jpeg)
![](https://github.com/ahmetnuysal/Cyber-Security/blob/ea1b4a490d0ac6a6eecd4a51ca2c1294070689a1/Websitesi%20Pentesting/Pict/WhatsApp%20Image%202022-09-06%20at%2017.15.46.jpeg)
> ## 4. Farklı subdomainleri deniyoruz
```
192.168.123.123/cola
192.168.123.123/sisi
192.168.123.123/beer
192.168.123.123/admin
192.168.123.123/administrator
```
- Sitedeki tüm subdomainler içecek ismi olduğu ayrıca ```fristi```'de bir içecek olduğu için ```192.168.123.123/fristi``` uzantısını deniyoruz
