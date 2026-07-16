# BizimSite Backend - API Nedir?

Bu doküman, BizimSite Backend projesinde kullanılacak API yapısını açıklamak amacıyla hazırlanmıştır.

---

# API Nedir?

API (Application Programming Interface), farklı yazılımların birbiriyle iletişim kurmasını sağlayan bir arayüzdür.

BizimSite projesinde API, istemcilerden (web uygulaması, mobil uygulama vb.) gelen istekleri karşılayan ve gerekli işlemleri başlatan katmandır.

---

# API Neden Kullanılır?

İstemci uygulamalarının doğrudan veritabanına erişmesi güvenlik, bakım ve yönetilebilirlik açısından uygun değildir.

Bu nedenle istemci ile veritabanı arasına bir API katmanı yerleştirilir.

API;

- İstekleri karşılar.
- Gerekli işlemleri başlatır.
- İşlem sonucunu istemciye döndürür.

---

# BizimSite Projesinde API'nin Görevi

BizimSite Backend projesinde API aşağıdaki işlemleri gerçekleştirecektir.

- Kullanıcı giriş isteklerini almak
- Ortak alan rezervasyon işlemlerini başlatmak
- Aidat bilgilerini istemciye sunmak
- Arıza ve hizmet taleplerini yönetmek
- Ortak gider kayıtlarını istemcilere ulaştırmak

API yalnızca işlemleri başlatır.

İş kuralları ve veri erişim işlemleri diğer katmanlarda gerçekleştirilecektir.

---

# API'nin Avantajları

API kullanımı sayesinde;

- Güvenlik artırılır.
- Kod tekrarları azaltılır.
- Farklı istemciler aynı sistemi kullanabilir.
- Bakım ve geliştirme süreçleri kolaylaşır.

---

# Genel Değerlendirme

API, BizimSite Backend projesinin dış dünya ile iletişim kuran giriş noktasıdır.

Sisteme yapılan tüm istekler API üzerinden karşılanacak ve ilgili katmanlara yönlendirilecektir.
