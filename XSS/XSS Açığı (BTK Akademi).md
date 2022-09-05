#### 1. Site ile etkileşime girebileceğimiz bir yere giriyoruz (form vb.)
#### 2. ```<script>alert("XSS Açığı")</script>``` kodunu yazarak deneme yapıyoruz
#### 3. Eğer açık var ise, bu JS kodunu siteye giren herkesin görebileceği bir kısıma yazarsak siteye giren herkesin ekranına bu bildirim düşer
#### 4. ```<script>window.location='https://google.com'</script>``` kodunu yazarsak siteye giren herkesi otomatik olarak belirtilen siteye yönlendirir (bu kod için google'a)
#### 5. Bazı sitelerde ```JavaScript``` filtreleri bulunur, bu filtrelerden kaçmak için ```<scr<script>ipt>alert("XSS Açığı")</scr</script>ipt>``` şeklinde yazarız
