# Aidat Görüntüleme İş Akışı

## Amaç

Bu doküman, BizimSite Backend projesinde kullanıcıların aidat bilgilerini görüntüleme sürecinin backend tarafında nasıl yönetileceğini açıklamak amacıyla hazırlanmıştır.

---

## İş Akışı

```text
Kullanıcı

↓

Aidat bilgilerini görüntüleme isteği gönderir.

↓

API isteği alır.

↓

Kimlik doğrulama yapılır.

↓

Kullanıcının yetkisi kontrol edilir.

↓

Aidat bilgileri alınır.

↓

Başarılı cevap döndürülür.
```

---

## Açıklama

1. Kullanıcı aidat bilgilerini görüntülemek için istekte bulunur.
2. API gelen isteği karşılar.
3. Kullanıcının kimliği doğrulanır.
4. Kullanıcının ilgili bilgilere erişim yetkisi kontrol edilir.
5. Aidat bilgileri sistemden alınır.
6. Sonuç istemciye başarılı bir şekilde iletilir.

---

## Tasarım Kararları

Bu iş akışı kapsamında;

- Aidat bilgilerine yalnızca yetkili kullanıcılar erişebilecektir.
- Kimlik doğrulama yapılmadan işlem gerçekleştirilmeyecektir.
- İşlem sonucunda yalnızca ilgili kullanıcıya ait bilgiler döndürülecektir.

---

## İlgili Dokümanlar

- 02_API_Tasarimi.md
- 04_Veritabani_Tasarimi.md
- 05_Kimlik_Dogrulama.md
- 06_Hata_Yonetimi.md
