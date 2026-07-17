# BizimSite Backend - Hata Yönetimi

## Amaç

Bu doküman, BizimSite Backend projesinde uygulanacak hata yönetimi yaklaşımını açıklamak amacıyla hazırlanmıştır.

API tarafından döndürülecek hata cevapları, standart hata yapısı ve hata yönetimi prensipleri bu dokümanda tanımlanmaktadır.

---

# Kapsam

Bu doküman aşağıdaki konuları kapsamaktadır.

- Hata yönetimi yaklaşımı
- Standart hata cevapları
- HTTP durum kodlarının kullanımı
- Beklenmeyen hataların yönetimi

---

# Hata Yönetimi Yaklaşımı

API içerisinde oluşabilecek hatalar istemciye standart bir cevap yapısı ile iletilecektir.

Bu yaklaşım sayesinde istemci uygulamaları hata durumlarını daha kolay yorumlayabilecektir.

---

# Standart Hata Cevabı

API tarafından döndürülen hata cevapları ortak bir yapı kullanacaktır.

Örnek hata cevabı;

```json
{
  "statusCode": 404,
  "message": "The requested resource could not be found."
}
```

---

# HTTP Durum Kodları

Hata durumlarında uygun HTTP durum kodları kullanılacaktır.

| Kod | Açıklama |
|-----|----------|
| 400 | Geçersiz istek |
| 401 | Kimlik doğrulaması gerekli |
| 403 | Yetkisiz işlem |
| 404 | Kayıt bulunamadı |
| 500 | Beklenmeyen sunucu hatası |

---

# Beklenmeyen Hatalar

Beklenmeyen sistem hataları istemciye teknik detay içermeyecek şekilde iletilecektir.

Sistem içerisindeki hata kayıtları log mekanizması üzerinden takip edilecektir.

---

# Tasarım Kararları

Bu proje kapsamında;

- Standart hata cevapları kullanılacaktır.
- HTTP durum kodları doğru amaçlarla kullanılacaktır.
- Teknik hata detayları istemci ile paylaşılmayacaktır.

---

# İlgili Dokümanlar

- 02_API_Tasarimi.md
- 03_API_Standartlari.md
