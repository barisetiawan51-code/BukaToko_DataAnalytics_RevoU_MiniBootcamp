# Analisis Data Log Aktivitas User pada Sebuah Platform E-commerce yaitu BukaToko

## Deskripsi Proyek
Proyek ini bertujuan untuk melakukan analisis perilaku pengguna pada platform e-commerce BukaToko, yang beroperasi di Asia Tenggara, US, dan Australia, dengan akses melalui web dan aplikasi mobile. Dataset mencatat seluruh perjalanan pengguna mulai dari browse produk, search barang, melihat detail produk, add to cart, hingga checkout, termasuk transaksi yang berhasil maupun yang gagal (drop-off).

Analisis ini memungkinkan:
* Pemahaman conversion funnel, yaitu jalur pembelian pengguna.
* Identifikasi drop-off points, yaitu tahap di mana pengguna meninggalkan proses belanja.
* Evaluasi efektivitas channel pemasaran, termasuk organic search, paid ads, email campaigns, social media, dan referral/direct visits.

## Dataset
Dataset yang digunakan bersifat dirty dummy data fiktif, sehingga ideal untuk latihan data cleaning dan preprocessing. ataset memiliki beberapa tantangan:
* Missing values di beberapa kolom penting.
* Tipe data yang kurang tepat, misalnya kolom tanggal atau numerik yang tersimpan sebagai string.

## Kolom Utama
| Kolom | Deskripsi |
|-------|-----------|
| event_id | ID unik untuk setiap event/log |
| user_id  | ID unik pengguna |
| session_id | ID sesi pengguna |
| event_type | Jenis event (browse, search, add_to_cart, checkout, dll.) |
| event_timestamp | Waktu event terjadi |
| product_id | ID produk yang terkait dengan event |
| country | Negara pengguna |
| device | Perangkat yang digunakan (web/mobile) |
| channel | Channel pemasaran yang membawa pengguna ke plattform |

## Tujuan Analisis
* Membersihkan dan memvalidasi data agar siap digunakan untuk analisis lebih lanjut, termasuk menangani missing values dan transformasi tipe data.
* Menganalisis perilaku pengguna untuk memahami jalur konversi.
* Mengidentifikasi tahap kritis (drop-off points) dalam proses belanja.
* Menilai efektivitas berbagai channel pemasaran dalam mendatangkan dan mempertahankan pengguna.
* Memberikan insight actionable untuk meningkatkan konversi penjualan.

# Tools & Teknologi
Beberapa tools dan teknologi yang dapat digunakan dalam proyek ini:
* Python (pandas, numpy, matplotlib, seaborn, plotly)
* Jupyter Notebook / Google Colab untuk eksplorasi data dan visualisasi
* Data cleaning & preprocessing tools: missing value handling, data type conversion, deduplication
* Analisis perilaku pengguna: conversion funnel, cohort analysis, event frequency analysis

## Output yang Diharapkan
* Dataset yang bersih, valid, dan siap dianalisis, termasuk handling missing values dan transformasi tipe data.
* Visualisasi conversion funnel dan drop-off points
* Insight mengenai channel pemasaran paling efektif
* Rekomendasi untuk meningkatkan engagement dan konversi pengguna, antara lain:
  
  1. Indonesia merupakan pasar utama dengan aktivitas pengguna tertinggi; fokus strategi di negara ini dan pasar menengah seperti US, Filipina, Malaysia, Singapura, dan Vietnam.
  2. Mayoritas pengguna menggunakan smartphone, menekankan pentingnya optimalisasi pengalaman mobile.
  3. Email marketing masih menjadi channel paling efektif, sementara social media, referral, dan organic juga berkontribusi merata; strategi personalisasi per channel dianjurkan.
  4. Meski interaksi awal tinggi, konversi ke add to cart dan purchase masih rendah, menandakan potensi peningkatan user journey dari eksplorasi ke transaksi.
  5. Strategi rekomendasi: optimalisasi funnel konversi, peningkatan engagement di perangkat mobile, dan personalisasi strategi akuisisi per channel dan negara target utama.
