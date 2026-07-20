# BizimSite Backend - Veritabanı Tasarımı

## Amaç

Bu doküman, BizimSite Backend projesinde uygulanacak veritabanı tasarım yaklaşımını açıklamak amacıyla hazırlanmıştır.

Veri modeli oluşturulurken benimsenen temel prensipler, tablo ilişkileri ve veri bütünlüğünü korumaya yönelik tasarım kararları bu dokümanda açıklanmaktadır.

---

# Kapsam

Bu doküman aşağıdaki konuları kapsamaktadır.

- Veritabanı yönetim sistemi
- Veri modelleme yaklaşımı
- Tablo ilişkileri
- Anahtar yapıları
- Veri bütünlüğü

---

# Veritabanı Yönetim Sistemi

BizimSite Backend projesinde ilişkisel veritabanı yönetim sistemi olarak Microsoft SQL Server kullanılacaktır.

Uygulama verileri ilişkisel yapıda saklanacak ve veri bütünlüğü veritabanı kısıtları ile desteklenecektir.

---

# Veri Modelleme Yaklaşımı

Veritabanı tasarımında normalizasyon prensipleri esas alınacaktır.

Her tablo belirli bir sorumluluğa sahip olacak ve gereksiz veri tekrarından kaçınılacaktır.

Tablolar arasındaki ilişkiler birincil anahtar (Primary Key) ve yabancı anahtar (Foreign Key) yapıları kullanılarak oluşturulacaktır.

---

# Tablo İlişkileri

Sistemde yer alan tablolar, iş kurallarına uygun şekilde birbirleriyle ilişkilendirilecektir.

İlişkiler sayesinde veri tutarlılığı korunacak ve tekrar eden kayıtların oluşması önlenecektir.

---

# Anahtar Yapıları

Her tabloda benzersiz bir Primary Key bulunacaktır.

Tablolar arasındaki ilişkiler Foreign Key kullanılarak kurulacaktır.

Bu yapı sayesinde ilişkili kayıtların yönetimi güvenli ve tutarlı şekilde gerçekleştirilecektir.

---

# Veri Bütünlüğü

Veritabanında veri bütünlüğünü korumak amacıyla;

- Primary Key kullanılacaktır.
- Foreign Key ilişkileri tanımlanacaktır.
- Zorunlu alanlar boş bırakılamayacaktır.
- Veri tipleri ihtiyaca uygun şekilde belirlenecektir.

---

# Tasarım Kararları

Bu proje kapsamında;

- Microsoft SQL Server kullanılacaktır.
- İlişkisel veritabanı modeli tercih edilmiştir.
- Normalizasyon prensipleri uygulanacaktır.
- Veri bütünlüğü veritabanı seviyesinde korunacaktır.

---

# İlgili Dokümanlar

- 01_Proje_Mimarisi.md
- ER Diyagramı
