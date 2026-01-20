# Analisis Data Taksi NYC (NYC TLC Trip Record)

Proyek ini berfokus pada eksplorasi dan analisis data perjalanan taksi di New York City menggunakan Python.  
Tujuannya adalah untuk memahami pola perjalanan, mendeteksi outlier, dan menyiapkan data agar siap digunakan untuk analisis lanjutan seperti prediksi atau machine learning.

---

## Dataset
Dataset yang digunakan adalah **NYC TLC Trip Record**, yang berisi informasi mengenai:
- Waktu pengambilan dan penurunan penumpang  
- Jarak perjalanan  
- Biaya perjalanan (fare amount, tips, tax, dll.)  
- Jenis pembayaran dan tipe perjalanan

---

## Tahapan Analisis

### 1. Pemeriksaan Nilai Hilang (Missing Values)
Menelusuri nilai **NaN** di kolom penting seperti:
- `Ehail Fee`
- `RatecodeID`
- `Trip Type`
- `Congestion Surcharge`
- `Payment Type`

### 2. Pembersihan dan Transformasi Data
- Mengubah tipe data tanggal ke format `datetime`
- Konversi nilai `float` ke `int` untuk kolom nominal
- Menangani nilai anomali atau tidak logis pada data numerik

### 3. Deteksi Outlier
Mengidentifikasi data ekstrem di kolom seperti:
- `Trip Distance`
- `Fare Amount`
- `Total Amount`

Analisis dilakukan menggunakan metode statistik (seperti boxplot dan deskripsi kuartil).

### 4. Analisis Statistik
Melakukan uji coba terhadap distribusi pendapatan dan menghitung peluang rata-rata dari sejumlah sampel data perjalanan.

---

## Tools dan Library
- **Python 3.x**
- **Pandas** untuk pembersihan dan manipulasi data  
- **NumPy** untuk perhitungan numerik  
- **Matplotlib / Seaborn** untuk visualisasi data  
- **Jupyter Notebook** untuk dokumentasi analisis

---

## 🚀 Cara Menjalankan
1. Clone repository ini:
   ```bash
   git clone https://github.com/username/NYC_TLC_Trip_Record.git
   cd NYC_TLC_Trip_Record
