# BizimSite Backend - Veritabanı Varlıkları

Bu doküman, BizimSite Backend projesinde kullanılacak temel veritabanı varlıklarını açıklamak amacıyla hazırlanmıştır.

---

# Veritabanı Varlığı Nedir?

Veritabanı varlığı (Entity), sistem içerisinde saklanacak bilgileri temsil eden temel yapılardır.

Her varlık belirli bir iş alanını ifade eder ve ilerleyen aşamalarda bir veritabanı tablosu olarak modellenebilir.

---
# Projede Kullanılacak Varlıklar

| Varlık | Açıklama |
|--------|----------|
| Daire | Site içerisindeki bağımsız bölümleri temsil eder. |
| Kullanici | Sisteme giriş yapan kullanıcı bilgilerini temsil eder. |
| Duyuru | Yönetim tarafından paylaşılan duyuruları temsil eder. |
| Aidat | Kullanıcılara ait aidat bilgilerini temsil eder. |
| Rezervasyon | Ortak alan rezervasyon kayıtlarını temsil eder. |
| ArizaTalebi | Kullanıcıların oluşturduğu arıza taleplerini temsil eder. |
| HizmetTalebi | Kullanıcıların oluşturduğu hizmet taleplerini temsil eder. |

---

# Tasarım Kararları

Bu proje kapsamında;

- Her varlık tek bir iş alanını temsil edecektir.
- Her varlık ilerleyen aşamalarda ayrı bir veritabanı tablosu olarak tasarlanacaktır.
- Varlıklar arasında gerekli ilişkiler daha sonraki tasarım aşamalarında belirlenecektir.

---

# Genel Değerlendirme

Veritabanı varlıkları, BizimSite Backend projesinin veri modelinin temelini oluşturmaktadır.

İlerleyen aşamalarda bu varlıkların özellikleri ve aralarındaki ilişkiler ayrıntılı olarak tasarlanacaktır.
