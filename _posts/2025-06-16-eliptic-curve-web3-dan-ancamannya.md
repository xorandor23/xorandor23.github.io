---
title: Mengenal Eliptic Curve Cryptography (ECC) & Web3
published: false
tags: bootcamp-note
katex: True
---
Halo teman-teman, selamat datang kembali di halaman saya :D. Kali ini saya akan membahas tentang *Eliptic Curve Cryptography* (ECC) dan Web3. Pembahasan ini akan cukup banyak membawa istilah matematika, dan juga cryptocurrency yang mungkin jarang teman-teman dengar sebelumnya. Kalau teman-teman penasaran, yuk baca blog saya selanjutnya!

# Apa itu Eliptic Curve Cryptography (ECC)?
Pertama, kita harus tahu dulu *Eliptic Curve* itu apa. *Eliptic Curve* atau Kurva Elipsis adalah rumus yang dihasilkan dari integral orbit elips pada planet. Rumus ini sudah digunakan pada banyak bidang matematika, salah satunya untuk melakukan pemfaktoran dan pembuktian *Last Fermat Theorem*. Persamaan *Elliptic Curve* didefinisikan dengan persamaan:

$$y^{2} = x^{3} + ax + b$$

dimana $$a$$ dan $$b$$ adalah konstanta. 

*Elliptic Curve Cryptography* (ECC) adalah algoritma pembentuk kunci publik yang menggunakan persamaan *Elliptic Curve* dalam pembentukan kunci publik. Alasan penggunaan *Elliptic Curve* adalah karena tidak membutuhkan bilangan besar dalam pembentukan kuncinya, sehingga tidak menggunakan banyak sumber daya. ECC adalah hasil pembaharuan dari algoritma pembentuk kunci publik pertama, yaitu RSA (Rivest–Shamir–Adleman). 

RSA menggunakan dua bilangan prima untuk membentuk kuncinya. Namun, bilangan prima yang harus dibutuhkan sangat besar agar pemfaktoran dua bilangan tersebut lama. Bilangan yang besar membutuhkan memori yang besar, penggunaan CPU yang banyak, dan waktu yang lama. Dari sinilah, ECC hadir untuk menjadi alternatif dari RSA karena dapat memberikan keamanan dengan level yang sama pada RSA.

# Apa itu Web3?
Web3 adalah konsep generasi ketiga dari perkembangan internet, yang berfokus pada desentralisasi, keterbukaan, dan kepemilikan data oleh pengguna. Jika Web1 bersifat statis dan Web2 memunculkan interaktivitas dan platform besar (seperti Google dan Facebook), maka Web3 hadir untuk memberikan kontrol lebih besar kepada pengguna melalui teknologi blockchain.

Web3 memungkinkan pengguna untuk mengakses layanan tanpa perantara, menyimpan dan mengelola data pribadi secara independen, menggunakan aplikasi terdesentralisasi (DApps) dan kontrak pintar (smart contracts) melakukan transaksi menggunakan cryptocurrency. Web3 menjanjikan sejumlah manfaat besar, di antaranya:

1. Desentralisasi
Tidak ada entitas tunggal yang mengontrol data atau aplikasi. Ini mengurangi risiko penyalahgunaan kekuasaan oleh perusahaan besar.
2. Kepemilikan Data
Pengguna memiliki kontrol penuh atas identitas dan data mereka, termasuk bagaimana dan kepada siapa data tersebut dibagikan.
3. Transparansi
Karena menggunakan blockchain, semua transaksi dapat diaudit secara publik dan tidak mudah dimanipulasi.
4. Inklusi Keuangan
Web3 membuka akses ke layanan keuangan tanpa memerlukan rekening bank atau identitas formal.

# Ancaman dan Risiko Web3
Meski menjanjikan masa depan yang terbuka dan bebas dari dominasi platform raksasa, Web3 juga membawa berbagai ancaman dan tantangan serius, antara lain:

1. Keamanan dan Penipuan
Banyak proyek Web3 belum matang dan rentan terhadap peretasan. Maraknya penipuan (scam), seperti rug pulls atau proyek palsu, menyebabkan banyak investor kehilangan aset. Tidak adanya otoritas pusat mempersulit pelaporan atau pemulihan dana jika terjadi kejahatan.
2. Ketergantungan pada Infrastruktur Terpusat
Meskipun Web3 berusaha untuk terdesentralisasi, banyak proyek masih menggunakan server cloud terpusat (misalnya Amazon Web Services), Gateway terpusat (seperti Infura untuk Ethereum). Hal ini menimbulkan kontradiksi internal dalam visi Web3.
3. Skalabilitas dan Biaya
Beberapa blockchain (seperti Ethereum) mengalami masalah kecepatan transaksi dan biaya gas yang tinggi. Ini menghambat penggunaan Web3 secara luas dan membuatnya tidak ramah untuk pengguna umum.
4. Kesenjangan Akses dan Pengetahuan
Teknologi Web3 masih sulit dipahami oleh pengguna awam. Memerlukan pemahaman teknis seperti private key, wallet, smart contract, dsb. Risiko kehilangan aset tinggi jika pengguna melakukan kesalahan kecil (seperti kehilangan seed phrase).
5. Regulasi dan Legalitas
Banyak negara belum memiliki regulasi jelas terkait aset digital dan Web3. Hal ini menciptakan ketidakpastian hukum, baik untuk pengguna maupun pengembang.


