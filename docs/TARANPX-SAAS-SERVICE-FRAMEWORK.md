# TaranPx SaaS Service Framework
## Kerangka Operasional dan Verifikasi Layanan

Dokumen ini mencatat keputusan Direktur, persyaratan layanan, dan bukti yang masih perlu diverifikasi. Ini bukan pengganti SLA pelanggan yang telah ditandatangani.

## 1. Model Layanan

TaranPx terutama disediakan sebagai SaaS pada lingkungan hosting yang dikelola PT Taran Rainmaker Group. Opsi on-premise memiliki pembagian tanggung jawab yang berbeda dan harus disepakati per implementasi.

## 2. Keputusan Perusahaan

| Area | Keputusan Direktur | Bukti/status |
|---|---|---|
| Backup SaaS | Harian | Jadwal dikonfirmasi; konfigurasi, log sukses, cakupan, retensi, enkripsi, akses, dan restore belum diperiksa |
| Dukungan pelanggan | 24 jam / 7 hari | Keputusan dikonfirmasi; kanal, roster, eskalasi, dan operasional aktual perlu dibuktikan |
| SLA | Perusahaan menyatakan SLA tertulis sudah tersedia | Salinan SLA belum ditemukan/ditelaah dalam berkas asesmen yang diperiksa |
| Website analytics | Google Analytics | Nama penyedia diketahui; property, konfigurasi, cookies, event, dan retensi perlu diperiksa |

## 3. Dukungan 24/7

Dukungan pelanggan 24/7 merupakan keputusan layanan perusahaan. Untuk menyatakan layanan ini benar-benar operasional, siapkan:
- Kanal pelaporan yang dapat diakses setiap saat.
- Jadwal petugas/piket dan pengganti.
- Jalur eskalasi teknis dan manajerial.
- Definisi severity/prioritas.
- Target respons, pembaruan status, dan pemulihan sesuai SLA.
- Sistem pencatatan tiket dan bukti penyelesaian.

Jangan memublikasikan angka waktu respons atau uptime sebelum dicocokkan dengan SLA.

## 4. Backup Harian dan Pemulihan

Perusahaan menetapkan backup TaranPx SaaS dilakukan setiap hari. Pelaksanaan dan hasilnya harus dibuktikan secara terpisah.

Checklist:
- [ ] Scheduler dan zona waktu.
- [ ] Cakupan database, file/dokumen, dan konfigurasi pemulihan.
- [ ] Lokasi penyimpanan terpisah dan tidak publik.
- [ ] Enkripsi backup dan kontrol akses.
- [ ] Retensi dan penghapusan.
- [ ] Log sukses/gagal dan notifikasi.
- [ ] Uji restore dan catatan hasil.
- [ ] RPO/RTO sesuai SLA.

Workbook Security Self-Assessment yang tersedia menilai kontrol penyimpanan backup SaaS sebagai 0 (belum diterapkan/tidak tersedia) dan meminta bukti storage aman, akses terbatas, retensi, monitoring, serta enkripsi jika tersedia. Konfirmasi jadwal harian tidak otomatis mengubah skor ini. Nilai hanya boleh diperbarui setelah bukti aktual dinilai.

## 5. SLA

Direktur mengonfirmasi bahwa SLA tertulis sudah ada. Dokumen SLA aktual belum berhasil diidentifikasi dari berkas asesmen yang diperiksa. Untuk sinkronisasi, perlu salinan versi berlaku yang telah disetujui/ditandatangani (boleh disamarkan).

Periksa ruang lingkup, uptime, pengecualian, dukungan 24/7, target respons, backup, retensi, RPO/RTO, uji pemulihan, keamanan, insiden, peran pengendali/prosesor, subprosesor, ekspor/penghapusan data, dan masa berlaku.

## 6. Pengelolaan Data dan Insiden

Perjanjian harus mengatur tujuan pemrosesan, instruksi pelanggan, pembatasan akses, subprosesor, retensi, ekspor, pengembalian, dan penghapusan data. Data kesehatan dan data pribadi harus ditangani sesuai ketentuan berlaku.

## 7. Status Klaim Publik

| Klaim | Status yang diperbolehkan saat ini |
|---|---|
| Jadwal backup ditetapkan harian | Dapat dicatat sebagai keputusan perusahaan |
| Backup berhasil setiap hari | Belum boleh diklaim tanpa log |
| Backup terenkripsi dan privat | Belum boleh diklaim tanpa konfigurasi |
| Restore telah diuji | Belum boleh diklaim tanpa laporan uji |
| Dukungan 24/7 | Keputusan layanan; bukti roster/kanal masih diperlukan |
| SLA telah ditandatangani | Menunggu pemeriksaan dokumen SLA |
| Uptime/RPO/RTO tertentu | Jangan diklaim sebelum diverifikasi terhadap SLA dan bukti |

## Status

Keputusan operasional dicatat; implementasi dan bukti masih diverifikasi. Gunakan bersama [Backup & Recovery Procedure](BACKUP-AND-RECOVERY-PROCEDURE.md) dan [Operational Evidence Checklist](OPERATIONAL-EVIDENCE-CHECKLIST.md).

Kontak: hallo@taranrainmaker.my.id

© PT Taran Rainmaker Group. All rights reserved.
