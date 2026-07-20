# BizimSite Backend - Loglama Stratejisi

## Amaç

Bu doküman, BizimSite Backend projesinde uygulanacak loglama yaklaşımını açıklamak amacıyla hazırlanmıştır.

Sistem içerisinde gerçekleşen önemli olayların kayıt altına alınması, hata analizlerinin kolaylaştırılması ve sistem davranışlarının izlenebilmesi için uygulanacak temel loglama prensipleri bu dokümanda tanımlanmaktadır.

---

# Kapsam

Bu doküman aşağıdaki konuları kapsamaktadır.

- Loglama yaklaşımı
- Loglanacak olaylar
- Log seviyeleri
- Güvenlik prensipleri

---

# Loglama Yaklaşımı

Sistem içerisinde gerçekleşen önemli işlemler ve beklenmeyen hatalar kayıt altına alınacaktır.

Log kayıtları; sistemin izlenebilirliğini artırmak, hata analizlerini kolaylaştırmak ve bakım süreçlerini desteklemek amacıyla kullanılacaktır.

---

# Loglanacak Olaylar

Aşağıdaki işlemler loglanacaktır.

- Kullanıcı giriş işlemleri
- Başarısız giriş denemeleri
- Ortak alan rezervasyonu oluşturma ve iptal işlemleri
- Aidat işlemleri
- Ortak gider işlemleri
- Beklenmeyen sistem hataları

Her işlem için yalnızca gerekli teknik bilgiler kayıt altına alınacaktır.

---

# Log Seviyeleri

Sistemde farklı önem derecelerine sahip log seviyeleri kullanılacaktır.

| Seviye | Açıklama |
|--------|----------|
| Information | Normal sistem olayları |
| Warning | Beklenmeyen ancak sistemin çalışmasını durdurmayan durumlar |
| Error | İşlemin başarısız olmasına neden olan hatalar |
| Critical | Sistemin çalışmasını etkileyen kritik hatalar |

---

# Güvenlik Prensipleri

Log kayıtlarında güvenlik açısından aşağıdaki kurallar uygulanacaktır.

- Hassas kullanıcı bilgileri loglanmayacaktır.
- Şifreler hiçbir durumda log kayıtlarına yazılmayacaktır.
- Log kayıtları yalnızca yetkili kişiler tarafından görüntülenebilecektir.

---

# Tasarım Kararları

Bu proje kapsamında;

- Önemli sistem olayları kayıt altına alınacaktır.
- Hata kayıtları standart bir yapıda tutulacaktır.
- Hassas bilgiler loglanmayacaktır.
- Loglama sistemi bakım ve hata analizlerini destekleyecek şekilde tasarlanacaktır.

---

# İlgili Dokümanlar

- 02_API_Tasarimi.md
- 05_Kimlik_Dogrulama.md
- 06_Hata_Yonetimi.md
