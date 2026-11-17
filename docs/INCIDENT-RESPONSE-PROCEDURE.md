# Prosedur Respons Insiden Keamanan Informasi
**PT Taran Rainmaker Group**

| Kendali dokumen | Nilai |
|---|---|
| Kode | TRG-SOP-SEC-002 |
| Versi | 1.0 |
| Status | Draft final untuk pengesahan dan penunjukan PIC |
| Tanggal | 17 November 2026 |

## 1. Tujuan dan Cakupan

Prosedur ini mengatur penerimaan, pencatatan, penanganan, pemulihan, dan evaluasi insiden yang berdampak pada sistem, data, layanan, personel, atau pelanggan perusahaan.

Contoh insiden: akun diambil alih, akses tidak sah, kebocoran data, malware, kehilangan perangkat, secret terungkap, perubahan data tidak sah, gangguan layanan, backup gagal, atau kerentanan kritis.

## 2. Kanal Pelaporan

Laporan awal dapat disampaikan melalui kanal dukungan/komunikasi resmi perusahaan dan diteruskan kepada PIC Keamanan Informasi. Kontak operasional internal, nomor piket, dan kanal eskalasi 24/7 harus ditetapkan dalam lampiran terbatas, bukan dipublikasikan dalam dokumen umum.

Email perusahaan: hallo@taranrainmaker.my.id

## 3. Peran

- **PIC Keamanan Informasi:** koordinator triase, investigasi, bukti, dan laporan.
- **Pemilik Sistem:** isolasi teknis, pemulihan, validasi layanan.
- **PIC Privasi:** menilai keterlibatan data pribadi dan kewajiban pemberitahuan.
- **Direktur:** keputusan eskalasi, sumber daya, komunikasi material, dan persetujuan penutupan insiden besar.
- **Pihak ketiga/penyedia:** dukungan sesuai kontrak dan ruang lingkup akses.

Nama PIC dan pengganti harus ditetapkan secara formal.

## 4. Tahapan Penanganan

1. **Penerimaan:** catat waktu, pelapor, sistem, gejala, dan dampak awal.
2. **Klasifikasi:** nilai kerahasiaan, integritas, ketersediaan, cakupan data, dan jumlah pengguna terdampak.
3. **Containment:** batasi akses, cabut token/credential terdampak, isolasi komponen, atau hentikan fungsi yang berisiko bila diperlukan.
4. **Preservasi bukti:** simpan log, timestamp, versi, dan artefak relevan secara aman; jangan mengubah bukti asli tanpa pencatatan.
5. **Investigasi:** identifikasi vektor, akar masalah, cakupan, dan data yang terdampak.
6. **Eradikasi dan pemulihan:** perbaiki penyebab, rotasi secret, pulihkan dari backup tervalidasi, dan lakukan pengujian.
7. **Komunikasi:** informasikan pelanggan, mitra, regulator, atau subjek data sesuai kontrak dan kewajiban hukum.
8. **Penutupan:** catat dampak, keputusan, bukti, tindakan korektif, pemilik, dan tenggat.
9. **Lessons learned:** evaluasi kontrol dan perbarui prosedur.

## 5. Prioritas

| Prioritas | Contoh | Tindakan |
|---|---|---|
| Kritis | Kebocoran/akses tidak sah data kesehatan skala besar, kompromi privileged account, gangguan luas | Eskalasi segera ke Direktur dan PIC terkait; containment segera |
| Tinggi | Akses tidak sah terbatas, malware pada sistem penting, gangguan layanan utama | Penanganan prioritas dan pembaruan berkala |
| Sedang | Gangguan terbatas atau kerentanan dengan mitigasi sementara | Tindak lanjut terjadwal dan pemantauan |
| Rendah | Anomali tanpa bukti dampak material | Dicatat, dianalisis, dan ditutup dengan alasan |

Target waktu respons kontraktual mengikuti SLA yang berlaku; angka target tidak ditetapkan oleh SOP ini.

## 6. Insiden Data Pribadi

Jika insiden melibatkan data pribadi, PIC Privasi harus menilai jenis data, subjek terdampak, akibat, pengendali/prosesor yang terlibat, dan kewajiban pemberitahuan. Tenggat dan isi pemberitahuan mengikuti ketentuan hukum yang berlaku dan peran para pihak. Jangan menunda eskalasi sambil menunggu seluruh investigasi selesai.

## 7. Catatan Insiden

Setiap insiden memiliki nomor unik dan catatan minimal:
- waktu diketahui dan dilaporkan;
- pelapor dan sistem terdampak;
- klasifikasi dan alasan;
- tindakan containment;
- bukti yang diamankan;
- dampak dan pihak terdampak;
- komunikasi dan keputusan;
- tindakan pemulihan;
- akar masalah dan pencegahan;
- persetujuan penutupan.

Log insiden harus disimpan dengan akses terbatas.

## 8. Latihan dan Peninjauan

Prosedur diuji melalui tabletop exercise atau simulasi yang terdokumentasi. Hasil latihan, temuan, dan perbaikan dicatat. Frekuensi latihan ditetapkan Direktur/PIC.

## 9. Pengesahan

Disetujui oleh: **Direktur PT Taran Rainmaker Group**

Nama: ______________________________

Tanda tangan: ________________________

Tanggal pengesahan: __________________

© PT Taran Rainmaker Group. All rights reserved.
