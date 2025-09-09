# datamining-bookstore-apriori
Tugas Akhir

PENERAPAN DATA MINING PADA PENJUALAN TOKO BUKU MENGGUNAKAN ALGORITMA APRIORI DALAM STRATEGI PENJUALAN BUNDLING PRODUK

Proyek ini merupakan implementasi Tugas Akhir dengan topik penerapan algoritma Apriori pada data penjualan toko buku untuk menyusun strategi penjualan bundling produk.


Latar Belakang

Toko buku menyediakan beragam koleksi buku dan produk pelengkap, namun menghadapi tantangan seperti stok menumpuk pada produk yang kurang diminati dan rendahnya nilai rata-rata transaksi. Untuk meningkatkan penjualan, strategi pemasaran yang tepat diperlukan, salah satunya dengan product bundling, yaitu menggabungkan beberapa produk terkait dalam satu paket. Pemilihan bundling yang efektif dapat didukung dengan data mining menggunakan algoritma apriori, yang mampu menemukan pola asosiasi antar produk yang sering dibeli bersamaan. Dengan penerapan strategi ini, toko buku dapat meningkatkan volume penjualan, mengurangi penumpukan stok, serta menciptakan pengalaman belanja yang lebih menarik bagi konsumen.

Identifikasi Masalah
1) Pola penjualan produk yang tidak diterapkan dalam penjualan pada Toko Buku, menyebabkan tingkat penjualan yang tidak stabil terhadap produk yang kurang diminati oleh pembeli.
2) Adanya penumpukan stok produk secara berkelanjutan, mengakibatkan buku tidak terjual.

Tujuan
1) Melakukan identifikasi terhadap kombinasi produk yang paling sering dibeli secara bersamaan oleh konsumen.
2) Mengetahui kombinasi produk yang terjual berdasarkan nilai- nilai yang telah ditentukan sebelumnya, agar stok tidak menumpuk.

Manfaat Penulisan:
Untuk menghasilkan sebuah pengetahuan pada pola belanja konsumen untuk merencanakan strategi penjualan bundling produk yang efektif sehingga dapat meningkatkan performa pada toko buku.

Metode: Algoritma Apriori

Tools: Jupyter Notebook (Bahasa pemrograman python) dan RapidMiner

Objectives
1) Melakukan data cleaning dan transformasi pada dataset transaksi toko buku.
2) Menggunakan algoritma Apriori untuk menemukan association rules antar produk.
3) Menghitung nilai Support, Confidence, dan Lift Ratio sebagai dasar evaluasi.
4) Memberikan rekomendasi strategi bundling produk berdasarkan hasil aturan asosiasi.

Struktur Folder: 
- notebooks/      # Jupyter Notebooks untuk preprocessing & perhitungan
- data/           # Dataset mentah dan hasil transformasi
- rapidminer/     # File project RapidMiner (.rmp & .rmhdf5table)
- results/        # Visualisasi hasil (rules, tabel, grafik)
- README.md

Penjelasan Folder Results: 
1) AssociationRules.png → Visualisasi aturan asosiasi
2) Rules Summary.png → Grafik Penyajian model terbaik
3) Table View.png → Tabel hasil perhitungan support, confidence & lift
4) Perhitungan Lift Ratio Dataset.png → Hasil perhitungan lift ratio pada tools jupyter

Hasil Aturan Asosiasi
1) {Majalah Seni, Buku Anak-Anak} → {Alat Tulis}
Support = 13.7% | Confidence = 80.5% | Lift = 1.374
2) {Majalah Fashion, Buku Anak-Anak} → {Alat Tulis}
Support = 13.1% | Confidence = 82.9% | Lift = 1.415
3) {Majalah Berita, Buku Anak-Anak} → {Alat Tulis}
Support = 14.8% | Confidence = 83.5% | Lift = 1.425
4) {Buku Anak-Anak, Novel Fiksi Ilmiah} → {Alat Tulis}
Support = 13.1% | Confidence = 84.0% | Lift = 1.433
5) {Aksesoris Buku, Buku Anak-Anak} → {Alat Tulis}
Support = 19.1% | Confidence = 84.4% | Lift = 1.440
6) {Buku Biografi, Buku Anak-Anak} → {Alat Tulis}
Support = 14.6% | Confidence = 86.4% | Lift = 1.474
7) {Novel Romansa, Buku Anak-Anak} → {Alat Tulis}
Support = 14.1% | Confidence = 87.1% | Lift = 1.486
8) {Buku Anak-Anak, Buku Fiksi} → {Alat Tulis}
Support = 13.5% | Confidence = 87.8% | Lift = 1.498
9) {Buku Anak-Anak, Novel Misteri} → {Alat Tulis}
Support = 13.9% | Confidence = 88.1% | Lift = 1.503
10) {Buku Anak-Anak, Buku Sejarah} → {Alat Tulis}
Support = 14.6% | Confidence = 93.3% | Lift = 1.592
