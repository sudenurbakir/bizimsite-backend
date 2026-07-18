# Kullanıcı Giriş İş Akışı

## Amaç

Bu doküman, BizimSite Backend projesinde kullanıcı giriş işleminin backend tarafında nasıl yönetileceğini açıklamak amacıyla hazırlanmıştır.

---

## İş Akışı

```text
Kullanıcı

↓

Giriş bilgilerini gönderir.

↓

API isteği alır.

↓

Kimlik doğrulama yapılır.

↓

Kimlik bilgileri geçerli mi?

├── Evet
│
├── Kullanıcının sisteme erişimine izin verilir.
│
└── Başarılı cevap döndürülür.

└── Hayır

↓

Hata cevabı döndürülür.
```

---

## Açıklama

1. Kullanıcı giriş bilgilerini API'ye gönderir.
2. API gelen isteği karşılar.
3. Kullanıcının kimlik bilgileri doğrulanır.
4. Kimlik doğrulama başarılıysa kullanıcının sisteme erişimine izin verilir.
5. İşlem sonucu istemciye uygun cevap döndürülür.

---

## Tasarım Kararları

Bu iş akışı kapsamında;

- Giriş işlemleri API üzerinden gerçekleştirilecektir.
- Tüm giriş denemelerinde kimlik doğrulama yapılacaktır.
- Başarısız giriş denemelerinde standart hata cevabı döndürülecektir.
- Hassas kullanıcı bilgileri istemciye geri gönderilmeyecektir.

---

## İlgili Dokümanlar

- 02_API_Tasarimi.md
- 05_Kimlik_Dogrulama.md
- 06_Hata_Yonetimi.md
- 08_Validasyon_Stratejisi.md
