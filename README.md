# Submission 1 : Proyek Pengembangan Machine Learning Pipeline

Nama : Farhan Al Farizy </br>
Username dicoding : Belguga

| | Deskripsi |
| ----------- | ----------- |
| Dataset | [Fakenews-dataset](https://www.kaggle.com/datasets/iamrahulthorat/fakenews-csv) |
| Masalah | Proyek Fake News Detection ini berkaitan dengan penyebaran informasi yang tidak benar atau menyesatkan yang seringkali menjadi masalah dalam lingkungan media sosial dan platform online lainnya. Isu ini memiliki dampak yang signifikan, termasuk mempengaruhi opini publik, keamanan informasi, dan stabilitas sosial. |
| Solusi machine learning | Model ini akan membantu user dalam mendeteksi berita palsu dengan lebih akurat. Ini memberikan perlindungan kepada user dari informasi yang menyesatkan atau tidak benar, sehingga mereka dapat membuat keputusan yang lebih cerdas dan terinformasi. Stakeholder juga akan mendapatkan manfaat dalam hal pengambilan keputusan yang lebih baik. Dengan informasi yang lebih akurat dan terpercaya, mereka dapat membuat keputusan yang lebih tepat dan strategis dalam berbagai bidang, termasuk politik, bisnis, dan sosial.|
| Metode pengolahan | Dalam dataset fakenews-prediction, terdapat dua fitur utama, yaitu fitur teks (text) yang merupakan konten dari berita, dan fitur label (label) yang menunjukkan kategori berita sebagai berita benar atau berita palsu. Data kemudian dibagi menjadi dua set, yaitu data training dan data evaluasi, dengan rasio 80:20. Sebelum proses pelatihan, data teks diubah menjadi huruf kecil (lowercase) untuk konsistensi, sementara fitur label diubah menjadi bentuk integer untuk memfasilitasi proses klasifikasi oleh model machine learning.|
| Arsitektur model | Dalam arsitektur model ini, terdapat beberapa lapisan kunci yang digunakan untuk memproses data teks. Pertama, terdapat lapisan Vectorization untuk mengubah teks menjadi bentuk numerik yang dapat dipahami oleh model. Selanjutnya, ada lapisan Embedding dengan dimensi embedding 16 untuk memetakan kata-kata ke dalam vektor numerik. Dilanjutkan dengan lapisan AveragePooling1D untuk menyatukan informasi dari vektor-vektor tersebut. Kemudian, terdapat dua lapisan Dense dengan aktivasi ReLU dan sigmoid untuk melakukan klasifikasi antara dua label. Loss yang digunakan adalah binary_crossentropy dengan optimizer Adam, dan metrik yang dipantau adalah BinaryAccuracy. bersifat biner. |
| Metrik evaluasi | Metrik evaluasi yang digunakan yaitu ExampleCount, AUC, FalsePositives, TruePositives, FalseNegatives, TrueNegatives, dan BinaryAccuracy. |
| Performa model | Evaluasi model diperoleh yaitu AUC sebesar 76.6%, kemudian example_count 952, dengan BinaryAccuracy 71.7%, dan loss sebesar 2.021. Untuk False Negatives 15.66%, False Positive 12.61%, True Negative 46.43% dan True Positive 25.30%. Model yang telah dibuat dapat dilakukan peningkatan performa, karena model belum cukup baik karena BinaryAccuracy masih dibawah 80%. |


