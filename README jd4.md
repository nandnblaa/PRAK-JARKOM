# Praktikum Jaringan Komputer
## Access User & Login Page (Judul 4)

### Identitas
- Kelompok 2D
- Nama:
  1. Nanda Nabila Fauziah | 2415061009
  2. Muhammad Imran Harun | 2415061013
  3. Muhammad Akbar Prayuga | 2415061017
  4. M. Rizky Bintang Samhadi | 2415061020
  5. Cantika Rybi Cahya Insani | 2415061029
- Mata Kuliah: Praktikum Jaringan Komputer
- Materi: Access User & Login Page (Judul 4)

### Deskripsi
Praktikum ini membahas konfigurasi manajemen user pada MikroTik, pembuatan halaman login (Hotspot Login Page), serta penerapan sistem autentikasi jaringan menggunakan FreeRADIUS dan daloRADIUS.

Konfigurasi dilakukan menggunakan MikroTik RouterOS melalui aplikasi WinBox untuk mengelola hak akses pengguna, membuat user baru, mengatur layanan Hotspot, dan membangun halaman login agar pengguna dapat terhubung ke jaringan melalui proses autentikasi.

Selain itu, dilakukan instalasi dan konfigurasi FreeRADIUS serta daloRADIUS pada Ubuntu 24.04 yang terintegrasi dengan database MariaDB. Integrasi ini memungkinkan MikroTik menggunakan server RADIUS untuk memverifikasi username dan password pengguna yang tersimpan di database.

### Pengujian
Pengujian dilakukan dengan mencoba login menggunakan beberapa akun yang telah dibuat, baik melalui menu User pada MikroTik maupun melalui halaman Hotspot Login Page.

Pengujian juga dilakukan dengan menghubungkan perangkat ke jaringan Wi-Fi "AP Jarkom", kemudian mengakses halaman login dan memasukkan username serta password yang telah didaftarkan melalui daloRADIUS.

Apabila proses login berhasil dan halaman status Hotspot ditampilkan, maka konfigurasi autentikasi MikroTik dengan FreeRADIUS dan daloRADIUS telah berhasil dilakukan.

### Video Praktikum
[Klik di sini untuk melihat video praktikum](https://youtu.be/_cCS0LFSMEE)
