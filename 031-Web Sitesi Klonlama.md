# Web Sitesi Klonlama
> # 1.Bazı Ayarları Değiştiriyoruz
#### 1. ```locate etter.conf``` ettercap'in conf dosyalarının yerini görürüz
#### 2. ```leafpad /etc/ettercap/etter.conf``` ettercap'i açarız (etter.conf konumu değişebilir)
#### 3. ``` ec_vid=0 ve ec_gid=0``` olarak değiştiriyoruz
#### 4. ```locate etter.dns``` ettercap'in dns dosyalarının bulunduğu yeri görürüz
#### 5. ```leafpad /etc/ettercap/etter.dns``` açıyoruz
#### 6. Klonlamak istediğimiz web sitesine girip IP kısmına ```kendi IP``` adresimizi giriyoruz 
> # 2.SETOOLKIT Açıyoruz
#### 1. ```Social-Enginnering Attack``` seçiyoruz
#### 2. ```Website Attack Vectors``` seçiyoruz
#### 3. ```Credetial Harvester Attack Method``` seçiyoruz
#### 4. ```Site Cloner``` seçiyoruz
#### 5. ```Kendi IP```'mizi giriyoruz
#### 6. Sitenin adını yazıyoruz 
> # 3.EtterCap'i Açıyoruz
#### 1. ```target 1 ve target 2```'yi ekliyoruz
#### 2. ```MITM ARP``` seçiyoruz
#### 3. ```sniff remote.com.```seçiyoruz
#### 4. ```Pluging``` içinden ```dns_spoof``` aktif ediyoruz
#### 5. ```Setoolkit``` üzerinden dinliyoruz
