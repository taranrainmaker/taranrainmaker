# TaranPx — SATUSEHAT Security Assessment Findings Register

## Ringkasan dan dasar pencatatan

| Elemen | Keterangan |
|---|---|
| Sumber assessment | Security_Assessment_SATUSEHAT_Taranhealth_dengan_SS.xlsx |
| Sheet | Template Vendor SaaS |
| Tanggal file sumber | 27 Oktober 2026 |
| Status dokumen | Register tindak lanjut berdasarkan workbook dan pernyataan Direktur |
| Pemilik | Direksi PT Taran Rainmaker Group dan PIC yang ditunjuk |

**Pernyataan manajemen:** atas instruksi Direktur, untuk kelanjutan penyusunan dokumen ini bukti pendukung dianggap tersedia dalam arsip internal perusahaan. Ketersediaan tersebut dicatat sebagai konfirmasi manajemen, bukan sebagai hasil pemeriksaan independen oleh penyusun dokumen. Tim perusahaan harus memasangkan setiap bukti dengan nomor kontrol yang tepat, memeriksa tanggal/versi dan ruang lingkupnya, lalu mengunggahnya melalui kanal assessment resmi.

Nama workbook menggunakan istilah “Taranhealth”. Sebelum submission, pastikan workbook/versi tersebut memang merupakan template dan hasil assessment yang berlaku untuk TaranPx.

## 1. Aturan pengelolaan skor

- Nilai pada workbook adalah nilai yang tercatat saat workbook dibuat/diperbarui.
- Jangan mengubah skor 0 menjadi 1 hanya karena dokumen kebijakan baru dibuat atau karena bukti dinyatakan tersedia.
- Skor hanya diperbarui oleh pemilik assessment setelah bukti aktual ditemukan, relevan, masih berlaku, dan memenuhi definisi kontrol pada workbook.
- Simpan salinan asli, salinan kerja, tanggal pembaruan, pemilik kontrol, serta jejak persetujuan.
- Jangan mengunggah kredensial, private key, token, data pasien, atau data pribadi yang tidak diperlukan.

Petunjuk workbook yang tersedia menyebutkan agar pengguna membuat salinan, mempertahankan struktur/formula/nama sheet, menggunakan sheet sesuai model layanan, dan mengunggah hasil serta evidence ke SATUSEHAT Platform. Ikuti instruksi versi workbook yang benar-benar digunakan pada saat pengajuan.

## 2. Temuan bernilai 0 pada workbook

| No. kontrol | Area | Nilai tercatat |
|---:|---|---|
| 1 | Governance & Legal — kebijakan keamanan informasi formal | 0 |
| 2 | Governance & Legal — kebijakan privasi/perlindungan data pribadi formal | 0 |
| 3 | Governance & Legal — NDA personel pengembang/pengelola | 0 |
| 4 | Arsitektur & Network Security — IP allowlist | 0 |
| 5 | Arsitektur & Network Security — firewall/security group/ACL least privilege | 0 |
| 6 | Arsitektur & Network Security — pemisahan production, staging, development | 0 |
| 8 | Arsitektur & Network Security — backup produksi aman, non-public, akses terbatas | 0 |
| 9 | Application Security — laporan penetration test sesuai cakupan dan periode | 0 |
| 11 | Application Security — pengelolaan secret di luar source/repository | 0 |
| 14 | API Security — secure storage/secret manager | 0 |
| 16 | Data Protection — encryption at rest untuk data sensitif dan backup | 0 |
| 18 | Data Protection — MFA akun administratif/privileged | 0 |
| 19 | Data Protection — larangan penggunaan data produksi di development/testing | 0 |
| 20 | Data Protection — penanggung jawab pelindungan data pribadi | 0 |
| 21 | Monitoring & Incident Response — centralized/managed logging dengan retensi minimal 90 hari | 0 |
| 22 | Monitoring & Incident Response — monitoring akses data sensitif/anomali | 0 |
| 23 | Monitoring & Incident Response — uji Disaster Recovery berkala | 0 |
| 24 | Monitoring & Incident Response — PIC keamanan informasi dan respons insiden | 0 |

## 3. Temuan bernilai 1 pada workbook

| No. kontrol | Area | Catatan yang harus ditindaklanjuti |
|---:|---|---|
| 7 | Arsitektur & Network Security | Ada screenshot log transaksi FHIR; cakupan retensi dan pembatasan akses perlu dicocokkan dengan kontrol |
| 10 | Application Security | Hashing password perlu dibuktikan melalui implementasi/source code |
| 12 | Secure Development | composer.json dan composer.lock tersedia; evaluasi apakah SBOM formal diperlukan |
| 13 | API Security | Periksa pengelolaan secret dan riwayat arsip; lakukan rotasi bila ada indikasi secret pernah terekspos |
| 15 | API Security | Ada model/migration log sinkronisasi API; validasi kelengkapan dan minimisasi data |
| 17 | Data Protection | Audit trail ada namun tercatat belum lengkap |

## 4. Matriks bukti dan status

| Kelompok kontrol | Bukti yang harus dipasangkan dari arsip internal | Status pencatatan |
|---|---|---|
| Governance | Kebijakan disahkan, NDA, surat penunjukan PIC | Dinyatakan tersedia/akan dipasangkan |
| Network security | Konfigurasi firewall/ACL, IP restrictions, diagram environment | Dinyatakan tersedia/akan dipasangkan |
| Backup & recovery | Jadwal, log backup, lokasi/storage, enkripsi, retensi, akses, restore test | Dinyatakan tersedia/akan dipasangkan |
| Application security | Hasil pentest, remediation, password hashing, secure development | Dinyatakan tersedia/akan dipasangkan |
| Secret management | Konfigurasi secret manager, bukti secret tidak tersimpan di repository, rotasi | Dinyatakan tersedia/akan dipasangkan |
| Data protection | Enkripsi at rest, MFA privileged accounts, data masking/non-production | Dinyatakan tersedia/akan dipasangkan |
| Monitoring | Log terpusat, retensi 90 hari, monitoring akses sensitif, audit trail | Dinyatakan tersedia/akan dipasangkan |
| DR | Rencana DR, hasil uji, tindak lanjut | Dinyatakan tersedia/akan dipasangkan |
| Vendor/third party | SLA, DPA/kerahasiaan, daftar subprosesor, bukti Sertisign | Dinyatakan tersedia/akan dipasangkan |

## 5. Keputusan Direktur yang dicatat

- Backup TaranPx SaaS: harian.
- Dukungan pelanggan: 24 jam/7 hari.
- SLA tertulis: dinyatakan tersedia oleh perusahaan.
- Website analytics: Google Analytics.
- TaranSignature: menggunakan Sertisign sebagai mitra penyedia layanan tanda tangan elektronik.

Pernyataan di atas merupakan konfirmasi manajemen. Detail teknis, legal, tanggal berlaku, dan kesesuaian setiap bukti harus mengikuti dokumen sumber yang berlaku. Perusahaan tidak menyatakan PT Taran Rainmaker Group sebagai PSrE.

## 6. Urutan finalisasi

1. Pasangkan bukti untuk setiap nomor kontrol pada workbook.
2. Pastikan bukti masih berlaku dan mencakup lingkungan produksi TaranPx yang dinilai.
3. Tutup gap yang masih nyata; jangan menganggap dokumen kebijakan sebagai pengganti kontrol teknis.
4. Perbarui skor hanya setelah pemilik kontrol menyetujui bukti.
5. Simpan salinan workbook final dan evidence pack dengan kontrol akses yang sesuai.
6. Lakukan pemeriksaan akhir sebelum submission.

## Status

**Evidence availability: dinyatakan tersedia oleh Direktur; pemetaan dan validasi per kontrol menjadi tahap finalisasi internal.** Nilai pada workbook tidak otomatis berubah melalui dokumen ini dan tidak ada pernyataan bahwa SATUSEHAT telah menyetujui assessment.

Kontak: hallo@taranrainmaker.my.id

© PT Taran Rainmaker Group. All rights reserved.
