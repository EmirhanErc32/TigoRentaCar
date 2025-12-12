# 🚀 Proje Özellikleri ve Modüller

## 🔐 1. Kimlik Doğrulama & Güvenlik (Auth)
- **Kullanıcı Girişi ve Kayıt Sistemi:** Müşteri ve admin için ayrı giriş ekranı.  
- **Basit Şifreleme:** Kullanıcı şifrelerinin güvenli saklanması (dosya tabanlı veya Java hashing ile).  
- **Rol Yönetimi:** `Admin` ve `User` rollerine göre farklı panel erişimleri.

---

## 👤 2. Kullanıcı Paneli (Customer App)
- **Araç Kategorileri:**  
  - 🚘 Otomobil  
  - 🚙 SUV  
  - 🚚 Ticari  
- **Araç Listeleme:** Her kategoride uygun araçların marka, model, fiyat ve müsaitlik durumuyla görüntülenmesi.  
- **Araç Kiralama:** Seçilen araç için kiralama süresi belirleme ve toplam fiyat hesaplama.  
- **Filo Kiralama Modülü:** Birden fazla araç seçip toplu kiralama yapabilme.

---

## 🚗 3. Araç Yönetim Sistemi (Core)
- **Araç Ekleme:** Admin tarafından yeni araç eklenmesi.  
- **Araç Silme:** Sistemdeki herhangi bir aracın kaldırılması.  
- **Araç Güncelleme:**  
  - Fiyat  
  - Müsaitlik durumu  
  - Kategori  
- **Araç Arama & Filtreleme:**  
  Marka, kategori ve fiyat aralığına göre filtreleme.

---

## 🛠️ 4. Admin Paneli (Management)
- **Fiyat Yönetimi:** Günlük kiralama ücretlerinin güncellenmesi.  
- **Araç Durumu Yönetimi:** Kiralanan araçların durumunun takip edilmesi.  
- **Kiralama Kayıtları:**  
  - Kullanıcı kim kiraladı  
  - Hangi aracı kiraladı  
  - Başlangıç–bitiş tarihleri  
  - Toplam ücret  
- **Loglama (İsteğe bağlı):** Sistem hareketlerinin kayıt altına alınması.

---

## 📦 5. Veri İşleme & Depolama (Temporary Storage)
> Projede veritabanı yoktur. Bunun yerine:  
> - **Dosya Tabanlı Kayıt (TXT/JSON)** veya  
> - **Java Collection'ları (ArrayList, HashMap)** kullanılır.

Depolanan veriler:  
- Kullanıcı listesi  
- Araç listesi  
- Kiralama kayıtları  

---

## 🧱 6. OOP Yapısı
- **Sınıflar:**  
  - `User`  
  - `Admin`  
  - `Car`  
  - `Rental`  
  - `CarManager`  
  - `UserManager`  
  - `RentalManager`  
- **Prensipler:**  
  - Encapsulation  
  - Inheritance  
  - Polymorphism  
  - Clean Code mantığı

---

## 🧮 7. Fiyat Hesaplama Araçları
- **Günlük Ücret Hesaplayıcı:** Kiralama gününe göre otomatik toplam maliyet.  
- **Filo Kiralama Hesaplama:** Araç sayısı × gün × kategori fiyatı.  
