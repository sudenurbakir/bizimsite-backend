# Duyuru Görüntüleme İş Akışı

## Amaç

Bu doküman, BizimSite Backend projesinde kullanıcıların duyuruları görüntüleme sürecinin backend tarafında nasıl yönetileceğini açıklamak amacıyla hazırlanmıştır.

---

## İş Akışı

```text
Kullanıcı

↓

Duyuruları görüntüleme isteği gönderir.

↓

API isteği alır.

↓

Kimlik doğrulama yapılır.

↓

Duyurular sistemden alınır.

↓

Başarılı cevap döndürülür.
```

---

## Açıklama

1. Kullanıcı duyuruları görüntülemek için istekte bulunur.
2. API gelen isteği karşılar.
3. Kullanıcının kimliği doğrulanır.
4. Duyurular sistemden alınır.
5. Sonuç istemciye başarılı bir şekilde iletilir.

---

## Tasarım Kararları

Bu iş akışı kapsamında;

- Duyurular API üzerinden sunulacaktır.
- Kimlik doğrulaması tamamlanmadan işlem gerçekleştirilmeyecektir.
- İşlem sonucunda standart API cevabı döndürülecektir.

---

## İlgili Dokümanlar

- 02_API_Tasarimi.md
- 04_Veritabani_Tasarimi.md
- 05_Kimlik_Dogrulama.md
- 06_Hata_Yonetimi.md
