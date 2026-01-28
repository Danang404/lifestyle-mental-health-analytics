<div align="center">

# 🧠 Student Mental Health Prediction with Big Data
### Analisis Risiko Depresi Mahasiswa Menggunakan Apache Spark

![Python](https://img.shields.io/badge/Python-3.8%2B-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Apache Spark](https://img.shields.io/badge/Apache%20Spark-PySpark-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white)
![Hadoop](https://img.shields.io/badge/Hadoop-HDFS-66CCFF?style=for-the-badge&logo=apachehadoop&logoColor=black)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

<p align="center">
  <a href="#-latar-belakang">Latar Belakang</a> •
  <a href="#-fitur-utama">Fitur Utama</a> •
  <a href="#-teknologi">Teknologi</a> •
  <a href="#-hasil-analisis">Hasil Analisis</a> •
</div>

---

## 📖 Latar Belakang

Kesehatan mental mahasiswa adalah isu krusial yang sering kali luput dari perhatian. Proyek ini bertujuan untuk membangun sistem **Big Data Analytics** yang mampu memprediksi risiko depresi pada mahasiswa berdasarkan pola gaya hidup dan aktivitas akademik mereka.

Menggunakan **Student Lifestyle Dataset** (100.000 data) dan framework **PySpark**, proyek ini mensimulasikan pemrosesan data berskala besar mulai dari penyimpanan di HDFS hingga pemodelan Machine Learning.

## 🚀 Fitur Utama

Proyek ini dirancang untuk memenuhi karakteristik **Big Data 5V** dan standar industri:

* ✅ **Big Data Processing:** Mengelola dataset 100k baris dengan Apache Spark.
* ✅ **Distributed Storage:** Integrasi penyimpanan data menggunakan HDFS.
* ✅ **MapReduce:** Implementasi algoritma MapReduce menggunakan RDD untuk agregasi data.
* ✅ **Advanced Analytics:** Analisis statistik menggunakan Spark SQL.
* ✅ **Machine Learning Pipeline:** Komparasi algoritma **Random Forest vs Logistic Regression** untuk klasifikasi.
* ✅ **Hyperparameter Tuning:** Optimasi model menggunakan Cross-Validation.

## 🛠 Teknologi & Tools

| Kategori | Teknologi | Deskripsi |
| :--- | :--- | :--- |
| **Language** | 🐍 Python | Bahasa pemrograman utama. |
| **Framework** | 🔥 PySpark | Pemrosesan Big Data & MLlib. |
| **Storage** | 🐘 Hadoop HDFS | Sistem file terdistribusi. |
| **Visualization**| 📊 Matplotlib/Seaborn | Eksplorasi Data (EDA). |
| **Dataset** | 📄 CSV | Student Lifestyle Dataset (100k Rows). |

## 📊 Pipeline Project

Berikut adalah alur kerja (*workflow*) yang diterapkan dalam proyek ini:

1.  **Data Ingestion:** Upload data CSV ke Hadoop Distributed File System (HDFS).
2.  **Preprocessing:** * Cleaning Data (Handling Missing Values & Anomalies).
    * Feature Engineering (Vector Assembler, String Indexer).
3.  **Exploratory Data Analysis (EDA):** Visualisasi korelasi antar fitur (Stress Level, Sleep, GPA).
4.  **Modeling:** Training model menggunakan Spark MLlib.
5.  **Evaluation:** Mengukur performa dengan F1-Score & Accuracy.

## 📈 Hasil Analisis & Evaluasi

Berdasarkan eksperimen, berikut adalah perbandingan performa model:

| Model | Akurasi | F1-Score | Keterangan |
| :--- | :--- | :--- | :--- |
| **Logistic Regression** | ~89.7% | Low | Cenderung bias ke kelas mayoritas. |
| **Random Forest** | **~89.6%** | **High** | **Lebih stabil menangani data imbalance.** |

> **Insight:** Faktor *Tingkat Stres (Stress Level)* dan *Durasi Tidur (Sleep Duration)* ditemukan sebagai prediktor terkuat terhadap risiko depresi mahasiswa.
