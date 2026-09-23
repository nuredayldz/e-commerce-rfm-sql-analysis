# 📊 E-Commerce Customer Segmentation (RFM) & SQL Analytics

Bu projede, İngiltere merkezli bir online perakende işletmesinin işlem verileri analiz edilerek müşteri sadakati ölçülmüş, **RFM (Recency, Frequency, Monetary)** skorlaması ile müşteri segmentasyonu yapılmış ve ilişkisel veritabanı sorguları (**SQLite**) ile toptan sipariş ve ürün trendleri incelenmiştir.

---

## 🛠️ Kullanılan Teknolojiler & Kütüphaneler
* **Python**: Veri ön işleme, istatistiksel analiz ve görselleştirme
* **Pandas & NumPy**: Veri manipülasyonu ve qcut ile metrik skorlama
* **Matplotlib & Seaborn**: Keşifçi veri analizi (EDA) ve görselleştirme
* **SQLite3**: Python içi in-memory ilişkisel veritabanı sorgulamaları

---

## 📈 Proje Adımları

### 1. Veri Temizleme & Keşifçi Veri Analizi (EDA)
* 500.000+ satırlık ham verideki eksik müşteri ID'leri ve iptal edilen (negatif miktarlı) işlemler ayıklandı.
* Fatura bazında toplam sepet tutarı (`TotalPrice`) hesaplandı.
* En çok sipariş veren ülkeler ve en çok satan ürünler görselleştirildi.

### 2. RFM ile Müşteri Segmentasyonu
* 4.300'den fazla tekil müşteri için temel metrikler hesaplandı:
  * **Recency (Yenilik):** Müşterinin son alışverişinden bu yana geçen gün sayısı.
  * **Frequency (Sıklık):** Müşterinin gerçekleştirdiği toplam sipariş adedi.
  * **Monetary (Parasal Değer):** Müşterinin bıraktığı toplam ciro.
* `pd.qcut` kullanılarak müşteriler 1-5 arası skorlandı ve davranışlarına göre segmentlere ayrıldı:
  * *Champions (Şampiyonlar)*
  * *Loyal Customers (Sadık Müşteriler)*
  * *Hibernating (Kış Uykusundakiler)*
  * *At Risk (Risk Altındakiler)* vb.

### 3. SQLite ile Veritabanı Sorguları
* Veri çerçeveleri bellek içi (in-memory) SQLite veritabanına aktarıldı.
* Standart SQL sözdizimi (`GROUP BY`, `HAVING`, `LIKE`) kullanılarak:
  * 1.000 £ üzeri toptan siparişlerin tespiti yapıldı.
  * VIP segmentlerdeki en yüksek harcamaya sahip müşteriler sorgulandı.

---

## 💡 Temel İş Çıkarımları (Business Insights)
* **Kış Uykusu Tehlikesi:** Müşterilerin yaklaşık %25'i *Hibernating* grubunda yer almaktadır; bu kitleye yönelik geri kazanım kampanyaları önceliklendirilmelidir.
* **Ciro Omurgası:** Cironun büyük kısmı *Champions* ve *Loyal Customers* segmentleri tarafından sağlanmaktadır; bu gruplar için özel sadakat teşvikleri tasarlanmalıdır.# 📊 E-Commerce Customer Segmentation (RFM) & SQL Analytics

Bu projede, İngiltere merkezli bir online perakende işletmesinin işlem verileri analiz edilerek müşteri sadakati ölçülmüş, **RFM (Recency, Frequency, Monetary)** skorlaması ile müşteri segmentasyonu yapılmış ve ilişkisel veritabanı sorguları (**SQLite**) ile toptan sipariş ve ürün trendleri incelenmiştir.

---

## 🛠️ Kullanılan Teknolojiler & Kütüphaneler
* **Python**: Veri ön işleme, istatistiksel analiz ve görselleştirme
* **Pandas & NumPy**: Veri manipülasyonu ve qcut ile metrik skorlama
* **Matplotlib & Seaborn**: Keşifçi veri analizi (EDA) ve görselleştirme
* **SQLite3**: Python içi in-memory ilişkisel veritabanı sorgulamaları

---

## 📈 Proje Adımları

### 1. Veri Temizleme & Keşifçi Veri Analizi (EDA)
* 500.000+ satırlık ham verideki eksik müşteri ID'leri ve iptal edilen (negatif miktarlı) işlemler ayıklandı.
* Fatura bazında toplam sepet tutarı (`TotalPrice`) hesaplandı.
* En çok sipariş veren ülkeler ve en çok satan ürünler görselleştirildi.

### 2. RFM ile Müşteri Segmentasyonu
* 4.300'den fazla tekil müşteri için temel metrikler hesaplandı:
  * **Recency (Yenilik):** Müşterinin son alışverişinden bu yana geçen gün sayısı.
  * **Frequency (Sıklık):** Müşterinin gerçekleştirdiği toplam sipariş adedi.
  * **Monetary (Parasal Değer):** Müşterinin bıraktığı toplam ciro.
* `pd.qcut` kullanılarak müşteriler 1-5 arası skorlandı ve davranışlarına göre segmentlere ayrıldı:
  * *Champions (Şampiyonlar)*
  * *Loyal Customers (Sadık Müşteriler)*
  * *Hibernating (Kış Uykusundakiler)*
  * *At Risk (Risk Altındakiler)* vb.

### 3. SQLite ile Veritabanı Sorguları
* Veri çerçeveleri bellek içi (in-memory) SQLite veritabanına aktarıldı.
* Standart SQL sözdizimi (`GROUP BY`, `HAVING`, `LIKE`) kullanılarak:
  * 1.000 £ üzeri toptan siparişlerin tespiti yapıldı.
  * VIP segmentlerdeki en yüksek harcamaya sahip müşteriler sorgulandı.

---

## 💡 Temel İş Çıkarımları (Business Insights)
* **Kış Uykusu Tehlikesi:** Müşterilerin yaklaşık %25'i *Hibernating* grubunda yer almaktadır; bu kitleye yönelik geri kazanım kampanyaları önceliklendirilmelidir.
* **Ciro Omurgası:** Cironun büyük kısmı *Champions* ve *Loyal Customers* segmentleri tarafından sağlanmaktadır; bu gruplar için özel sadakat teşvikleri tasarlanmalıdır.# 📊 E-Commerce Customer Segmentation (RFM) & SQL Analytics

Bu projede, İngiltere merkezli bir online perakende işletmesinin işlem verileri analiz edilerek müşteri sadakati ölçülmüş, **RFM (Recency, Frequency, Monetary)** skorlaması ile müşteri segmentasyonu yapılmış ve ilişkisel veritabanı sorguları (**SQLite**) ile toptan sipariş ve ürün trendleri incelenmiştir.

---

## 🛠️ Kullanılan Teknolojiler & Kütüphaneler
* **Python**: Veri ön işleme, istatistiksel analiz ve görselleştirme
* **Pandas & NumPy**: Veri manipülasyonu ve qcut ile metrik skorlama
* **Matplotlib & Seaborn**: Keşifçi veri analizi (EDA) ve görselleştirme
* **SQLite3**: Python içi in-memory ilişkisel veritabanı sorgulamaları

---

## 📈 Proje Adımları

### 1. Veri Temizleme & Keşifçi Veri Analizi (EDA)
* 500.000+ satırlık ham verideki eksik müşteri ID'leri ve iptal edilen (negatif miktarlı) işlemler ayıklandı.
* Fatura bazında toplam sepet tutarı (`TotalPrice`) hesaplandı.
* En çok sipariş veren ülkeler ve en çok satan ürünler görselleştirildi.

### 2. RFM ile Müşteri Segmentasyonu
* 4.300'den fazla tekil müşteri için temel metrikler hesaplandı:
  * **Recency (Yenilik):** Müşterinin son alışverişinden bu yana geçen gün sayısı.
  * **Frequency (Sıklık):** Müşterinin gerçekleştirdiği toplam sipariş adedi.
  * **Monetary (Parasal Değer):** Müşterinin bıraktığı toplam ciro.
* `pd.qcut` kullanılarak müşteriler 1-5 arası skorlandı ve davranışlarına göre segmentlere ayrıldı:
  * *Champions (Şampiyonlar)*
  * *Loyal Customers (Sadık Müşteriler)*
  * *Hibernating (Kış Uykusundakiler)*
  * *At Risk (Risk Altındakiler)* vb.

### 3. SQLite ile Veritabanı Sorguları
* Veri çerçeveleri bellek içi (in-memory) SQLite veritabanına aktarıldı.
* Standart SQL sözdizimi (`GROUP BY`, `HAVING`, `LIKE`) kullanılarak:
  * 1.000 £ üzeri toptan siparişlerin tespiti yapıldı.
  * VIP segmentlerdeki en yüksek harcamaya sahip müşteriler sorgulandı.

---

## 💡 Temel İş Çıkarımları (Business Insights)
* **Kış Uykusu Tehlikesi:** Müşterilerin yaklaşık %25'i *Hibernating* grubunda yer almaktadır; bu kitleye yönelik geri kazanım kampanyaları önceliklendirilmelidir.
* **Ciro Omurgası:** Cironun büyük kısmı *Champions* ve *Loyal Customers* segmentleri tarafından sağlanmaktadır; bu gruplar için özel sadakat teşvikleri tasarlanmalıdır.
