# BizimSite Backend - İş Akışları

## Amaç

Bu doküman, BizimSite Backend projesinde yer alan temel iş akışlarını açıklamak amacıyla hazırlanmıştır.

Sistem içerisinde gerçekleşen işlemlerin hangi adımlardan oluştuğu ve backend tarafında nasıl yönetileceği bu dokümanda tanımlanmaktadır.

---

# Kapsam

Bu doküman aşağıdaki iş akışlarını kapsamaktadır.

- Kullanıcı giriş işlemi
- Ortak alan rezervasyonu oluşturma
- Aidat görüntüleme
- Arıza talebi oluşturma

---

# Kullanıcı Giriş İş Akışı

1. Kullanıcı giriş bilgilerini gönderir.
2. API isteği alır.
3. Kimlik doğrulama işlemi gerçekleştirilir.
4. Doğrulama başarılıysa kullanıcı sisteme erişir.
5. Başarısız olması durumunda uygun hata cevabı döndürülür.

---

# Ortak Alan Rezervasyonu İş Akışı

1. Kullanıcı rezervasyon isteği gönderir.
2. Gönderilen bilgiler doğrulanır.
3. Rezervasyon uygunluğu kontrol edilir.
4. Uygun ise rezervasyon oluşturulur.
5. Sonuç kullanıcıya bildirilir.

---

# Aidat Görüntüleme İş Akışı

1. Kullanıcı aidat bilgilerini talep eder.
2. Kullanıcının yetkisi doğrulanır.
3. Aidat bilgileri veritabanından alınır.
4. Sonuç kullanıcıya iletilir.

---

# Arıza Talebi Oluşturma İş Akışı

1. Kullanıcı arıza talebini gönderir.
2. Gönderilen bilgiler doğrulanır.
3. Talep sisteme kaydedilir.
4. Talep başarıyla oluşturuldu bilgisi kullanıcıya iletilir.

---

# Tasarım Kararları

Bu proje kapsamında;

- Tüm işlemler belirli bir iş akışı izlenerek gerçekleştirilecektir.
- Her iş akışı doğrulama adımından geçecektir.
- İşlem sonuçları standart API cevapları ile istemciye iletilecektir.

---

# İlgili Dokümanlar

- 02_API_Tasarimi.md
- 05_Kimlik_Dogrulama.md
- 06_Hata_Yonetimi.md
- 08_Validasyon_Stratejisi.md
