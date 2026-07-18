# BizimSite Backend - Veritabanı İlişkileri

Bu doküman, BizimSite Backend projesinde kullanılacak temel veritabanı ilişkilerini açıklamak amacıyla hazırlanmıştır.

---

# Veritabanı İlişkisi Nedir?

Veritabanı ilişkisi, sistemde bulunan varlıkların birbirleriyle nasıl bağlantılı olduğunu ifade eder.

Bu ilişkiler sayesinde veriler düzenli bir şekilde saklanabilir ve birbirleriyle ilişkilendirilebilir.

---

# Projede Kullanılacak İlişkiler

| Varlık | İlişkili Varlık | İlişki |
|--------|-----------------|---------|
| Kullanici | Aidat | Bir kullanıcı birden fazla aidat kaydına sahip olabilir. |
| Kullanici | Rezervasyon | Bir kullanıcı birden fazla rezervasyon oluşturabilir. |
| Kullanici | ArizaTalebi | Bir kullanıcı birden fazla arıza talebi oluşturabilir. |
| Kullanici | HizmetTalebi | Bir kullanıcı birden fazla hizmet talebi oluşturabilir. |
| Duyuru | Kullanici | Duyurular tüm kullanıcılara gösterilebilir. |

---

# Tasarım Kararları

Bu proje kapsamında;

- Varlıklar arasındaki ilişkiler veri bütünlüğünü koruyacak şekilde tasarlanacaktır.
- İlişkiler, veritabanında yabancı anahtarlar (Foreign Key) kullanılarak kurulacaktır.
- Her ilişkinin iş kurallarına uygun olması sağlanacaktır.

---

# Genel Değerlendirme

Veritabanı ilişkileri, BizimSite Backend projesinin veri modelinin temel yapı taşlarından biridir.

Bu ilişkiler sayesinde sistem içerisindeki veriler tutarlı ve düzenli bir şekilde yönetilecektir.
