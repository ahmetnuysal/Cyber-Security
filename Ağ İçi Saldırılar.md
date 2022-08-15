# Monitör Mod / Manage Mod
---
-wifi adaptörümüzü bilgisayarımıza bağlıyoruz, daha sonra kalimizi monitör moda almamız gerekiyor

> 1.Yöntem

**airmon -ng start wlan0** -> interneti monitör moda alır !! Monitör modda iken internete bağlanamayız sadece bağlı olmadığımız ağların bilgilerini elde edebiliriz
**airmon -ng stop wlan0** -> interneti manage moda alır 

> 2.Yöntem

**ifconfig wlan0 down**

**ifconfig wlan0 mode monitor**   

**ifconfig wlan0 up**

# Çevredeki Modemleri Bulma
---
