# TaranPx SaaS Service Framework
## Kerangka Operasional dan Verifikasi Layanan

Dokumen ini mencatat keputusan Direktur dan kerangka layanan TaranPx. Rincian operasional mengacu pada dokumen SLA dan bukti internal yang berlaku.

## 1. Model Layanan

TaranPx terutama disediakan sebagai SaaS pada lingkungan hosting yang dikelola PT Taran Rainmaker Group. Opsi on-premise memiliki pembagian tanggung jawab berbeda dan harus disepakati per implementasi.

## 2. Komitmen Perusahaan

| Area | Ketetapan perusahaan | Acuan bukti |
|---|---|---|
| Backup SaaS | Harian | Konfigurasi, log, retensi, storage, akses, enkripsi, dan restore test |
| Dukungan pelanggan | 24 jam/7 hari | SLA, kanal dukungan, roster, tiket, dan eskalasi |
| SLA | Dokumen tertulis dinyatakan tersedia | Gunakan salinan versi berlaku yang disetujui |
| Website analytics | Google Analytics | Property, tag/cookies, event, retensi, dan disclosure |

## 3. Dukungan 24/7

Dukungan pelanggan 24/7 merupakan ketetapan layanan perusahaan. Operasionalnya dijalankan melalui kanal dan tata cara yang tercantum pada SLA serta prosedur dukungan internal. Pencatatan tiket, prioritas, eskalasi, dan komunikasi pelanggan harus mengikuti prosedur tersebut.

## 4. Backup Harian dan Pemulihan

Perusahaan menetapkan backup TaranPx SaaS dilakukan setiap hari. Pelaksanaan, keamanan penyimpanan, dan pemulihan dikelola sesuai prosedur backup internal. Bukti yang menjadi acuan assessment mencakup:
- Scheduler, zona waktu, dan cakupan backup.
- Database, file/dokumen, dan konfigurasi yang diperlukan untuk pemulihan.
- Lokasi penyimpanan terpisah, non-public, serta pembatasan akses.
- Enkripsi, retensi, dan penghapusan.
- Log sukses/gagal dan notifikasi.
- Hasil uji restore.
- RPO/RTO sesuai SLA.

## 5. SLA

Perusahaan menyatakan SLA tertulis tersedia. Seluruh angka dan komitmen layanan—termasuk uptime, target respons, pemulihan, retensi, RPO/RTO, pemeliharaan, dan pengecualian—mengikuti versi SLA yang berlaku. Jangan membuat angka atau komitmen tambahan di luar dokumen tersebut.

## 6. Pengelolaan Data dan Insiden

Pemrosesan data, akses, subprosesor, retensi, ekspor, pengembalian, penghapusan, serta penanganan insiden mengikuti kebijakan dan perjanjian yang berlaku. Data kesehatan dan data pribadi harus ditangani sesuai ketentuan yang berlaku dan prinsip minimisasi akses.

## 7. Pernyataan dan Batas Klaim

- Backup harian: ketetapan perusahaan.
- Dukungan 24/7: ketetapan layanan perusahaan.
- SLA: dinyatakan tersedia oleh perusahaan; gunakan versi resmi yang berlaku.
- Google Analytics: penyedia analytics yang dinyatakan digunakan perusahaan.
- Status kontrol teknis dan nilai SATUSEHAT: mengikuti hasil pemeriksaan bukti pada workbook; tidak berubah otomatis karena dokumen ini.

## Status

Kerangka layanan diperbarui berdasarkan arahan Direktur. Untuk evidence pack dan assessment, gunakan [TaranPx SATUSEHAT Assessment Findings](TARANPX-SATUSEHAT-ASSESSMENT-FINDINGS.md) dan [Operational Evidence Register](OPERATIONAL-EVIDENCE-CHECKLIST.md).

Kontak: hallo@taranrainmaker.my.id

© PT Taran Rainmaker Group. All rights reserved.
