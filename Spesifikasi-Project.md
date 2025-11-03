# MODUL STUDI KASUS: LAUNDRYCRAFTY (TEMPLATE)

| Nama | NRP |
| --- | --- |
| Royan Habibi Alfatih | 5025241115 |
| Bara Semangat Rohmani | 5025241144 |

## 1. Deskripsi Umum
<p>
LaundryCrafty adalah sistem manajemen usaha laundry berbasis web yang membantu pengelola
laundry dalam mengelola transaksi, pelanggan, layanan, dan laporan pendapatan. Aplikasi ini
dirancang untuk mengotomatisasi pencatatan dan pengelolaan data laundry agar lebih cepat,
efisien, dan terintegrasi menggunakan database MySQL.
</p>
<br>

## 2. Tujuan Proyek
<ul>
<li>Mempermudah pengelolaan data pelanggan dan transaksi laundry.</li>
<li>Mengotomatisasi perhitungan biaya berdasarkan berat cucian atau jenis layanan.</li>
<li>Menyediakan laporan pendapatan harian, mingguan, dan bulanan.</li>
<li>Memberikan pengalaman pengguna yang mudah digunakan bagi admin maupun pelanggan.</li>
</ul>
  
<br>

## 3. Fitur Utama
- Manajemen Pelanggan: Tambah, ubah, hapus, dan lihat data pelanggan.
- Manajemen Layanan: Menyediakan daftar jenis layanan seperti Cuci Kering, Cuci Setrika, dan Express.
- Transaksi Laundry: Input data transaksi pelanggan, jenis layanan, berat, harga, tanggal masuk & selesai.
- Status Cucian: Update status cucian (Proses, Selesai, Sudah Diambil).
- Laporan Keuangan: Menampilkan pendapatan harian, mingguan, dan bulanan.
- Autentikasi Admin: Login dan logout admin untuk keamanan sistem.
- Dashboard Statistik: Tampilan grafik transaksi dan pendapatan.
- Pencarian Data: Mencari pelanggan atau transaksi berdasarkan nama atau tanggal.

<br>

## 4. Peran Pengguna
- Admin: Mengelola seluruh data (pelanggan, layanan, transaksi, laporan).
- Kasir/Operator: Input transaksi laundry, memperbarui status, mencetak nota.
- Pelanggan (opsional): Melihat status cucian dan riwayat transaksi melalui login pelanggan.
 
<br>

## 5. Spesifikasi Teknis
- Front-End: HTML5, CSS3, Bootstrap, JavaScript
- Back-End: PHP (versi 8.x)
- Database: MySQL / MariaDB
- Server: Apache (XAMPP / Laragon)
- Tools: VS Code, phpMyAdmin
- Integrasi API (opsional): API laporan JSON untuk akses data transaksi

<br>

## 6. Struktur Database (Tabel Utama)
- Tabel pelanggan: id_pelanggan, nama, alamat, no_hp
- Tabel layanan: id_layanan, nama_layanan, harga_per_kg
- Tabel transaksi: id_transaksi, id_pelanggan, id_layanan, tanggal_masuk, tanggal_selesai, berat, total_harga, status
- Tabel user: id_user, username, password, role

<br>

## 7. Desain Tampilan (Front-End)
- Dashboard: Menampilkan statistik jumlah pelanggan, transaksi, dan grafik pendapatan.
- Halaman Pelanggan: Form tambah pelanggan dan tabel daftar pelanggan.
- Halaman Transaksi: Form input transaksi dan tabel daftar transaksi.
- Halaman Laporan: Laporan pendapatan dengan filter tanggal.

<br>

## 8. Alur Proses Sistem
- Admin login ke sistem.
- Kasir menambahkan data pelanggan baru (jika belum terdaftar).
- Kasir mencatat transaksi laundry baru.
- Sistem menghitung total harga otomatis.
- Kasir memperbarui status cucian.
- Admin melihat laporan pendapatan.

<br>

## 9. API Endpoints (Opsional)
- GET /api/pelanggan – Menampilkan semua data pelanggan
- POST /api/transaksi – Menambah transaksi baru
- GET /api/transaksi/{id} – Menampilkan detail transaksi
- PUT /api/transaksi/{id} – Memperbarui status transaksi
- GET /api/laporan?periode=bulan – Menampilkan laporan keuangan bulanan

<br>

## 10. Keamanan dan Validasi
- Validasi input di sisi client (JavaScript) dan server (PHP).
- Password dienkripsi menggunakan password_hash().
- Akses dibatasi menggunakan session dan role-based authentication.

<br>

## 11. Pengembangan Lanjutan (Versi 2.0)
- Fitur notifikasi WhatsApp otomatis ketika cucian selesai.
- QR Code untuk nota pelanggan.
- Dashboard analitik menggunakan Chart.js atau Google Charts.
- Integrasi dengan Payment Gateway (Midtrans / DOKU).

<br><br>
