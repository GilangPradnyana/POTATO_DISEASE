# Klasifikasi Penyakit Daun Kentang (Potato Disease Classification)

Model Convolutional Neural Network (CNN) berbasis TensorFlow/Keras untuk mengklasifikasikan kondisi daun kentang ke dalam tiga kategori:  **Early Blight**, **Late Blight**, dan **Healthy**.

##  Deskripsi Project

Project ini bertujuan membantu petani dan pekerja pertanian dalam mengidentifikasi penyakit daun kentang secara cepat menggunakan deep learning. Dengan mengunggah gambar daun kentang, model dapat memprediksi jenis penyakit beserta tingkat keyakinannya (confidence score).

### Kelas yang Tersedia
- `Potato___Early_blight` (Bercak Daun Awal)
- `Potato___Late_blight` (Bercak Daun Akhir)
- `Potato___healthy` (Sehat)

##  Fitur

- Klasifikasi gambar penyakit daun kentang
- Arsitektur CNN menggunakan TensorFlow/Keras
- Pipeline data dengan `tf.keras.preprocessing.image_dataset_from_directory`
- Evaluasi model dan visualisasi prediksi
- Siap untuk dideploy (Gradio / Streamlit / Flask)

##  Teknologi yang Digunakan

- **Bahasa**: Python
- **Deep Learning**: TensorFlow & Keras
- **Pemrosesan Gambar**: TensorFlow Image Dataset API
- **Visualisasi**: Matplotlib
- **Notebook**: Jupyter Notebook

##  Dataset

Dataset yang digunakan terdiri dari **2152 gambar** daun kentang yang terbagi ke dalam 3 kelas:
dataset/

├── Potato___Early_blight/

├── Potato___Late_blight/

└── Potato___healthy/


**Spesifikasi Dataset:**
- Jumlah total gambar : 2152
- Ukuran gambar       : 256 × 256 piksel
- Batch size          : 32
- Channel warna       : 3 (RGB)
- Format data         : Folder-based (menggunakan `image_dataset_from_directory`)

---

## Teknologi yang Digunakan

| Komponen              | Teknologi                  |
|-----------------------|----------------------------|
| Bahasa Pemrograman    | Python                     |
| Framework Deep Learning | TensorFlow & Keras       |
| Processing Data       | TensorFlow Dataset API     |
| Visualisasi           | Matplotlib                 |
| Environment           | Jupyter Notebook           |

---

## Arsitektur Model

Model yang digunakan adalah **Convolutional Neural Network (CNN)** dengan konfigurasi dasar sebagai berikut:

- Input size: `(256, 256, 3)`
- Beberapa layer Convolution + MaxPooling
- Flatten layer
- Dense layer
- Output layer dengan 3 class (softmax)

## Hasil dan Evaluasi
Setelah proses training, model dapat melakukan prediksi terhadap gambar daun kentang dengan menampilkan:

- Kelas aktual
- Kelas prediksi
- Nilai confidence (tingkat keyakinan)
- Visualisasi hasil prediksi ditampilkan dalam bentuk grid gambar beserta labelnya.

## Kesimpulan
Project ini berhasil membangun model CNN untuk mengklasifikasikan penyakit daun kentang menjadi tiga kategori. Model mampu memberikan prediksi beserta tingkat keyakinan, sehingga berpotensi untuk dikembangkan menjadi sistem deteksi penyakit tanaman berbasis AI.
