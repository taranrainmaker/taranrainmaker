# TaranPx — Technical Overview

Dokumen ini memberikan gambaran teknis tingkat tinggi mengenai TaranPx berdasarkan dokumentasi produk yang tersedia. Dokumen ini bukan spesifikasi lengkap, dokumen arsitektur rinci, pernyataan hasil audit keamanan, atau Service Level Agreement (SLA).

## 1. Ringkasan Produk

TaranPx adalah Sistem Informasi Manajemen Rumah Sakit (SIMRS) dengan kapabilitas Rekam Medis Elektronik (RME), dikembangkan oleh tim internal PT Taran Rainmaker Group. Pengembangan dimulai pada 2025.

Produk mencakup alur informasi fasilitas kesehatan dan kapabilitas integrasi Satu Sehat menggunakan resource FHIR R4, disertai pencatatan transaksi pengiriman.

## 2. Model Penyediaan Layanan

### SaaS — model utama

TaranPx terutama disediakan sebagai Software as a Service (SaaS). Aplikasi diakses melalui layanan hosting yang dikelola PT Taran Rainmaker Group.

Detail layanan seperti kapasitas, pemisahan lingkungan dan data, backup, pemulihan, pemeliharaan, dukungan, SLA, serta tanggung jawab masing-masing pihak harus ditetapkan dalam dokumen penawaran atau perjanjian layanan. Dokumen ini tidak menetapkan nilai atau jaminan SLA.

### On-premise — opsi tambahan

TaranPx juga memiliki opsi instalasi pada infrastruktur milik fasilitas kesehatan. Panduan instalasi teknis tersedia pada [readmed.md](https://github.com/taranrainmaker/taranpx/blob/main/readmed.md).

Kebutuhan server, konfigurasi, keamanan jaringan, backup, pemeliharaan, dukungan, dan pembagian tanggung jawab harus dievaluasi serta disepakati sebelum implementasi.

## 3. Teknologi Aplikasi

Berdasarkan dokumentasi teknis repositori:

| Komponen | Teknologi |
|---|---|
| Framework aplikasi | Laravel 13 |
| Runtime | PHP 8.3+ |
| Antarmuka | Blade |
| UI framework | Bootstrap 5 |
| Komponen interaksi | SweetAlert2 |
| Integrasi kesehatan | Satu Sehat API dengan resource FHIR R4 |
| Database pada panduan on-premise | MySQL/MariaDB atau SQLite |

Konfigurasi dan kebutuhan aktual dapat berbeda menurut model penyediaan serta versi aplikasi yang diimplementasikan.

## 4. Area Fungsional Terdokumentasi

- Data pasien: Nomor Rekam Medis, NIK, dan IHS ID.
- Kunjungan: rawat jalan, IGD, dan rawat inap.
- Data tenaga kesehatan, unit, lokasi, jadwal dokter, dan master obat KFA.
- Asesmen awal dan detail kunjungan.
- Pemetaan data ke resource FHIR, termasuk Encounter, Condition, Observation, Procedure, MedicationRequest, MedicationDispense, AllergyIntolerance, ServiceRequest, DiagnosticReport, QuestionnaireResponse, dan Composition.
- Monitoring transaksi integrasi, termasuk waktu, method, status HTTP, FHIR ID, serta keterangan kegagalan.
- Peran pengguna aplikasi yang terdokumentasi: admin, dokter, perawat, dan farmasi.
- Kapabilitas Digital Nurse Calling.

Daftar ini merupakan ringkasan area yang tercantum dalam dokumentasi produk; ruang lingkup dan ketersediaan fitur pada implementasi tertentu perlu dikonfirmasi saat demonstrasi.

## 5. Gambaran Alur Data

Alur konseptual yang terdokumentasi:

1. Petugas melakukan pendaftaran pasien.
2. Data kunjungan dicatat pada aplikasi.
3. Data klinis seperti asesmen, diagnosa, dan resep diinput sesuai alur kerja.
4. Data yang relevan dipetakan ke resource FHIR.
5. Proses pengiriman integrasi dijalankan sesuai konfigurasi fasilitas kesehatan.
6. Hasil transaksi dicatat agar proses berhasil atau gagal dapat ditelusuri.

## 6. Integrasi Satu Sehat

Dokumentasi aplikasi mencantumkan penggunaan environment Sandbox/Development untuk pengujian dan Production untuk pertukaran data nyata.

Kredensial seperti Client ID, Client Secret, dan Organization ID harus dikelola secara aman dan dikonfigurasi sesuai fasilitas kesehatan. Kredensial nyata, token, data pasien, dan data produksi tidak boleh dimasukkan ke repositori publik atau materi dokumentasi publik.

Penggunaan Production harus dilakukan setelah konfigurasi, otorisasi, dan kesiapan implementasi diverifikasi oleh pihak yang bertanggung jawab.

## 7. Keamanan dan Pengelolaan Data

Prinsip dokumentasi dan implementasi:

- Jangan menyimpan secret, token, private key, atau kredensial produksi di source control.
- Jangan menggunakan data pasien nyata dalam contoh, issue, atau demonstrasi publik tanpa dasar dan perlindungan yang sesuai.
- Batasi akses berdasarkan peran dan kebutuhan kerja.
- Gunakan HTTPS pada layanan yang diakses melalui jaringan publik.
- Tetapkan prosedur backup, retensi, pemulihan, patching, pemantauan, dan respons insiden sesuai model layanan.
- Untuk SaaS dan on-premise, jelaskan pembagian tanggung jawab pengelolaan infrastruktur dan data sebelum layanan digunakan.

Poin-poin di atas adalah prinsip dan hal yang perlu dikelola; dokumen ini tidak menyatakan bahwa audit independen atau sertifikasi keamanan tertentu telah dilakukan.

## 8. PSE Lingkup Privat

Informasi pendaftaran yang diberikan untuk TaranPx:

- Sistem elektronik: TaranPx
- Kategori: Penyelenggara Sistem Elektronik Lingkup Privat
- Nomor referensi: **023357.01/DJAI.PSE/05/2026**

Nomor tersebut dicantumkan sebagai referensi pendaftaran, bukan sebagai sertifikasi keamanan, hasil audit, atau persetujuan menyeluruh atas seluruh aspek produk.

## 9. Referensi

- [TaranPx README](https://github.com/taranrainmaker/taranpx/blob/main/README.md)
- [Product positioning](https://github.com/taranrainmaker/taranpx/blob/main/PRODUCT.md)
- [Panduan instalasi on-premise](https://github.com/taranrainmaker/taranpx/blob/main/readmed.md)
- [Security policy](https://github.com/taranrainmaker/taranpx/blob/main/SECURITY.md)
- Product access and demonstration: https://px.taranrainmaker.my.id
- Company website: https://taranrainmaker.my.id
- Business contact: hallo@taranrainmaker.my.id

---

**Dokumen informasi teknis tingkat tinggi.** Detail implementasi, konfigurasi, integrasi, keamanan, dan tanggung jawab layanan harus dikonfirmasi untuk setiap proyek.

© PT Taran Rainmaker Group. All rights reserved.
