# Prosedur Backup dan Pemulihan Data
**TaranPx SaaS — PT Taran Rainmaker Group**

| Kendali dokumen | Nilai |
|---|---|
| Kode | TRG-SOP-OPS-003 |
| Versi | 1.0 |
| Status | Draft operasional — perlu verifikasi konfigurasi aktual |
| Keputusan jadwal | Backup harian |
| Tanggal | 17 November 2026 |

## 1. Tujuan

Menetapkan tata cara backup dan pemulihan untuk mengurangi risiko kehilangan data serta memastikan proses pemulihan dapat diuji dan dipertanggungjawabkan.

## 2. Pernyataan Jadwal

Keputusan awal perusahaan adalah melakukan backup data TaranPx SaaS setiap hari. Pernyataan ini mencatat kebijakan jadwal yang dikonfirmasi Direktur; bukan bukti bahwa setiap backup telah berhasil, terenkripsi, atau dapat dipulihkan.

## 3. Cakupan yang Harus Ditentukan

Inventaris backup harus menetapkan apakah komponen berikut termasuk:
- Database produksi.
- File/dokumen yang diunggah.
- Konfigurasi aplikasi yang diperlukan untuk pemulihan.
- Artefak integrasi dan konfigurasi operasional yang tidak mengandung secret terbuka.
- Metadata penting untuk konsistensi pemulihan.

Jangan memasukkan file sementara, cache, atau secret yang tidak diperlukan.

## 4. Pelaksanaan Backup

- Jalankan backup harian melalui mekanisme terjadwal yang disetujui.
- Gunakan akun layanan dengan hak minimum.
- Simpan backup pada lokasi yang tidak terbuka untuk publik dan terpisah dari akses pengguna aplikasi.
- Terapkan enkripsi dan kontrol akses sesuai kemampuan platform.
- Catat waktu mulai/selesai, cakupan, ukuran, hasil, dan status.
- Beri notifikasi kepada petugas jika job gagal.
- Jangan menghapus backup sebelum masa retensi dan prosedur penghapusan disetujui.

## 5. Monitoring dan Kegagalan

Petugas memeriksa status job dan menindaklanjuti kegagalan. Kegagalan harus dicatat, diselidiki, dijalankan ulang setelah penyebab ditangani, dan dieskalasikan jika memengaruhi kemampuan pemulihan.

## 6. Uji Restore

- Tetapkan lingkungan pemulihan yang aman.
- Gunakan salinan backup yang dipilih dan catat identitas/timestamp-nya.
- Pulihkan database dan file terkait sesuai urutan teknis.
- Validasi konsistensi data, fungsi aplikasi, integritas dokumen, dan akses.
- Catat durasi, hasil, masalah, dan tindakan korektif.
- Jangan melakukan uji restore yang berisiko pada produksi tanpa persetujuan dan rencana rollback.

## 7. Retensi, RPO, dan RTO

Masa retensi, Recovery Point Objective (RPO), dan Recovery Time Objective (RTO) harus mengikuti SLA dan hasil analisis risiko. Nilai belum dicantumkan di SOP ini karena salinan SLA belum diperiksa.

## 8. Bukti Minimum

- Konfigurasi scheduler dan zona waktu.
- Log backup sukses/gagal.
- Cakupan dan lokasi penyimpanan.
- Konfigurasi akses dan enkripsi.
- Kebijakan retensi.
- Catatan uji restore.
- Persetujuan RPO/RTO.
- Penanggung jawab dan eskalasi.

## 9. Catatan terhadap SATUSEHAT Assessment

Workbook asesmen yang tersedia menilai kontrol backup SaaS dan perlindungan data sebagai belum terpenuhi pada beberapa butir. Konfirmasi jadwal backup harian tidak mengubah skor tersebut. Nilai baru dapat diperbarui setelah bukti konfigurasi, keamanan penyimpanan, akses terbatas, monitoring, retensi, dan pemulihan diverifikasi.

## 10. Pengesahan

Disetujui oleh: **Direktur PT Taran Rainmaker Group**

Nama: ______________________________

Tanda tangan: ________________________

Tanggal pengesahan: __________________

© PT Taran Rainmaker Group. All rights reserved.
