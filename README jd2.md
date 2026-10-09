# Praktikum Jaringan Komputer

## VLAN and Trunking Configuration

### Identitas

- **Nama:** Nanda Nabila Fauziah
- **Mata Kuliah:** Praktikum Jaringan Komputer
- **Materi:** VLAN dan Trunking
- **Tools:** Cisco Packet Tracer

### Deskripsi

Praktikum ini membahas konfigurasi Virtual Local Area Network (VLAN) dan trunking menggunakan Cisco Packet Tracer. VLAN digunakan untuk membagi jaringan switch menjadi beberapa jaringan logis sehingga perangkat dapat dikelompokkan berdasarkan fungsi atau kebutuhan tertentu.

Trunking digunakan untuk menghubungkan dua switch agar dapat membawa lalu lintas data dari beberapa VLAN melalui satu koneksi fisik.

Topologi yang digunakan terdiri dari dua switch yang dihubungkan menggunakan trunk, dengan perangkat yang dikelompokkan ke dalam VLAN 10 (Operations) dan VLAN 99 (Management).

### Konfigurasi VLAN

| **VLAN ID** | **Nama VLAN** | **Fungsi** |
|---|---|---|
| 10 | Operations | Mengelompokkan perangkat untuk bagian operasional |
| 99 | Management | Mengelompokkan perangkat untuk kebutuhan manajemen jaringan |

### Konfigurasi Jaringan

| **Perangkat** | **Interface** | **Mode** | **Keterangan** |
|---|---|---|---|
| S1 | Port yang terhubung ke PC Operations | Access | Menghubungkan PC ke VLAN 10 |
| S1 | Port yang terhubung ke PC Management | Access | Menghubungkan PC ke VLAN 99 |
| S1 | Port yang terhubung ke S2 | Trunk | Membawa lalu lintas VLAN 10 dan VLAN 99 |
| S2 | Port yang terhubung ke PC Operations | Access | Menghubungkan PC ke VLAN 10 |
| S2 | Port yang terhubung ke PC Management | Access | Menghubungkan PC ke VLAN 99 |
| S2 | Port yang terhubung ke S1 | Trunk | Membawa lalu lintas VLAN 10 dan VLAN 99 |

*Catatan: Nomor interface disesuaikan dengan port yang digunakan pada topologi Packet Tracer.*

### Konfigurasi yang Dilakukan

1. Membuat VLAN 10 dengan nama Operations dan VLAN 99 dengan nama Management pada switch.
2. Mengatur port yang terhubung ke PC sebagai access port sesuai VLAN masing-masing.
3. Mengonfigurasi port penghubung antara S1 dan S2 sebagai trunk.
4. Mengatur VLAN yang diizinkan melewati trunk, yaitu VLAN 10 dan VLAN 99.
5. Menggunakan kabel Copper Straight-Through untuk menghubungkan perangkat sesuai topologi praktikum.

### Pengujian

Pengujian dilakukan untuk memastikan konfigurasi VLAN dan trunking berjalan dengan benar. Pemeriksaan meliputi:

- Memastikan VLAN 10 dan VLAN 99 telah dibuat menggunakan perintah `show vlan brief`.
- Memastikan port access telah masuk ke VLAN yang sesuai.
- Memastikan koneksi trunk aktif menggunakan perintah `show interfaces trunk`.
- Melakukan pengujian konektivitas menggunakan perintah `ping` antar-PC yang berada pada VLAN yang sama.

PC dalam VLAN yang sama diharapkan dapat berkomunikasi melalui trunk jika konfigurasi IP dan port sudah benar. Sementara itu, komunikasi antar-VLAN memerlukan konfigurasi routing.

### Video Praktikum

Klik di sini untuk melihat video praktikum (https://youtu.be/VlNXkiGKww8)

### File Packet Tracer

File konfigurasi Cisco Packet Tracer tersedia pada folder `packet-tracer`.

File tersebut berisi topologi jaringan, konfigurasi VLAN, pengaturan access port, serta konfigurasi trunking antara switch S1 dan S2.
