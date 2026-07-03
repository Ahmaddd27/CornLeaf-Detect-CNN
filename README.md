

Readme · MD
# 🌽 CornLeaf Detect
 
Aplikasi web untuk mendeteksi penyakit pada daun jagung menggunakan model **Convolutional Neural Network (CNN)** dengan pendekatan **Transfer Learning MobileNetV2**. Dibangun dengan **Streamlit** agar mudah diakses melalui browser.
 
## 📋 Deskripsi
 
CornLeaf Detect membantu mengidentifikasi jenis penyakit pada daun jagung hanya dari sebuah foto. Pengguna cukup mengunggah gambar daun jagung, dan sistem akan mengklasifikasikan kondisi daun tersebut menggunakan model CNN yang telah dilatih.
 
## ✨ Fitur
 
- Upload gambar daun jagung langsung dari perangkat
- Crop gambar interaktif sebelum diproses (via `streamlit-cropper`)
- Klasifikasi otomatis menggunakan model MobileNetV2 hasil transfer learning
- Antarmuka sederhana dan responsif berbasis Streamlit
## 🛠️ Teknologi yang Digunakan
 
| Teknologi | Kegunaan |
|---|---|
| Python | Bahasa pemrograman utama |
| TensorFlow / Keras | Membangun dan menjalankan model CNN (MobileNetV2) |
| Streamlit | Antarmuka web aplikasi |
| Streamlit-Cropper | Fitur crop gambar sebelum prediksi |
| NumPy & Pillow | Pra-pemrosesan gambar |
 
## 🚀 Cara Menjalankan Secara Lokal
 
1. **Clone repository**
```bash
   git clone https://github.com/Ahmaddd27/CornLeaf-Detect-CNN.git
   cd CornLeaf-Detect-CNN
```
 
2. **Buat virtual environment**
```bash
   python -m venv venv
   venv\Scripts\activate      # Windows
   source venv/bin/activate   # macOS/Linux
```
 
3. **Install dependencies**
```bash
   pip install -r requirements.txt
```
 
4. **Jalankan aplikasi**
```bash
   streamlit run app.py
```
 
5. Buka browser ke `http://localhost:8501`
## 📁 Struktur Project
 
```
CornLeaf-Detect-CNN/
├── app.py                              # File utama aplikasi Streamlit
├── model_jagung_mobilenetv2.keras      # Model CNN terlatih (MobileNetV2)
├── requirements.txt                    # Daftar dependency Python
├── static/
│   └── field_bg.jpg                    # Aset gambar latar belakang
└── README.md
```
 
## 🧠 Tentang Model
 
Model diklasifikasikan menggunakan arsitektur **MobileNetV2** dengan pendekatan **transfer learning**, yaitu memanfaatkan bobot model yang telah dilatih sebelumnya (pre-trained) pada dataset besar, kemudian di-*fine-tune* pada dataset citra daun jagung untuk mengenali kelas-kelas penyakit yang menjadi target klasifikasi.
 
## 👤 Author
 
**Ahmad** Teknik Informatika / Sistem Informasi
NIM: A11.2024.15653
 
---
 
*Project ini dibuat sebagai bagian dari tugas akademik.*
 
