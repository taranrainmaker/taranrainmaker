# TaranSignature
## Product Datasheet

**Electronic Document Signing & Verification Platform**

TaranSignature adalah platform pengelolaan dokumen, alur tanda tangan elektronik, dan verifikasi dokumen yang dikembangkan oleh PT Taran Rainmaker Group.

## 1. Informasi Produk

| Item | Keterangan |
|---|---|
| Nama | TaranSignature |
| Pengembang | PT Taran Rainmaker Group |
| Kategori | Pengelolaan dokumen, tanda tangan elektronik, verifikasi |
| Aplikasi | https://e-sign.taranrainmaker.my.id |
| Verifikasi | https://verify.taranrainmaker.my.id |
| Repository | https://github.com/taranrainmaker/taransignature |
| Model PSrE | Menggunakan mitra pihak ketiga; perusahaan mengidentifikasi mitra sebagai Sertisign |
| Kontak | hallo@taranrainmaker.my.id |

## 2. Fitur yang Terdokumentasi

- Pengelolaan dokumen.
- Alur tanda tangan dokumen elektronik.
- Verifikasi dokumen berbasis QR Code.
- Verifikasi dokumen.
- Pengelolaan pengguna, peran, dan hak akses.
- Notifikasi email.

Ruang lingkup fitur, otorisasi penandatangan, jenis tanda tangan, dan kesesuaian terhadap ketentuan tanda tangan elektronik harus dievaluasi secara terpisah.

## 3. Mitra PSrE — Sertisign

Perusahaan mengonfirmasi bahwa TaranSignature menggunakan Sertisign sebagai mitra PSrE pihak ketiga.

Identitas badan hukum penyedia, status pengakuan PSrE yang berlaku, nama layanan, hubungan kontraktual, ruang lingkup sertifikat/layanan, dan bukti integrasi belum diverifikasi secara independen dalam dokumen ini.

Sebelum klaim layanan tersertifikasi dipublikasikan, lengkapi:
- Nama badan hukum dan nama resmi layanan Sertisign.
- Bukti status PSrE dan pengakuan resmi yang masih berlaku.
- Perjanjian, kontrak layanan, atau bukti hubungan kerja sama.
- Jenis layanan dan sertifikat elektronik yang benar-benar digunakan.
- Bukti integrasi teknis dan alur penandatanganan/validasi.
- Pembagian tanggung jawab, dukungan, biaya, dan penanganan insiden.

**Batas klaim:** PT Taran Rainmaker Group/TaranSignature tidak menyatakan dirinya sebagai PSrE atau penerbit sertifikat elektronik. Klaim bahwa TTE tersertifikasi disediakan melalui mitra hanya digunakan setelah badan hukum, status, dan alur layanan mitra diverifikasi. QR verification tidak dengan sendirinya membuktikan sertifikat elektronik atau keabsahan semua dokumen.

## 4. Teknologi dan Komponen

| Komponen | Teknologi terdokumentasi |
|---|---|
| Application | PHP |
| Database | MySQL / MariaDB |
| Container | Docker |
| Web server | Nginx dan PHP-FPM |
| Dependency management | Composer |
| File storage | Local dan S3-compatible object storage |

## 5. Deployment dan Isolasi

Deployment saat ini menggunakan Biznet Gio NEO App, managed MySQL, dan S3-compatible object storage privat berdasarkan catatan handover internal. Bukti konfigurasi produksi dan pengujian harus dipelihara secara internal; jangan mempublikasikan credential atau detail sensitif.

TaranSignature menggunakan resource database dan storage tersendiri. Jangan menggunakan ulang resource TaranPx.

## 6. Keamanan Dokumen

- Jangan commit file konfigurasi yang berisi kredensial, private key, dump database, atau dokumen pengguna.
- Simpan object storage dalam konfigurasi privat.
- Lindungi akses dokumen melalui otorisasi aplikasi.
- Kelola secret melalui konfigurasi environment hosting.
- Batasi akses database dan storage sesuai kebutuhan.

## 7. Referensi

- [Repository TaranSignature](https://github.com/taranrainmaker/taransignature)
- [NEO App Deployment Guide](https://github.com/taranrainmaker/taransignature/blob/neoapp-deploy-clean/NEOAPP-DEPLOY.md)
- [Permenkominfo No. 11 Tahun 2022](https://jdih.komdigi.go.id/produk_hukum/view/id/833/t/peraturan%2Bmenteri%2Bkomunikasi%2Bdan%2Binformatika%2Bnomor%2B11%2Btahun%2B2022)
- [Portal PSrE Komdigi](https://tte.komdigi.go.id/)

## 8. Kontak

PT Taran Rainmaker Group  
Email: hallo@taranrainmaker.my.id  
Website: https://taranrainmaker.my.id

© PT Taran Rainmaker Group. All rights reserved.
