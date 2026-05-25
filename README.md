# Deep Learning-Based Plant Disease Identification Using Convolutional Neural Networks

## Deskripsi Proyek
Proyek ini bertujuan untuk mengembangkan sistem identifikasi penyakit daun tanaman berbasis *Deep Learning* menggunakan *Convolutional Neural Network* (**CNN**). Fokus utama proyek adalah klasifikasi penyakit daun tomat menggunakan *PlantVillage Dataset*.

Dalam proyek ini dilakukan perbandingan antara model *baseline CNN* sederhana dengan pendekatan *transfer learning* menggunakan *MobileNetV2* untuk mengevaluasi performa klasifikasi penyakit tanaman. Selain itu, dilakukan analisis performa model menggunakan beberapa metrik evaluasi seperti *accuracy*, *F1-score*, *classification report*, dan *confusion matrix*.

Proyek ini disusun sebagai proyek pengganti UAS mata kuliah Kecerdasan Buatan, Departemen Teknik Komputer, Universitas Indonesia.

---

# Anggota Kelompok 5 (Rabu)

| Nama | NPM |
|---|---|
| Nabiel Harits Utomo | 2306267044 |
| Muhammad Pavel | 2306242363 |
| R. Aisha Syauqi Ramadhani | 2306250554 |
| Zhafira Zahra Alfarisy | 2306250636 |

---

# Latar Belakang
Penyakit daun tanaman tomat merupakan salah satu faktor yang dapat menurunkan **kualitas** dan **hasil panen** secara signifikan apabila tidak terdeteksi sejak dini. Proses identifikasi penyakit secara manual membutuhkan waktu, ketelitian, dan **pengetahuan khusus** sehingga kurang efisien apabila dilakukan dalam skala besar.

Perkembangan *Deep Learning*, khususnya *Convolutional Neural Network* (**CNN**), menunjukkan performa yang baik dalam tugas **klasifikasi citra** dan berpotensi membantu proses **identifikasi penyakit tanaman secara otomatis** melalui citra daun digital. Oleh karena itu, penelitian ini mengembangkan sistem klasifikasi penyakit daun tomat menggunakan pendekatan *baseline CNN* dan *transfer learning MobileNetV2* pada *PlantVillage Dataset*.

---

# Tujuan Proyek

Tujuan dari proyek ini adalah:

- Mengembangkan model klasifikasi citra berbasis CNN untuk identifikasi penyakit daun tomat
- Mengimplementasikan *baseline CNN* dan *MobileNetV2* untuk klasifikasi penyakit tanaman
- Mengevaluasi performa model menggunakan *accuracy*, *F1-score*, dan *confusion matrix*
- Membandingkan performa *baseline CNN* dengan metode *transfer learning MobileNetV2*

---

# Dataset

## Nama Dataset
**PlantVillage Dataset (Tomato Disease)**

## Sumber Dataset
Kaggle

## Link Dataset
https://www.kaggle.com/datasets/emmarex/plantdisease

## Kelas yang Digunakan
Proyek ini menggunakan subset penyakit daun tomat berikut:
- Tomato Healthy
- Tomato Early Blight
- Tomato Late Blight
- Tomato Leaf Mold
- Tomato Septoria Leaf Spot

## Karakteristik Dataset
- Dataset berbasis citra RGB
- Total dataset: **7.223 citra**
- Jumlah kelas: **5 kelas**
- Dataset telah terorganisir dalam struktur folder klasifikasi
- Ukuran input gambar: **224×224 piksel**

---

# Metodologi Proyek

## 1. Data Preprocessing
Tahapan preprocessing meliputi:
- Resize gambar menjadi 224×224
- Normalisasi piksel (`rescale = 1./255`)
- Data augmentation
- Pembagian data training dan validation

Data augmentation yang digunakan:
- Rotation
- Zoom
- Horizontal Flip

---

## 2. Baseline CNN
Model *baseline CNN* terdiri dari:
- Convolution Layer
- Fungsi aktivasi ReLU
- MaxPooling Layer
- Dense Layer
- Dropout Regularization
- Softmax Output Layer

Model digunakan sebagai baseline awal untuk mengevaluasi performa klasifikasi citra penyakit daun tomat.

---

## 3. Transfer Learning
Selain *baseline CNN*, proyek ini juga menggunakan:
- *MobileNetV2 pretrained ImageNet*
- Fine-tuning pada beberapa layer terakhir
- Transfer learning untuk meningkatkan performa klasifikasi

---

## 4. Evaluasi Model
Performa model dievaluasi menggunakan:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix
- Training & Validation Loss Curve

---

# Teknologi dan Framework

| Teknologi | Kegunaan |
|---|---|
| Python | Bahasa pemrograman utama |
| TensorFlow / Keras | Framework Deep Learning |
| Google Colab | Lingkungan training model |
| Matplotlib | Visualisasi data |
| Scikit-learn | Evaluasi model |
| NumPy | Komputasi numerik |

---

# Struktur Repository

```text
CNN-Rabu-5/
│
├── README.md
├── requirements.txt
├── Tugas_UAS_AI_Kelompok5(ProgCheck).ipynb
├── Tugas_UAS_AI_Kelompok5RabuFINAL.ipynb
├── LaporanProgressReport_Kelompok5Rabu.pdf
├── LaporanAkhir_Kelompok5Rabu.pdf
├── MetadataProgressReport_Kelompok5Rabu.json
├── MetadataLaporanAkhir_Kelompok5Rabu.json
├── PPTAkhir_Kelompok5Rabu.pptx
```

---

# Progress Awal (Senin, 18 Mei 2026)

## Selesai
- Penentuan topik proyek
- Persiapan dataset
- Setup Google Drive untuk dataset
- Pembuatan repository GitHub
- Studi literatur terkait CNN dan klasifikasi penyakit tanaman
- Persiapan preprocessing data

## Sedang Dikerjakan
- Implementasi baseline CNN
- Pipeline preprocessing data
- Training awal model

## Rencana Selanjutnya
- Implementasi transfer learning
- Hyperparameter tuning
- Evaluasi model
- Penyusunan laporan akhir

## Hasil Awal
- Dataset PlantVillage berhasil dipersiapkan dan diorganisir untuk proses training.
- Pipeline preprocessing berhasil diimplementasikan menggunakan TensorFlow/Keras.
- Struktur repository dan notebook eksperimen berhasil disusun.

## Analisis Awal
Tahap awal proyek berfokus pada persiapan lingkungan eksperimen dan pengelolaan dataset. Pada tahap ini belum dilakukan evaluasi performa model, namun preprocessing dan struktur pipeline berhasil disiapkan sebagai dasar implementasi baseline CNN dan transfer learning.

---

# Progress Pengembangan (Selasa, 19 Mei 2026)

## Selesai
- Penyusunan laporan Bab 1 hingga Bab 4
- Perbaikan struktur README GitHub
- Penyusunan arsitektur *Baseline CNN* dan *MobileNetV2*

## Sedang Dikerjakan
- Implementasi baseline CNN
- Pipeline preprocessing data
- Training awal model

## Rencana Selanjutnya
- Implementasi transfer learning
- Hyperparameter tuning
- Evaluasi model
- Penyempurnaan laporan akhir

## Hasil Pengembangan
- Arsitektur baseline CNN berhasil diimplementasikan.
- Struktur transfer learning MobileNetV2 berhasil dipersiapkan.
- Proses training awal baseline CNN mulai menunjukkan peningkatan accuracy.

## Analisis Pengembangan
Tahap pengembangan menunjukkan bahwa model CNN mulai mampu mempelajari pola visual penyakit daun tomat. Selain itu, implementasi MobileNetV2 dipersiapkan untuk meningkatkan performa klasifikasi melalui pendekatan transfer learning berbasis pretrained ImageNet.

---

# Progress Lanjutan (Sabtu, 23 Mei 2026)

## Selesai
- Penyempurnaan Bab 1 hingga Bab 5 laporan final
- Implementasi baseline CNN
- Implementasi transfer learning MobileNetV2
- Implementasi confusion matrix dan classification report
- Penyusunan Error Analysis dan evaluasi model
- Sinkronisasi metadata proyek dengan Bab 4 laporan
- Penyusunan outline dan desain presentasi final proyek

## Sedang Dikerjakan
- Penyempurnaan visualisasi hasil eksperimen
- Finalisasi notebook eksperimen
- Finalisasi evaluasi model
- Persiapan presentasi akhir

## Rencana Selanjutnya
- Menambahkan data *test set* terpisah untuk evaluasi akhir model
- Penyempurnaan fine-tuning MobileNetV2
- Penyempurnaan confusion matrix dan evaluasi akhir
- Persiapan demo presentasi final

## Hasil Lanjutan
- Baseline CNN berhasil mencapai *training accuracy* sebesar **88,74%**.
- Validation accuracy baseline CNN mencapai sekitar **91–92%**.
- Implementasi confusion matrix berhasil menunjukkan performa klasifikasi tiap kelas.
- MobileNetV2 mulai menunjukkan performa yang lebih stabil dibanding baseline CNN.

## Analisis Lanjutan
Hasil eksperimen menunjukkan bahwa baseline CNN sudah mampu melakukan klasifikasi penyakit daun tomat dengan cukup baik. Selain itu, penggunaan transfer learning MobileNetV2 membantu meningkatkan stabilitas proses training dan kemampuan feature extraction model. Error analysis juga menunjukkan bahwa kesalahan klasifikasi paling sering terjadi pada kelas dengan karakteristik visual yang mirip seperti *Early Blight* dan *Late Blight*.

---

# Final Progress (25/05/2026)

## Selesai
- Finalisasi notebook eksperimen CNN dan MobileNetV2
- Implementasi evaluasi model menggunakan:
  - Accuracy
  - Precision
  - Recall
  - F1-score
  - Confusion Matrix
- Penyusunan bagian Hyperparameter Tuning
- Penyusunan Error Analysis
- Penyempurnaan visualisasi accuracy/loss history
- Penyempurnaan laporan final Bab 1–Bab 5
- Sinkronisasi laporan, notebook, metadata.json, dan PPT final
- Penyusunan slide presentasi final

## Hasil Final

### Baseline CNN
- Validation Accuracy: **≈91.8%**
- Training Accuracy: **88.74%**

### MobileNetV2 Fine-tuned
- Validation Accuracy: **≈92.24%**
- Weighted F1-score: **≈0.9201**
- Macro F1-score: **≈0.9075**

## Analisis Final
- *MobileNetV2* menunjukkan performa yang lebih stabil dibanding baseline CNN.
- Transfer learning membantu model mempelajari fitur visual penyakit daun secara lebih efektif.
- Model memiliki performa terbaik pada kelas *Healthy*.
- Kesalahan klasifikasi paling sering terjadi pada kelas dengan karakteristik visual yang mirip seperti *Early Blight* dan *Late Blight*.
- Grafik accuracy dan loss menunjukkan proses training yang stabil dengan indikasi overfitting yang masih dapat dikendalikan menggunakan *dropout* dan *data augmentation*.

## Finalisasi yang Masih Dilakukan
- Penyempurnaan formatting laporan akhir
- Final checking notebook dan PDF
- Persiapan presentasi dan simulasi demo

---

# Hasil Akhir Proyek

## Performa Model
Proyek berhasil mengimplementasikan sistem klasifikasi penyakit daun tomat menggunakan pendekatan *Deep Learning* berbasis CNN dan transfer learning MobileNetV2. Berdasarkan hasil eksperimen, MobileNetV2 Fine-tuned memberikan performa terbaik dengan validation accuracy sekitar **92.24%** dan weighted F1-score sekitar **0.9201**.

## Analisis Akhir
Hasil eksperimen menunjukkan bahwa pendekatan transfer learning mampu meningkatkan performa klasifikasi dibanding baseline CNN. Selain itu, preprocessing data, data augmentation, dan fine-tuning MobileNetV2 membantu model mempelajari pola visual penyakit daun secara lebih efektif. Meskipun demikian, proyek masih memiliki keterbatasan berupa belum adanya *test set* terpisah sehingga evaluasi model masih berfokus pada validation set.
---

# Referensi
- PlantVillage Dataset (Kaggle)
- Dokumentasi TensorFlow/Keras
- Materi CNN Mata Kuliah Kecerdasan Buatan
- Literatur Deep Learning terkait klasifikasi penyakit tanaman

