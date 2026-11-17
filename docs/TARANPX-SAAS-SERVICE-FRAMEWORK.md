# TaranPx SaaS Service Framework
## Kerangka Operasional dan Verifikasi Layanan

Dokumen ini mencatat keputusan awal perusahaan untuk layanan SaaS TaranPx dan hal yang masih harus diverifikasi. Dokumen ini bukan pengganti SLA pelanggan yang telah ditandatangani.

## 1. Model Layanan

TaranPx terutama disediakan sebagai SaaS pada lingkungan hosting yang dikelola PT Taran Rainmaker Group. Opsi on-premise dibahas dan didokumentasikan secara terpisah.

## 2. Keputusan Operasional Awal

| Area | Keputusan awal perusahaan | Status verifikasi |
|---|---|---|
| Backup SaaS | Harian | Jadwal job, cakupan, retensi, lokasi, enkripsi, monitoring, dan bukti keberhasilan perlu diperiksa |
| Dukungan pelanggan | 24 jam / 7 hari | Kanal, roster petugas, eskalasi, target respons dan pemulihan perlu dicocokkan dengan SLA tertulis |
| SLA | Perusahaan menyatakan SLA tertulis sudah tersedia | Salinan dan versi yang berlaku belum ditelaah dalam dokumentasi ini |
| Pemrosesan data | Mengikuti perjanjian dan peran masing-masing pihak | Data map, subprosesor, retensi, dan prosedur permintaan subjek data perlu dilengkapi |

**Penting:** keputusan backup harian dan dukungan 24/7 adalah informasi yang diberikan perusahaan. Pernyataan ini belum menjadi bukti bahwa backup berhasil setiap hari atau bahwa seluruh target dukungan dalam SLA telah diuji.

## 3. Dukungan 24/7

Perusahaan menetapkan dukungan pelanggan 24 jam sehari dan 7 hari seminggu sebagai keputusan awal layanan.

Hal yang harus dicantumkan atau diverifikasi terhadap SLA yang berlaku:
- Kanal pelaporan resmi dan mekanisme akses di luar jam kerja.
- Kontak eskalasi dan petugas piket.
- Definisi severity/prioritas insiden.
- Target respons awal, pembaruan status, dan pemulihan per kategori.
- Pengecualian, dependensi pihak ketiga, serta prosedur pemeliharaan.
- Pencatatan tiket dan bukti penutupan insiden.

Jangan mengiklankan target menit/jam atau jaminan uptime sebelum nilainya dicocokkan dengan SLA yang berlaku dan kemampuan operasional.

## 4. Backup Harian dan Pemulihan

Keputusan awal perusahaan: backup TaranPx SaaS dilakukan setiap hari.

Checklist bukti operasional:
- [ ] Jadwal dan zona waktu job backup.
- [ ] Cakupan database, file unggahan, konfigurasi, dan komponen terkait.
- [ ] Lokasi penyimpanan dan pemisahan dari lingkungan produksi.
- [ ] Enkripsi saat transit dan saat tersimpan, jika diterapkan.
- [ ] Retensi dan prosedur penghapusan backup.
- [ ] Monitoring job gagal dan notifikasi petugas.
- [ ] Pembatasan akses backup.
- [ ] Uji restore berkala dan catatan hasil.
- [ ] RPO dan RTO yang disepakati pada SLA.

Backup harian tidak otomatis berarti pemulihan telah berhasil diuji. Jangan menyatakan RPO/RTO atau retensi tertentu tanpa bukti dan kesepakatan.

## 5. SLA dan Dokumen Pelanggan

Perusahaan menyatakan telah memiliki SLA tertulis. Sebelum kerangka ini diselaraskan, diperlukan salinan SLA terbaru yang telah disetujui/ditandatangani (boleh disamarkan untuk data pelanggan).

Pastikan perjanjian memuat:
- Ruang lingkup modul dan layanan.
- Definisi ketersediaan dan pengecualian.
- Dukungan 24/7, kanal, prioritas, respons, dan eskalasi.
- Backup harian, retensi, tanggung jawab, dan pengujian restore.
- Keamanan, pengelolaan akses, dan penanganan insiden.
- Peran pengendali/prosesor data, subprosesor, dan instruksi pemrosesan.
- Ekspor, pengembalian, retensi, dan penghapusan data saat layanan berakhir.
- Masa berlaku, perubahan, dan mekanisme persetujuan.

## 6. Pengelolaan Data dan Insiden

Perjanjian perlu mengatur tujuan pemrosesan, instruksi pelanggan, pembatasan akses, penggunaan subprosesor, retensi, ekspor, pengembalian, dan penghapusan data. Data kesehatan dan data pribadi harus ditangani sesuai ketentuan yang berlaku.

Tetapkan jalur komunikasi, penanggung jawab, pencatatan, investigasi, pembaruan status, serta mekanisme pemberitahuan insiden.

## 7. Daftar Verifikasi Sebelum Pernyataan Publik

| Pernyataan | Bukti yang diperlukan |
|---|---|
| Backup harian berjalan | Konfigurasi scheduler dan log sukses terbaru |
| Backup dapat dipulihkan | Catatan uji restore |
| Dukungan 24/7 tersedia | Kanal aktif, jadwal petugas, prosedur eskalasi |
| SLA berlaku | Dokumen SLA terkini dan persetujuan para pihak |
| Target uptime/respons/pemulihan | Klausul SLA dan data monitoring/operasional |

## Status Dokumen

**Status: keputusan awal operasional dicatat; verifikasi bukti masih berlangsung.** Dokumen ini bukan SLA final dan tidak menetapkan angka uptime, target respons, RPO, RTO, atau kompensasi baru.

Kontak: hallo@taranrainmaker.my.id

© PT Taran Rainmaker Group. All rights reserved.
