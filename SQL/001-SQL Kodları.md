# SQL Kodları

* ```INSERT INTO demo (id,name,hint) VALUES (18,"james","Guitar");``` Veri tabanına veri eklememizi sağlar
* ```DELETE FROM demo WHERE name="james":```: Veri tabanında ```james``` isimine kayıt edilmiş verileri siler
* ```UPDATE demo SET id=22 WHERE name="james";```: Veri tabanına ```james``` isimiyle kayıt olan kişini id'sini 22 olarak günceller
* ```SELECT*FROM demo WHERE name LIKE "A%";```: Veri tabanında ```A``` ile başlayan verileri listeler
* ```SELECT*FROM demo WHERE name LIKE "%A";```: Veri tabanında ```A``` ile biten verileri listeler
