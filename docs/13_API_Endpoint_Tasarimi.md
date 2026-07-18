# BizimSite Backend - API Endpoint Tasarımı

Bu doküman, BizimSite Backend projesinde kullanılacak temel API endpointlerini açıklamak amacıyla hazırlanmıştır.

---

# API Endpoint Nedir?

API endpoint, istemci uygulamalarının backend üzerinde belirli bir işlemi gerçekleştirmek için kullandığı adresi ifade eder.

Her endpoint belirli bir amaca hizmet eder ve uygun HTTP yöntemi ile birlikte kullanılır.

---

# Authentication Endpointleri

| HTTP Metodu | Endpoint | Açıklama |
|--------------|----------|----------|
| POST | /api/auth/login | Kullanıcı giriş işlemini gerçekleştirir. |
| POST | /api/auth/logout | Kullanıcı oturumunu sonlandırır. |

---

# Duyuru Endpointleri

| HTTP Metodu | Endpoint | Açıklama |
|--------------|----------|----------|
| GET | /api/announcements | Duyuruları listeler. |
| GET | /api/announcements/{id} | Belirli bir duyurunun detayını getirir. |

---

# Aidat Endpointleri

| HTTP Metodu | Endpoint | Açıklama |
|--------------|----------|----------|
| GET | /api/payments | Aidat listesini getirir. |
| GET | /api/payments/{id} | Aidat detayını getirir. |

---

# Ortak Alan Rezervasyonu Endpointleri

| HTTP Metodu | Endpoint | Açıklama |
|--------------|----------|----------|
| GET | /api/reservations | Rezervasyonları listeler. |
| POST | /api/reservations | Yeni rezervasyon oluşturur. |
| DELETE | /api/reservations/{id} | Rezervasyonu iptal eder. |

---

# Arıza Talebi Endpointleri

| HTTP Metodu | Endpoint | Açıklama |
|--------------|----------|----------|
| GET | /api/fault-reports | Arıza taleplerini listeler. |
| POST | /api/fault-reports | Yeni arıza talebi oluşturur. |

---

# Hizmet Talebi Endpointleri

| HTTP Metodu | Endpoint | Açıklama |
|--------------|----------|----------|
| GET | /api/service-requests | Hizmet taleplerini listeler. |
| POST | /api/service-requests | Yeni hizmet talebi oluşturur. |

---

# Tasarım Kararları

Bu proje kapsamında;

- Endpoint isimlendirmelerinde tutarlı bir yapı kullanılacaktır.
- Endpointler REST mimarisine uygun şekilde tasarlanacaktır.
- Her endpoint yalnızca tek bir işlevden sorumlu olacaktır.
- Uygun HTTP metodları kullanılacaktır.

---

# Genel Değerlendirme

API endpointleri, istemci uygulamaları ile backend arasındaki iletişimin temelini oluşturur.

Bu dokümanda belirlenen endpoint yapısı, BizimSite Backend projesinin geliştirme sürecinde temel referans olarak kullanılacaktır.
