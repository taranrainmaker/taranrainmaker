# TaranSignature
## Product Datasheet

**Electronic Document Signing & Verification Platform**

TaranSignature adalah platform pengelolaan dokumen, alur tanda tangan elektronik, dan verifikasi dokumen berbasis QR yang dikembangkan oleh PT Taran Rainmaker Group.

## 1. Informasi Produk

| Item | Keterangan |
|---|---|
| Nama | TaranSignature |
| Pengembang | PT Taran Rainmaker Group |
| Kategori | Pengelolaan dokumen, tanda tangan elektronik, verifikasi |
| Aplikasi | https://e-sign.taranrainmaker.my.id |
| Verifikasi | https://verify.taranrainmaker.my.id |
| Repository | https://github.com/taranrainmaker/taransignature |
| Kontak | hallo@taranrainmaker.my.id |

## 2. Fitur yang Terdokumentasi

- Pengelolaan dokumen.
- Alur tanda tangan dokumen elektronik.
- Verifikasi dokumen berbasis QR Code.
- Verifikasi keaslian dokumen.
- Pengelolaan pengguna, peran, dan hak akses.
- Notifikasi email.

Ruang lingkup fitur, otorisasi penandatangan, jenis tanda tangan, dan kesesuaian terhadap ketentuan tanda tangan elektronik yang berlaku harus dievaluasi secara terpisah. Dokumen ini tidak menyatakan bahwa produk memiliki sertifikasi PSrE atau bahwa seluruh tanda tangan yang dibuat otomatis merupakan tanda tangan elektronik tersertifikasi.

## 3. Teknologi dan Komponen

| Komponen | Teknologi terdokumentasi |
|---|---|
| Application | PHP |
| Database | MySQL / MariaDB |
| Container | Docker |
| Web server | Nginx dan PHP-FPM |
| Dependency management | Composer |
| File storage | Local dan S3-compatible object storage |

## 4. Deployment dan Isolasi

Dokumentasi repository menyebut target deployment NEO App dengan database MySQL khusus dan private S3-compatible object storage.

Panduan deployment menjelaskan konfigurasi serta checklist verifikasi. Konfigurasi deployment tidak dengan sendirinya membuktikan seluruh pengujian end-to-end atau kesiapan produksi.

TaranSignature menggunakan resource database dan storage tersendiri. Jangan menggunakan ulang resource TaranPx.

## 5. Keamanan Dokumen

- Jangan commit .env, config.local.php, kredensial, private key, dump database, atau dokumen pengguna.
- Simpan object storage dalam konfigurasi privat.
- Lindungi akses dokumen melalui otorisasi aplikasi.
- Kelola secret melalui konfigurasi environment hosting.
- Batasi akses database dan storage sesuai kebutuhan.

## 6. Referensi

- [Repository TaranSignature](https://github.com/taranrainmaker/taransignature)
- [NEO App Deployment Guide](https://github.com/taranrainmaker/taransignature/blob/neoapp-deploy-clean/NEOAPP-DEPLOY.md)
- Application: https://e-sign.taranrainmaker.my.id
- Verification: https://verify.taranrainmaker.my.id

## 7. Kontak

PT Taran Rainmaker Group  
Email: hallo@taranrainmaker.my.id  
Website: https://taranrainmaker.my.id

© PT Taran Rainmaker Group. All rights reserved.
