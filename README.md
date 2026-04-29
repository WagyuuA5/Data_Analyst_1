# 📊 Dashboard Analysis Penjualan & ROI

**Proyek Analisis Data Penjualan** dengan fokus pada performa produk, efektivitas Return on Investment (ROI), serta rekomendasi strategi bisnis berbasis data.

---

## 📌 Ringkasan Proyek

| Metrik | Nilai |
|--------|-------|
| Total Transaksi | 150 |
| Total Pendapatan | **Rp473,9 Juta** |
| Rata-rata Transaksi | Rp3,16 Juta |
| Total Quantity Terjual | 460 unit |
| Rata-rata ROI | **163,9%** |

Proyek ini menganalisis **150 transaksi** dari 5 kategori produk (Books, Electronics, Fashion, Gadget, Home Decor) untuk mengidentifikasi:
- Kategori produk terlaris
- Efektivitas budget iklan
- Pola musiman penjualan
- Customer premium (top 5 pelanggan)

---

## 🎯 Tujuan Analisis

1. Menghitung statistik deskriptif variabel numerik
2. Mengukur **ROI (Return on Investment)** per produk & kategori
3. Mengidentifikasi korelasi antara budget iklan, quantity, dan total penjualan
4. Memberikan **rekomendasi bisnis** berbasis data

---

## 📂 Dataset

**Sumber:** `data_analis_1.csv`  
**Jumlah data:** 150 baris × 8 kolom  
**Periode:** Januari - Desember 2023

### 5 Baris Pertama Data

| Order_ID | CustomerID | Order_Date | Product_Category | Quantity | Price_Per_Unit | Ad_Budget | Total_Sales |
|----------|------------|------------|------------------|----------|----------------|-----------|-------------|
| 1001 | 5039 | 2023-08-19 | Books | 4 | 1.184.000 | 982.000 | 4.736.000 |
| 1002 | 5029 | 2023-08-29 | Fashion | 5 | 1.733.000 | 3.513.000 | 8.665.000 |
| 1003 | 5015 | 2023-02-21 | Fashion | 4 | 1.767.000 | 2.117.000 | 7.068.000 |
| 1004 | 5043 | 2023-04-06 | Fashion | 2 | 512.000 | 4.384.000 | 1.024.000 |
| 1005 | 5008 | 2023-08-10 | Home Decor | 2 | 1.820.000 | 2.625.000 | 3.640.000 |

---

## 📈 Statistik Deskriptif

| Statistik | Quantity | Price_Per_Unit | Ad_Budget | Total_Sales |
|-----------|----------|----------------|-----------|-------------|
| **Mean** | 3,07 | Rp1.024.640 | Rp2.618.947 | Rp3.155.287 |
| **Std** | 1,45 | Rp540.444 | Rp1.415.329 | Rp2.479.314 |
| **Min** | 1 | Rp77.000 | Rp113.000 | Rp77.000 |
| **25%** | 2 | Rp575.000 | Rp1.385.000 | Rp1.401.750 |
| **Median** | 3 | Rp988.000 | Rp2.722.500 | Rp2.336.000 |
| **75%** | 4 | Rp1.493.000 | Rp3.768.500 | Rp4.369.500 |
| **Max** | 5 | Rp1.992.000 | Rp4.987.000 | Rp9.810.000 |

---

## 📊 Performa per Kategori Produk

| Kategori | Jumlah Transaksi | Total Penjualan | Rata-rata Penjualan | Median Penjualan |
|----------|-----------------|----------------|---------------------|------------------|
| **Electronics** | 31 | **Rp114,1 Juta** | Rp3.680.484 | Rp2.818.000 |
| **Books** | 34 | Rp112,9 Juta | Rp3.321.588 | Rp2.628.500 |
| **Fashion** | 31 | Rp97,5 Juta | Rp3.144.065 | Rp1.868.000 |
| **Home Decor** | 24 | Rp76,3 Juta | Rp3.178.833 | Rp2.663.000 |
| **Gadget** | 30 | Rp72,5 Juta | Rp2.416.867 | Rp1.981.500 |

> ✅ **Insight:** Electronics menyumbang **24,1%** dari total pendapatan, menjadikannya kategori terlaris.

---

## 💰 Analisis ROI (Return on Investment)

| Metrik | Nilai |
|--------|-------|
| **Rata-rata ROI** | 163,89% |
| **Median ROI** | 13,49% |
| **ROI Tertinggi** | 4.491,15% |
| **ROI Terendah** | -97,36% |

### Rata-rata ROI per Kategori Produk

| Kategori | Rata-rata ROI |
|----------|---------------|
| **Home Decor** | **231,5%** ✅ (paling menguntungkan) |
| **Gadget** | 106,1% |
| **Books** | 29% |
| **Fashion** | 28% |
| **Electronics** | 25% |

> ✅ **Insight:** Home Decor memberikan ROI tertinggi meskipun total penjualannya tidak paling besar.

---

## 🔍 Insight & Rekomendasi Bisnis

### Insight 1: Kategori Produk Terlaris
- **Electronics** → Total Penjualan: **Rp114,1 Juta** (24,1% dari total)
- **Gadget** → Total Penjualan: Rp72,5 Juta

📌 **Rekomendasi:** Fokus promosi dan perluas lini produk Electronics.

---

### Insight 2: Efektivitas Budget Iklan (ROI)
- **Home Decor** → ROI: **231,5%** (paling menguntungkan)
- **Gadget** → ROI: 106,1% (perlu evaluasi)

📌 **Rekomendasi:** Alokasikan **40% budget iklan** ke kategori Home Decor.

---

### Insight 3: Hubungan Antar Variabel
| Korelasi | Nilai |
|----------|-------|
| Budget Iklan vs Penjualan | **0,035** (sangat lemah) |
| Quantity vs Penjualan | **0,642** (korelasi sedang/kuat) |

📌 **Rekomendasi:** Budget iklan bukan faktor utama penjualan. Perlu **evaluasi ulang strategi iklan** dan fokus pada peningkatan quantity.

---

### Insight 4: Customer Premium
- **Customer 5015** → Kontribusi: **Rp27,74 Juta**
- **Top 5 Customer** → Total kontribusi: **Rp113,58 Juta**

📌 **Rekomendasi:** Program loyalitas (diskon khusus, early access) untuk top 10% customer.

---

### Insight 5: Pola Musiman Penjualan
📌 **Rekomendasi:** Sesuaikan stok dan promosi berdasarkan pola penjualan per bulan.

---

## 📉 Visualisasi Dashboard

Dashboard mencakup:
- **Total Penjualan per Kategori** (Bar Chart)
- **Frekuensi Transaksi per Kategori**
- **Hubungan Budget Iklan vs Penjualan** (Scatter Plot + Trend Line)
- **Trend Penjualan per Bulan (2023)**
- **Distribusi Nilai Penjualan per Kategori** (Boxplot)
- **Matriks Korelasi Antar Variabel** (Heatmap)

---

## 🛠 Tools yang Digunakan

| Tools | Fungsi |
|-------|--------|
| **Python 3.9.12** | Bahasa pemrograman |
| **Pandas** | Manipulasi & analisis data |
| **Jupyter Notebook** | Environment analisis interaktif |
| **Matplotlib / Seaborn** | Visualisasi data |

---

## 📂 Struktur Proyek
├── data_analis_1.csv # Dataset utama (150 transaksi)
├── data_analis_1.ipynb # Notebook analisis lengkap
├── README.md # Dokumentasi proyek
└── requirements.txt # Daftar dependencies (opsional)


---

## 🚀 Cara Menjalankan

1. **Clone repositori**
```bash
git clone https://github.com/WagyuuA5/Data_Analyst_1.git
cd Data_Analyst_1

2. Install dependencies :
pip install pandas matplotlib seaborn jupyter

3. Buka Jupyter Notebook :
jupyter notebook data_analis_1.ipynb

4. Jalankan semua cell untuk melihat analisis lengkap

📋 Monitoring KPI yang Direkomendasikan
✅ Pantau ROI mingguan
✅ Evaluasi efektivitas iklan secara berkala
✅ Track penjualan per kategori produk
✅ Analisis retention customer premium

👤 Author
Anggoro Ravi (WagyuuA5)

📝 Catatan
Terdapat beberapa missing values pada kolom Total_Sales yang perlu ditangani dalam analisis lanjutan.

Dashboard interaktif dapat dikembangkan lebih lanjut menggunakan Tableau atau Power BI.

📌 Proyek ini diselesaikan sebagai bagian dari portofolio analisis data.

