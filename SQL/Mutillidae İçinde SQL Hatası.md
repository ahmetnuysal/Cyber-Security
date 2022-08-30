# Mutillidae İçine SQL Hatası

### Mutillidae içine girip create account yapıyoruz ve hata alıyoruz, bu hatayı düzeltmek için
* #### 1. Metasploitable makinemize giriyoruz
* #### 2. ```sudo nano /var/www/mutullidae/config.ınc``` çalıştırıyoruz
* #### 3. Çıkan kodlar içinden ```$dbname=`metasploitable`;``` yerine ```$dbname=`mowasp10`;``` yazıyoruz
