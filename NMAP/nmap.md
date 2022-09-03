# NMAP ile Açık İnceleme

  ```nmap -v -sS -A -T4 XX:XX:XX:XX:XX```  Taranan adresteki açıkları gösterir

> ### NMAP Komutları

* -A: Farklı işletim sistemi versiyon vs verir.
* -sn: Port taraması yapma anlamına gelir.
* -n: DNS Çözümlemesi yapma anlamına gelir.
* -v, -vv, -vvv: Ekrana gösterilecek detayları arttırır.
* -F: Daha hızlı tarama yapar. Daha az sonuç bulur.
* -sS:Syn Taraması Yapar
* --reason: Bulduğu bir sonucun sebebini gösterir.
* --open: Sadece açık Portları gösterir.
* -p-: Bir IP üzerinde bulunması muhteme 65535 portun hepsini tarar.
* -sV: Açık portta çalışan servisin ne olduğunu bulmaya çalışır.
* -sC ile birlikte kullanılırsa işe yarar.
* -sC: -sV ile versiyon tespiti yapılırken nmap scriptlerini kullanır.
* -p: Sadece bu parametreden sonra belirtilen portları tarar.
* -o: İşletim sistemi bilgilerini gösterir.
