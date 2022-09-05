# Fristileaks 1
> ## 1. netdiscover ile IP öğrenme
- ```netdiscover -i eth0 192.168.123.0/24 -c 10``` ağdaki cihazların MAC adresilerini ve IP adreslerini eşleştirerek hedef cihazın IP adresini öğreniyoruz
> ## 2. nmap ile açık arıyoruz
- ```nmap -v -sS -A -T4 192.168.123.123``` 
> ## 3. IP adresinin internet sitesinde robots.txt çalıştırıyoruz
- Google'a ```192.168.123.123/robots.txt``` yazıyoruz ve sonuçlara bakıyoruz
[]()
