# BizimSite Backend - JWT ve Token Yapısı

Bu doküman, BizimSite Backend projesinde kullanılacak JWT (JSON Web Token) yapısını açıklamak amacıyla hazırlanmıştır.

---

# Token Nedir?

Token, kullanıcının sisteme giriş yaptıktan sonra kimliğini doğrulamak amacıyla kullanılan dijital bir bilgidir.

Kullanıcı başarılı bir şekilde giriş yaptıktan sonra backend tarafından oluşturulur ve istemciye gönderilir.

İstemci, daha sonraki isteklerinde bu token'ı göndererek tekrar kullanıcı adı ve şifre girmeden kimliğini doğrulayabilir.

---

# JWT Nedir?

JWT (JSON Web Token), kullanıcı kimliğini güvenli bir şekilde taşımak için kullanılan yaygın bir token standardıdır.

Backend uygulamaları, kullanıcı giriş yaptıktan sonra bir JWT oluşturur.

İstemci uygulaması bu JWT'yi saklar ve sonraki isteklerde backend'e gönderir.

---

# JWT Nasıl Çalışır?

```text
Kullanıcı

↓

Giriş bilgilerini gönderir.

↓

Backend bilgileri doğrular.

↓

JWT oluşturulur.

↓

JWT istemciye gönderilir.

↓

İstemci sonraki isteklerde JWT'yi gönderir.

↓

Backend JWT'yi doğrular.

↓

İşlem gerçekleştirilir.
```

---

# JWT Kullanmanın Avantajları

JWT kullanımı sayesinde;

- Kullanıcı her istekte tekrar giriş yapmak zorunda kalmaz.
- Kimlik doğrulama işlemleri kolaylaşır.
- API daha güvenli hale gelir.
- İstemci ve backend arasındaki iletişim standartlaşır.

---

# BizimSite Projesinde Kullanımı

Bu proje kapsamında;

- Başarılı giriş işlemlerinde JWT oluşturulacaktır.
- Sonraki API isteklerinde JWT kullanılacaktır.
- Kimlik doğrulama işlemleri JWT üzerinden gerçekleştirilecektir.

---

# Genel Değerlendirme

JWT, kullanıcıların güvenli bir şekilde kimlik doğrulaması yapabilmesini sağlayan yaygın bir teknolojidir.

Bu yapı sayesinde kullanıcı deneyimi iyileşirken sistem güvenliği de artırılmış olur.
