# Rezervasyon İptal İş Akışı

## Amaç

Bu doküman, BizimSite Backend projesinde kullanıcıların rezervasyon iptal sürecinin backend tarafında nasıl yönetileceğini açıklamak amacıyla hazırlanmıştır.

---

## İş Akışı

```text
Kullanıcı

↓

Rezervasyon iptal isteği gönderir.

↓

API isteği alır.

↓

Kimlik doğrulama yapılır.

↓

Rezervasyon kontrol edilir.

↓

İptal işlemi gerçekleştirilir.

↓

Başarılı cevap döndürülür.
```

---

## Açıklama

1. Kullanıcı rezervasyon iptal isteğini gönderir.
2. API gelen isteği karşılar.
3. Kullanıcının kimliği doğrulanır.
4. İptal edilmek istenen rezervasyon kontrol edilir.
5. Rezervasyon iptal edilir.
6. İşlem sonucu istemciye başarılı bir şekilde iletilir.

---

## Tasarım Kararları

Bu iş akışı kapsamında;

- Kullanıcı yalnızca kendi rezervasyonunu iptal edebilecektir.
- Kimlik doğrulaması tamamlanmadan işlem gerçekleştirilmeyecektir.
- İptal işlemi tamamlandıktan sonra standart API cevabı döndürülecektir.

---

## İlgili Dokümanlar

- 02_API_Tasarimi.md
- 04_Veritabani_Tasarimi.md
- 05_Kimlik_Dogrulama.md
- 06_Hata_Yonetimi.md
- 08_Validasyon_Stratejisi.md
