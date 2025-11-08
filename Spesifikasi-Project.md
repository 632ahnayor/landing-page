# MODUL STUDI KASUS: LAUNDRYCRAFTY (TEMPLATE)

| Nama | NRP |
| --- | --- |
| Royan Habibi Alfatih | 5025241115 |
| Bara Semangat Rohmani | 5025241144 |

## 1. Deskripsi Umum (masih template)

LaundryCrafty adalah sistem manajemen usaha laundry berbasis web yang membantu pengelola
laundry dalam mengelola transaksi, pelanggan, layanan, dan laporan pendapatan. Aplikasi ini
dirancang untuk mengotomatisasi pencatatan dan pengelolaan data laundry agar lebih cepat,
efisien, dan terintegrasi menggunakan database MySQL.

<br>

## 2. Tujuan Proyek (masih template)
- Mempermudah pengelolaan data pelanggan dan transaksi laundry.
- Mengotomatisasi perhitungan biaya berdasarkan berat cucian atau jenis layanan.
- Menyediakan laporan pendapatan harian, mingguan, dan bulanan.
- Memberikan pengalaman pengguna yang mudah digunakan bagi admin maupun pelanggan.

  
<br>

## 3. Fitur Utama (work in progress)
- Manajemen Pelanggan: Tambah, ubah, hapus, dan lihat data pelanggan.
- Manajemen Layanan: Menyediakan daftar jenis layanan seperti Cuci Kering, Cuci Setrika, dan Express.
- Transaksi Laundry: Input data transaksi pelanggan, jenis layanan, berat, harga, tanggal masuk & selesai.
- Status Cucian: Update status cucian (Proses, Selesai, Sudah Diambil).
- Laporan Keuangan: Menampilkan pendapatan harian, mingguan, dan bulanan.
- Autentikasi Admin: Login dan logout admin untuk keamanan sistem.
- Dashboard Statistik: Tampilan grafik transaksi dan pendapatan.
- Pencarian Data: Mencari pelanggan atau transaksi berdasarkan nama atau tanggal.
- .
- Rating and Review: Pelanggan dapat memberi nilai rating (1-5) dan menambahkan review.
- Konten: Dokumentasi kegiatan, Artikel edukatif, Foto & video lokasi.
- Pemesanan Tiket: Formulir pemesanan tiket untuk kunjungan dan naik perahu.
- Status Tiket: Update status tiket (Aktif, Digunakan, Kadaluarsa)
- 

<br>

## 4. Peran Pengguna (work in progress)
- Admin: Mengelola seluruh data (pelanggan, layanan, transaksi, laporan).
- Kasir/Operator: Input transaksi laundry, memperbarui status, mencetak nota.
- Pelanggan (opsional): Melihat status cucian dan riwayat transaksi melalui login pelanggan.
- .
- Admin: Mengelola seluruh data 
- Operator: Validasi tiket di lokasi
- Pelanggan: Melihat halaman utama dan informasi yang tersedia, Memberi rating dan review, Memesan tiket
 
<br>

## 5. Spesifikasi Teknis (masih template)
- Front-End: HTML5, CSS3, Bootstrap, JavaScript
- Back-End: PHP (versi 8.x)
- Database: MySQL / MariaDB
- Server: Apache (XAMPP / Laragon)
- Tools: VS Code, phpMyAdmin
- Integrasi API (opsional): API laporan JSON untuk akses data transaksi

<br>

## 6. Struktur Database (Tabel Utama) (work in progress)
- Tabel pelanggan: id_pelanggan, nama, alamat, no_hp
- Tabel layanan: id_layanan, nama_layanan, harga_per_kg
- Tabel transaksi: id_transaksi, id_pelanggan, id_layanan, tanggal_masuk, tanggal_selesai, berat, total_harga, status
- Tabel user: id_user, username, password, role
- .
- Tabel pengunjung: id_pengunjung, nama, no_hp, email
- Tabel tiket: id_tiket, id_pengunjung, status
- 

<br>

## 7. Desain Tampilan (Front-End) (work in progress)
- Dashboard: Menampilkan statistik jumlah pelanggan, transaksi, dan grafik pendapatan.
- Halaman Pelanggan: Form tambah pelanggan dan tabel daftar pelanggan.
- Halaman Transaksi: Form input transaksi dan tabel daftar transaksi.
- Halaman Laporan: Laporan pendapatan dengan filter tanggal.
- .
- Landing Page: Menampilkan informasi utama, akses untuk membeli tiket, dan akses untuk memberikan review
- Halaman Pemesanan:
- Halaman Review:
- Halaman Admin: Menampilkan informasi dan akses khusus admin

<br>

## 8. Alur Proses Sistem (work in progress)
- Admin login ke sistem.
- Kasir menambahkan data pelanggan baru (jika belum terdaftar).
- Kasir mencatat transaksi laundry baru.
- Sistem menghitung total harga otomatis.
- Kasir memperbarui status cucian.
- Admin melihat laporan pendapatan.
- .
- Pengunjung dapat melihat informasi tentang objek wisata
- Pengunjung memesan tiket berkunjung
- Sistem menyimpan data tiket
- Pengunjung memberikan review setelah berkunjung
- 

<br>

## 9. API Endpoints (Opsional) (masih template)
- GET /api/pelanggan – Menampilkan semua data pelanggan
- POST /api/transaksi – Menambah transaksi baru
- GET /api/transaksi/{id} – Menampilkan detail transaksi
- PUT /api/transaksi/{id} – Memperbarui status transaksi
- GET /api/laporan?periode=bulan – Menampilkan laporan keuangan bulanan

<br>

## 10. Keamanan dan Validasi (masih template)
- Validasi input di sisi client (JavaScript) dan server (PHP).
- Password dienkripsi menggunakan password_hash().
- Akses dibatasi menggunakan session dan role-based authentication.

<br>

## 11. Pengembangan Lanjutan (Versi 2.0) (masih template)
- Fitur notifikasi WhatsApp otomatis ketika cucian selesai.
- QR Code untuk nota pelanggan.
- Dashboard analitik menggunakan Chart.js atau Google Charts.
- Integrasi dengan Payment Gateway (Midtrans / DOKU).

<br><br>
