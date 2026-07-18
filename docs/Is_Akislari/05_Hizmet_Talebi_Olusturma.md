# Hizmet Talebi Oluşturma İş Akışı

## Amaç

Bu doküman, BizimSite Backend projesinde kullanıcıların hizmet talebi oluşturma sürecinin backend tarafında nasıl yönetileceğini açıklamak amacıyla hazırlanmıştır.

---

## İş Akışı

```text
Kullanıcı

↓

Hizmet talebini gönderir.

↓

API isteği alır.

↓

Kimlik doğrulama yapılır.

↓

Gönderilen veriler doğrulanır.

↓

Talep sisteme kaydedilir.

↓

Başarılı cevap döndürülür.
```

---

## Açıklama

1. Kullanıcı hizmet talebini sisteme gönderir.
2. API gelen isteği karşılar.
3. Kullanıcının kimliği doğrulanır.
4. Gönderilen bilgiler kontrol edilir.
5. Hizmet talebi sisteme kaydedilir.
6. İşlem sonucu istemciye başarılı bir şekilde iletilir.

---

## Tasarım Kararları

Bu iş akışı kapsamında;

- Hizmet talepleri yalnızca kimliği doğrulanmış kullanıcılar tarafından oluşturulabilecektir.
- Gönderilen bilgiler işleme alınmadan önce doğrulanacaktır.
- Başarılı talepler sistemde kayıt altına alınacaktır.
- İşlem sonucunda standart API cevabı döndürülecektir.

---

## İlgili Dokümanlar

- 02_API_Tasarimi.md
- 04_Veritabani_Tasarimi.md
- 05_Kimlik_Dogrulama.md
- 06_Hata_Yonetimi.md
- 08_Validasyon_Stratejisi.md
