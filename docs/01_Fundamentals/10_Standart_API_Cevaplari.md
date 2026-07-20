# BizimSite Backend - Standart API Cevapları

Bu doküman, BizimSite Backend projesinde API isteklerine verilecek standart cevap yapısını açıklamak amacıyla hazırlanmıştır.

---

# Standart API Cevabı Nedir?

Backend uygulamalarında istemcilere döndürülen cevapların belirli bir standartta olması önemlidir.

Tüm API uç noktalarının benzer yapıda cevap vermesi;

- Tutarlılığı artırır.
- İstemci uygulamalarının geliştirilmesini kolaylaştırır.
- Hata yönetimini standart hale getirir.
- API'nin daha okunabilir olmasını sağlar.

Bu nedenle BizimSite Backend projesinde tüm API cevapları ortak bir yapı kullanacaktır.

---

# Başarılı İşlem Cevabı

Başarılı işlemlerde API aşağıdaki bilgileri döndürecektir.

- İşlemin başarılı olup olmadığı
- Kullanıcıya gösterilecek açıklayıcı mesaj
- İşlem sonucunda dönen veri (varsa)

## Örnek

```json
{
  "success": true,
  "message": "İşlem başarıyla tamamlandı.",
  "data": {}
}
```

---

# Hatalı İşlem Cevabı

Hatalı işlemlerde API aşağıdaki bilgileri döndürecektir.

- İşlemin başarısız olduğu bilgisi
- Hata mesajı
- Hata detayları (varsa)

## Örnek

```json
{
  "success": false,
  "message": "İşlem gerçekleştirilemedi.",
  "errors": []
}
```

---

# Cevap Alanlarının Açıklaması

| Alan | Açıklama |
|------|----------|
| success | İşlemin başarılı olup olmadığını belirtir. |
| message | İşlem sonucu hakkında açıklayıcı bilgi içerir. |
| data | Başarılı işlemlerde dönen veriyi içerir. |
| errors | Hatalı işlemlerde hata detaylarını içerir. |

---

# Tasarım Kararları

Bu proje kapsamında;

- Tüm API uç noktaları ortak cevap yapısını kullanacaktır.
- Başarılı ve başarısız işlemler tutarlı bir formatta döndürülecektir.
- Başarılı işlemlerde işlem sonucu `data` alanında döndürülecektir.
- Hata detayları yalnızca gerekli durumlarda `errors` alanında yer alacaktır.

---

# Genel Değerlendirme

Standart API cevap yapısı, backend ve istemci uygulamaları arasında tutarlı bir iletişim kurulmasını sağlar.

Bu yaklaşım sayesinde API'nin geliştirilmesi, test edilmesi ve bakımının yapılması daha kolay hale gelir.
