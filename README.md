# 📊 Customer Segmentation using K-Means Clustering

Proyek ini bertujuan untuk mengelompokkan pelanggan berdasarkan pola perilaku mereka, seperti rata-rata limit kredit, kunjungan ke bank atau layanan online, dan aktivitas panggilan, dengan menggunakan algoritma **K-Means Clustering**.

---

## 🔍 Project Overview

Dalam industri perbankan dan keuangan, memahami perilaku nasabah sangat penting untuk menyusun strategi pemasaran, layanan, dan pengambilan keputusan berbasis data. Dengan pendekatan unsupervised learning (K-Means Clustering), kita dapat mengelompokkan nasabah ke dalam beberapa segmen berdasarkan:

- `Avg_Credit_Limit` (Limit Kredit Rata-rata)  
- `Total_visits_online` (Kunjungan ke layanan online)  
- `Total_visits_bank`  
- `Total_calls_made`  
- `Total_credit_cards`

---

## 📁 Dataset Information

Dataset ini berisi **660 baris data pelanggan**, masing-masing dengan atribut berikut:

| Column Name           | Description                                  |
|-----------------------|----------------------------------------------|
| `Sl_No`               | Nomor urut data                              |
| `Customer Key`        | ID unik pelanggan                            |
| `Avg_Credit_Limit`    | Rata-rata batas kredit pelanggan             |
| `Total_Credit_Cards`  | Jumlah kartu kredit yang dimiliki            |
| `Total_visits_bank`   | Total kunjungan langsung ke bank             |
| `Total_visits_online` | Total kunjungan ke layanan digital/online    |
| `Total_calls_made`    | Jumlah panggilan yang dilakukan ke bank      |

---

## 🧪 Tools & Libraries Used

- Python  
- Pandas  
- NumPy  
- Matplotlib & Seaborn  
- Scikit-learn (StandardScaler, KMeans, Elbow Method)

---

## 🧭 Project Steps

1. **Data Understanding**  
   Menjelaskan isi dataset, statistik deskriptif, dan tipe data.
   
2. **Data Preprocessing**  
   - Menghapus kolom ID (`Sl_No`, `Customer Key`)  
   - Melakukan *Standard Scaling* agar data dalam skala yang sebanding

3. **Elbow Method**  
   Menganalisis jumlah cluster optimal menggunakan Within-Cluster-Sum-of-Squares (WCSS).

4. **K-Means Clustering**  
   Membangun model K-Means dengan jumlah cluster = 4.

5. **Visualization**  
   - Visualisasi hasil clustering dengan dua fitur utama:  
     `Avg_Credit_Limit` vs `Total_visits_online`

6. **Interpretation**  
   Analisis karakteristik masing-masing cluster.

---

## 📊 Cluster Interpretation

| Cluster | Ciri-ciri Utama |
|--------|-----------------|
| 0 | Limit kredit rendah, aktivitas digital minim |
| 1 | Limit kredit menengah-tinggi, kunjungan ke bank dan online moderat |
| 2 | Limit kredit rendah-menengah, aktif online |
| 3 | Limit kredit sangat tinggi, sangat aktif secara digital |

---

## 🚀 How to Run

1. Clone repo ini:
   ```bash
   git clone https://github.com/username/customer-segmentation-kmeans.git
   cd customer-segmentation-kmeans
