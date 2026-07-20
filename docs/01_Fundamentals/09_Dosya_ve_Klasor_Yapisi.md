# BizimSite Backend - Dosya ve Klasör Yapısı

## Amaç

Bu doküman, BizimSite Backend projesinde kullanılacak proje ve klasör organizasyonunu açıklamak amacıyla hazırlanmıştır.

Katmanların sorumlulukları, proje yapısı ve klasör düzeni bu dokümanda tanımlanmaktadır.

---

# Kapsam

Bu doküman aşağıdaki konuları kapsamaktadır.

- Proje yapısı
- Katmanlar
- Katman sorumlulukları
- Dosya organizasyonu

---

# Proje Yapısı

Backend çözümü (Solution), farklı sorumluluklara sahip projelerden oluşacaktır.

Her proje yalnızca kendi sorumluluğuna ait kodları içerecektir.

Önerilen yapı;

```text
BizimSite.sln

├── BizimSite.API
├── BizimSite.Application
├── BizimSite.Domain
└── BizimSite.Infrastructure
```

---

# Katmanlar

## API

İstemcilerden gelen HTTP isteklerini karşılar.

İstekleri ilgili uygulama akışına yönlendirir ve sonuçları istemciye döndürür.

---

## Application

Uygulamanın iş akışlarını yönetir.

API ile Domain katmanı arasındaki koordinasyonu sağlar.

---

## Domain

Sistemin temel iş kurallarını içerir.

Projeye ait varlıklar (Entities), kurallar ve iş mantığı bu katmanda yer alacaktır.

---

## Infrastructure

Veritabanı işlemleri, harici servis bağlantıları ve teknik altyapı bileşenlerini içerir.

---

# Tasarım Prensipleri

Katmanlar birbirinden bağımsız olacak şekilde tasarlanacaktır.

Her katman yalnızca kendi sorumluluk alanındaki işlemleri gerçekleştirecektir.

Bu yaklaşım sayesinde sistem daha okunabilir, geliştirilebilir ve sürdürülebilir olacaktır.

---

# Tasarım Kararları

Bu proje kapsamında;

- Katmanlı mimari kullanılacaktır.
- Her katman tek bir sorumluluğa sahip olacaktır.
- Kod organizasyonu proje yapısına uygun şekilde gerçekleştirilecektir.

---

# İlgili Dokümanlar

- 01_Proje_Mimarisi.md
- 02_API_Tasarimi.md
- 04_Veritabani_Tasarimi.md
