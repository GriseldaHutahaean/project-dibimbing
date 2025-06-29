# ProjectDibimbing_Python_EDA
## Project Portfolio: Python Basics and Exploratory Data Analysis on Social Media Addiction
---

### Deskripsi Tugas

Proyek ini merupakan tugas portofolio dari program pelatihan **Dibimbing.id**, yang mencakup dua komponen utama:

1. **Dasar Pemrograman Python**  
   Membuat skrip interaktif menggunakan dasar-dasar Python seperti input pengguna, tipe data, dan logika kondisi.

2. **Exploratory Data Analysis (EDA)**  
   Melakukan analisis data eksploratif pada dataset *Students Social Media Addiction* yang diperoleh dari Kaggle.

---

### Deskripsi Pengerjaan

Tugas dikerjakan secara individual dengan menggunakan Google Colab sebagai platform analisis. Dataset diunduh dari Kaggle dan diproses menggunakan library Python seperti Pandas, Matplotlib, dan Seaborn.  
Proyek ini terdiri dari dua file utama:  
- Notebook Python dasar (`intro_to_python_.py`)  
- Notebook EDA (`EDA-socialmediaaddiction.ipynb`)

---

### Dataset

Dataset berisi informasi terkait perilaku mahasiswa dalam menggunakan media sosial, dengan fitur-fitur seperti:

- Usia
- Jenis kelamin
- Durasi penggunaan media sosial per hari
- Skor kecanduan media sosial
- Nilai akademik dan variabel dukungan lainnya

Sumber dataset:  
🔗 [https://www.kaggle.com/datasets/pratyushpuri/students-social-media-addiction]

---

### Komponen Proyek

#### 1. Dasar Python

- Menginput nama mahasiswa, NIM, dan nilai ujian
- Menampilkan tipe data dari setiap input
- Mengklasifikasikan nilai ke dalam kategori:
    A (Sangat Baik): 85–100
    B (Baik): 75–84
    C (Cukup): 60–74
    D (Kurang): 40–59
    E (Sangat Kurang): < 40

📄 File      : `intro_to_python_.py`

🔗 gcollab   : [https://colab.research.google.com/drive/1_DPAZc0r0psWe1PiKWE3mvya3hIWOwQP?usp=sharing]

#### 2. EDA: Kecanduan Media Sosial

- Pembersihan data dan penanganan nilai hilang
- Visualisasi data menggunakan histogram, boxplot, dan bar chart
- Eksplorasi korelasi antar variabel (durasi penggunaan vs skor kecanduan)
- Analisis pola berdasarkan usia dan jenis kelamin

📄 File: `EDA-socialmediaaddiction.ipynb`  
📂 Data: `Students Social Media Addiction.csv`

---

### Metodologi EDA

1. **Membaca Dataset**  
   Dataset dibaca menggunakan `pd.read_csv()` dan ditampilkan 5 data pertama dengan `cel.head()`.

2. **Memahami Struktur Dataset**  
   Menggunakan `cel.columns`, `cel.shape`, dan `cel.info()` untuk melihat struktur dan tipe data.  
   Dataset terdiri dari 12 kolom dan 100 baris.

3. **Pemeriksaan Nilai Hilang**  
   Diperiksa dengan `cel.isnull().sum()`  
   **Hasil:** Tidak ada nilai kosong (missing value) yang ditemukan.

4. **Analisis Statistik Deskriptif**  
   Menggunakan `cel.describe()` untuk melihat nilai minimum, maksimum, rata-rata, dan distribusi dari kolom numerik.

5. **Analisis Univariate (Satu Variabel)**  
   Histogram untuk:  `Time spent on social media`, `Addiction score`,
                     `Daily usage`  

   Countplot untuk `Gender`

7. **Analisis Bivariate (Dua Variabel)**  
     Boxplot: `Gender vs Addiction Score`  
     Scatterplot:  
      1. `Daily usage vs Addiction Score`  
      2. Time spent on social media vs Addiction Score`

8. **Validasi Duplikat**  
   Data dicek menggunakan `cel.duplicated()`  
   **Hasil:** Tidak ditemukan data duplikat.
---

### Tools dan Library

- Python (Google Colab)
- Pandas
- Matplotlib
- Seaborn
- File CSV (dataset)

---

###  Temuan Utama

- Mahasiswa usia 15–25 tahun cenderung memiliki skor kecanduan media sosial yang lebih tinggi
- Rata-rata skor kecanduan sedikit lebih tinggi pada perempuan
- Durasi penggunaan media sosial per hari berkorelasi positif dengan tingkat kecanduan

---

### 🗂️ Struktur Repositori

project-dibimbing

├── intro_to_python.py

├── EDA-socialmediaaddiction.ipynb

├── Students Social Media Addiction.csv

└── README.md

---

### Rencana Pengembangan

- Menambahkan model prediksi untuk mengklasifikasi tingkat kecanduan
- Membangun dashboard interaktif menggunakan Streamlit
- Melakukan analisis tambahan seperti segmentasi usia & rekomendasi digital wellbeing

---

### Penulis

**Griselda Tabitha Nathania Hutahaean**  
Portofolio Proyek – Dibimbing.id  
GitHub: [@GriseldaHutahaean](https://github.com/GriseldaHutahaean)
