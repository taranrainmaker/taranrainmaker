# TaranPx SaaS Service Framework
## Kerangka Pembahasan Layanan

Dokumen ini merupakan kerangka untuk menyusun penawaran dan perjanjian layanan SaaS TaranPx. Dokumen ini bukan SLA yang telah berlaku dan tidak menetapkan jaminan uptime, waktu respons, RPO, RTO, atau kompensasi.

## 1. Model Layanan

TaranPx terutama disediakan sebagai SaaS pada lingkungan hosting yang dikelola PT Taran Rainmaker Group. Fasilitas kesehatan mengakses aplikasi melalui koneksi yang disepakati. Opsi on-premise dibahas dan didokumentasikan secara terpisah.

## 2. Hal yang Wajib Disepakati

| Area | Hal yang perlu ditetapkan |
|---|---|
| Ruang lingkup | Modul, fitur, lokasi, fasilitas, dan batas penggunaan |
| Akun dan akses | Pembuatan akun, peran, otorisasi, penonaktifan |
| Infrastruktur | Lingkungan hosting, kapasitas, batas penggunaan, dependensi |
| Ketersediaan | Target layanan, jadwal pemeliharaan, pengecualian |
| Dukungan | Kanal, jam layanan, klasifikasi prioritas, eskalasi |
| Backup | Frekuensi, retensi, cakupan, tanggung jawab, pengujian pemulihan |
| Keamanan | Pengendalian akses, pengelolaan secret, logging, penanganan insiden |
| Data | Kepemilikan, tujuan pemrosesan, akses, ekspor, retensi, penghapusan |
| Integrasi | Ruang lingkup, kredensial, dependensi pihak ketiga, penanganan kegagalan |
| Perubahan | Pemberitahuan, jadwal rilis, persetujuan perubahan berdampak |
| Pengakhiran | Ekspor data, masa transisi, penghapusan, dan penutupan akses |

## 3. Dukungan dan Eskalasi

Perjanjian layanan perlu menyebutkan:
- Kanal resmi pelaporan.
- Jam operasional dukungan.
- Kategori insiden dan informasi yang harus disertakan.
- Target respons dan target pembaruan status.
- Proses eskalasi dan penutupan tiket.

Tidak ada target waktu yang dijanjikan oleh dokumen kerangka ini.

## 4. Backup dan Pemulihan

Sebelum layanan digunakan, para pihak perlu menyepakati:
- Data dan konfigurasi yang dicadangkan.
- Frekuensi serta lokasi penyimpanan backup.
- Masa retensi dan pembatasan akses.
- Prosedur uji pemulihan.
- Target RPO/RTO jika disepakati.
- Penanggung jawab dan komunikasi saat pemulihan.

Jangan menyatakan backup atau pemulihan telah diuji sebelum bukti pengujian tersedia.

## 5. Pengelolaan Data

Perjanjian perlu mengatur peran para pihak, instruksi pemrosesan, pembatasan akses, penggunaan subprosesor, retensi, ekspor, pengembalian, dan penghapusan data. Data kesehatan dan data pribadi harus ditangani sesuai ketentuan yang berlaku dan kesepakatan yang relevan.

## 6. Insiden dan Perubahan

Tetapkan jalur komunikasi, penanggung jawab, pencatatan, investigasi, pembaruan status, serta mekanisme pemberitahuan insiden. Perubahan aplikasi atau infrastruktur yang berdampak pada pelanggan harus mengikuti prosedur perubahan yang disepakati.

## 7. Lampiran Komersial per Pelanggan

Setiap penawaran/perjanjian perlu melengkapi:
- Nama fasilitas dan badan hukum pelanggan.
- Paket dan modul yang disepakati.
- Biaya, pajak, masa berlangganan, dan termin pembayaran.
- Kapasitas dan batas penggunaan.
- SLA dan dukungan.
- Ketentuan data dan keamanan.
- Jadwal implementasi dan kriteria penerimaan.
- Penanggung jawab kedua pihak.

## Status Dokumen

**Status: kerangka pembahasan, bukan SLA final.** Dokumen hanya dapat dinaikkan menjadi perjanjian layanan setelah kemampuan operasional, prosedur, kapasitas, dan persetujuan para pihak diverifikasi.

Kontak: hallo@taranrainmaker.my.id

© PT Taran Rainmaker Group. All rights reserved.
