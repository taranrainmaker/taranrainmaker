# TaranMidwife
## Product & Project Datasheet

**Digital Midwifery & Maternal Healthcare Platform**

TaranMidwife merupakan inisiatif teknologi kesehatan digital dari PT Taran Rainmaker Group untuk mendukung alur layanan kebidanan, kesehatan maternal, keterlibatan pasien, dan operasional layanan kesehatan komunitas.

**Status: Dalam pengembangan.** Dokumen ini membedakan kapabilitas yang tercantum dalam source code dari kesiapan alur end-to-end atau rilis produksi.

## 1. Informasi Proyek

| Item | Keterangan |
|---|---|
| Nama | TaranMidwife |
| Pengembang | PT Taran Rainmaker Group |
| Kategori | Platform digital kebidanan dan kesehatan maternal |
| Status | Dalam pengembangan |
| Model teknis | Backend API dan aplikasi pasien Flutter |
| Repository | https://github.com/taranrainmaker/taranmidwife |
| Kontak | hallo@taranrainmaker.my.id |

## 2. Kapabilitas pada Source Code

### Backend dan API
- Autentikasi dan otorisasi berbasis peran.
- Alur akun pasien dan mitra tenaga kesehatan.
- Katalog layanan dan pengelolaan area layanan.
- Appointment dan booking.
- Penugasan booking dan penawaran kepada mitra.
- Verifikasi mitra dan penanganan masa berlaku kredensial.
- Cakupan layanan dan pencocokan berbasis lokasi.
- Pengelolaan pengaduan.
- Mekanisme penghapusan akun dan anonimisasi.
- Rate limiting API dan fungsi terkait audit.

### Aplikasi Pasien
Source Flutter saat ini mencakup antarmuka autentikasi, navigasi beranda, daftar layanan, formulir booking, daftar pesanan, profil, komponen informasi darurat, serta komponen retry dan error.

Keberadaan layar atau komponen tidak otomatis berarti seluruh alur telah lulus pengujian end-to-end.

## 3. Arsitektur dan Teknologi

| Komponen | Teknologi |
|---|---|
| Backend | PHP 8.3+ |
| Framework | Laravel 13 |
| Authentication | Laravel Sanctum |
| Database | PostgreSQL |
| API | REST |
| Patient application | Flutter / Dart |
| Shared components | taran_core |
| Automation | GitHub Actions |

Repository disusun sebagai monorepo yang mencakup backend, aplikasi pasien, shared package, dokumentasi, dan skrip utilitas infrastruktur.

## 4. Status Pengembangan

| Area | Status dalam dokumentasi proyek |
|---|---|
| Fondasi backend | Diimplementasikan; pengujian lokal terdokumentasi |
| REST API | Diimplementasikan; pengujian lokal terdokumentasi |
| Source aplikasi pasien Flutter | Tersedia; validasi berlangsung |
| Shared Dart package | Tersedia |
| Web interfaces | Tingkat implementasi dan pengujian bervariasi |
| Deployment produksi | Belum ditetapkan |
| Rilis produksi aplikasi mobile | Belum disetujui |
| Tinjauan legal dan klinis | Menunggu |
| Penilaian keamanan | Berlangsung |

## 5. Privasi dan Keamanan

Pengembangan menggunakan prinsip kehati-hatian:
- Gunakan data sintetis untuk pengembangan dan pengujian.
- Jangan commit data pasien nyata atau kredensial produksi.
- Tinjau autentikasi, otorisasi, dan akses data.
- Laporkan kerentanan melalui kanal privat sesuai Security Policy repository.

TaranMidwife tidak dipresentasikan sebagai produk siap produksi atau tersertifikasi klinis.

## 6. Referensi

- [Repository dan README](https://github.com/taranrainmaker/taranmidwife)
- [Development Status](https://github.com/taranrainmaker/taranmidwife/blob/main/backend/docs/DEVELOPMENT_STATUS.md)
- [Roadmap](https://github.com/taranrainmaker/taranmidwife/blob/main/ROADMAP.md)
- [Security Policy](https://github.com/taranrainmaker/taranmidwife/blob/main/SECURITY.md)

## 7. Kontak

PT Taran Rainmaker Group  
Email: hallo@taranrainmaker.my.id  
Website: https://taranrainmaker.my.id

© PT Taran Rainmaker Group. All rights reserved.
