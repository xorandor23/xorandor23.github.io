---
title: Cara Menggunakan GNS3 Untuk Pemula
published: true
tags: bootcamp-note
---
Halo teman-teman selamat datang di laman blog saya ini :D. Jadi disini saya mau berbagi ilmu tentang bagaimana cara menggunakan GNS3 untuk pemula. Bagi kalian yang baru mengenal GNS3, yuk simak penjelasan dibawah ini!

# Apa itu GNS3?
![gns3-image](/assets/images/gns3-image.png)

GNS3 (Graphical Network Simulation-3) adalah perangkat lunak simulasi jaringan yang dirilis pada tahun 2008. Perangkat lunak ini memungkinkan kita untuk memodelkan jaringan seperti di dunia nyata. Jika dibandingkan dengan Cisco Packet Tracer, GNS3 memiliki fitur yang lebih lengkap. Kita bisa menambahkan Sistem operasi sendiri dari Virtualbox atau VMWare ke dalam GNS3, yang membuat simulasi jaringan terasa lebih nyata. Kita juga bisa menambahkan router Cisco sendiri di GNS3 karena sudah dilengkapi Dynamips Emulation Software untuk menjalankan Cisco IOS. 

# Cara Menginstall GNS3
1. GNS3 dapat diunduh secara langsung melalui tautan berikut: [https://www.gns3.com/software/download](https://www.gns3.com/software/download){:target="_blank"}. Pilihlah sesuai dengan sistem operasi yang kalian gunakan.
![gns3-image](/assets/images/gns3-tutorial-1.png)

2. Setelah diunduh, klik filenya. Kemudian kalian akan diarahkan untuk menginstall GNS3 ke komputer kita. Pastikan memilih opsi "Local Installation" pada tahap "Choose Components".
![gns3-image](/assets/images/gns3-tutorial-2.png)

3. Kita dapat mengubah lokasi direktori dimana GNS3 akan disimpan. Namun sebaiknya, saya sarankan agar menggunakan direktori Default dari GNS3 saja jika ruang penyimpanan pada Local Disk masih cukup.
![gns3-image](/assets/images/gns3-tutorial-3.png)

4. Klik "Next", tunggu hingga instalasai selesai. Jika ada muncul pesan seperti pada gambar ini, kalian bisa klik "Ok". Pesan tersebut menandakan bahwa WinPCAP sudah diinstal sebelumnya di komputer kalian.
![gns3-image](/assets/images/gns3-tutorial-4.png)

5. Jika WinPCAP belum diinstal, maka akan keluar pesan seperti gambar dibawah. Kalian ikuti arahannya saja untuk menginstall.
![gns3-image](/assets/images/gns3-tutorial-5.png)

5. Pada tahap "Solarwinds Standard Toolset", saya sarankan kalian pilih "No" lalu klik "Next".
![gns3-image](/assets/images/gns3-tutorial-6.png)

6. Instalasi yang berhasil akan memberikan pesan seperti gambar dibawah ini.
![gns3-image](/assets/images/gns3-tutorial-7.png)

# Tahap Awal setelah Instalasi GNS3
Tampilan awal GNS3 setelah diinstal akan terlihat seperti pada gambar dibawah ini. 



