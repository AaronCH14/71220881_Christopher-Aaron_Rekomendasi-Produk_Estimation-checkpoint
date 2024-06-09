# 71220881_Christopher-Aaron_Rekomendasi-Produk_Estimation-checkpoint
https://drive.google.com/drive/folders/10aZ4h0CrRM0p1vyG_ukq_E5krj4RuCrm?usp=sharing (link ini adalah dataset yang digunakan dalam pembuatan model AI dikarenakan ukuran dataset yang terlalu besar maka saya lampirkan link ini)
file bisa diakses langsung atau menggunakan format zip




Berikut penjelasan mengenai cara kerja file ini dan algoritma yang digunakan:

Algoritma yang Digunakan: SVD
SVD adalah teknik dekomposisi matriks yang digunakan untuk memprediksi rating produk yang belum pernah dirating oleh pengguna berdasarkan pola rating dari pengguna lain. Algoritma ini mengurangi dimensi dari matriks rating untuk menemukan hubungan laten antara pengguna dan produk.

​1. Import Libraries dan Load Dataset
Notebook ini pertama-tama mengimpor pustaka yang diperlukan dan memuat dataset yang berisi informasi mengenai userID, productID, rating, dan timestamp dari file CSV.
2. Define Reader and Load Data
Menggunakan objek Reader untuk menginterpretasikan data dengan benar, dan fungsi Dataset.load_from_df untuk memuat data ke dalam format yang dapat digunakan oleh pustaka Surprise.
3. Split Data into Training and Test Sets
Data dibagi menjadi set pelatihan dan pengujian dengan proporsi 80% untuk pelatihan dan 20% untuk pengujian.
4. Train the SVD Algorithm
Algoritma SVD dilatih menggunakan data pelatihan.
5. Evaluate the Model
Kinerja model dievaluasi menggunakan Root Mean Square Error (RMSE) pada data pengujian.
6. Generate Recommendations
Fungsi get_top_n_recommendations didefinisikan untuk mendapatkan rekomendasi produk terbaik untuk setiap pengguna berdasarkan prediksi. Rekomendasi untuk pengguna contoh (userID=1) kemudian ditampilkan.

Dengan implementasi di atas, notebook ini membuat sistem rekomendasi yang dapat memberikan rekomendasi produk kepada pengguna berdasarkan riwayat rating mereka. 
