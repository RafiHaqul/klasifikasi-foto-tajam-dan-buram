# Implementasi algoritma canny dan laplacian untuk klasifikasi gambar buram dan gambar tajam

Saya bereksperimen membuat program untuk *klasifikasi gambar buran dan gambar tajam* mengunakan 2 algoritma yaitu `canny` dan `laplacian`.
Program ini berjalan meggunakan notebook python versi 3.

Dataset : https://www.kaggle.com/datasets/kwentar/blur-dataset

Pada experimen proggram yang menggunakan algoritma canny bahwa algoritma ini memiliki parameter threshold yang dapat diatur untuk memnentukan tingkat sensitifitas klasifikasi.
Lalu saya mencoba mencari nilai optimal untuk mencapai akurasi terbaik pada dataset tersebut dengan cara melakukan perulangan perbandingan data prediksi dengan data truth hinga mencapai treshold yang sesuai.

**Kelemahan** program ini ketika memproses gambar selain dataset (seperti gambar atau foto pribadi) yaitu
- **Gambar dengan efek bokeh** jika nilai threshold kurang dari batas threshold yang ditetapkan akan diklasifikasi sebagai gambar buram.
- **gambar gelap atau pencahayaan minim** algoritma pendeteksi tepi sangat kesulitan dengan gambar gelap jika parameter min dan max thershold menggunakan setingan optimal dari dataset blur dari kaggle sebelumnya pada canny.
