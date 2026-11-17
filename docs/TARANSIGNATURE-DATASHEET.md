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
| Kontak | hallo@taranrainmaker.my.id |

## 2. Fitur yang Terdokumentasi

- Pengelolaan dokumen.
- Alur tanda tangan dokumen elektronik.
- Verifikasi dokumen berbasis QR Code.
- Verifikasi keaslian dokumen.
- Pengelolaan pengguna, peran, dan hak akses.
- Notifikasi email.

Ruang lingkup fitur, otorisasi penandatangan, jenis tanda tangan, dan kesesuaian terhadap ketentuan tanda tangan elektronik yang berlaku harus dievaluasi secara terpisah.

## 3. Integrasi PSrE Pihak Ketiga — Perlu Verifikasi

Perusahaan menyampaikan bahwa model TaranSignature menggunakan mitra PSrE pihak ketiga.

Informasi tersebut dicatat sebagai model kerja sama yang dinyatakan perusahaan. Namun, identitas mitra, status pengakuan, ruang lingkup layanan, dan bukti integrasi belum diverifikasi dalam dokumen ini.

Sebelum dipublikasikan sebagai klaim komersial, lengkapi:
- Nama badan hukum dan nama layanan PSrE mitra.
- Bukti status PSrE dan status pengakuan yang masih berlaku.
- Perjanjian/otorisasi kerja sama atau bukti hubungan layanan.
- Jenis layanan yang digunakan (misalnya penerbitan sertifikat elektronik atau layanan TTE).
- Alur integrasi teknis dan pembagian tanggung jawab.
- Cara validasi sertifikat, status tanda tangan, dan bukti audit.
- Batasan layanan, biaya, dan ketergantungan pada pihak mitra.

**Batas klaim:** TaranSignature tidak boleh disebut sebagai PSrE atau penerbit sertifikat elektronik milik sendiri. Klaim bahwa TTE tersertifikasi disediakan melalui mitra hanya boleh digunakan setelah mitra dan alur layanan diverifikasi. Fitur QR verification tidak dengan sendirinya membuktikan tanda tangan tersertifikasi atau keabsahan semua dokumen.

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

Dokumentasi repository menyebut target deployment NEO App dengan database MySQL khusus dan private S3-compatible object storage.

Panduan deployment menjelaskan konfigurasi serta checklist verifikasi. Konfigurasi deployment tidak dengan sendirinya membuktikan seluruh pengujian end-to-end atau kesiapan produksi.

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
- [Portal PSrE Komdigi](https://tte.komdigi.go.id/)
- [Permenkominfo No. 11 Tahun 2022](https://jdih.komdigi.go.id/produk_hukum/view/id/833/t/peraturan%2Bmenteri%2Bkomunikasi%2Bdan%2Binformatika%2Bnomor%2B11%2Btahun%2B2022)

## 8. Kontak

PT Taran Rainmaker Group  
Email: hallo@taranrainmaker.my.id  
Website: https://taranrainmaker.my.id

© PT Taran Rainmaker Group. All rights reserved.
