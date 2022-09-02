|   Class Name  | Network Numbers |  Network Mask |    # of Hosts   |
| ------------- | --------------- | ------------- | --------------- |
| Class A  | 10.0.0.0   | 255.0.0.0  | 16777214   |
| Class B | 172.16.0.0    | 255.255.0.0  | 65534   |
| Class C | 192.168.0.0    | 255.255.255.0  | 254   |
| Loopback (local) | 127.0.0.0    | 255.255.255.0  |     |

* ### ! 255 olan kısımlar değiştirilemez sadece 0 olan kısımlar değişebilir

* ### ```# of Host``` total olabilecek host sayısı - 2'dir. Çünkü 1 IP modeme ve son IP broadcast'e gider. Öğneğin Class C'de 256 tane host olabilir fakat # of hosts 254 dür. (256-2)

