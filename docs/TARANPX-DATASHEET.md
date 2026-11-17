# TaranPx
## Product Datasheet

**SIMRS • Rekam Medis Elektronik • Digital Nurse Calling**

TaranPx adalah platform Sistem Informasi Manajemen Rumah Sakit (SIMRS) dengan kapabilitas Rekam Medis Elektronik (RME), dikembangkan oleh tim internal PT Taran Rainmaker Group sejak 2025.

<sub>Dokumen ringkasan produk. Ruang lingkup implementasi dan ketersediaan fitur harus dikonfirmasi melalui demonstrasi dan evaluasi kebutuhan.</sub>

## 1. Ringkasan Produk

| Informasi | Keterangan |
|---|---|
| Nama produk | TaranPx |
| Kategori | SIMRS dan RME |
| Pengembang | PT Taran Rainmaker Group |
| Model layanan utama | SaaS |
| Model tambahan | Instalasi on-premise |
| Status | Live dan tersedia untuk demonstrasi |
| Akses produk | https://px.taranrainmaker.my.id |
| Kontak | hallo@taranrainmaker.my.id |

## 2. Model Penyediaan

### SaaS — model utama

Aplikasi disediakan melalui lingkungan hosting yang dikelola PT Taran Rainmaker Group. Fasilitas kesehatan mengakses layanan tanpa perlu mengelola seluruh infrastruktur aplikasi sendiri.

Kapasitas, lingkungan, backup, retensi, dukungan, pemeliharaan, ketersediaan layanan, dan SLA harus ditentukan dalam penawaran/perjanjian layanan. Dokumen ini tidak menjanjikan angka uptime atau target pemulihan tertentu.

### On-premise — opsi tambahan

TaranPx dapat dievaluasi untuk dipasang pada infrastruktur milik fasilitas kesehatan. Persyaratan server, jaringan, keamanan, database, backup, pemeliharaan, dan tanggung jawab operasional dibahas sebelum implementasi.

Panduan teknis: [Panduan instalasi on-premise](https://github.com/taranrainmaker/taranpx/blob/main/readmed.md).

## 3. Area Fungsional Terdokumentasi

- **Data pasien:** Nomor Rekam Medis, NIK, dan IHS ID.
- **Kunjungan:** rawat jalan, IGD, dan rawat inap.
- **Tenaga kesehatan:** Practitioner ID, unit, lokasi, dan jadwal dokter.
- **Farmasi:** master obat KFA serta alur resep/obat yang terdokumentasi.
- **Rekam medis:** asesmen awal dan detail kunjungan, diagnosa, dan resep.
- **Digital Nurse Calling:** kapabilitas pemanggilan pasien secara digital.
- **Integrasi Satu Sehat:** pemetaan resource FHIR R4 dan monitoring transaksi.

Daftar ini adalah ringkasan kemampuan yang tercantum dalam dokumentasi produk, bukan jaminan bahwa setiap modul telah dikonfigurasi atau tersedia pada setiap paket implementasi.

## 4. Integrasi Satu Sehat

Dokumentasi produk mencantumkan pemetaan resource FHIR R4, termasuk:
- Encounter
- Condition
- Observation
- Procedure
- MedicationRequest
- MedicationDispense
- AllergyIntolerance
- ServiceRequest
- DiagnosticReport
- QuestionnaireResponse
- Composition

Monitoring transaksi mencatat informasi seperti waktu, method, status HTTP, FHIR ID, dan keterangan kegagalan.

Koneksi memerlukan konfigurasi serta kredensial fasilitas kesehatan yang sesuai. Penggunaan environment Production hanya dilakukan dengan otorisasi dan kesiapan yang telah diverifikasi.

## 5. Teknologi

| Komponen | Teknologi terdokumentasi |
|---|---|
| Framework | Laravel 13 |
| Runtime | PHP 8.3+ |
| UI | Blade |
| UI framework | Bootstrap 5 |
| Interaksi | SweetAlert2 |
| Integrasi | Satu Sehat API / FHIR R4 |
| Database panduan on-premise | MySQL/MariaDB atau SQLite |

Konfigurasi aktual dapat berbeda mengikuti versi, model layanan, dan kebutuhan implementasi.

## 6. Pendaftaran PSE

Informasi pendaftaran yang diberikan untuk sistem TaranPx:

- Kategori: Penyelenggara Sistem Elektronik Lingkup Privat.
- Nomor: **023357.01/DJAI.PSE/05/2026**.

Nomor tersebut ditampilkan sebagai referensi pendaftaran sesuai materi yang diberikan, bukan sebagai sertifikasi keamanan, hasil audit independen, atau jaminan kepatuhan menyeluruh.

## 7. Ruang Lingkup Evaluasi Sebelum Implementasi

Hal-hal berikut dibahas bersama calon fasilitas kesehatan:
- Jenis fasilitas dan alur operasional yang dibutuhkan.
- Modul dan fitur yang termasuk dalam ruang lingkup.
- Jumlah pengguna dan kebutuhan akses.
- Migrasi atau input data awal.
- Integrasi dan kredensial yang diperlukan.
- Infrastruktur dan konektivitas.
- Pelatihan, dukungan, dan pemeliharaan.
- Backup, retensi, keamanan, dan tanggung jawab pengelolaan data.
- Jadwal, biaya, kriteria penerimaan, dan ketentuan layanan.

## 8. Keamanan dan Privasi

Data kesehatan dan informasi pribadi harus ditangani sesuai kewenangan, dasar pemrosesan, dan pengamanan yang relevan. Data pasien nyata, kredensial, token, serta konfigurasi produksi tidak boleh dimasukkan ke repositori atau materi demonstrasi publik.

Rincian kontrol keamanan dan tanggung jawab operasional harus dikonfirmasi untuk model SaaS atau on-premise yang dipilih.

## 9. Demo dan Informasi

- **Akses produk:** https://px.taranrainmaker.my.id
- **Website perusahaan:** https://taranrainmaker.my.id
- **Email:** hallo@taranrainmaker.my.id
- **Repositori produk:** https://github.com/taranrainmaker/taranpx

Untuk meminta demonstrasi atau penawaran, sertakan nama fasilitas kesehatan, PIC, dan gambaran kebutuhan.

---

**PT Taran Rainmaker Group**  
Technology • Digital Solutions • Integrated Systems

© PT Taran Rainmaker Group. All rights reserved.
