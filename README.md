# Prediksi Risiko Kredit ( Project Base Intership: Homecredit Indonesia x Rakamin Academy)

## Latar Belakang
**CLIENT BACKGROUD** \
Home Credit Indonesia adalah perusahaan pembiayaan yang berupaya memberikan solusi keuangan yang mudah bagi masyarakat Indonesia melalui berbagai produk dan layanan berbasis teknologi. Dengan menggunakan data-data yang telah disedikan diharapkan dapat memastikan nasabah yang mampu melakukan pelunasan tidak ditolak ketika melakukan pengajuan pinjaman.

**PROBLEM** 
1. Resiko gagal bayar cukup tinggi dalam pemberian kredit kepada nasabah.
2. Diperlukan sebuah sistem prediktif yang mampu membantu memberikan keputusan mengenai pemberian pinjaman kepada nasabah

**TUJUAN** 
1. Mengembangkan model prediksi risiko gagal bayar menggunakan algoritma machine learning untuk mengidentifikasi calon nasabah yang berisiko gagal bayar.
2. Mengidentifikasi model terbaik untuk prediksi berdasarkan metrik evaluasi.
3. Memberikan insight bisnis terkait karakteristik nasabah dengan risiko kredit tinggi untuk mendukung proses screening dan mitigasi risiko.

**WORKFLOW** \
<img width="600" alt="Image" src="https://github.com/user-attachments/assets/f22f2c3f-1fa8-458d-8cf5-69f031d8985c" />

## EDA
<img width="500" alt="Image" src="https://github.com/user-attachments/assets/5f47b074-a9bb-4179-88a0-dcde117c491a" /> \
Nasabah wanita lebih berisiko gagal bayar

<img width="500" alt="Image" src="https://github.com/user-attachments/assets/abd549ce-bac5-40a9-9855-3b346ae4d9e5" /> \
Nasabah dengan tingkat pendidikan terakhir secondary/secondary special lebih berisiko gagal bayar

<img width="500" alt="Image" src="https://github.com/user-attachments/assets/5bbf31f9-94c9-4a92-bffe-71d5fce4dcdd" /> \
Terlihat bahwa dataset imbalance karena dataset berisi lebih banyak nasabah yang tidak berisiko gagal bayar (Target = 0) dibandingkan dengan nasabah yang berisiko gagal bayar (Target =1). Kedepannya akan dilakukan penanganan lebih lanjut terkait hal tersebut.

<img width="500" alt="Image" src="https://github.com/user-attachments/assets/34a8d5b7-e503-4f5c-8f4e-d96f3936f4d4" /> \
Heatmap di atas menjelaskan bahwa adanya korelasi antar fitur yang kedepannya dapat digunakan untuk memprediksi nasabah yang gagal bayar.

## Machine Learning Implementation
Ada 3 Model Machine Learning yang digunakan untuk memprediksi nasabah gagal bayar
1. Logistic Regression
2. Random Forest
3. XGBoost

<img width="600" alt="Image" src="https://github.com/user-attachments/assets/8570363c-b250-409f-aaf1-aba426b3178d" /> \
**INSIGHT**
1. Mayoritas nasabah tidak berisiko gagal bayar
2. Logistic Regression merupakan model paling baik digunakan untuk memprediksi nasabah karena memiliki recall paling tinggi (~0.61) dan ROC-AUC paling tinggi (~0.63)

## Rekomendasi
1. Update Model secara berkala (Setiap 3–6 Bulan) Untuk memastikan akurasi dan relevansi model credit scoring terhadap data terkini. Proses ini melibatkan retraining model dengan data terbaru agar mampu menyesuaikan diri terhadap perubahan perilaku finansial nasabah dan dinamika pasar.
2. Lakukan implementasi kebijakan penilaian kredit yang mempertimbangkan faktor usia sebagai salah satu variabel penting dalam menentukan tingkat risiko peminjam. Pendekatan ini membantu perusahaan dalam menyusun strategi penyaluran kredit yang lebih tepat sasaran, khususnya untuk membedakan antara profil risiko generasi muda dan kelompok usia yang lebih senior.
3. Terapkan pendekatan segmentasi risiko yang mempertimbangkan latar belakang pendidikan peminjam. Dengan mengelompokkan calon nasabah berdasarkan tingkat pendidikan, perusahaan dapat memperoleh insight yang lebih dalam terhadap potensi risiko kredit, serta menyesuaikan kebijakan penilaian dan strategi mitigasi secara lebih efektif.

