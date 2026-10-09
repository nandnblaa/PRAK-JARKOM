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

### Video Praktikum

Klik di sini untuk melihat video praktikum (https://youtu.be/VlNXkiGKww8)

### File Packet Tracer

File konfigurasi Cisco Packet Tracer tersedia pada folder `packet-tracer`.

File tersebut berisi topologi jaringan, konfigurasi VLAN, pengaturan access port, serta konfigurasi trunking antara switch S1 dan S2.
