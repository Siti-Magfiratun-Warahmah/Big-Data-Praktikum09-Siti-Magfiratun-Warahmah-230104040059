# PRAKTIKUM 9 – Smart City Traffic Monitoring & Prediction (Spark + Parquet + Streamlit)

**Proyek:** BIGDATA-PRAKTIKUM09-230104040059

Program ini dibuat untuk memenuhi instruksi **Praktikum 9 Mata Kuliah Teknologi Big Data**. Praktikum ini berfokus pada pembangunan sistem **monitoring dan prediksi kepadatan kendaraan** menggunakan Apache Spark (PySpark), penyimpanan Parquet, serta visualisasi dashboard interaktif dengan Streamlit.

Sistem ini merupakan pengembangan dari praktikum sebelumnya dengan fokus pada **batch processing, analisis data, serta prediksi berbasis Machine Learning**.

---

# 👩‍🎓 Identitas Mahasiswa

| Keterangan     | Informasi                        |
| -------------- | -------------------------------- |
| Mata Kuliah    | Teknologi Big Data               |
| Dosen Pengampu | Muhayat, S.Ag., M.IT             |
| Praktikum      | Praktikum 9 – Traffic Monitoring |
| Nama Mahasiswa | Siti Magfiratun Warahmah         |
| NIM            | 230104040059                     |
| Kelas          | TI23B                            |

---

# 🚀 Deskripsi Program

Program ini merupakan implementasi sistem **monitoring dan prediksi kepadatan kendaraan** berbasis Big Data.

Sistem bekerja dengan cara:

* Menghasilkan data simulasi kendaraan (timestamp, lokasi, jumlah kendaraan)
* Memproses data menggunakan Apache Spark
* Melakukan agregasi berdasarkan lokasi dan waktu
* Menyimpan data dalam format **Parquet**
* Menampilkan data dalam dashboard interaktif menggunakan Streamlit
* Melakukan prediksi jumlah kendaraan menggunakan **Linear Regression**

Sistem ini menggambarkan konsep **Smart City** dalam pengelolaan lalu lintas berbasis data.

---

# 🏗️ Arsitektur Pipeline

```
Data Generation
   ↓
Spark Transformation
   ↓
Parquet Columnar Storage
   ↓
ML Modeling (Linear Regression)
   ↓
Serving (Streamlit Dashboard)
```

Penjelasan alur:

1. Data kendaraan dibuat secara simulasi.
2. Spark digunakan untuk melakukan transformasi dan agregasi data.
3. Data disimpan dalam format **Parquet** untuk efisiensi.
4. Model Machine Learning digunakan untuk prediksi jumlah kendaraan.
5. Dashboard menampilkan data dan hasil prediksi secara interaktif.

---

# 🛠️ Teknologi yang Digunakan

* Python 3
* Apache Spark (PySpark)
* Pandas
* Streamlit
* Plotly
* Scikit-learn (Linear Regression)
* WSL (Linux)
* VS Code

---

# 📂 Struktur Folder Project

```
bigdata-praktikum09-230104040059
│
├── main_uts_230104040059.py
├── dashboard_230104040059.py
├── output/
│   ├── traffic/
│   ├── traffic_time/
│   └── ml_data/
│
├── venv/
├── .gitignore
└── README.md
```

---

# ⚙️ Cara Menjalankan Program

## 1️⃣ Aktifkan Virtual Environment

```
source venv/bin/activate
```

---

## 2️⃣ Jalankan Engine (Spark)

```
python3 main_uts_230104040059.py
```

Output:

* Data Parquet akan tersimpan di folder `output/`

---

## 3️⃣ Jalankan Dashboard

```
streamlit run dashboard_230104040059.py
```

---

# 🌐 Akses Dashboard

Buka di browser:

```
http://localhost:8501
```

---

# 📊 Output Sistem

Sistem menghasilkan:

* Total kendaraan (semua lokasi)
* Total kendaraan per lokasi (AreaA, AreaB, AreaC)
* Grafik tren kendaraan berdasarkan waktu
* Prediksi jumlah kendaraan berdasarkan jam

Contoh hasil:

* Total kendaraan: **17.294**
* AreaB: **5.939**
* Prediksi jam 08.00: **58 kendaraan**

---

# 📸 Output Wajib

* Script Python:

  * main_uts_NIM.py
  * dashboard_NIM.py
* Screenshot:

  * Terminal saat Parquet berhasil disimpan
  * Dashboard Streamlit (full tampilan)

---

# 📈 Analisis

Berdasarkan hasil dashboard, kepadatan kendaraan mengalami peningkatan pada pagi hari dan mencapai puncaknya pada sekitar pukul **08.00–08.10**. Hal ini menunjukkan bahwa waktu tersebut merupakan **jam tersibuk (peak hour)**, terutama pada AreaB dan AreaC. Model prediksi juga menunjukkan hasil yang konsisten dengan kondisi tersebut.

---

# 🎯 Kesimpulan

Praktikum ini berhasil membangun sistem monitoring dan prediksi kepadatan kendaraan berbasis Big Data menggunakan Apache Spark, Parquet, dan Streamlit. Sistem mampu mengolah data secara efisien, menampilkan visualisasi interaktif, serta melakukan prediksi menggunakan Linear Regression.

Hasil analisis menunjukkan bahwa puncak kepadatan kendaraan terjadi pada pagi hari, sehingga sistem ini dapat digunakan sebagai dasar dalam pengembangan Smart City berbasis data.

---

# 📦 Repository

```
https://github.com/Siti-Magfiratun-Warahmah/Big-Data-Praktikum09-Siti-Magfiratun-Warahmah-230104040059
```
