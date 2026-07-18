# BizimSite Backend - Entity Tasarımları

Bu doküman, BizimSite Backend projesinde kullanılacak temel entity yapılarını taslak olarak göstermektedir.

---

# Kullanici

| Alan | Açıklama |
|------|----------|
| Id | Benzersiz kullanıcı numarası |
| Ad | Kullanıcının adı |
| Soyad | Kullanıcının soyadı |
| Eposta | E-posta adresi |
| SifreHash | Şifre özeti |
| Telefon | Telefon numarası |
| DaireNo | Oturduğu daire |
| Rol | Kullanıcının sistemdeki rolü |
| OlusturmaTarihi | Kayıt tarihi |

---

# Duyuru

| Alan | Açıklama |
|------|----------|
| Id | Benzersiz duyuru numarası |
| Baslik | Duyuru başlığı |
| Icerik | Duyuru içeriği |
| YayinTarihi | Yayın tarihi |

---

# Aidat

| Alan | Açıklama |
|------|----------|
| Id | Benzersiz aidat kaydı |
| KullaniciId | Aidatın ait olduğu kullanıcı |
| Tutar | Aidat tutarı |
| SonOdemeTarihi | Son ödeme tarihi |
| Durum | Ödeme durumu |
