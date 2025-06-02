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
1. GNS3 dapat diunduh secara langsung melalui tautan berikut: [https://www.gns3.com/software/download](https://www.gns3.com/software/download){:target="_blank"}. Pilihlah sesuai dengan sistem operasi yang kalian gunakan.<br><br>
![gns3-image](/assets/images/gns3-tutorial-1.png){: width="500" }

2. Setelah diunduh, klik filenya. Kemudian kalian akan diarahkan untuk menginstall GNS3 ke komputer kita. Pastikan memilih opsi "Local Installation" pada tahap "Choose Components".<br><br>
![gns3-image](/assets/images/gns3-tutorial-2.png){: width="500" }

3. Kita dapat mengubah lokasi direktori dimana GNS3 akan disimpan. Namun sebaiknya, saya sarankan agar menggunakan direktori Default dari GNS3 saja jika ruang penyimpanan pada Local Disk masih cukup.<br><br>
![gns3-image](/assets/images/gns3-tutorial-3.png){: width="500" }

4. Klik "Next", tunggu hingga instalasai selesai. Jika ada muncul pesan seperti pada gambar ini, kalian bisa klik "Ok". Pesan tersebut menandakan bahwa WinPCAP sudah diinstal sebelumnya di komputer kalian.<br><br>
![gns3-image](/assets/images/gns3-tutorial-4.png){: width="550" }

5. Jika WinPCAP belum diinstal, maka akan keluar pesan seperti gambar dibawah. Kalian ikuti arahannya saja untuk menginstall.<br><br>
![gns3-image](/assets/images/gns3-tutorial-5.png){: width="500" }

5. Pada tahap "Solarwinds Standard Toolset", saya sarankan kalian pilih "No" lalu klik "Next".<br><br>
![gns3-image](/assets/images/gns3-tutorial-6.png){: width="500" }

6. Instalasi yang berhasil akan memberikan pesan seperti gambar dibawah ini.<br><br>
![gns3-image](/assets/images/gns3-tutorial-7.png){: width="500" }

# Penjelasan Bagian pada GNS3
![gns3-image](/assets/images/gns3-tutorial-8.png)

Tampilan awal GNS3 setelah diinstal akan terlihat seperti pada gambar diatas ini. Setiap perangkat pada topologi disebut Nodes. 

### Bagian 1:
- Bagian **1.1** berisi daftar perangkat router yang tersedia. Untuk saat ini, routernya mungkin tidak ada karena kita harus menambahkan image routernya secara manual ke GNS3. Akan saya jelaskan cara untuk menambahkan router pada bagian selanjutnya. Router yang bisa kita tambahkan adalah router Cisco IOS.

- Bagian **1.2** berisi daftar perangkat Switch yang tersedia. GNS3 sudah menyediakan perangkat Switch yang bisa langsung kita gunakan, yakni ATM Switch, Ethernet Hub, Ethernet Switch, dan Frame Relay switch.

- Bagian **1.3** berisi daftar End Devices yang tersedia. End Devices adalah istilah yang merujuk pada perangkat yang menjadi sumber atau tujuan data dalam sebuah jaringan komputer, seperti komputer, laptop, ponsel, atau printer. Untuk saat ini hanya beberapa End Devices yang disediakan oleh GNS3 seperti Virtual PCs (VPCS), NAT (Network Address Translation), dan Cloud. Kita bisa menambahkan Komputer sendiri dari emulator seperti VirtualBox atau VMWare.

- Bagian **1.4** berisi daftar dari Security Devices. Untuk saat ini Security Devicesnya belum ada disediakan karena kita harus menambahkannya secara manual. Biasanya, bagian ini berisi perangkat Firewall, Intrusion Detection System (IDS), dan Intrusion Prevention System (IPS).

- Bagian **1.5** adalah bagian yang menampilkan seluruh daftar perangkat yang ada pada GNS3.

- Bagian **1.6** adalah logo kabel untuk menghubungkan perangkat satu sama lain.

### Bagian 2:
- Bagian **2.1** adalah bagian untuk menambahkan project (logo kiri) dan membuka project yang sudah ada (logo kanan).

- Bagian **2.2** terdapat dua logo, yakni logo Jam dan logo Huruf dengan Kabel. Logo Jam adalah fitur Snapshot yang digunakan untuk menyimpan keadaan topologi saat ini, dan mengembalikan topologi ke keadaan sebelumnya jika terjadi kesalahan. Logo Huruf dengan Kabel digunakan untuk menampilkan Interface yang digunakan pada masing-masing perangkat untuk terhubung ke perangkat lain.

- Bagian **2.3** terdapat lima logo:
1. Logo pertama dari kiri, untuk menampilkan terminal emulator yang terhubung pada protokol SSH. Terminal emulator ini seperti Command Line pada sistem operasi Windows, fungsinya untuk berinteraksi dengan sistem melalui teks saja. 
2. Logo kedua, berfungsi untuk menghidupkan semua perangkat pada topologi. 
3. Logo ketiga berfungsi untuk mengpause semua aktivitas pada topologi. 
4. Logo keempat berfungsi untuk mematikan semua perangkat pada topologi. Dan 
5. Logo terakhir untuk merestart semua perangkat.

-  Bagian ****

# Cara Menambahkan Cisco IOS
