# TaranPx — SATUSEHAT Security Assessment Findings Register
## Ringkasan berdasarkan workbook yang tersedia

| Kendali dokumen | Nilai |
|---|---|
| Sumber | Security_Assessment_SATUSEHAT_Taranhealth_dengan_SS.xlsx |
| Sheet yang dirujuk | Template Vendor SaaS |
| Tanggal file | 27 Oktober 2026 |
| Status | Ringkasan kerja; bukan pengganti workbook resmi |
| Pemilik tindak lanjut | Direksi dan PIC yang ditunjuk |

## 1. Catatan Penting

Dokumen ini merangkum nilai dan catatan pada sheet **Template Vendor SaaS** dari workbook yang tersedia di Library. Nama workbook menggunakan istilah “Taranhealth”; kesesuaian nama/versi tersebut dengan submission TaranPx yang akan diajukan harus dipastikan oleh pemilik proses.

Jangan mengubah skor hanya karena kebijakan baru dibuat. Skor harus mencerminkan kondisi kontrol dan bukti aktual pada saat asesmen diperbarui.

Petunjuk workbook menyatakan:
- Pengguna membuat salinan sebelum mengisi.
- Mengisi sheet sesuai model layanan.
- Tidak mengubah struktur, formula, atau nama sheet.
- Membagikan tautan dengan akses Anyone with the link — Viewer jika diminta.
- Mengunggah hasil penilaian/evidence pada SATUSEHAT Platform.
- Skor 0 berarti kontrol tidak tersedia; untuk kontrol mandatory nilai minimum 1, dan nilai 0 harus diperbaiki sebelum integrasi dapat dilanjutkan.

## 2. Temuan Bernilai 0 pada Template Vendor SaaS

| No. kontrol | Area | Temuan / skor pada workbook |
|---:|---|---|
| 1 | Governance & Legal | Kebijakan keamanan informasi formal — 0 |
| 2 | Governance & Legal | Kebijakan privasi/perlindungan data pribadi formal — 0 |
| 3 | Governance & Legal | NDA personel pengembang/pengelola — 0 |
| 4 | Arsitektur & Network Security | IP allowlist — 0 |
| 5 | Arsitektur & Network Security | Firewall/security group/ACL least privilege — 0 |
| 6 | Arsitektur & Network Security | Pemisahan production, staging, development — 0 |
| 8 | Arsitektur & Network Security | Backup produksi aman, non-public, akses terbatas — 0 |
| 9 | Application Security | Laporan penetration test sesuai cakupan dan periode — 0 |
| 11 | Application Security | Pengelolaan secret di luar source/repository — 0 |
| 14 | API Security | Secure storage/secret manager — 0 |
| 16 | Data Protection | Encryption at rest untuk data sensitif dan backup — 0 |
| 18 | Data Protection | MFA seluruh akun administratif/privileged — 0 |
| 19 | Data Protection | Larangan penggunaan data produksi di development/testing — 0 |
| 20 | Data Protection | Penanggung jawab pelindungan data pribadi — 0 |
| 21 | Monitoring & Incident Response | Centralized/managed logging dengan retensi minimal 90 hari — 0 |
| 22 | Monitoring & Incident Response | Monitoring akses data sensitif/anomali — 0 |
| 23 | Monitoring & Incident Response | Uji Disaster Recovery berkala — 0 |
| 24 | Monitoring & Incident Response | PIC keamanan informasi dan respons insiden — 0 |

## 3. Temuan Bernilai 1 pada Template Vendor SaaS

| No. kontrol | Area | Catatan workbook |
|---:|---|---|
| 7 | Arsitektur & Network Security | Ada screenshot log transaksi FHIR; bukti terbatas pada log aplikasi, retensi dan akses perlu diverifikasi |
| 10 | Application Security | Hashing password perlu diverifikasi dari source code; tampilan login bukan bukti algoritma |
| 12 | Secure Development | composer.json dan composer.lock tersedia; SBOM formal belum ditemukan |
| 13 | API Security | Screenshot UI tidak membuktikan secret tidak hardcoded; arsip lama memuat .deploy.env sehingga audit/rotasi secret diminta |
| 15 | API Security | Ada model/migration log sinkronisasi API; kelengkapan log dan tidak adanya data sensitif perlu diverifikasi |
| 17 | Data Protection | Audit trail sudah ada namun belum lengkap |

## 4. Bukti yang Tidak Boleh Disalahartikan

Workbook secara eksplisit membedakan apa yang dapat dan tidak dapat dibuktikan oleh screenshot:
- Screenshot login hanya menunjukkan form login; bukan bukti MFA, rate limiting, session timeout, TLS, atau password hashing.
- Screenshot dashboard log FHIR tidak membuktikan retensi, pembatasan akses, monitoring infrastruktur, atau tidak adanya payload sensitif.
- Screenshot daftar pasien/kunjungan tidak membuktikan enkripsi, consent, access control, atau kepatuhan PDP.
- Screenshot panduan instalasi tidak membuktikan konfigurasi aktual server produksi, firewall, backup, TLS, atau pentest.

Semua screenshot yang memuat data pasien, NIK, nomor rekam medis, IHS ID, data klinis, identifier, atau kredensial harus disamarkan sebelum dibagikan.

## 5. Hubungan dengan Keputusan Direktur

| Keputusan | Cara pencatatan terhadap assessment |
|---|---|
| Backup harian | Dicatat sebagai jadwal yang ditetapkan; skor kontrol backup tetap 0 sampai bukti penyimpanan aman, akses, monitoring, retensi, dan enkripsi dinilai |
| Dukungan 24/7 | Dicatat sebagai keputusan layanan; harus dicocokkan dengan SLA dan roster/kanal operasional |
| SLA tertulis tersedia | Salinan SLA belum diperiksa; jangan menambahkan angka SLA ke dokumen publik sebelum verifikasi |
| Google Analytics | Dicatat pada draft privasi; konfigurasi aktual perlu dipetakan |
| Sertisign | Dicatat sebagai mitra yang dinyatakan perusahaan; status PSrE, badan hukum, perjanjian, dan integrasi harus dibuktikan |

## 6. Urutan Prioritas Tindak Lanjut

1. Sahkan kebijakan keamanan informasi dan kebijakan privasi setelah review.
2. Tunjuk PIC Keamanan Informasi dan PIC Pelindungan Data Pribadi.
3. Pastikan MFA pada seluruh privileged accounts, termasuk akun infrastruktur/hosting.
4. Verifikasi backup harian, keamanan storage, retensi, dan uji restore.
5. Pisahkan environment produksi dan non-produksi; tegaskan larangan data produksi di development/testing.
6. Terapkan firewall/ACL, IP restrictions pada komponen kritis, dan secure secret management.
7. Lengkapi logging, audit trail, retensi 90 hari, dan monitoring akses data sensitif.
8. Lakukan penetration test sesuai cakupan yang diminta dan tutup seluruh temuan.
9. Lakukan DR test dan dokumentasikan hasilnya.
10. Lengkapi NDA, SBOM, perjanjian pemrosesan data, dan bukti vendor/subprosesor.

## 7. Status

**Belum siap dinyatakan memenuhi seluruh kontrol.** Dokumen kebijakan yang dibuat merupakan fondasi governance. Kontrol teknis, bukti, pengujian, penunjukan PIC, dan pembaruan workbook masih diperlukan.

Sumber: workbook asesmen SATUSEHAT yang tersedia pada Library perusahaan. Periksa workbook asli sebelum melakukan perubahan nilai atau mengirim submission.

© PT Taran Rainmaker Group. All rights reserved.
