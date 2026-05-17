
# 📊 LogicShield Data Pipeline & Analytics (ETL)

Bu proje, büyük hacimli (1000+ satır) Excel verilerini canlı bir PostgreSQL bulut veritabanına aktaran ve Pandas kullanarak otonom İş Zekası (BI) raporları üreten bir **Veri Mühendisliği (Data Pipeline)** mimarisidir.

## 🚀 Proje Amacı
Manuel veri girişi süreçlerini ortadan kaldırarak; Excel şablonlarındaki devasa veritabanı simülasyonlarını tek tıkla buluta taşımak ve bu veriler üzerinden finansal/kategorik analizler üreten bir **HTML Yönetim Paneli (Dashboard)** oluşturmak.

## 🛠️ Kullanılan Teknolojiler (Tech Stack)
* **Python 3.10+** (Veri işleme motoru)
* **Pandas & Numpy** (Veri manipülasyonu ve istatistiksel analiz)
* **SQLAlchemy & psycopg2** (PostgreSQL ORM ve veritabanı bağlantısı)
* **PostgreSQL (Supabase)** (Canlı bulut veritabanı)
* **GitHub Actions** (CI/CD, Otonom tetikleme ve Rapor üretimi)
* **Openpyxl** (Excel dosya yönetimi)

## 🏗️ Mimari Akış (ETL Process)
1. **Extract (Çıkarma):** Python, `logic_shield_1000_kayit.xlsx` dosyasındaki Orders, Products, Subscriptions ve Order_Items sayfalarını okur.
2. **Load (Yükleme):** SQLAlchemy kullanılarak bu binlerce satırlık veri, sıfırdan kurulan canlı Supabase veritabanına saniyeler içinde basılır (`to_sql` metodu ile).
3. **Transform & Analyze (İşleme):** Pandas devreye girerek veritabanındaki ham veriyi işler. Ciro özetleri, kategori bazlı satış trendleri ve finansal anomali kontrolleri hesaplanır.
4. **Deliver (Sunum):** Hesaplanan metrikler, otomatik olarak oluşturulan şık bir `dashboard.html` raporuna dönüştürülerek yönetici onayına sunulur.

## 👤 Geliştirici
**Eda Nur Çavuş** | Mathematics & Data Enthusiast
