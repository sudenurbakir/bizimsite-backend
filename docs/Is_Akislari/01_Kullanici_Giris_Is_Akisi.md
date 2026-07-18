# Kullanıcı Giriş İş Akışı

## Amaç

Bu doküman, BizimSite Backend projesinde kullanıcı giriş işleminin backend tarafında nasıl yönetileceğini açıklamak amacıyla hazırlanmıştır.

---

## İş Akışı

```text
Kullanıcı

↓

Giriş bilgilerini gönderir

↓

API isteği alır

↓

Kimlik doğrulama yapılır

↓

Kimlik bilgileri geçerli mi?

├── Evet
│
├── JWT oluşturulur.
│
└── Başarılı cevap döndürülür.

└── Hayır

↓

Hata cevabı döndürülür.
```

---

## Açıklama

1. Kullanıcı giriş bilgilerini API'ye gönderir.
2. API isteği karşılar.
3. Kullanıcının kimlik bilgileri doğrulanır.
4. Kimlik doğrulama başarılıysa kullanıcı için bir JWT oluşturulur.
5. Oluşturulan JWT istemciye gönderilir.
6. Kimlik doğrulama başarısızsa uygun hata cevabı döndürülür.

---

## Tasarım Kararları

Bu iş akışı kapsamında;

- Kimlik doğrulama işlemi API üzerinden başlatılacaktır.
- Başarılı giriş işlemlerinde JWT kullanılacaktır.
- Başarısız giriş denemelerinde standart hata cevabı döndürülecektir.
- Kullanıcının şifresi hiçbir durumda istemciye geri gönderilmeyecektir.

---

## İlgili Dokümanlar

- 02_API_Tasarimi.md
- 05_Kimlik_Dogrulama.md
- 06_Hata_Yonetimi.md
- 08_Validasyon_Stratejisi.md
