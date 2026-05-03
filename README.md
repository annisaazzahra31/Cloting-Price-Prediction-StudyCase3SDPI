# Cloting-Price-Prediction-StudyCase3SDPI

## Overview
Project ini bertujuan untuk membangun model machine learning yang mampu memprediksi harga pakaian berdasarkan berbagai fitur seperti brand, kategori, kondisi, dan atribut lainnya.

Permasalahan ini diformulasikan sebagai **regression problem**, di mana target yang diprediksi adalah nilai harga (price).

---

## Tujuan
- Menganalisis faktor-faktor yang mempengaruhi harga pakaian  
- Melakukan preprocessing data untuk meningkatkan kualitas data  
- Membangun dan membandingkan beberapa model machine learning  
- Mengevaluasi performa model untuk mendapatkan hasil terbaik  

---

## Objectives
- Menganalisis faktor-faktor yang mempengaruhi harga pakaian
- Melakukan preprocessing data untuk meningkatkan kualitas input
- Membangun dan membandingkan beberapa model machine learning
- Mengevaluasi performa model untuk mendapatkan hasil terbaik

---

## Dataset
Dataset yang digunakan berisi informasi terkait produk pakaian, seperti:
- Brand
- Category / Type
- Condition
- Size / Color (jika ada)
- Price (target)

> - jumlah data : 1000 baris dan 6 kolom
> - tidak ada missing value ataupun duplikasi pada data
> - distribusi harga

---

## Exploratory Data Analysis (EDA)

### Distribusi Harga
- Distribusi harga cenderung tidak normal (skewed)  
- Terdapat outlier pada harga tinggi  

### Missing Values
- Beberapa data memiliki nilai kosong dan telah ditangani  

### Analisis Fitur
- Brand dan kategori berpengaruh terhadap harga  
- Kondisi produk mempengaruhi nilai harga  

### Insight Awal
- Data memerlukan encoding untuk fitur kategorikal  
- Transformasi diperlukan untuk mengatasi skewness  

---

## Data Preprocessing
- Handling missing values  
- Encoding fitur kategorikal  
- Feature transformation  
- Scaling data  

---

## Pemodelan

Model yang digunakan dalam proyek ini:
- **Ridge Regression**
- **XGBoost Regressor**

Ridge Regression digunakan sebagai model baseline dengan pendekatan linear, sedangkan XGBoost digunakan untuk menangkap hubungan non-linear yang lebih kompleks pada data.

---

## Evaluasi Model

Metrik evaluasi yang digunakan:
- Mean Absolute Error (MAE)  
- Root Mean Squared Error (RMSE)  
- R² Score  

---

## Result

Model terbaik: **Ridge Regression**

Hasil evaluasi:
- Ridge Regression
MAE: 46.32
RMSE: 54.13
R²: 0.0017

- XGBoost Regression
MAE: 47.74
RMSE: 56.42
R²: -0.0861 

Perbandingan menunjukkan bahwa model terbaik mampu menangkap pola data dengan lebih baik dibandingkan model lainnya.

---

## 📉 Visualisasi
- Distribusi Data Target (Price)
- Rata-Rata Harga per Brand  
- Rata-Rata Harga per Kategori
- Rata-Rata Harga berdasarkan Size Pakaian
- Rata-Rata Harga berdasarkan Material Pakaian
- Pengaruh Kombinasi Brand dan Material terhadap Harga
- Grafik Perbandingan Hasil

---

## 🚀 How to Run

1. Clone repository ini:
```bash
git clone https://github.com/annisaazzahra31/Cloting-Price-Prediction-StudyCase3SDPI.git
