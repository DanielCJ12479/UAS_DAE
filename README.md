# 🥣 Analisis Nutrisi Sereal & Prediksi Rating

Proyek ini menganalisis dataset 80 produk sereal untuk memahami faktor nutrisi apa saja yang mempengaruhi penilaian (rating) konsumen. Menggunakan Exploratory Data Analysis (EDA) dan Machine Learning, kami mengidentifikasi faktor kunci penentu sereal berkualitas tinggi.

## 👥 Penulis
* **Daniel Christopher Juwono** (C14220006)
* **Harvey Kristandi** (C14220244)

## 🎯 Tujuan Proyek
1. **Menganalisis** faktor nutrisi (kalori, gula, serat, dll.) yang paling mempengaruhi rating produk.
2. **Memprediksi** kategori tingkat kesehatan/rating dari setiap sereal.

## 📊 Tentang Dataset
Dataset mencakup variabel berikut untuk 80 produk sereal:
* **Metadata:** Nama, Manufaktur, Tipe.
* **Nutrisi:** Kalori, Protein, Lemak, Sodium, Serat, Karbohidrat, Gula, Potasium, Vitamin.
* **Target:** Rating.

> **Catatan Data Cleaning:** Data dengan nilai `-1` (menandakan *missing value*) telah dihapus pada tahap pra-pemrosesan.

## 🔍 Temuan Utama (Insights)

### 1. Analisis Manufaktur
* **Kualitas vs Kuantitas:** **Kellogg's (K)** dan **General Mills (G)** memiliki jumlah produk terbanyak, namun rating rata-rata mereka moderat karena portofolio produk yang bercampur (sehat & manis).
* **Performa Terbaik:** **Nabisco (N)** memimpin pasar dalam hal kepuasan konsumen (rating tertinggi), berkat fokus strategi mereka pada produk gandum utuh yang minim gula.

### 2. Korelasi Nutrisi
* **Musuh Rating:** **Gula (Sugars)** dan **Kalori** memiliki korelasi negatif yang kuat. Semakin tinggi gula, semakin anjlok rating produk.
* **Pendorong Rating:** **Serat (Fiber)** memiliki korelasi positif terkuat. Produk tinggi serat konsisten berada di peringkat atas.

### 3. Hasil Machine Learning
Menggunakan **Random Forest**, ditemukan fitur terpenting (*Feature Importance*) dalam penentuan kualitas sereal:
1. **Gula** (Paling dominan)
2. **Kalori**
3. **Serat**

Faktor lain seperti lemak atau vitamin memiliki dampak yang jauh lebih kecil.

## 🛠️ Metodologi
1. **Data Cleaning:** Menghapus nilai error/NaN (`-1`).
2. **EDA:** Visualisasi perbandingan Manufaktur vs Rating dan pengaruh Makronutrisi, Mikronutrisi, dll
3. **Modeling:**
   * **Random Forest:** Klasifikasi dan analisis fitur penting.

## 🚀 Kesimpulan
Kunci keberhasilan produk dalam metrik rating ini terletak pada keseimbangan makronutrisi dasar: **Rendah Gula, Rendah Kalori, dan Tinggi Serat**.

---
*Dibuat untuk tugas mata kuliah Eksplorasi & Analisis Data.*
