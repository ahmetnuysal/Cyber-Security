# Google'a ```send anonymous e-mail``` aratıyoruz
#### Göndermek istediğimiz trojan'i .zip dosyasına çevirerek mail ile yollayabiliriz
---
# Terminal Üzerinden Fake E-Mail Yollama
```sendemail -f admin@gmail -t hedefmailadresi@gmail.com -s smtp.gmail.com:587 -xu gerçekmailadresi@gmail.com -xp MY-PASSWORD -u test email -m your gmail has been hacked```
* -f: Mail'i Gönderen Fake E-mail Adresi
* -t: Hedef E-mail Adresi
* -s: Mail'in Smtp'si (Google Üzerinde Bakılabilir)
* -xu: Kendi E-mail Adresimiz
* -xp: Kendi E-mail Adresimizin Şifresi
* -u: Mail'in Başlığı
* -m: Mail'in İçeriği
