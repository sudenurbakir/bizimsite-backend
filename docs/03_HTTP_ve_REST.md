# BizimSite Backend - HTTP ve REST

Bu doküman, BizimSite Backend projesinde kullanılacak HTTP protokolü ve REST mimarisini açıklamak amacıyla hazırlanmıştır.

---

# HTTP Nedir?

HTTP (HyperText Transfer Protocol), istemci ile sunucu arasında veri iletişimini sağlayan uygulama katmanı protokolüdür.

BizimSite Backend projesinde web ve mobil istemciler ile backend arasındaki tüm iletişim HTTP üzerinden gerçekleştirilecektir.

---

# HTTP Nasıl Çalışır?

İstemci bir HTTP isteği gönderir.

Sunucu isteği işler.

İşlem sonucunda istemciye bir HTTP cevabı döndürülür.

Bu iletişim modeli "İstek (Request) - Cevap (Response)" yapısına dayanır.

---

# HTTP İstekleri

HTTP üzerinde farklı amaçlar için kullanılan yöntemler bulunmaktadır.

| Yöntem | Açıklama |
|--------|----------|
| GET | Veri görüntülemek için kullanılır. |
| POST | Yeni veri oluşturmak için kullanılır. |
| PUT | Mevcut veriyi güncellemek için kullanılır. |
| DELETE | Veriyi silmek için kullanılır. |

BizimSite Backend projesinde bu yöntemler REST mimarisine uygun şekilde kullanılacaktır.

---

# REST Nedir?

REST (Representational State Transfer), HTTP tabanlı servislerin geliştirilmesinde kullanılan bir mimari yaklaşımdır.

REST, istemci ile sunucu arasındaki iletişimin belirli kurallar çerçevesinde gerçekleştirilmesini sağlar.

---

# BizimSite Projesinde REST Kullanımı

Sistem içerisinde;

- Aidat işlemleri
- Ortak alan rezervasyonları
- Arıza talepleri
- Hizmet talepleri
- Ortak gider işlemleri

REST prensiplerine uygun API uç noktaları üzerinden yönetilecektir.

---

# REST Kullanmanın Avantajları

REST mimarisi sayesinde;

- API daha okunabilir olur.
- İstemciler API'yi daha kolay kullanabilir.
- Standart bir yapı oluşturulur.
- Bakım ve geliştirme süreçleri kolaylaşır.

---

# Genel Değerlendirme

BizimSite Backend projesinde istemci ve sunucu arasındaki tüm iletişim HTTP protokolü üzerinden gerçekleştirilecek olup API tasarımında REST mimari yaklaşımı esas alınacaktır.
