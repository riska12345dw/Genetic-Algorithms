# Algoritma Genetika untuk Optimasi Klasifikasi Penyakit Kanker Payudara
## Kelompok 4
- Almas Digya W (5311421005)
- Riska Dwi Astia Ningrum (5311421007)
- Dimas Dwiki R (5311421015)
- Hilmy Kurnia A (5311421044)

#### Latar Belakang
Optimasi klasifikasi kanker payudara dengan algoritma genetika membawa inovasi signifikan di bidang kesehatan, khususnya dalam deteksi dini penyakit yang memerlukan perhatian khusus. Algoritma genetika mengatasi kompleksitas dataset kanker payudara dengan memilih subset fitur-fitur paling informatif, meningkatkan keakuratan model prediktif. Pemilihan fitur yang tepat juga meningkatkan pemahaman terhadap faktor-faktor yang memengaruhi perkembangan kanker payudara. Melalui pengoptimalan model menggunakan algoritma genetika, diharapkan dapat memajukan pendekatan prediktif yang canggih dan akurat dalam deteksi dini kanker payudara, membuka peluang untuk perbaikan prognosis pasien dan pengembangan strategi intervensi yang lebih efektif.


#### Genetic Algorithms
Algoritma genetika termasuk dalam algoritma evolusi yang paling populer dalam hal keragaman aplikasinya. Sebagian besar masalah optimasi terkenal telah diuji menggunakan algoritma genetika. Algoritma genetika bersifat berbasis populasi, dan banyak algoritma evolusi modern secara langsung berdasarkan algoritma genetika atau memiliki beberapa kemiripan yang kuat.
Algoritma genetika telah dikenal sejak tahun 1960-an dan masih luas digunakan hingga saat ini. Algoritma genetika adalah algoritma berbasis populasi yang menggunakan seleksi, crossover, dan mutasi untuk membentuk populasi baru yang lebih baik.  Istilah lain yang digunakan dalam algoritma genetika: gen, kromosom, populasi, fungsi kecocokan.
![alt text](https://github.com/AlmasDiqya22/Genetic-Algorithms/assets/148710085/288c5ab1-07be-46bc-b8e0-b7e958fc1fe6)

#### Langkah
- Dari bentuk kromosom x yang merepresentasikan solusi dari masalah yang dibahas.
- Menentukan fungsi kecocokan f(x) yang akan digunakan untuk menghitung nilai suatu kromosom.
- Hasil populasi awal yang terdiri dari n kromosom.
- Menentukan probabilitas crossover (pc), probabilitas mutasi (pm), dan jumlah generasi (g).
- Lakukan seleksi untuk memilih dua kromosom dari populasi.
- Membuat kromosom baru dengan melakukan crossover pada dua kromosom yang dipilih. Crossover merupakan prosedur utama untuk menciptakan kromosom baru.
- Membuat kromosom baru melalui mutasi. Mutasi digunakan untuk keluar dari minimum lokal.
- Mengulangi langkah 5-7 untuk menghasilkan lebih banyak kromosom baru.
- Menggabungkan semua kromosom dari populasi awal dan kromosom yang dihasilkan melalui crossover dan mutasi.
- Menghitung fungsi kecocokan untuk semua kromosom, urutkan kromosom berdasarkan fungsi kecocokan, dan lakukan eliminasi. Eliminasi digunakan untuk memilih n kromosom terbaik sebagai populasi baru.
- Mengulangi langkah 5-10.


##### Kanker Payudara
Kanker payudara merupakanjenis kanker yang terjadi ketika sel-sel di dalam jaringan payudara mengalami pertumbuhan yang tidak terkendali. Pertumbuhan sel yang tidak normal ini dapat membentuk massa atau benjolan yang disebut tumor. Tumor ini bisa menjadi ganas (kanker) atau jinak (tidak kanker).

##### Data Kanker Payudara
Dataset mengenai Kanker Payudara (Breast Cancer) yang bersumber daeri Kaggle, berisi dataset mengenai informasi diagnosis tumor payudara, yang terdiri dari 569 data dan 30 fitur numerik. Dataset ini dikumpulkan dari gambar mikroskopis sel-sel payudara yang diambil dari pasien dengan diagnosis tumor jinak dan ganas.
Dataset kanker payudara (breast cancer) untuk mengklasifikasikan pasien dengan kanker payudara menjadi dua kategori, yaitu pasien dengan kanker payudara jinak (benign = B) dan pasien dengan kanker payudara ganas (malignant = M) yang berdasarkan berdasarkan fitur-fitur data klinis yang telah dikumpulkan dari dataset. Fitur-fitur ini dapat termasuk usia pasien, ukuran tumor, karakter sel, dan hasil tes diagnostik lainnya. 


#### Analisis

![alt text](https://github.com/AlmasDiqya22/Genetic-Algorithms/assets/148710085/118dba4f-18ea-46fd-a03f-11fefbe1d6a4)

  Perhitungan akurasi model menggunakan fungsi 'acc_score' yang telah definisikan sebelumnya.
  DataFrame yang berisi akurasi dari berbagai model klasifikasi yang diterapkan pada dataset kanker payudara menggunakan algoritma genetika. DataFrame ini disusun dalam urutan menurun berdasarkan akurasi, dan dapat memberikan informasi tentang model mana yang memberikan hasil terbaik.


![alt text](https://github.com/AlmasDiqya22/Genetic-Algorithms/assets/148710085/8cb84e2d-b672-4120-b5f5-4c1239a11dd6)

  Menggunakan model RandomForestClassifier dengan konfigurasi tertentu dan menjalankan algoritma genetika untuk mengoptimalkan model tersebut. Kemudian berisi kromosom terbaik dari setiap generasi dan daftar skor kecocokan (score_bc) dari setiap generasi.
  - Pada generasi pertama, akurasi terbaik yang dicapai oleh model adalah sekitar 98.60%.
  - Pada generasi kedua, akurasi terbaik tetap sekitar 98.60%. Tidak terjadi peningkatan pada generasi ini.
  - Pada generasi ketiga, hasil akurasi terbaik masih sekitar 98.60%, tidak ada perubahan signifikan.
  - Pada generasi keempat, terjadi peningkatan signifikan dalam akurasi, mencapai sekitar 99.30%.
  - Pada generasi kelima, akurasi kembali ke sekitar 98.60%, tidak ada peningkatan dibandingkan dengan generasi keempat.


#### Hasil Plot Grafik

![alt text](https://github.com/AlmasDiqya22/Genetic-Algorithms/assets/148710085/43f8a5c3-1144-42b9-a6e5-7430bc0c0e9d)

Hasil diatas merupakan grafik visualisasi dari skor akurasi yang diperoleh dari hasil optimasi algoritma genetika. 
Jadi, hasil ini menunjukkan bahwa algoritma genetika mampu meningkatkan performa model pada beberapa generasi, mencapai akurasi tertinggi sekitar 99.30% pada generasi keempat. Namun, performa ini mungkin bervariasi di setiap percobaan, dan tergantung pada konfigurasi parameter serta kebetulan dalam evolusi populasi kromosom.
