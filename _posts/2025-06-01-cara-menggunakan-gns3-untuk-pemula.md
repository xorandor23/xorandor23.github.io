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

Tampilan awal GNS3 setelah diinstal akan terlihat seperti pada gambar diatas ini. Nantinya kita akan mencoba membuat topologi sederhana. Setiap perangkat pada topologi disebut Node. 

### Bagian 1:
- Bagian **1.1** berisi daftar perangkat router yang tersedia. Untuk saat ini, routernya mungkin tidak ada karena kita harus menambahkan image routernya secara manual ke GNS3. Akan saya jelaskan cara untuk menambahkan router pada bagian selanjutnya. Router yang bisa kita tambahkan adalah router Cisco IOS.

- Bagian **1.2** berisi daftar perangkat Switch yang tersedia. GNS3 sudah menyediakan perangkat Switch yang bisa langsung kita gunakan, yakni ATM Switch, Ethernet Hub, Ethernet Switch, dan Frame Relay switch.

- Bagian **1.3** berisi daftar End Devices yang tersedia. End Devices adalah istilah yang merujuk pada perangkat yang menjadi sumber atau tujuan data dalam sebuah jaringan komputer, seperti komputer, laptop, ponsel, atau printer. Untuk saat ini hanya beberapa End Devices yang disediakan oleh GNS3 seperti Virtual PCs (VPCS), NAT (Network Address Translation), dan Cloud. Kita bisa menambahkan Komputer sendiri dari emulator seperti VirtualBox atau VMWare.

- Bagian **1.4** berisi daftar dari Security Devices. Untuk saat ini Security Devicesnya belum ada disediakan karena kita harus menambahkannya secara manual. Biasanya, bagian ini berisi perangkat Firewall, Intrusion Detection System (IDS), dan Intrusion Prevention System (IPS).

- Bagian **1.5** adalah bagian yang menampilkan seluruh daftar perangkat yang ada pada GNS3.

- Bagian **1.6** adalah logo kabel untuk menghubungkan perangkat satu sama lain.

### Bagian 2:
- Bagian **2.1** adalah bagian untuk menambahkan project (logo kiri) dan membuka project yang sudah ada (logo kanan).

- Bagian **2.2** terdapat dua logo, yakni logo Jam dan logo Huruf dengan Kabel. Logo Jam adalah fitur Snapshot yang berfungsi untuk menyimpan keadaan topologi saat ini, dan mengembalikan topologi ke keadaan sebelumnya jika terjadi kesalahan. Logo Huruf dengan Kabel berfungsi untuk menampilkan Interface yang digunakan pada masing-masing perangkat untuk terhubung ke perangkat lain.

- Bagian **2.3** terdapat lima logo:

    - Logo pertama dari kiri, berfungsi untuk menampilkan terminal emulator dari perangkat yang memiliki protokol SSH. Terminal emulator ini seperti Command Line pada sistem operasi Windows, fungsinya untuk berinteraksi dengan sistem melalui teks saja. 
    - Logo kedua, berfungsi untuk menghidupkan semua perangkat pada topologi. 
    - Logo ketiga berfungsi untuk mengpause semua aktivitas pada topologi. 
    - Logo keempat berfungsi untuk mematikan semua perangkat pada topologi. Dan 
    - Logo terakhir berfungsi untuk merestart semua perangkat.

- Bagian **2.4**:

    - Logo pertama dari kiri, berfungsi untuk menambahkan teks pada kotak 4.1 (area sekitar topologi).
    - Logo kedua berfungsi untuk menambahkan gambar.
    - Logo ketiga, keempat, dan kelima berfungsi untuk menambahkan Bentuk kotak, lingkaran, dan garis pada topologi.
    - Logo keenam berfungsi untuk mengunci agar tidak bisa memindahkan Node.
    - Logo ketujuh dan kedelapan berfungsi untuk memperbesar dan memperkecil tampilan topologi. Dan
    - Logo kesembilan, berfungsi untuk melakukan screenshot pada topologi.

- Bagian **3.1** adalah tampilan list dari perangkat yang tersedia berdasarkan kategori perangkat.

- Bagian **3.2** adalah log, yang menampilkan aktivitas yang sedang berlangsung dalam GNS3.

- Bagian **3.3** berisi daftar perangkat yang digunakan pada topologi.

- Bagian **3.4** berisi daftar server GNS3 yang tersedia. Server ini berperan penting agar GNS3 bisa berjalan dengan baik.

- Bagian **4.1** adalah area dimana topologi ditampilkan.

# Cara Membuat Topologi Sederhana

1. Buka GNS3, lalu tunggu sampai muncul pesan ini.<br><br>
![gns3-image](/assets/images/gns3-connecting-1.png)

2. Kemudian, kalian akan diberikan tampilan seperti gambar dibawah. Ganti nama "untitled" menjadi nama untuk project yang akan dibuat. Jika sudah, klik "Ok".<br><br>
![gns3-image](/assets/images/gns3-connecting-2.png)

3. Tambahkan 1 Switch dan 2 Virtual PCs (VPCS). Klik logo kabel (Bagian 1.6), lalu hubungkan perangkat satu sama lain seperti gambar dibawah ini.<br><br> 
![alt text](/assets/images/gns3-connecting-4.png)

    - Pastikan mengklik pada port yang statusnya masih kotak. Jika status port adalah lingkaran, berarti port sedang digunakan. <br><br> 
    ![alt text](/assets/images/gns3-connecting-3.png)
<br>

4. Sekarang, kita akan menambahkan IP address ke PC1 dan PC2. Klik tombol Play (Bagian 2.3) untuk menghidupkan seluruh perangkat. Lalu klik dua kali pada PC1 hingga muncul Terminal. Ketik perintah dibawah ini:
```sh
ip 10.0.0.1/24 
```
Lakukan hal yang sama dengan PC2, tapi IP nya diganti menjadi `10.0.0.2/24`.

5. Kita akan mencoba melakukan ping di setiap PC untuk memastikan bisa saling terhubung satu sama lain. Ketik perintah `ping 10.0.0.2` pada PC1 dan `ping 10.0.0.2` pada PC2.

# Akhir Kata
Kurang lebih ini ilmu yang dapat saya bagikan kepada teman-teman untuk belajar GNS3. Selanjutnya, saya akan memposting bagaimana cara menambahkan Router Cisco dan Mengimport Virtual Machine dari VirtualBox dan VMWare. Saya harap apa yang saya bagikan ini bisa bermanfaat untuk kedepannya. Keep Learning!