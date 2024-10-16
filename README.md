# Perbandingan Metode KNN dan Naive Bayes dalam Memprediksi Kualitas Udara di Jakarta Tahun 2021 
--------

# DESKRIPSI 
Proyek ini membandingkan dua metode klasifikasi, yaitu K-Nearest Neighbors (KNN) dan Naive Bayes, untuk memprediksi kualitas udara di beberapa wilayah Jakarta pada tahun 2021. Penelitian ini difokuskan pada analisis data yang dikumpulkan dari Stasiun Pemantauan Kualitas Udara (SPKU) di lima lokasi: Bundaran HI, Kelapa Gading, Jagakarsa, Lubang Buaya, dan Kebon Jeruk. Kinerja kedua model dievaluasi berdasarkan empat metrik utama: accuracy, precision, recall, dan f1-score. Hasil menunjukkan bahwa metode KNN memiliki performa lebih baik dengan akurasi 97%, sementara Naive Bayes mencapai akurasi 96%.

# TUJUAN 
- Memprediksi kualitas udara di lima lokasi di Jakarta berdasarkan data SPKU tahun 2021.
- Membandingkan performa dua metode klasifikasi untuk menangani dataset ini, yaitu KNN dan Naive Bayes. 
- Menilai efektivitas kedua metode berdasarkan empat indikator pengukuran, yaitu akurasi, presisi, recall, dan f1-score.
- Mengidentifikasi model terbaik untuk memprediksi kualitas udara yang telah terbagi ke dalam tiga kategori utama, yaitu Baik, Sedang, dan Tidak Sehat.

# ALUR KERJA 
1. Pengumpulan Data:

   - Data yang digunakan dalam proyek ini berasal dari data kualitas udara di Jakarta, yang terdiri dari 1820 baris dengan variabel PM10, PM25, SO2, CO, O3, NO2, dan Max.
2. Pre-Processing Data:
   - Pembersihan Data: Menghapus data yang hilang dan menangani outlier dalam dataset.
   - Transformasi Data: Mengonversi variabel "kategori" menjadi nilai numerik untuk memudahkan proses klasifikasi. Dimana, nilai 0 menunjukkan "Tidak Sehat", nilai 1 menunjukkan "Sedang", dan nilai 2 menunjukkan "Baik" 
3. Exploratory Data Analysis (EDA):
   - Melakukan visualisasi dan analisis korelasi antar variabel, serta menampilkan distribusi outlier dalam data menggunakan boxplot dan heatmap korelasi.
4. Pemodelan dengan KNN dan Naive Bayes:

   - KNN: Pemodelan menggunakan algoritma KNN dengan pemilihan parameter terbaik melalui grid search. Nilai parameter k terbaik untuk KNN adalah 7.
   - Naive Bayes: Menggunakan Naive Bayes dengan tuning parameter var_smoothing melalui grid search, dengan parameter terbaik adalah 0.01.
   
   Melakukan pemodelan baik dengan dan tanpa outlier untuk mengevaluasi pengaruh outlier pada performa model.
5. Evaluasi Model:

   - Model dievaluasi berdasarkan accuracy, precision, recall, dan f1-score untuk data training dan testing.
   - Perbandingan model dilakukan untuk memilih model terbaik antara KNN dan Naive Bayes.
  
# KESIMPULAN 
Dari hasil perbandingan, model KNN dengan k = 7 terbukti menjadi model terbaik dalam memprediksi kualitas udara di Jakarta dengan akurasi 97%, precision 96%, recall 96%, dan f1-score 96%. Model Naive Bayes juga memberikan hasil yang baik, namun sedikit lebih rendah dengan akurasi 96%, precision 93%, recall 94%, dan f1-score 93%. Berdasarkan hasil tersebut, KNN lebih direkomendasikan untuk dataset ini.
  
# TIM 
- Sherryl Kurniawan
- Angelica
- Gabriel Matthew Mintana 
