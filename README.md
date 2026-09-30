# 🛒 Market Basket Analysis & Product Association Intelligence

> Proyek portofolio Data Science end-to-end yang mengimplementasikan Market Basket Analysis (MBA) menggunakan algoritma Apriori untuk menemukan pola pembelian pelanggan, mengoptimalkan strategi ritel, dan mendorong pengambilan keputusan bisnis berbasis data.

---

## 📊 Live Dashboard Preview
Jelajahi dashboard interaktif Looker Studio yang dibangun untuk proyek ini:
👉 [Lihat Dashboard Looker Studio](https://datastudio.google.com/reporting/4294e830-608e-4ed3-ba07-d7e1a1ba7b14)

---

## 🎯 Tujuan Proyek (Project Objective)
Proyek ini dirancang untuk menganalisis perilaku pembelian pelanggan melalui data transaksi. Tujuan utamanya adalah mengubah data transaksi mentah menjadi wawasan bisnis yang aplikatif dan rekomendasi strategis, meliputi:
* Cross-Selling: Merekomendasikan produk yang relevan saat checkout atau di keranjang belanja.
* Product Bundling: Mengelompokkan produk dengan afinitas tinggi ke dalam paket promosi khusus.
* Product Placement: Menempatkan barang secara strategis untuk meningkatkan Nilai Rata-rata Transaksi (Average Order Value / AOV).

---

## 🛠️ Tech Stack & Libraries
* Bahasa Pemrograman: Python
* Environment: Google Colab, Visual Studio Code
* Manipulasi & Pembersihan Data: Pandas, NumPy, SciPy (Penghapusan outlier Z-score)
* Machine Learning / Association Mining: mlxtend (Algoritma Apriori, Association Rules)
* Visualisasi Data & BI: Google Looker Studio, Matplotlib

---

## 📈 Penjelasan Metrik Utama
Market Basket Analysis mengevaluasi aturan asosiasi menggunakan tiga metrik inti:
1. Support: Mengukur seberapa sering suatu produk atau kombinasi produk muncul di seluruh transaksi.
2. Confidence: Mengukur peluang produk B dibeli jika produk A sudah dibeli.
3. Lift: Mengukur apakah pembelian produk A dan B terjadi lebih sering daripada ekspektasi acak. Nilai Lift > 1 menunjukkan korelasi positif.

---

## 📂 Struktur Proyek (Project Structure)
- assets/ (Tangkapan layar dashboard dan aset visual)
- market_basket_rules.csv (Dataset aturan asosiasi hasil olahan untuk BI)
- Market_Basket_Analysis.ipynb (Notebook Google Colab utama yang berisi kode end-to-end)
- README.md (Dokumentasi proyek)

---

## 🚀 Langkah & Metodologi Utama
1. Pemuatan & Pembersihan Data: Mengimpor data, menangani nilai hilang, menyeragamkan nama produk menjadi huruf kecil, serta menghapus pesanan yang dibatalkan dan outlier dengan Z-score.
2. Transformasi Keranjang: Membuat matriks keranjang (sparse matrix) dan memfilter transaksi dengan lebih dari 1 produk unik.
3. Penambangan Frequent Itemsets: Menerapkan algoritma Apriori dengan minimum support (0.01).
4. Pembangkitan Aturan Asosiasi: Menghasilkan aturan menggunakan metrik confidence (0.7).
5. Integrasi BI: Mengekspor aturan ke Looker Studio untuk membangun dashboard interaktif.

---

## 💡 Wawasan Bisnis & Rekomendasi Strategis
* Bundling Item Ber-Lift Tinggi: Menjadikan produk dengan skor Lift tinggi sebagai paket diskon khusus untuk mendongkrak volume penjualan.
* Cross-Selling Cerdas: Menerapkan rekomendasi otomatis "Pelanggan yang membeli ini juga membeli..." di e-commerce.
* Perencanaan Stok: Memantau produk dengan Support tertinggi untuk memastikan ketersediaan stok terlaris tetap terjaga.

---
## 👤 Penulis (Author)
* Elieser Pasaribu — Data Analyst / Data Scientist / Machine Learning
