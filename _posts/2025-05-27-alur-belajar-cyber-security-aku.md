---
title: Alur Belajar Cyber Security Aku
published: true
tags: bootcamp-note
---
Halo teman-teman, jadi sekarang aku lagi ikut bootcamp IDN nih dan aku diminta untuk membuat roadmap aku dalam 5 tahun kedepan untuk belajar Cyber Security. Berikut roadmap yang aku buat sendiri, dan aku harap dengan roadmap ini aku bisa konsisten untuk terus mengikuti path yang ada :D

# Gambar Roadmap
![Roadmap Learning](/assets/images/roadmap-learning.jpg)

Nah teman-teman kurang lebih seperti diatas roadmap aku untuk belajar Cyber Security -- pasti teman-teman ingin tahu alasannya kenapa aku menyusun roadmap seperti itu. Okee disini bakal aku jelasin alasan-alasan nya berdasarkan setiap kotak yang ada pada diagramnya.

## Perkuat Fundamental IT (Infromasi dan Teknologi)
Alasan aku buat milih belajar Fundamental IT dulu adalah karena aku dari lulusan SMA yang backgroundnya adalah Ilmu Pengetahuan Alam (IPA). Alasan keduaku karena belajar Fundamental atau Dasar IT itu penting banget, karena dari kata "cyber security" itu sendiri artinya adalah keamanan di dunia maya. Nah, dunia maya itu sendiri terdapat banyak data yang disimpan dan bisa diakses dimana saja. Bahkan, data pribadi kita juga ada lho di sana!. Makanya, kita perlu belajar IT dulu sebelum kenal ke Cyber Security.

Alasan ketigaku adalah karena banyak pertanyaan yang muncul dari pikiranku. Aku sempat bertanya-tanya "Kok bisa ya ponsel sekecil ini, bisa nyimpen banyak data yang melebihi buku?", "Gimana caranya ponsel ini nyimpen data sebanyak itu?", "Kenapa kalau kita mau nyari data lewat google, harus hidupin Wi-FI atau Data Seluler?", "Kok bisa kita ngomong sama orang yang jaraknya antar kota, bahkan antar benua?" dan masih banyak lagi karena pertanyaanku banyak dipenuhi dengan "kok bisa?" wkwkwk. Nah, semua itu bisa terjawab kalau kita mengenal teknologi yang digunakan itu sendiri. Dengan apa? YA BELAJAR FUNDAMENTAL IT LAH!.

## Belajar Jaringan Komputer
Belajar jaringan itu penting, karena dosenku pernah bertanya kepada kami, "kapan dunia ngga butuh keamanan siber?" kami semua mencoba untuk menjawab tapi tidak ada satupun yang tepat. Kemudian beliau menjawab, "ketika di dunia ini sudah tidak ada yang namanya jaringan internet!" wow, ga nyangka banget jawabannya sesederhana itu. Dari situ aku tangkap, selama ada jaringan internet, maka ancaman siber akan terus ada. Selain itu, kita juga harus tahu gimana perangkat terhubung satu dengan yang lainnya.

## Belajar Cyber Security
Nahh setelah memperkuat Fundamental IT dan Jaringan Komputer, kita bisa lanjut nih belajar Dasar Keamanan Siber. Kalau aku belajar Cyber Security di kampus, mula-mulanya aku akan dikenalkan dengan definisi dari Cyber Security itu sendiri, kenapa harus belajar Cyber Security, *McCumber Cube*, dan jenis serangan yang umum terjadi.

![mc-cumber-cube](/assets/images/mccumber-cube.png)

Sekedar info dari yang udah aku pelajari, *McCumber Cube* merupakan framework (kerangka kerja) untuk meningkatkan keamanan dari data. Nah, di framework ini terdapat tiga prinsip utama, yakni *Confidentiality* (Kerahasiaan), *Integrity* (Integritas), dan *Availability* (Keteserdiaan).

*Confidentiality* (Kerahasiaan) berarti memastikan data tersebut hanya diketahui oleh pihak yang berwenang. Salah satu upaya yang dapat kita lakukan agar data tetap rahasia adalah dengan mengenkripsi data dengan menggunakan algortima tertentu seperi SHA-256, RSA, XOR Cipher, dan lain sebagainya. Jadi, mengenkripsi adalah mengubah data dari yang awalnya bisa dibaca menjadi gak bisa dibaca dengan menggunakan kunci dan algoritma khusus. 

Algortima tuh ibaratnya pola yang digunakan untuk nge-enkripsi data kita. Hasil enkripsi ini disebut Ciphertext, adalah data yang terlihat acak, sehingga orang yang gak punya kuncinya dan gak tau algortimanya gak bakal bisa tahu isi data sebenarnya. Agar data yang sudah di enkripsi bisa dibaca kembali, kita perlu tahu kunci dan jenis algoritma yang digunakan. Proses untuk mengembalikan data yang tidak bisa dibaca menjadi bisa dibaca kembali dinamakan Dekripsi.

Contoh dari Enkripsi: Misal, aku punya kata "PISANG" dengan algortima Caesar Cipher dengan kunci geser ke kanan 1. Hasil enkripsinya adalah "QJTBOH". Nah, pola yang digunakan pada algoritma ini adalah dengan menggeser tiap huruf sebanyak satu kali ke kanan. 

*Integrity* (Integritas) berarti memastikan data tetap asli hingga sampai ke pihak yang berwenang. Maksud dari datanya tetap asli adalah tidak berubah isinya, tetap utuh, dan akurat. Maksudnya gimana tuh? Analoginya adalah seperti ini, andaikan aku pesan Hape Siyoumee secara COD dari Aplikasi Sopi. Waktu paket nya udah sampai ke rumah, aku cek paketnya kok ada yang robek bungkusnya. Pas di buka, isinya malah keramik. Nah, itu berarti paketnya udah di colong trus diganti ama keramik. Kasian bet dah.

Kalau dari pesen paket, kita bisa tahu paketnya udah berubah dari bungkusan luarnya yang udah robek-robek. Nah, kalau dalam Keamanan Siber, kita bisa cek datanya apakah sudah berubah sebelum sampai ke pihak yang berwenang dengan menggunakan Digital Signature. Digital Signature adalah tanda tangan elektronik yang menggunakan teknologi kriptografi untuk memastikan keaslian data. Sebelum data dikirim ke pihak yang berwenang, biasanya pihak pengirim memberikan Digital Signature terlebih dahulu ke pihak penerima.

*Availability* (Ketersediaan) berarti data tersebut tersedia kapanpun saat kita butuh. Maksudnya gimana tuh? Misalkan, atasan minta untuk ngirim file laporan bulan ini, ehh tapi kitanya lagi di luar nongkrong ama temen, dan ngga bawa laptop. Mau ngga mau, kita pulang dulu dong ke rumah buka laptop buat ngirim filenya. Pastinya ribet banget. Nah, solusinya adalah kita bisa nyimpen file-nya di layanan penyimpanan awan (*cloud storage*) seperti Google Drive, Onedrive, atau layanan *cloud storage* lainnya. Umumnya, layanan ini sudah memiliki aplikasi yang dapat kita install di ponsel kita. Dengan ini, file bisa diakses kapan saja dan dimana saja. Kalau kita lagi diluar, kita bisa buka aplikasi layanan penyimpanan cloud aja, bagikan link file ke atasan, selesai. Kurang lebih seperti itu contoh dari *Availability* (Ketersediaan).

## Belajar Linux
Menurutku, belajar Linux itu penting banget karena belum bisa disebut hecker kalau belum pakai Linux awowkwkwk, candaa. **INGAT! Linux adalah sebuah kernel, bukan Sistem Operasi**. Kernel adalah inti dari sistem operasi yang menjembatani antara hardware (perangkat keras) dan software (perangkat lunak).
Sedangkan Sistem Operasi adalah kumpulan software dengan kernel didalamnya yang berfungsi untuk mengelola perangkat keras pada komputer dan menjalankan software tambahan. Nah, didalam Sistem Operasi terdapat kernel. Kalau sistem operasi ga ada kernel, komputernya ga bakal bisa hidup.

Umumnya, Sistem Operasi berbasis Linux digunakan oleh kebanyakan hacker karena lebih bebas dari Windows. Linux memiliki lisensi khusus yang membuatnya open-source. Tidak seperti Windows, yang lisensinya yang membuat sistem operasi tersebut menjadi closed-source. Karena lisensinya inilah, Linux dapat di customisasi sesuai kebutuhan. Kita bisa menemukan banyak jenis sistem operasi linux yang tersebar di Internet. Istilah yang terkenal untuk Sistem Operasi berbasis Linux adalah "Linux Distro", yang berarti "Linux Distribution". Beberapa dari Linux Distro yang umum digunakan adalah Kali Linux untuk hacking, Linux Mint dan Ubuntu untuk kebutuhan desktop, dan Alpine Linux untuk containerization.

## Bermain CTF (Capture The Flag)
kompetisi keamanan siber di mana peserta (baik individu maupun tim) ditantang untuk menemukan dan mengeksploitasi kerentanan dalam sistem komputer atau aplikasi untuk mendapatkan "bendera" (flag). Bermain Capture The Flag ini penting banget ya manteman, karena ini ibaratkan simulasi melakukan Penetration Testing. Jadi alur bermain CTF ini mirip seperti pentesting. Tahap pertama yang kita lakukan adalah mengumpulkan informasi tentang sistem (reconnaisance). Kemudian, dari informasi yang sudah didapat kita bisa mulai menyerang (exploitation). Jika serangan berhasil, maka kita akan mendapatkan flag nya. Umumnya flag ini dalam bentuk teks khusus ya teman-teman, seperti contohnya "noirCTF{m3_g0t_th3_fl4g_0a3x5w2p1}".

## Mengambil Sertifikasi

