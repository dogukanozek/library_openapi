# OpenAPI Tasarımı Ödevi Teslim Raporu

## 🎓 Ders: Açık Kaynak Kodlu Yazılımlar
**Teslim Tarihi**: [26.05.2025]
**Teslim Yeri**: Google Classroom (Yalnızca `DELIVERY.md` dosyası)


## 👤 Öğrenci Bilgileri
- **Ad Soyad**: Doğukan Özek
- **Öğrenci Numarası**: 171422001

---

## 📂 OpenAPI YAML Dosyası

- **openapi.yaml** dosyasını projenizin GitHub reposuna yükleyiniz.
- Swagger Editor ile test ettiğinizden emin olunuz.

### 🔗 GitHub Repo Linki
https://github.com/dogukanozek/library_openapi.git

---

## 📝 API Açıklaması

Bu API, üniversiteye ait çevrim içi kütüphane sistemi için tasarlanmıştır. Üç temel varlık üzerinde işlem yapılmasını sağlar:

- **books**: Kitaplar ile ilgili işlemleri içerir.
  - `GET /books`: Sayfalama destekli kitap listesi döner.
  - `GET /books/{id}`: Belirli kitabın detaylarını getirir.
  - `POST /books`: Yeni kitap ekler.
  - `PUT /books/{id}`: Mevcut kitabı günceller.
  - `DELETE /books/{id}`: Kitabı siler.

- **students**: Öğrenciler ile ilgili işlemleri içerir.
  - `GET /students`: Tüm öğrencileri listeler.
  - `GET /students/{id}`: Belirli öğrencinin detaylarını getirir.
  - `POST /students`: Yeni öğrenci kaydı oluşturur.
  - `PUT /students/{id}`: Mevcut öğrenci kaydını günceller.
  - `DELETE /students/{id}`: Öğrenci kaydını siler.

- **loans**: Kitap ödünç alma ve iade işlemleri ile ilgilenir.
  - `GET /loans`: Tüm ödünç kayıtlarını listeler.
  - `GET /loans/{id}`: Belirli ödünç kaydını getirir.
  - `POST /loans`: Kitap ödünç alır.
  - `PATCH /loans/{id}/return`: Kitabı iade eder.

### Kullanılan Bileşenler
- `components/schemas` ile tüm veri modelleri tanımlandı (`Book`, `Student`, `Loan`).
- `parameters` kısmında `path` ve `query` parametreleri (örn. `page`, `id`) kullanıldı.
- `responses` altında 200, 201, 400, 404 gibi durumlara özel yanıtlar tanımlandı.
- `example` alanı ile örnek veri gösterimi sağlandı.
- `GET /books` endpointinde sayfalama desteği sağlandı (`page`, `size`).
- Açıklayıcı `tags` ve `description` alanları kullanıldı.

---

## 🧪 Test Notları (Opsiyonel)

- `GET /books` çağrısında kitap listesi JSON formatında döner.
- `POST /books` için örnek `requestBody`:
```json
{
  "id": "1",
  "title": "OpenAPI Guide",
  "author": "Jane Doe",
  "isbn": "978-3-16-148410-0",
  "publisher": "TechBooks",
  "pageCount": 200,
  "stock": 3
}
```
- Geçersiz `isbn` ile gönderilen POST isteği için `400 Bad Request` döner.

---

## 📌 Ek Açıklamalar

Proje Swagger Editor üzerinde test edilmiştir. Tüm zorunlu endpoint ve şemalar OpenAPI 3.0.3 standardına uygun şekilde tanımlanmıştır.
