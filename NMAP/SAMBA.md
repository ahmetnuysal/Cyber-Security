#### Samba linux sunucuları ile windows sunucularını birbirine bağlar
#### Şirketlerdeki PC, yazıcı vb şeyleri birbirine bağlar
---
#### 1. Samba Numarasını ```(samba smbd 3.x-4.x) exploit``` ile google'da ararız
#### 2. ```msfconsole ``` açarız
#### 3. Google üzerinde çıkan komutları yazıyoruz
#### 4. ```LHOST``` bizim IP adresimiz
#### 5. ```exploit -j -z``` dinleyeme başlıyoruz ```-j -z``` dersek dinlemeyi arka planda yapar
#### 6. ```sessions -l``` açık olan portları görürüz
#### 7. ```session 1``` 1. session açık olduğu için o porttan giriş yapar
