# Operational Evidence Checklist
## TaranPx SaaS, Privacy, and TaranSignature PSrE Partner

Dokumen kerja ini digunakan untuk mengumpulkan bukti sebelum memperbarui klaim operasional atau menerbitkan kebijakan final. Jangan masukkan password, token, private key, data pasien, atau informasi rahasia pelanggan ke repositori publik.

## A. TaranPx — Backup Harian

- [ ] Konfigurasi jadwal backup (screenshot yang telah disamarkan atau export konfigurasi tanpa secret).
- [ ] Cakupan backup: database, dokumen/file, konfigurasi penting.
- [ ] Lokasi penyimpanan dan pemisahan dari produksi.
- [ ] Retensi dan prosedur penghapusan.
- [ ] Enkripsi dan pembatasan akses.
- [ ] Log keberhasilan/kegagalan beberapa hari terakhir.
- [ ] Notifikasi jika backup gagal.
- [ ] Hasil uji restore terakhir.
- [ ] RPO/RTO yang tercantum dalam SLA.

**Bukti yang diperlukan:** konfigurasi scheduler, log backup, kebijakan retensi, dan catatan uji restore. Redaksi publik baru boleh menyatakan “backup harian berhasil” setelah bukti log diperiksa.

## B. TaranPx — Dukungan 24/7 dan SLA

- [ ] Salinan SLA terbaru (boleh disamarkan untuk nama, harga, kontak, dan data pelanggan).
- [ ] Tanggal berlaku, nomor versi, dan status persetujuan/penandatanganan.
- [ ] Kanal dukungan 24/7 dan prosedur akses di luar jam kerja.
- [ ] Jadwal petugas dan jalur eskalasi.
- [ ] Kategori prioritas insiden.
- [ ] Target respons dan pembaruan status.
- [ ] Target pemulihan/penyelesaian jika dijanjikan.
- [ ] Definisi uptime, pengecualian, dan jadwal pemeliharaan.
- [ ] Kontak dan tanggung jawab masing-masing pihak.

**Bukti yang diperlukan:** SLA terkini dan bukti kesiapan kanal serta jadwal piket. Jangan menambahkan angka target baru di dokumen publik sebelum dicocokkan.

## C. Website — Analytics dan Cookies

- [ ] Nama penyedia analytics dan akun/properti yang digunakan.
- [ ] Daftar script/tag yang aktif di website.
- [ ] Daftar cookies dan identifier yang dipasang.
- [ ] Jenis event dan data yang dikumpulkan.
- [ ] Tujuan penggunaan masing-masing data.
- [ ] Retensi data pada penyedia analytics.
- [ ] Lokasi pemrosesan dan kemungkinan transfer lintas negara.
- [ ] Pengaturan IP masking/anonimisasi jika tersedia.
- [ ] Mekanisme pemberitahuan dan pilihan pengguna yang sesuai.
- [ ] Daftar subprosesor/pihak penerima data.

**Bukti yang diperlukan:** nama vendor, konfigurasi analytics, daftar cookies/tag, dan dokumentasi vendor.

## D. TaranSignature — Mitra PSrE

- [ ] Nama badan hukum mitra PSrE.
- [ ] Nama produk/layanan yang digunakan.
- [ ] Bukti status pengakuan/daftar resmi terkini.
- [ ] Perjanjian kerja sama atau bukti hubungan layanan.
- [ ] Jenis sertifikat/layanan TTE yang digunakan.
- [ ] Bukti integrasi teknis tanpa kredensial rahasia.
- [ ] Alur penerbitan, penandatanganan, dan validasi.
- [ ] Pembagian tanggung jawab jika terjadi kegagalan/insiden.
- [ ] Ketentuan biaya, masa berlaku, dan dukungan mitra.

**Bukti yang diperlukan:** identitas mitra, bukti status resmi, perjanjian atau konfirmasi layanan, serta dokumen integrasi. Rahasia API/private key tidak boleh diunggah.

## E. Cara Menyerahkan Bukti

Kirim atau unggah hanya dokumen yang relevan dan telah disamarkan. Untuk SLA, kontrak, dan bukti mitra, cukup lampirkan salinan yang menghilangkan data pelanggan, harga sensitif, tanda tangan, nomor pribadi, kredensial, dan informasi rahasia yang tidak diperlukan.

## Status

**Terbuka — menunggu bukti perusahaan.** Checklist ini bukan bukti bahwa kontrol telah diterapkan atau kewajiban hukum telah dipenuhi.

Kontak: hallo@taranrainmaker.my.id

© PT Taran Rainmaker Group. All rights reserved.
