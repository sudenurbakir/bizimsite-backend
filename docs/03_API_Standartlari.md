# BizimSite Backend - API Standartları

## Amaç

Bu doküman, BizimSite Backend projesinde uygulanacak API standartlarını açıklamak amacıyla hazırlanmıştır.

API geliştirme sürecinde kullanılacak HTTP yöntemleri, URL isimlendirme kuralları, veri formatı ve genel tasarım prensipleri bu dokümanda tanımlanmaktadır.

---

# Kapsam

Bu doküman aşağıdaki konuları kapsamaktadır.

- HTTP yöntemlerinin kullanımı
- REST mimari yaklaşımı
- URL isimlendirme standartları
- Veri alışverişi formatı
- HTTP durum kodlarının kullanımı

---

# HTTP Yöntemleri

BizimSite Backend projesinde API uç noktaları aşağıdaki HTTP yöntemlerine uygun şekilde tasarlanacaktır.

| Yöntem | Kullanım Amacı |
|--------|----------------|
| GET | Veri görüntüleme |
| POST | Yeni kayıt oluşturma |
| PUT | Mevcut kaydı güncelleme |
| DELETE | Kayıt silme |

Her HTTP yöntemi yalnızca kendi amacı doğrultusunda kullanılacaktır.

---

# REST Yaklaşımı

API tasarımında REST mimari yaklaşımı esas alınacaktır.

REST prensipleri doğrultusunda;

- Kaynak odaklı URL yapısı kullanılacaktır.
- HTTP yöntemleri doğru amaçlarla kullanılacaktır.
- İstekler ve cevaplar stateless (durumsuz) yapıda olacaktır.
- İstemci ile backend arasındaki iletişim HTTP üzerinden gerçekleştirilecektir.

---

# URL İsimlendirme Standardı

API uç noktaları oluşturulurken aşağıdaki kurallar uygulanacaktır.

- URL'ler küçük harflerle yazılacaktır.
- Kaynak isimleri çoğul kullanılacaktır.
- Türkçe karakter kullanılmayacaktır.
- Boşluk kullanılmayacaktır.

Örnek URL yapıları;

```text
/api/users
/api/apartments
/api/reservations
/api/dues
/api/service-requests
```

---

# Veri Formatı

İstemci ile backend arasındaki veri alışverişinde JSON formatı kullanılacaktır.

Alan isimlerinde camelCase isimlendirme standardı tercih edilecektir.

Örnek:

```json
{
  "userId": 1,
  "apartmentId": 12,
  "reservationDate": "2026-01-15"
}
```

---

# HTTP Durum Kodları

API cevaplarında standart HTTP durum kodları kullanılacaktır.

| Kod | Açıklama |
|-----|----------|
| 200 | İşlem başarılı |
| 201 | Kayıt oluşturuldu |
| 400 | Geçersiz istek |
| 401 | Kimlik doğrulaması gerekli |
| 403 | Yetkisiz işlem |
| 404 | Kayıt bulunamadı |
| 500 | Sunucu hatası |

---

# Tasarım Kararları

Bu proje kapsamında;

- REST mimari yaklaşımı kullanılacaktır.
- HTTP yöntemleri standart kullanım amaçlarına uygun olacaktır.
- JSON veri formatı kullanılacaktır.
- URL isimlendirmelerinde İngilizce ifadeler tercih edilecektir.
- API cevaplarında standart HTTP durum kodları kullanılacaktır.

---

# İlgili Dokümanlar

- 01_Proje_Mimarisi.md
- 02_API_Tasarimi.md
