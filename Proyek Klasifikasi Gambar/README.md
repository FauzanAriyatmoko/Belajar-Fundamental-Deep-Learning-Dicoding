# Klasifikasi Tumor Otak Menggunakan Citra MRI

## Gambaran Proyek

Proyek ini bertujuan untuk mengembangkan model deep learning yang dapat mengklasifikasikan jenis tumor otak berdasarkan citra MRI. Dengan menggunakan data dari [Brain Tumor Classification MRI Dataset di Kaggle](https://www.kaggle.com/datasets/sartajbhuvaji/brain-tumor-classification-mri/data), model ini diharapkan dapat membantu dalam mendeteksi dan mengklasifikasikan tumor dengan lebih akurat. Proyek ini menggunakan jaringan saraf konvolusional (CNN) dan transfer learning untuk mendukung diagnostik otomatis, khususnya untuk daerah yang kekurangan tenaga medis spesialis.

### Motivasi Proyek
Tumor otak adalah masalah kesehatan yang serius, yang mencakup persentase besar dari tumor sistem saraf pusat (CNS). Karena sifatnya yang kompleks, deteksi dan klasifikasi tumor sering kali menjadi tantangan, bahkan bagi radiolog yang berpengalaman. Mengingat kekurangan spesialis di banyak wilayah, sistem klasifikasi otomatis dapat memberikan dukungan yang berharga, menyediakan diagnostik yang akurat, dan membantu dalam perencanaan perawatan pasien.

## Dataset

- **Sumber**: [Kaggle: Brain Tumor Classification MRI Dataset](https://www.kaggle.com/datasets/sartajbhuvaji/brain-tumor-classification-mri/data)
- **Abstrak**: Dataset ini menyediakan citra MRI yang telah diberi label dengan jenis tumor otak yang berbeda, termasuk tumor jinak, ganas, dan tumor hipofisis. Dataset ini menekankan pentingnya alat diagnostik yang lebih maju untuk meningkatkan hasil pengobatan pasien dengan tumor otak.
- **Skor Kegunaan**: 8.75
- **Lisensi**: MIT

### Struktur Data

- Dataset ini berisi citra MRI yang dilabeli sesuai jenis tumornya, memungkinkan model untuk mengklasifikasikan gambar berdasarkan kategori tumor.
- Citra-citra tersebut menunjukkan variasi yang signifikan dalam ukuran tumor, lokasi, dan karakteristik MRI.

## Struktur Proyek

- **CNN_Brain_Tumor_Classification.ipynb**: Notebook Jupyter utama yang berisi kode untuk pra-pemrosesan data, arsitektur model, pelatihan, dan evaluasi.
- **data/**: Direktori untuk menyimpan citra MRI yang diunduh untuk pelatihan dan pengujian.
- **models/**: Direktori untuk menyimpan bobot model yang telah dilatih dan file konfigurasi.
- **README.md**: Gambaran proyek, informasi dataset, dan instruksi penggunaan.

## Metodologi

1. **Pra-Pemrosesan Data**:
   - Mengubah ukuran citra agar konsisten untuk input model.
   - Teknik augmentasi data untuk meningkatkan ketahanan model.

2. **Arsitektur Model**:
   - Menggunakan model CNN yang dilatih dari awal atau transfer learning untuk mengklasifikasikan citra MRI berdasarkan jenis tumor.
   - Arsitektur dioptimalkan untuk akurasi tinggi dalam membedakan jenis tumor.

3. **Evaluasi**:
   - Kinerja model dievaluasi berdasarkan metrik akurasi, presisi, recall, dan skor F1.

## Instalasi

Untuk menjalankan proyek ini secara lokal, diperlukan library berikut:
- matplotlib==3.8.0
- mplcyberpunk==0.7.1
- numpy==2.1.2
- opencv_contrib_python==4.10.0.84
- opencv_python==4.10.0.84
- opencv_python_headless==4.10.0.84
- pandas==2.2.3
- Pillow==11.0.0
- protobuf==3.20.3
- scikit_learn==1.5.2
- seaborn==0.13.2
- tensorflow==2.17.0
- tqdm==4.66.6

