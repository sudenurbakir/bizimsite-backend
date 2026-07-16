# BizimSite Backend - API Tasarımı

## Amaç

Bu doküman, BizimSite Backend projesinde uygulanacak API tasarım yaklaşımını açıklamak amacıyla hazırlanmıştır.

API katmanının sistem içerisindeki sorumlulukları, temel tasarım kararları ve istemci uygulamalarıyla olan iletişim yapısı bu dokümanda açıklanmaktadır.

---

# Kapsam

Bu doküman aşağıdaki konuları kapsamaktadır.

- API katmanının sistem içerisindeki görevi
- API'nin sorumlulukları
- İstemci ile backend arasındaki iletişim yapısı
- API tasarımında benimsenen temel yaklaşım

---

# API Katmanının Görevi

BizimSite Backend projesinde API katmanı, istemciler ile backend sistemi arasındaki giriş noktasıdır.

Web ve mobil istemcilerden gelen tüm HTTP istekleri ilk olarak API katmanı tarafından karşılanacaktır.

API katmanı;

- İstekleri kabul eder.
- İlgili uygulama akışını başlatır.
- İşlem sonucunu istemciye döndürür.

API katmanında iş kuralları veya veri erişim işlemleri gerçekleştirilmez.

---

# API Tasarım Yaklaşımı

BizimSite Backend projesinde API tasarımında REST mimari yaklaşımı benimsenmiştir.

API uç noktaları, HTTP standartlarına uygun şekilde tasarlanacak ve istemciler ile backend arasındaki iletişim JSON veri formatı kullanılarak gerçekleştirilecektir.

Tüm istemci uygulamaları backend sistemine yalnızca API üzerinden erişecektir.

---

# API'nin Sorumlulukları

API katmanı aşağıdaki temel sorumluluklara sahiptir.

- İstemci isteklerini karşılamak
- Gelen istekleri ilgili uygulama akışına yönlendirmek
- İşlem sonucunu standart bir yapı ile istemciye döndürmek
- HTTP durum kodlarını uygun şekilde kullanmak

---

# Katmanlar ile İlişkisi

API katmanı yalnızca istemciler ile backend sistemi arasında iletişim kurar.

İş kuralları Application ve Domain katmanlarında uygulanırken, veri erişim işlemleri Infrastructure katmanı tarafından gerçekleştirilir.

Bu sayede katmanlar arasında sorumluluk ayrımı korunur.

---

# Tasarım Kararları

Bu proje kapsamında;

- API katmanı yalnızca istemci iletişiminden sorumludur.
- İş kuralları API katmanında yer almayacaktır.
- Veri erişim işlemleri API katmanında gerçekleştirilmeyecektir.
- API tasarımında REST prensipleri esas alınacaktır.

---

# İlgili Dokümanlar

- 01_Proje_Mimarisi.md
- 03_API_Standartlari.md
