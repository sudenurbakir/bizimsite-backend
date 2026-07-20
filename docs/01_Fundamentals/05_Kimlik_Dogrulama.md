# BizimSite Backend - Kimlik Doğrulama

## Amaç

Bu doküman, BizimSite Backend projesinde uygulanacak kimlik doğrulama ve yetkilendirme yaklaşımını açıklamak amacıyla hazırlanmıştır.

---

# Kapsam

Bu doküman aşağıdaki konuları kapsamaktadır.

- Kimlik doğrulama yaklaşımı
- Yetkilendirme yapısı
- Kullanıcı rolleri
- Güvenlik prensipleri

---

# Kimlik Doğrulama Yaklaşımı

Sisteme erişim sağlayacak kullanıcılar, kimlik doğrulama işlemi tamamlandıktan sonra yetkileri doğrultusunda sistem kaynaklarına erişebilecektir.

Kimlik doğrulama mekanizması, güvenli ve ölçeklenebilir bir yapı oluşturacak şekilde tasarlanacaktır.

---

# Kullanıcı Rolleri

Sistem içerisinde farklı yetki seviyelerine sahip kullanıcı rolleri bulunacaktır.

Örnek roller;

- Yönetici
- Site Sakini

Her rol yalnızca yetkili olduğu işlemleri gerçekleştirebilecektir.

---

# Yetkilendirme

Kimliği doğrulanan kullanıcıların erişebileceği işlemler sahip oldukları role göre belirlenecektir.

Yetkisiz erişim talepleri sistem tarafından reddedilecektir.

---

# Güvenlik Prensipleri

Bu proje kapsamında;

- Kimlik doğrulama zorunlu olacaktır.
- Yetkilendirme rol bazlı uygulanacaktır.
- Hassas işlemler yalnızca yetkili kullanıcılar tarafından gerçekleştirilecektir.

---

# Tasarım Kararları

Bu proje kapsamında;

- Kimlik doğrulama merkezi bir yapı üzerinden yönetilecektir.
- Yetkilendirme rol bazlı olacaktır.
- Güvenlik kontrolleri API seviyesinde uygulanacaktır.

---

# İlgili Dokümanlar

- 01_Proje_Mimarisi.md
- 02_API_Tasarimi.md
- 03_API_Standartlari.md
