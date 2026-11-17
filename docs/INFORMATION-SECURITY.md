# Information Security Principles

Dokumen ini menjelaskan prinsip umum yang menjadi acuan dalam pembahasan dan pelaksanaan pekerjaan teknologi informasi PT Taran Rainmaker Group. Dokumen ini bukan pernyataan bahwa perusahaan telah memperoleh sertifikasi keamanan, menyelesaikan audit independen, atau menerapkan seluruh kontrol teknis pada setiap sistem.

## 1. Kerahasiaan Informasi

- Informasi pelanggan, mitra, dan perusahaan diperlakukan sesuai sifat dan kewajiban kerahasiaannya.
- Informasi hanya dibagikan kepada pihak yang memiliki kebutuhan dan kewenangan.
- Data rahasia tidak boleh dimasukkan ke repositori publik, materi demo publik, atau kanal komunikasi yang tidak sesuai.

## 2. Pengelolaan Akses

- Akses sistem seharusnya diberikan berdasarkan kebutuhan tugas dan kewenangan.
- Kredensial tidak boleh dibagikan atau ditanamkan pada source code.
- Akses yang tidak lagi diperlukan perlu ditinjau dan dicabut melalui prosedur yang berlaku.
- Penggunaan autentikasi tambahan dan kontrol akses ditentukan berdasarkan risiko serta kebutuhan sistem.

## 3. Perlindungan Data

- Data pribadi dan data kesehatan memerlukan penanganan yang berhati-hati.
- Gunakan data dummy atau data yang telah dianonimkan untuk demonstrasi dan pengujian bila memungkinkan.
- Penggunaan data nyata harus memiliki dasar, otorisasi, dan perlindungan yang sesuai.
- Data tidak boleh dipindahkan ke lingkungan lain tanpa persetujuan dan kontrol yang diperlukan.

## 4. Secret dan Konfigurasi

Jangan pernah melakukan commit terhadap:
- Password, token, API key, Client Secret, atau private key.
- File konfigurasi produksi yang berisi kredensial.
- Dump database atau backup yang berisi data pribadi.
- Log yang memuat data sensitif.

Gunakan mekanisme penyimpanan secret yang sesuai dengan lingkungan implementasi. Jika secret terungkap, lakukan penilaian dampak dan rotasi melalui prosedur yang berlaku.

## 5. Pengembangan dan Perubahan Sistem

- Perubahan sistem perlu ditinjau sesuai risiko dan dampaknya.
- Pengujian dilakukan sebelum perubahan diterapkan ke lingkungan produksi.
- Perubahan yang berisiko perlu memiliki rencana pemulihan.
- Dependensi dan komponen pihak ketiga perlu dipertimbangkan dalam pemeliharaan.
- Akses produksi harus dibatasi dan dapat dipertanggungjawabkan.

## 6. Operasional Layanan

Untuk setiap proyek atau layanan, para pihak perlu menetapkan sesuai ruang lingkup:
- Penanggung jawab operasional.
- Pemantauan dan pencatatan kejadian.
- Backup, retensi, dan pengujian pemulihan.
- Patch dan pemeliharaan.
- Penanganan insiden dan jalur eskalasi.
- Pengelolaan akses pengguna.
- Tanggung jawab penyedia dan pelanggan.

Untuk TaranPx SaaS dan on-premise, pembagian tanggung jawab dapat berbeda dan perlu dituangkan dalam dokumen layanan.

## 7. Pelaporan Isu Keamanan

Laporkan dugaan kerentanan atau insiden melalui email resmi: hallo@taranrainmaker.my.id.

Sertakan deskripsi ringkas, dampak yang diamati, langkah reproduksi yang aman, serta informasi kontak pelapor. Jangan menyertakan data pasien nyata, password, token, atau rahasia lain dalam laporan awal.

Hindari pengujian yang dapat mengganggu layanan, mengakses data pihak lain, atau mengubah/menghapus data tanpa izin tertulis.

## 8. Batas Dokumen

Dokumen ini adalah pernyataan prinsip dan panduan umum. Persyaratan teknis yang mengikat, kontrol yang diterapkan, tanggung jawab operasional, waktu respons, dan kewajiban pelaporan harus ditetapkan pada dokumen proyek atau perjanjian layanan yang relevan.

Dokumen ini tidak boleh digunakan sebagai bukti sertifikasi, audit, penetration test, atau kepatuhan menyeluruh.

© PT Taran Rainmaker Group. All rights reserved.
