# Klasifikasi Penyakit Daun Kentang (Potato Disease Classification)

Model Convolutional Neural Network (CNN) yang dibangun menggunakan TensorFlow/Keras untuk mengklasifikasikan penyakit daun kentang menjadi tiga kategori: **Early Blight**, **Late Blight**, dan **Healthy**.

## 📋 Deskripsi Project

Project ini bertujuan membantu petani dan pekerja pertanian dalam mengidentifikasi penyakit daun kentang secara cepat menggunakan deep learning. Dengan mengunggah gambar daun kentang, model dapat memprediksi jenis penyakit beserta tingkat keyakinannya (confidence score).

### Kelas yang Tersedia
- `Potato___Early_blight` (Bercak Daun Awal)
- `Potato___Late_blight` (Bercak Daun Akhir)
- `Potato___healthy` (Sehat)

## 🚀 Fitur

- Klasifikasi gambar penyakit daun kentang
- Arsitektur CNN menggunakan TensorFlow/Keras
- Pipeline data dengan `tf.keras.preprocessing.image_dataset_from_directory`
- Evaluasi model dan visualisasi prediksi
- Siap untuk dideploy (Gradio / Streamlit / Flask)

## 🛠️ Teknologi yang Digunakan

- **Bahasa**: Python
- **Deep Learning**: TensorFlow & Keras
- **Pemrosesan Gambar**: TensorFlow Image Dataset API
- **Visualisasi**: Matplotlib
- **Notebook**: Jupyter Notebook

## 📁 Dataset

Dataset terdiri dari gambar daun kentang yang dikelompokkan ke dalam 3 folder:
