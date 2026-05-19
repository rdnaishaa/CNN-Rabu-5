# Deep Learning-Based Plant Disease Identification Using Convolutional Neural Networks

## Deskripsi Proyek
Proyek ini bertujuan untuk mengembangkan sistem identifikasi penyakit daun tanaman berbasis Deep Learning menggunakan Convolutional Neural Network (CNN). Fokus utama proyek adalah klasifikasi penyakit daun tomat menggunakan dataset PlantVillage.

Dalam proyek ini, dilakukan perbandingan antara model baseline CNN sederhana dengan pendekatan transfer learning menggunakan MobileNetV2 untuk mengevaluasi performa klasifikasi penyakit tanaman.

Proyek ini disusun sebagai proyek pengganti UAS mata kuliah Kecerdasan Buatan, Departemen Teknik Komputer, Universitas Indonesia.

---

## Anggota Kelompok 5 (Rabu)

| Nama | NPM |
|---|---|
| Nabiel Harits Utomo | 2306267044 |
| Muhammad Pavel | 2306242363 |
| R. Aisha Syauqi Ramadhani | 2306250554 |
| Zhafira Zahra Alfarisy | 2306250636 |

---

## Latar Belakang
Penyakit tanaman merupakan salah satu faktor utama yang memengaruhi produktivitas dan kualitas hasil pertanian. Identifikasi penyakit secara manual sering kali memerlukan waktu, tenaga ahli, dan rentan terhadap kesalahan manusia.

Perkembangan Deep Learning, khususnya Convolutional Neural Network (CNN), menunjukkan performa yang sangat baik dalam berbagai tugas klasifikasi citra, termasuk deteksi penyakit tanaman.

Melalui proyek ini, dilakukan implementasi model CNN untuk membantu proses identifikasi penyakit daun tanaman secara otomatis berdasarkan citra gambar.

---

## Tujuan Proyek
Tujuan dari proyek ini adalah:

- Mengembangkan model klasifikasi citra berbasis CNN untuk identifikasi penyakit tanaman
- Mengevaluasi performa arsitektur CNN pada dataset penyakit daun tanaman
- Membandingkan performa baseline CNN dengan model transfer learning
- Menganalisis performa model menggunakan metrik evaluasi seperti accuracy dan confusion matrix

---

## Dataset

### Nama Dataset
PlantVillage Dataset

### Sumber Dataset
Kaggle

### Link Dataset
https://www.kaggle.com/datasets/emmarex/plantdisease

### Kelas yang Digunakan
Proyek ini menggunakan subset penyakit daun tomat berikut:

- Tomato Healthy
- Tomato Early Blight
- Tomato Late Blight
- Tomato Leaf Mold
- Tomato Septoria Leaf Spot

### Karakteristik Dataset
- Dataset berbasis citra RGB
- Terdiri dari beberapa kategori penyakit tanaman
- Struktur folder telah terorganisir untuk kebutuhan klasifikasi

---

## Metodologi Proyek

### 1. Data Preprocessing
Tahapan preprocessing meliputi:
- Resize gambar
- Normalisasi piksel
- Data augmentation
- Pembagian data training dan validation

### 2. Baseline CNN
Model baseline CNN yang digunakan terdiri dari:
- Convolution layer
- Fungsi aktivasi ReLU
- MaxPooling layer
- Dense layer
- Dropout regularization

### 3. Transfer Learning
Selain baseline CNN, proyek ini juga menggunakan:
- MobileNetV2 pretrained ImageNet

### 4. Evaluasi Model
Performa model akan dievaluasi menggunakan:
- Accuracy
- Loss curve
- F1-score
- Confusion matrix

---

## Teknologi dan Framework

| Teknologi | Kegunaan |
|---|---|
| Python | Bahasa pemrograman utama |
| TensorFlow / Keras | Framework Deep Learning |
| Google Colab | Lingkungan training model |
| Matplotlib | Visualisasi data |
| NumPy | Komputasi numerik |

---

## Struktur Repository

```text
CNN-Rabu-5/
│
├── README.md
├── requirements.txt
├── Tugas_UAS_AI_Kelompok5.ipynb
├── progress_report_kelompok5.pdf 
└── metadata/
    └── metadata.json
```

---

## Progress Saat Ini (Senin, 18 Mei 2026)

### Selesai
- Penentuan topik proyek
- Persiapan dataset
- Setup Google Drive untuk dataset
- Pembuatan repository GitHub
- Studi literatur terkait CNN dan klasifikasi penyakit tanaman
- Persiapan preprocessing data

### Sedang Dikerjakan
- Implementasi baseline CNN
- Pipeline preprocessing data
- Training awal model

### Rencana Selanjutnya
- Implementasi transfer learning
- Hyperparameter tuning
- Evaluasi model
- Penyusunan laporan akhir

---

## Hasil Sementara
Eksperimen saat ini berfokus pada:
- Validasi pipeline loading dataset
- Persiapan arsitektur baseline CNN
- Implementasi preprocessing awal

Hasil training dan evaluasi model akan ditambahkan pada progress berikutnya.

---

## Kendala
Beberapa kendala yang sedang dihadapi:
- Pengelolaan dataset citra berukuran besar pada GPU terbatas
- Risiko overfitting pada training CNN
- Optimasi waktu training di Google Colab
- Pemilihan arsitektur CNN yang optimal

---

## Hasil yang Diharapkan
Proyek ini diharapkan menghasilkan model CNN yang mampu mengklasifikasikan penyakit daun tomat dengan akurasi tinggi dan kemampuan generalisasi yang baik.

Selain itu, proyek ini diharapkan dapat menunjukkan efektivitas pendekatan Deep Learning dalam membantu identifikasi penyakit tanaman secara otomatis.

---

## Referensi

- PlantVillage Dataset (Kaggle)
- Dokumentasi TensorFlow
- Materi CNN Mata Kuliah Kecerdasan Buatan
- Literatur Deep Learning terkait klasifikasi penyakit tanaman
