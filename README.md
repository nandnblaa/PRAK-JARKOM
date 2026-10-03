# Praktikum Jaringan Komputer
## Basic Network Configuration

### Identitas
- Nama: Nanda Nabila Fauziah
- Mata Kuliah: Praktikum Jaringan Komputer
- Materi: Basic Network Configuration
- Tools: Cisco Packet Tracer

### Deskripsi
Praktikum ini membahas konfigurasi dasar jaringan menggunakan Cisco Packet Tracer yang terdiri dari PC, switch, dan router.

Topologi yang digunakan:

PC-A → S1 → R1 → PC-B

### Konfigurasi IP

| Perangkat | Interface | IP Address | Subnet Mask | Default Gateway |
|---|---|---|---|---|
| PC-A | Fa0 | 192.168.1.10 | 255.255.255.0 | 192.168.1.1 |
| S1 | VLAN 1 | 192.168.1.2 | 255.255.255.0 | 192.168.1.1 |
| R1 | G0/0 | 192.168.1.1 | 255.255.255.0 | - |
| R1 | G0/1 | 192.168.0.1 | 255.255.255.0 | - |
| PC-B | Fa0 | 192.168.0.10 | 255.255.255.0 | 192.168.0.1 |

### Pengujian
Pengujian konektivitas dilakukan menggunakan perintah ping antara PC-A, PC-B, dan interface router.

### Video Praktikum
[Klik di sini untuk melihat video praktikum](https://youtu.be/-rkvfayupNQ)

### File Packet Tracer
File konfigurasi Cisco Packet Tracer tersedia pada folder `packet-tracer`.
