---
title: Alur Belajar Cyber Security Aku
published: true
tags: bootcamp-note
---
Halo teman-teman, jadi sekarang aku lagi ikut bootcamp IDN nih dan aku diminta untuk membuat roadmap aku dalam 5 tahun kedepan untuk belajar Cyber Security. Berikut roadmap yang aku buat sendiri, dan aku harap dengan roadmap ini aku bisa konsisten untuk terus mengikuti path yang ada :D

# Gambar Roadmap
![Roadmap Learning](/assets/images/roadmap-learning.jpg)

Nah teman-teman kurang lebih seperti diatas roadmap dari aku untuk belajar Cyber Security. Pasti teman-teman ingin tahu alasannya kenapa aku menyusun roadmap seperti itu. Disini aku jelasin alasan-alasan nya berdasarkan setiap kotak yang ada pada diagramnya.

## Perkuat Fundamental IT (Infromasi dan Teknologi)
Alasanku memilih belajar Fundamental IT untuk pertama kalinya adalah karena aku dari lulusan SMA yang latar belakangnya adalah Ilmu Pengetahuan Alam (IPA). Aku merasa bahwa jika belum belajar Fundamental IT, aku akan cukup kesulitan. Mengingat materi Cyber Security itu sendiri cukup banyak kata teknis yang digunakan di dalamnya seperti "Hardware", "Software", dan lain-lain. 

## Belajar Jaringan Komputer
Belajar jaringan itu penting, karena dosenku pernah bertanya kepada kami, "kapan dunia ngga butuh keamanan siber?" kami semua mencoba untuk menjawab tapi tidak ada satupun yang tepat. Kemudian beliau menjawab, "ketika di dunia ini sudah tidak ada yang namanya jaringan internet!" wow, ga nyangka banget jawabannya sesederhana itu. Dari situ aku tangkap, selama ada jaringan internet, maka ancaman siber akan terus ada.

## Belajar Cyber Security
Setelah memperkuat Fundamental IT dan Jaringan Komputer, kita bisa lanjut belajar Dasar Keamanan Siber. Saat aku pertama kali belajar Cyber Security di kampus, awalnya aku akan belajar definisi Cyber Security itu sendiri, kemudian dilanjutkan dengan belajar *McCumber Cube*, dan jenis-jenis serangan yang sering terjadi.

Sekedar info dari yang udah aku pelajari, *McCumber Cube* merupakan framework (kerangka kerja) untuk meningkatkan keamanan dari data. Nah, di framework ini terdapat tiga prinsip utama, yakni *Confidentiality* (Kerahasiaan), *Integrity* (Integritas), dan *Availability* (Keteserdiaan).

**Confidentiality** (Kerahasiaan) berarti memastikan data tersebut hanya diketahui oleh pihak yang berwenang. Agar data menjadi rahasia, data harus dienkripsi terlebih dahulu dengan menggunakan algortima tertentu seperi SHA-256, RSA, XOR Cipher, dan lain-lain. Enkripsi adalah mengubah data dari yang awalnya bisa dibaca menjadi tidak bisa dibaca dengan menggunakan kunci dan algoritma khusus. Hasil dari enkripsi, yakni data yang tidak dapat dibaca, disebut Ciphertext. Untuk mengubah data menjadi seperti semula, data perlu dilakukan proses Dekripsi. Proses Dekripsi adalah mengubah ciphertext menjadi data seperti semula dengan menggunakan key dan algoritma yang sama pada saat proses enkripsi.

**Integrity** (Integritas) berarti memastikan data tetap asli hingga sampai ke pihak yang berwenang. Data tetap asli memiliki arti bahwa data tidak berubah isinya, tetap utuh, dan akurat. Untuk memastikan data tetap asli sampai ke tujuan, pengrim memberikan *Digital Signature* terlebih dahulu kepada penerima sebelum data dikirim.

**Availability** (Ketersediaan) berarti data tersebut tersedia kapanpun saat kita butuh. Kita bisa menyimpan data di layanan penyimpanan awan (Cloud Storage) seperti Google Drive, Onedrive, atau yang lain. Layanan ini umumnya sudah menyediakan aplikasi yang dapat diinstal di ponsel, sehingga data yang disimpan bisa diakses kapan saja dan dimana saja. 

## Belajar Linux
Banyak hacker yang lebih memilih untuk menggunakan Sistem Operasi berbasis Linux. Berbeda dengan Windows, Linux memiliki lisensi *GNU General Public License version 2* (GPL-2.0) yang membuatnya open-source. Karena lisensi tersebut, hacker dapat memodifikasi Linux sesuai kebutuhan dan membagikan sumber kode kepada publik. Selain itu, Linux tidak memiliki update terjadwal seperti Windows yang dapat mengganggu pekerjaan.

Kita bisa menemukan banyak jenis sistem operasi linux yang tersebar di Internet. Istilah yang digunakan untuk Sistem Operasi berbasis Linux adalah "Linux Distro", yang berarti "Linux Distribution". Beberapa dari Linux Distro yang umum digunakan adalah Kali Linux untuk hacking, Linux Mint dan Ubuntu untuk kebutuhan desktop, dan Alpine Linux untuk containerization.

## Bermain CTF (Capture The Flag)
Capture The Flag (CTF) adalah sebuah permainan untuk menemukan dan mengeksploitasi kerentanan dalam sistem komputer atau aplikasi untuk mendapatkan "bendera" (flag). Alur permainan ini mirip dengan langkah Penetration Testing. Tahap pertama yang kita lakukan adalah mengumpulkan informasi tentang sistem (reconnaisance). Dari informasi yang sudah dikumpulkan, kita bisa gunakan untuk melakukan serangan (exploitation). Jika serangan berhasil, maka kita akan mendapatkan flag. Umumnya flag ini ditulis dengan format khusus, seperti contohnya "noirCTF{m3_g0t_th3_fl4g_0a3x5w2p1}".

## Mengambil Sertifikasi
Menurutku sertifikasi itu sangat penting agar kita bisa mengetahui lebih luas mengenai Cyber Security. Sertifikasi dapat meningkatkan keterampilan teknis, memberikan pengetahuan yang mendalam tentang berbagai ancaman siber dan teknik mitigasi yang tepat. Selain itu, sertifikasi juga meningkatkan peluang kita untuk bekerja di perusahaan yang membutuhkan ahli keamanan siber.

## Membuat Project
Agar kita tahu penerapan langsung dari yang sudah dipelajari, kita bisa mencoba untuk membuat project. Selama aku kuliah, project yang sudah aku buat adalah Image Location Detector menggunakan Exiftool dan Simulasi Serangan DDoS menggunakan GNS3 yang memanfaatkan tools seperti hping3 untuk melakukan serangan. Tujuan dari pembuatan project ini adalah agar tidak kaget dan bingung ketika menemukan kasus yang serupa saat bekerja di perusahaan.

## Susun CV
Susun CV ini sudah tidak perlu dipertanyakan lagi tujuannya -- karena jika ingin bekerja di perusahaan, kita perlu menyusn CV sebagai riwayat hidup dan bukti pencapaian yang telah dilakukan.

## Magang dan Kerja
Magang bertujuan untuk memperluas wawasan tentang dunia kerja, membangun jaringan profesional, dan meningkatkan peluang kerja di masa depan.

Seperti itulah penjelasan Alur Belajarku untuk Cyber Security, semoga menginspirasi dan bisa menjadi referensi teman-teman  :)

