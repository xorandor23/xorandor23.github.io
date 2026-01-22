---
title: Melakukan Hardening Linux
published: true
tags: bootcamp-note
---
Halo teman-teman, selamat datang kembali di halaman saya :D. Kali ini saya akan membahas tentang Hardening Linux. Pembahasan ini adalah pembahasan yang menarik untuk saya, karena ketetartikan saya terhadap Linux.

# Apa itu Hardening?
Hardening adalah upaya untuk mengurangi ancaman dan potensi kerentanan, dengan memaksimalkan perlindungan yang ada. Hardening juga berarti mengoptimalkan konfigurasi untuk operasi yang aman dan perlindungan data. Untuk mengurangi kerentanan yang dapat dieksploitasi, ada tiga aturan umum yang dapat diikuti:
1. Update Software dan Sistem Operasi Secara Berkala.
Seiring berjalannya waktu, pasti ada kerentanan yang ditemukan dalam sistem operasi dan software. Update sangat penting untuk menutupi (patch) kerentanan yang ditemukan.
2. Menghapus Aplikasi yang Usang.
Aplikasi yang sudah lama, sudah tidak dijalankan lagi, karena sudah tidak menerima update di komputer dapat memunculkan kerentanan yang membahayakan sistem operasi. Hapus aplikasi yang mungkin sudah tidak terpakai untuk memberikan ruang penyimpanan lebih pada sistem operasi, dan mengurangi kerentanan yang dapat dieksploitasi.
3. Nonaktifkan Beberapa Aplikasi saat Booting.
Misalnya, ada beberapa aplikasi yang dimulai bersamaan dengan sistem operasi. Banyaknya aplikasi yang dimulai dapat memunculkan kerentanan dari sistem operasi itu sendiri, seperti sistem menjadi lambat. Nonaktifkan beberapa aplikasi yang tidak terlalu penting agar sistem operasi dapat berjalan lebih cepat.
4. Pertahankan Pengaturan Konfigurasi yang Aman.
Penting sekali untuk mempertahankan konfigurasi yang aman pada komputer. Contoh dari konfigurasi yang aman adalah memberikan password pada setiap user, dan menetapkan kebijakan pengguna pada sistem operasi.

# Hardening Pada Linux
Hardening pada Linux adalah melakukan perlindungan pada sistem operasi berbasis Linux untuk mengamankan data dan menghindari tangan-tangan jahil para hacker. Seseorang yang bertanggung jawab untuk keamanan linux adalah administrator sistem (*System Administrator*). Banyak cara yang dapat dilakukan untuk melakukan hardening pada linux, seperti mengganti password secara berkala, disable login sebagai root, mengenkripsi komunikasi data, dan lain-lain. Agar lebih spesifik, saya hanya akan membahas lebih detail tentang salah satu cara untuk melakukan hardening pada server linux.

# Hardening Linux dengan Port Scanning
Port Scanning adalah upaya untuk mengecek layanan yang sedang aktif pada suatu IP address atau domain, dengan mengetahui port yang terbuka. Banyak tools yang dapat digunakan untuk melakukan Port Scanning, salah satunya adalah `nmap`.

Kita bisa mengecek port yang terbuka dengan mengetikkan domainnya seperti ini:

```sh
nmap -sT -O google.com
```
Atau hanya dengan IP addressnya saja:

```sh
nmap -sT -O 127.0.0.1
```

Output yang ditampilkan dari `nmap` ketika melakukan port scanning adalah seperti dibawah ini (dari google.com). Tulisan `80/tcp` dan `443/tcp` adalah port yang terbuka. Jika port tersebut sedang tidak digunakan, sebaiknya matikan layanan yang menggunakan port tersebut.

```
Starting Nmap 7.95 ( https://nmap.org ) at 2025-06-12 15:47 +07
Nmap scan report for google.com (74.125.68.102)
Host is up (0.011s latency).
Other addresses for google.com (not scanned): 74.125.68.101 74.125.68.139 74.125.68.100 74.125.68.138 74.125.68.113 2404:6800:4003:c02::64 2404:6800:4003:c02::71 2404:6800:4003:c02::8b 2404:6800:4003:c02::8a
rDNS record for 74.125.68.102: sc-in-f102.1e100.net
Not shown: 998 filtered tcp ports (no-response)
PORT    STATE SERVICE
80/tcp  open  http
443/tcp open  https
Warning: OSScan results may be unreliable because we could not find at least 1 open and 1 closed port
OS fingerprint not ideal because: Missing a closed TCP port so results incomplete
No OS matches for host

OS detection performed. Please report any incorrect results at https://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 8.65 seconds
```

# Akhir Kata
Kurang lebih seperti itu yang dapat saya bagikan terkait Hardening Linux. Saya harap ilmu yang saya bagikan ini bisa bermanfaat untuk kedepannya. Keep Learning!