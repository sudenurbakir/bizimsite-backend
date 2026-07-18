# Ortak Alan Rezervasyonu İş Akışı

## Amaç

Bu doküman, BizimSite Backend projesinde ortak alan rezervasyonu oluşturma sürecinin backend tarafında nasıl yönetileceğini açıklamak amacıyla hazırlanmıştır.

---

## İş Akışı

```text
Kullanıcı

↓

Rezervasyon isteği gönderir.

↓

API isteği alır.

↓

Kimlik doğrulama yapılır.

↓

Gönderilen veriler doğrulanır.

↓

Rezervasyon uygun mu?

├── Evet
│
├── Rezervasyon oluşturulur.
│
└── Başarılı cevap döndürülür.

└── Hayır

↓

Hata cevabı döndürülür.
```

---

## Açıklama

1. Kullanıcı ortak alan rezervasyonu oluşturmak için istekte bulunur.
2. API gelen isteği karşılar.
3. Kullanıcının kimliği doğrulanır.
4. Gönderilen rezervasyon bilgileri kontrol edilir.
5. Rezervasyonun oluşturulmasına engel bir durum olup olmadığı değerlendirilir.
6. Uygun olması durumunda rezervasyon oluşturulur.
7. İşlem sonucu istemciye uygun cevap döndürülür.

---

## Tasarım Kararları

Bu iş akışı kapsamında;

- Rezervasyon işlemleri API üzerinden gerçekleştirilecektir.
- Tüm rezervasyon isteklerinde kimlik doğrulama yapılacaktır.
- Gönderilen veriler işleme alınmadan önce doğrulanacaktır.
- Uygun olmayan rezervasyon talepleri reddedilecektir.

---

## İlgili Dokümanlar

- 02_API_Tasarimi.md
- 05_Kimlik_Dogrulama.md
- 06_Hata_Yonetimi.md
- 08_Validasyon_Stratejisi.md
- 04_Veritabani_Tasarimi.md
