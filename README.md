# Submission 1 : Proyek Pengembangan Machine Learning Pipeline
Nama : Farhan Al Farizy

Username dicoding : Belguga

| | Deskripsi |
| ----------- | ----------- |
| Dataset | [Fakenews-dataset](https://www.kaggle.com/datasets/iamrahulthorat/fakenews-csv) |
| Masalah | Fake News |
| Solusi machine learning | Sebuah model klasifikasi yang dapat membedakan antara berita yang benar (true news) dan berita palsu (fake news) berdasarkan fitur-fitur yang ada pada teks berita.|
| Metode pengolahan | Dalam dataset fakenews-prediction, terdapat dua fitur utama, yaitu fitur teks (text) yang merupakan konten dari berita, dan fitur label (label) yang menunjukkan kategori berita sebagai berita benar atau berita palsu. Data kemudian dibagi menjadi dua set, yaitu data training dan data evaluasi, dengan rasio 80:20. Sebelum proses pelatihan, data teks diubah menjadi huruf kecil (lowercase) untuk konsistensi, sementara fitur label diubah menjadi bentuk integer untuk memfasilitasi proses klasifikasi oleh model machine learning.|
| Arsitektur model | Dalam arsitektur model ini, terdapat beberapa lapisan kunci yang digunakan untuk memproses data teks. Pertama, terdapat lapisan Vectorization untuk mengubah teks menjadi bentuk numerik yang dapat dipahami oleh model. Selanjutnya, ada lapisan Embedding dengan dimensi embedding 16 untuk memetakan kata-kata ke dalam vektor numerik. Dilanjutkan dengan lapisan AveragePooling1D untuk menyatukan informasi dari vektor-vektor tersebut. Kemudian, terdapat dua lapisan Dense dengan aktivasi ReLU dan sigmoid untuk melakukan klasifikasi antara dua label. Loss yang digunakan adalah binary_crossentropy dengan optimizer Adam, dan metrik yang dipantau adalah BinaryAccuracy. bersifat biner. |
| Metrik evaluasi | Metrik evaluasi yang digunakan yaitu ExampleCount, AUC, FalsePositives, TruePositives, FalseNegatives, TrueNegatives, dan BinaryAccuracy. |
| Performa model | Evaluasi model diperoleh yaitu AUC sebesar 75.9%, kemudian example_count 952, dengan BinaryAccuracy 70.2%, dan loss sebesar 2.026. Untuk False Negatives 14.29%, False Positive 15.55%, True Negative 43.49% dan True Positive 26.68%. Model yang telah dibuat dapat dilakukan peningkatan performa, karena model belum cukup baik karena BinaryAccuracy masih dibawah 80%. |
