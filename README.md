# Final_Project_UAS_AI_Davi-Sulaiman

Predictive Maintenance of Aircraft Engine Using GRU

Pendahuluan
Proyek ini bertujuan untuk mengembangkan model pemeliharaan prediktif untuk mesin pesawat menggunakan model Gated Recurrent Unit (GRU). Dengan menggunakan dataset operasi mesin, model ini diharapkan dapat memprediksi kegagalan mesin dan memperpanjang waktu operasi tanpa gangguan.

Deskripsi Proyek
Proyek ini terdiri dari beberapa tahapan utama, mulai dari pengolahan data hingga pengembangan dan evaluasi model GRU. Berikut ini adalah langkah-langkah yang diikuti dalam proyek ini.

1. Pesiapan dan Pengolahan Data
 - Import Pustaka yang Dibutuhkan: Menggunakan pustaka seperti pandas, numpy, scikit-learn, keras, dan lain-lain untuk pengolahan data dan pengembangan model.
Baca Dataset: Dataset pelatihan, pengujian, dan data kebenaran diambil dari sumber yang sudah ada.
- Hitung RUL (Remaining Useful Life): Menghitung sisa umur mesin untuk setiap mesin dalam dataset.
- Definisikan Jendela untuk Label: Membuat label klasifikasi biner dan tiga kelas untuk memudahkan pelatihan model.
- Normalisasi Data: Normalisasi fitur untuk menjaga skala data yang sebanding.
- Gabungkan Data Uji dan Kebenaran: Menggabungkan data uji dengan data kebenaran untuk menghitung RUL pada data uji.
- Plot Data Sensor: Visualisasi data sensor untuk analisis eksplorasi.
Matriks Korelasi: Menghitung dan memvisualisasikan matriks korelasi untuk memahami hubungan antar fitur.
 
2. Pembentukan Model
- Persiapan Data untuk Model: Membuat fungsi untuk membentuk data menjadi urutan dengan panjang tetap.
- Bentuk Data untuk Pelatihan: Mengonversi data menjadi urutan dan label untuk pelatihan model.
- Bangun Model GRU: Membangun model GRU dengan lapisan yang sesuai untuk memproses data sekuensial.

3. Pelatihan dan Evaluasi Model
- Pelatihan Model: Melatih model dengan data pelatihan.
- Evaluasi Model: Mengevaluasi kinerja model pada data pelatihan.
- Uji Model: Menggunakan data uji untuk mengevaluasi model dan memastikan kinerjanya dalam memprediksi kegagalan mesin.

Persyaratan
Sebelum menjalankan kode, pastikan Anda telah menginstal beberapa pustaka Python yang diperlukan, seperti pandas, numpy, scikit-learn, tensorflow, keras, dan matplotlib. Anda dapat menginstal pustaka tersebut menggunakan pip:
pip install pandas numpy scikit-learn tensorflow keras matplotlib

Struktur Direktori
├── data
│   ├── PM_train.csv
│   ├── PM_test.csv
│   └── PM_truth.csv
├── notebooks
│   └── G1A022001_DAVI SULAIMAN_UAS_AI.ipynb
└── README.md
 
Langkah-Langkah menjalankan kode
- Pastikan semua file dan direktori sesuai dengan struktur yang telah diberikan.
- Jalankan kode dalam notebook predictive_maintenance.ipynb untuk memulai proses pelatihan dan evaluasi model.

Kesimpulan
Proyek ini berhasil mengembangkan model GRU untuk prediksi pemeliharaan pesawat berdasarkan data sensor. Dengan mengikuti langkah-langkah yang dijelaskan, Anda dapat mereplikasi eksperimen ini dan memahami proses pengembangan model GRU untuk pemeliharaan prediktif mesin pesawat. Model ini diharapkan dapat meningkatkan efisiensi dan keandalan operasional dengan mengurangi waktu henti dan biaya pemeliharaan.
