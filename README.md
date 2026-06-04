# Identifikasi Jenis Kayu Menggunakan GLCM dan Euclidean Distance

## Deskripsi Proyek

Proyek ini merupakan aplikasi berbasis web yang digunakan untuk mengidentifikasi jenis kayu berdasarkan tekstur citra permukaan kayu. Sistem memanfaatkan metode Gray Level Co-occurrence Matrix (GLCM) untuk ekstraksi fitur tekstur dan metode Euclidean Distance untuk menentukan kemiripan antara citra uji dengan data latih.

Aplikasi ini dirancang sebagai implementasi pengolahan citra digital untuk membantu proses identifikasi jenis kayu secara otomatis berdasarkan karakteristik teksturnya.

---

## Tujuan

- Mengimplementasikan metode GLCM untuk ekstraksi fitur tekstur citra kayu.
- Mengimplementasikan metode Euclidean Distance untuk menghitung tingkat kemiripan antar citra.
- Membangun aplikasi berbasis web yang mampu melakukan identifikasi jenis kayu secara otomatis.

---

## Metode yang Digunakan

### 1. Preprocessing

Gambar kayu yang diunggah akan dikonversi menjadi citra grayscale untuk mempermudah proses ekstraksi fitur tekstur.

### 2. Ekstraksi Fitur GLCM

Fitur tekstur yang digunakan meliputi:

- Contrast
- Correlation
- Energy
- Homogeneity

Fitur-fitur tersebut digunakan sebagai representasi karakteristik tekstur dari setiap jenis kayu.

### 3. Perhitungan Euclidean Distance

Fitur hasil ekstraksi dari citra uji dibandingkan dengan fitur pada data latih menggunakan metode Euclidean Distance.

Citra dengan nilai jarak terkecil dianggap memiliki tingkat kemiripan tertinggi dan digunakan sebagai hasil identifikasi.

---

## Teknologi yang Digunakan

- Python
- Flask
- OpenCV
- NumPy
- Scikit-Image
- HTML
- CSS
- Bootstrap

---

## Struktur Proyek

```text
kelompok2_identifikasi_kayu/
│
├── dataset/
├── static/
├── templates/
├── uploads/
├── app.py
├── feature_extraction.py
├── requirements.txt
└── README.md
```

## Cara Menjalankan

### 1. Clone Repository

```bash
git clone https://github.com/hafidz-155/kelompok2_identifikasi_kayu.git
```

### 2. Masuk ke Folder Project

```bash
cd kelompok2_identifikasi_kayu
```

### 3. Install Dependency

```bash
pip install -r requirements.txt
```

### 4. Jalankan Aplikasi

```bash
python app.py
```

### 5. Buka Browser

```text
http://localhost:5000
```

---

## Cara Penggunaan

1. Jalankan aplikasi.
2. Upload gambar kayu yang akan diuji.
3. Sistem melakukan preprocessing citra.
4. Sistem mengekstraksi fitur tekstur menggunakan GLCM.
5. Sistem menghitung jarak menggunakan Euclidean Distance.
6. Jenis kayu dengan jarak terdekat ditampilkan sebagai hasil identifikasi.

---

## Mata Kuliah

Pengantar Citra Digital

---

## Institusi

Institut Teknologi Nasional Bandung (ITENAS)

---

## Pengembang

Kelompok 2

Tahun Akademik 2025/2026