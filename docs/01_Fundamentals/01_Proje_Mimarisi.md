# BizimSite Backend - Proje Mimarisi

Bu doküman, BizimSite Backend projesinde kullanılacak yazılım mimarisini açıklamak amacıyla hazırlanmıştır.

Proje, katmanlı mimari yaklaşımı kullanılarak geliştirilecektir. Bu yaklaşım sayesinde sistem bileşenleri sorumluluklarına göre ayrılarak daha okunabilir, sürdürülebilir ve geliştirilebilir bir yapı oluşturulması hedeflenmektedir.

---

# Katmanlı Mimari Nedir?

Katmanlı mimari, uygulamanın farklı sorumluluklarının ayrı katmanlarda yönetilmesini sağlayan yazılım tasarım yaklaşımıdır.

Her katman yalnızca kendi sorumluluğundan sorumludur ve diğer katmanlarla belirli kurallar çerçevesinde iletişim kurar.

Bu yaklaşım sayesinde;

- Kod okunabilirliği artar.
- Bakım ve geliştirme kolaylaşır.
- Test edilebilirlik artar.
- Katmanlar birbirinden bağımsız geliştirilebilir.

---

# Proje Katmanları

BizimSite Backend projesi aşağıdaki katmanlardan oluşacaktır.

- BizimSite.API
- BizimSite.Application
- BizimSite.Domain
- BizimSite.Infrastructure

Her katman farklı bir sorumluluğa sahiptir.

---

# BizimSite.API

API katmanı, istemcilerden gelen HTTP isteklerini karşılayan giriş noktasıdır.

Bu katmanda;

- HTTP istekleri alınır.
- İlgili işlemler başlatılır.
- İşlem sonuçları istemciye döndürülür.

API katmanı doğrudan iş kurallarını içermez.

---

# BizimSite.Application

Application katmanı, sistemde gerçekleştirilen iş akışlarını yönetir.

Bu katmanda;

- Kullanıcı istekleri işlenir.
- İşlemler sıralı şekilde yürütülür.
- Gerekli iş kuralları uygulanmak üzere Domain katmanı ile iletişim kurulur.

---

# BizimSite.Domain

Domain katmanı, sistemin temel iş kurallarını içerir.

Bu katmanda;

- Varlıklar (Entities)
- İş kuralları
- Domain mantığı

bulunacaktır.

Bu katman sistemin en önemli bölümünü oluşturur.

---

# BizimSite.Infrastructure

Infrastructure katmanı, uygulamanın dış dünya ile iletişimini sağlar.

Bu katmanda;

- SQL Server işlemleri
- Entity Framework Core
- Dosya işlemleri
- E-posta servisleri
- Harici servis bağlantıları

yer alacaktır.

---

# Katmanlar Arasındaki İlişki

Sistem içerisinde katmanlar aşağıdaki sırayla çalışacaktır.

```text
İstemci
    │
    ▼
BizimSite.API
    │
    ▼
BizimSite.Application
    │
    ▼
BizimSite.Domain
    │
    ▼
BizimSite.Infrastructure
    │
    ▼
SQL Server
```

---

# Genel Değerlendirme

Katmanlı mimari sayesinde sistem sorumlulukları ayrıştırılarak daha düzenli, sürdürülebilir ve geliştirilebilir bir yapı oluşturulması hedeflenmektedir.

Bu mimari, BizimSite Backend projesinin geliştirilmesi boyunca temel referans olarak kullanılacaktır.
