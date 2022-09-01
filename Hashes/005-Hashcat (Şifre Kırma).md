# HASHCAT

#### ```apt-get install hashcat``` 
#### ```hashcat --help``` çalıştırıyoruz ve moduna bakıyoruz ```hashcat --help | grep 512 (SHA512 için)``` diyerek sadece 512'leri listeleyebiliriz
![](https://github.com/ahmetnuysal/Cyber-Security/blob/3e4f0ff428baabc79bff59ab06abbf1a21aebd2c/Websitesi%20Pentesting/Pict/WhatsApp%20Image%202022-09-01%20at%2013.23.05.jpeg)
## ! Sistem hash'i kırarken ```operating system``` seçmemiz gerekiyor

> # 1.Kali Hash Kırma

#### ```hashcat -m 1800 mykalihash.txt /usr/share/wordlist/fasttrack.txt``` 
* ```-m 1800```: $ 6 $ (SHA512) sistemler için mod
* ```-m 500```: $ 1 $ (MD5) sistemler için mod
* ```mykalihash.txt```: Hash'imizi kaydettiğimiz dosya
* ```/usr/share/wordlist/fasttrack.txt```: Wordlistimiz

> # 2.Metasploitable Hash Kırma

#### ```hashcat -m 500 mylinuxhash.txt /usr/share/wordlist/fasttrack.txt> # Metasploitable Hash Kırma```

> # 3.Windows Hash Kırma

#### ```hashcat -m 1000 mywindowshash.txt /usr/share/wordlist/fasttrack.txt```
* ```-m 1000```: NTLM sistemler için mod
---
## Hatalar
#### 1. ```All hashes found in potfile``` hatası alırsak, daha önce bu hash kırılmış demektir
```hashcat -m 1800 mykalihash.txt /usr/share/wordlist/fasttrack.txt --show``` diyerek daha önceden kırılmış hash sonuçlarını görebiliriz
#### 2. ```Not enough allocatable device memory for this attack``` hatası alırsak, RAM'imiz yetersiz demektir 4GB RAM yeterli olacaktır
#### 3. ```Appraching final keyspace workload adjusted``` hatası alırsak, hash kırılamadı demektir
