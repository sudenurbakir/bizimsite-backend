# BizimSite Backend - Validasyon Stratejisi

## Amaç

Bu doküman, BizimSite Backend projesinde uygulanacak veri doğrulama yaklaşımını açıklamak amacıyla hazırlanmıştır.

Sisteme gönderilen verilerin doğruluğunu sağlamak, hatalı veri girişlerini önlemek ve veri bütünlüğünü korumak amacıyla uygulanacak temel validasyon prensipleri bu dokümanda tanımlanmaktadır.

---

# Kapsam

Bu doküman aşağıdaki konuları kapsamaktadır.

- Veri doğrulama yaklaşımı
- Zorunlu alan kontrolleri
- Veri formatı kontrolleri
- İş kurallarına uygunluk
- Hata yönetimi

---

# Veri Doğrulama Yaklaşımı

API'ye gönderilen tüm veriler işleme alınmadan önce doğrulanacaktır.

Doğrulama sürecini geçemeyen istekler işlenmeyecek ve istemciye uygun hata mesajı ile birlikte HTTP 400 (Bad Request) durum kodu döndürülecektir.

---

# Zorunlu Alan Kontrolleri

Sistemde zorunlu olarak tanımlanan alanlar boş bırakılamaz.

Eksik bilgi içeren istekler geçersiz kabul edilecektir.

---

# Veri Formatı Kontrolleri

Gönderilen veriler beklenen veri tipine ve formatına uygun olmalıdır.

Örnek kontroller;

- Tarih alanlarının geçerli formatta olması
- Sayısal alanların yalnızca sayısal değer içermesi
- Metin alanlarının belirlenen uzunluk sınırlarını aşmaması

---

# İş Kurallarına Uygunluk

Temel veri doğrulamalarının ardından sistem iş kuralları da kontrol edilecektir.

Örnek olarak;

- Aynı zaman aralığında birden fazla ortak alan rezervasyonu oluşturulamaması
- Geçmiş bir tarih için rezervasyon oluşturulamaması

Bu kontroller uygulamanın iş kurallarına göre gerçekleştirilecektir.

---

# Hata Yönetimi

Doğrulama başarısız olduğunda işlem durdurulacak ve istemciye standart hata yapısı ile cevap döndürülecektir.

Doğrulama hataları sistem hatası olarak değerlendirilmeyecektir.

---

# Tasarım Kararları

Bu proje kapsamında;

- Tüm istemci verileri doğrulanacaktır.
- Geçersiz veriler işleme alınmayacaktır.
- İş kuralları uygulama seviyesinde kontrol edilecektir.
- Standart hata cevapları kullanılacaktır.

---

# İlgili Dokümanlar

- 03_API_Standartlari.md
- 04_Veritabani_Tasarimi.md
- 06_Hata_Yonetimi.md
