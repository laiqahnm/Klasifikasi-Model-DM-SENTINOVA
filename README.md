# Klasifikasi-Model-DM-SENTINOVA

Proyek ini merupakan implementasi **model klasifikasi sentimen** yang dibangun menggunakan **RapidMiner** dan kemudian diekspor ke dalam bentuk `.pkl` untuk digunakan dan dievaluasi lebih lanjut di Python. Model ini dikembangkan untuk memprediksi apakah ulasan pelanggan bersentimen **Positive** atau **Negative**.

Model klasifikasi ini dilatih menggunakan dataset ulasan pelanggan yang sudah dilabeli sentimen dengan perbandingan 4 model klasifikasi, hasil evaluasi yang paling baik ditunjukkan pada model **Naive Bayes**. Proses pengembangan terbagi dalam dua tahap:

1. **RapidMiner** — digunakan untuk:
   - Preprocessing teks (tokenizing, filtering, stemming, dll.)
   - Pelatihan model klasifikasi (menggunakan 4 perbandingan model: Naive Bayes, Gradient Boosted Tree, Random Forest, Logistic Regression)
   - Evaluasi awal performa model
   - Mengambil hasil evaluasi model terbaik

2. **Python (Jupyter/Colab)** — digunakan untuk:
   - Membangun ulang model dan pipeline tf idf + naive bayes (model terbaik dari hasil proses RapidMiner)
   - Menyimpan model dalam format `.pkl`
   - Menjalankan dan menampilkan hasil prediksi, confidence, dan evaluasi
   - Visualisasi dan laporan akhir
