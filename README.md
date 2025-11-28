# Organik dan Anorganik Detection

## 📋 Deskripsi Project
Proyek ini bertujuan untuk mendeteksi dan mengklasifikasikan sampah menjadi kategori **Organik** dan **Anorganik** menggunakan algoritma YOLOv8. Aplikasi ini menyediakan antarmuka berbasis web menggunakan Streamlit serta skrip Python standalone untuk deteksi real-time maupun gambar statis.

## ✨ Fitur
- **Deteksi Real-time**: Deteksi sampah organik dan anorganik melalui webcam secara langsung.
- **Mode Upload**: Analisis gambar yang diunggah melalui antarmuka web.
- **Switch Kamera**: Kemampuan beralih antara kamera default dan eksternal.
- **Fleksibel**: Bisa dijalankan via Web App (Streamlit) atau Script Python biasa.

## 🛠️ Teknologi
- **Python 3.8+**
- **YOLOv8** (Ultralytics)
- **Streamlit** (Web Framework)
- **OpenCV** (Image Processing)

## 🚀 Cara Menggunakan

### 1. Instalasi
Pastikan Python sudah terinstal, lalu install library yang dibutuhkan:
```bash
pip install -r requirements.txt
```

### 2. Menjalankan Aplikasi (Rekomendasi)
Gunakan antarmuka grafis (GUI) berbasis web untuk kemudahan penggunaan:
```bash
streamlit run app.py
```
_Aplikasi akan terbuka otomatis di browser Anda._

### 3. Menjalankan Skrip Manual (Alternatif)
Jika Anda ingin menjalankan tanpa antarmuka web:

**Deteksi Gambar:**
Edit path gambar di `Image_detection.py` lalu jalankan:
```bash
python Image_detection.py
```

**Deteksi Real-time (Window OpenCV):**
```bash
python realtime.py
```

## 📂 Struktur Project
```
project/
├── app.py              # Aplikasi utama (Streamlit)
├── Image_detection.py  # Skrip deteksi gambar statis
├── realtime.py         # Skrip deteksi webcam window
├── Training/           # Folder hasil training
│   └── weights/
│        └── best.pt    # Model YOLOv8 terlatih
├── data.yaml           # Konfigurasi dataset
└── requirements.txt    # Daftar dependensi
```

*Dataset provided by Roboflow (License: CC BY 4.)