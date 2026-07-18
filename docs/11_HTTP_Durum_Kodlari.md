# BizimSite Backend - HTTP Durum Kodları

Bu doküman, BizimSite Backend projesinde kullanılacak temel HTTP durum kodlarını açıklamak amacıyla hazırlanmıştır.

---

# HTTP Durum Kodu Nedir?

HTTP durum kodları, istemcinin gönderdiği isteğin sonucunu ifade eden standart kodlardır.

Her API isteği sonucunda yalnızca veri değil, aynı zamanda işlemin başarılı veya başarısız olduğunu belirten bir HTTP durum kodu da döndürülür.

Bu sayede istemci, isteğin sonucunu daha kolay yorumlayabilir.

---

# Kullanılacak HTTP Durum Kodları

| Kod | Adı | Açıklama |
|------|------|----------|
| 200 | OK | İstek başarıyla tamamlandı. |
| 201 | Created | Yeni bir kayıt başarıyla oluşturuldu. |
| 400 | Bad Request | Gönderilen istek geçersizdir. |
| 401 | Unauthorized | Kimlik doğrulama başarısızdır veya kullanıcı giriş yapmamıştır. |
| 403 | Forbidden | Kullanıcının işlem yapma yetkisi bulunmamaktadır. |
| 404 | Not Found | İstenen kaynak bulunamadı. |
| 500 | Internal Server Error | Sunucu tarafında beklenmeyen bir hata oluştu. |

---

# BizimSite Projesinde Kullanımı

Bu proje kapsamında;

- Başarılı veri okuma işlemlerinde **200 OK**
- Yeni kayıt oluşturma işlemlerinde **201 Created**
- Geçersiz isteklerde **400 Bad Request**
- Kimlik doğrulaması başarısız olduğunda **401 Unauthorized**
- Yetki gerektiren işlemlerde **403 Forbidden**
- Bulunamayan kaynaklarda **404 Not Found**
- Beklenmeyen sistem hatalarında **500 Internal Server Error** kullanılacaktır.

---

# Tasarım Kararları

Bu proje kapsamında HTTP durum kodları standartlara uygun şekilde kullanılacaktır.

Her API isteğinde döndürülen cevap ile HTTP durum kodu birbiriyle uyumlu olacaktır.

---

# Genel Değerlendirme

HTTP durum kodlarının doğru kullanılması, API'nin daha anlaşılır, tutarlı ve yönetilebilir olmasını sağlar.

Bu yaklaşım sayesinde istemci uygulamaları, gelen cevapları daha doğru şekilde yorumlayabilir.
