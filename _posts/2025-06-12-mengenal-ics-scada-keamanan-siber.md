---
title: Mengenal ICS & SCADA dalam Keamanan Siber
published: true
tags: bootcamp-note
---

Halo teman-teman, selamat datang di halaman saya :D. Kali ini saya akan membahas tentang ICS & SCADA dalam keamanan siber. Halaman ini ditujukan kepada pembaca yang baru pertama kali mendengar tentang istilah ICS & SCADA. Saya juga ngga expect kalau dunia cyber security seluas itu ya, dan ternyata ngga cuma berkaitan dengan dunia maya saja, tapi juga ada yang berkaitan dengan industri haha.

# Industrial Control System (ICS)

Industrial Control System (ICS) merupakan istilah yang merujuk kepada kontrol dan pemantauan (*monitor*) fasilitas industri. ICS mencakup beberapa jenis sistem, seperti *process control system* (PCS), *distributed control system* (DCS), *supervisory control and data acquisition* (SCADA), dan lain-lain. Tanpa ICS, proses industri dapat berjalan lambat, rentan terhadap kesalahan manusia (*human-error*), dan berisiko tinggi.

# Apa itu SCADA dalam ICS?

Sesuai dengan namanya, *Supervisory control and data acquisition* (SCADA) yang berarti “Kontrol pengawasan dan akuisisi data”, adalah sistem yang digunakan untuk mengontrol aset yang tersebar secara geografis dalam industri, dimana akusisi data yang terpusat sama pentingnya dengan kontrol. Akusisi data dalam konteks ini berarti data yang dikumpulkan dari lapangan dan ditampilkan secara visual dan mudah dibaca. 

Oleh karena itu, SCADA dirancang untuk mengumpulkan informasi lapangan, mengirim data ke pusat kendali, dan menampilkan informasi kepada operator secara grafis atau tekstual, sehingga memungkinkan operator untuk memantau atau mengendalikan seluruh sistem dari lokasi pusat secara hampir real-time.

Implementasi dari sistem SCADA bisa dilihat pada gambar dibawah ini. Terdapat pusat kendali (Control Center), tiga lokasi lapangan (Field Site), dan perangkat telemetri radio seperti WAN, Satellite, dan menara seluler. 

Tugas pusat kendali dalam sistem ini adalah melakukan pengumpulan data pada interval yang ditentukan (setiap beberapa detik, atau menit) dan mengirim perintah ke perangkat lapangan sebagaimana diperlukan. Jaringan perusahaan memiliki akses ke semua pusat kendali melalui WAN, dan dapat diakses dari jarak jauh. Selain melakukan pengumpulan data dan mengirim perintah, server kendali juga mengawasi interupsi yang datang dari sistem alarm lokasi lapangan.

![alt text](/assets/images/2025-06-12/image.png)

# Apa Kaitannya dengan Keamanan Siber?

Karena ICS/SCADA dapat dipantau secara jarak jauh, tentu saja terhubung dengan jaringan internet. Hal ini tentunya berkaitan erat dengan keamanan siber. Ancaman dari dunia maya dapat mengganggu dan membahayakan proses industri. Misalnya, serangan siber dapat menyebabkan gangguan operasional, pencurian data, kerusakan fisik pada peralatan, atau bahkan membahayakan keselamatan manusia. 

# Contoh serangan terhadap ICS?

Contoh serangan ICS yang paling populer adalah Stuxnet. Stuxnet adalah worm komputer canggih yang secara khusus dibuat untuk menargetkan sistem kontrol industri Siemens yang digunakan dalam program pengayaan uranium di Iran. Cara kerja dari stuxnet adalah dengan menyebar melalui USB drive dan jaringan lokal. Ia mencari perangkat lunak SCADA Siemens Step7, lalu mengubah logika pada Programmable Logic Controller (PLC) untuk merusak sentrifugal yang memproses uranium, tanpa menunjukkan kesalahan pada panel kontrol.

Sekitar 1.000 dari 5.000 sentrifugal rusak terkena dampak serangan. Serangan ini menyebabkan gangguan besar pada program nuklir Iran tanpa perlu serangan militer terbuka. Stuxnet merupakan contoh pertama malware yang secara nyata merusak infrastruktur fisik melalui SCADA, dan diyakini dikembangkan oleh negara (kemungkinan AS dan Israel).

### Sumber
1. [NIST 800-802, Guide to Operational Technology (OT) Security.](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-82r3.ipd.pdf){:target="_blank"}

2. Book, CYBERSECURITY FOR INDUSTRIAL CONTROL SYSTEMS (SCADA, DCS, PLC, HMI), 2012.

