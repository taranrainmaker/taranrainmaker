# Kebijakan Keamanan Informasi
**PT Taran Rainmaker Group**

| Kendali dokumen | Nilai |
|---|---|
| Kode | TRG-POL-SEC-001 |
| Versi | 1.0 |
| Status | Draft final untuk pengesahan Direktur |
| Pemilik | Direksi |
| Tanggal penyusunan | 17 November 2026 |
| Tanggal berlaku | Diisi setelah pengesahan |

## 1. Pernyataan Kebijakan

PT Taran Rainmaker Group berkomitmen melindungi kerahasiaan, integritas, dan ketersediaan informasi perusahaan, pelanggan, mitra, serta pengguna layanan. Kebijakan ini menjadi acuan bagi Direksi, karyawan, tenaga kontrak, konsultan, dan pihak ketiga yang memperoleh akses terhadap informasi atau sistem perusahaan.

Kebijakan ini berlaku untuk aktivitas pengembangan, pengoperasian, dukungan, pemeliharaan, dan penyediaan produk/layanan digital perusahaan, termasuk TaranPx dan TaranSignature, sesuai ruang lingkup tanggung jawab masing-masing pihak.

## 2. Tujuan

1. Menetapkan tanggung jawab keamanan informasi.
2. Melindungi data pribadi, data kesehatan, kredensial, dokumen, dan aset informasi.
3. Mengatur kontrol akses, pengembangan aman, pencatatan aktivitas, backup, dan respons insiden.
4. Menyediakan dasar evaluasi dan perbaikan berkelanjutan.

## 3. Prinsip Umum

- Need-to-know dan least privilege.
- Akun individual; dilarang berbagi akun.
- Pemisahan tugas dan lingkungan sejauh dapat diterapkan.
- Data produksi tidak digunakan untuk pengembangan/pengujian kecuali ada dasar, persetujuan, dan perlindungan yang sesuai; utamakan data sintetis atau anonim.
- Secret, private key, token, dan password tidak boleh disimpan dalam source code atau repositori.
- Data sensitif tidak boleh dimasukkan ke log secara berlebihan.
- Perubahan sistem harus dapat ditelusuri dan diuji sesuai risiko.
- Vendor/subprosesor ditinjau berdasarkan kebutuhan dan risiko.

## 4. Tata Kelola dan Tanggung Jawab

**Direktur**
- Menyetujui kebijakan dan toleransi risiko.
- Menunjuk PIC keamanan informasi dan PIC pelindungan data pribadi.
- Menyediakan sumber daya untuk kontrol dan tindak lanjut temuan.
- Meninjau insiden material dan status perbaikan.

**PIC Keamanan Informasi**
- Mengkoordinasikan inventaris aset, kontrol akses, pemantauan, kerentanan, dan insiden.
- Menyimpan bukti pelaksanaan kontrol.
- Melaporkan temuan dan status perbaikan kepada Direktur.

**Pemilik Sistem / Pengelola Produk**
- Menjaga konfigurasi, akses, perubahan, backup, dan dokumentasi sistem.
- Memastikan pemisahan environment dan pengujian perubahan.
- Mengelola akses vendor dan mencabut akses yang tidak lagi diperlukan.

**Seluruh personel dan pihak ketiga**
- Menjaga kerahasiaan.
- Menggunakan akses hanya untuk tujuan yang disetujui.
- Segera melaporkan kehilangan perangkat, dugaan kebocoran, akses tidak sah, atau kerentanan.

Nama PIC dan surat penunjukan formal wajib ditetapkan terpisah; kebijakan ini tidak otomatis menunjuk orang tertentu.

## 5. Kontrol Akses dan Autentikasi

- Akses diberikan berdasarkan peran dan kebutuhan kerja.
- Akun administratif/privileged wajib dilindungi MFA.
- Akses harus ditinjau berkala dan dicabut saat tidak lagi diperlukan.
- Akun bersama dilarang kecuali ada kebutuhan teknis terdokumentasi dan kontrol kompensasi.
- Password harus disimpan menggunakan password hashing yang kuat; tidak plaintext atau reversible encryption.
- Akses remote dan akses vendor harus dibatasi, dicatat, dan diamankan.

## 6. Pengembangan dan Pengelolaan Perubahan

- Gunakan repositori privat untuk source code yang belum dipublikasikan.
- Aktifkan pemeriksaan dependency dan secret scanning bila tersedia.
- Catat versi dependency dan lakukan pembaruan keamanan.
- Perubahan produksi harus melalui review, pengujian, persetujuan, dan rencana rollback yang proporsional.
- Lakukan pengujian keamanan aplikasi dan jaringan sebelum integrasi/go-live sesuai persyaratan yang berlaku.
- Temuan keamanan harus dicatat, diprioritaskan, diperbaiki, dan diuji ulang.

## 7. Logging dan Monitoring

Sistem harus mencatat aktivitas relevan seperti autentikasi, perubahan hak akses, perubahan konfigurasi, transaksi API, dan aktivitas administratif. Log harus dilindungi dari perubahan/penghapusan tidak sah, memiliki retensi yang ditetapkan, dan tidak memuat password, token, private key, atau payload kesehatan yang tidak diperlukan.

Retensi log, sentralisasi, alerting, serta pemantauan akses data sensitif harus ditetapkan dalam standar operasional dan dibuktikan secara teknis.

## 8. Perlindungan Data

- Data diklasifikasikan sesuai sensitivitas.
- Data kesehatan dan data pribadi diproses hanya untuk tujuan yang sah dan sesuai peran para pihak.
- Enkripsi saat transit dan saat tersimpan diterapkan sesuai kemampuan sistem dan penilaian risiko.
- Backup data sensitif harus terlindungi, tidak publik, dan aksesnya dibatasi.
- Retensi, pengembalian, dan penghapusan data harus mengikuti perjanjian dan ketentuan yang berlaku.
- NDA/komitmen kerahasiaan harus diterapkan kepada personel yang memerlukan akses.

## 9. Backup, Kesinambungan, dan Pemulihan

Untuk TaranPx SaaS, keputusan operasional perusahaan adalah backup harian. Cakupan, retensi, enkripsi, lokasi, monitoring, uji restore, RPO, dan RTO harus didokumentasikan dan diverifikasi. Backup harian tidak dianggap bukti keberhasilan pemulihan.

Uji disaster recovery harus direncanakan dan hasilnya disimpan. Prosedur rinci tersedia pada dokumen Backup & Recovery setelah ditetapkan.

## 10. Pengelolaan Insiden

Insiden keamanan harus dilaporkan segera kepada PIC yang ditunjuk. Penanganan meliputi pencatatan, klasifikasi, pembatasan dampak, pengamanan bukti, pemulihan, analisis akar masalah, pemberitahuan kepada pihak terkait sesuai kewajiban, dan tindakan pencegahan berulang.

## 11. Pihak Ketiga

Akses pihak ketiga harus berdasarkan kebutuhan, perjanjian, kewajiban kerahasiaan, batas akses, dan evaluasi risiko. Subprosesor dan penyedia layanan yang memproses data harus diinventarisasi.

## 12. Kepatuhan dan Pengecualian

Pelanggaran kebijakan ditangani sesuai ketentuan internal dan perjanjian yang berlaku. Pengecualian harus memiliki alasan, pemilik risiko, kontrol kompensasi, masa berlaku, dan persetujuan Direktur.

## 13. Peninjauan

Kebijakan ditinjau minimal setahun sekali atau ketika terjadi perubahan material pada produk, infrastruktur, regulasi, atau risiko.

## 14. Pengesahan

Dokumen ini disiapkan sebagai naskah kebijakan perusahaan dan menunggu pengesahan formal.

Disetujui oleh: **Direktur PT Taran Rainmaker Group**

Nama: ______________________________

Tanda tangan: ________________________

Tanggal pengesahan: __________________

Tanggal berlaku: _____________________

## Catatan implementasi

Pengesahan dokumen tidak membuktikan bahwa seluruh kontrol teknis telah aktif. Bukti implementasi harus dilampirkan pada matriks kontrol dan asesmen keamanan secara terpisah.

© PT Taran Rainmaker Group. All rights reserved.
