Saya mencoba berekksperimen membuat program untuk klasifikasi gambar buran dan gambar tajam mengunakan 2 algoritma yaitu canny dan laplacian.
Program ini meggunakan notebook python3 dan menggunakan blur dataset yang saya donload pada kaggle.

dataset : https://www.kaggle.com/datasets/kwentar/blur-dataset

Pada experimen algoritma canny sendiri memiliki parameter threshold. Lalu saya mencoba mencari nilai optimal untuk mencapai akurasi terbaik pada dataset tersebut.

Kelemahan program ini ketika memproses gambar selain dataset (seperti gambar atau foto pribadi) yaitu
- <b>Gambar dengan efek bokeh</b> jika nilai threshold kurang dari batas threshold yang ditetapkan akan diklasifikasi sebagai gambar buram
- <b>gambar gelap atau pencahayaan minim</b> algoritma pendeteksi tepi sangat kesulitan dengan gambar gelap jika parameter min dan max thershold menggunakan setingan optimal dari dataset blur dari kaggle sebelumnya pada canny
