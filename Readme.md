# UAS PBW-Akasha Library Management System

## Deskripsi 
Website ini dibuat bertujuan untuk memenuhi UAS Mata Kuliah Pemrogaman Berbasis Web. Akasha Library Management System adalah aplikasi manajemen perpustakaan berbasis web yang memanfaatkan Laravel Blade sebagai engine untuk rendering tampilan. Aplikasi ini dirancang untuk membantu pengelolaan buku, anggota, dan riwayat peminjaman secara efisien dengan antarmuka yang ramah pengguna.
## Fitur Utama
1. **Dashboard**
   - Menampilkan ringkasan data seperti jumlah buku, kategori, anggota, dan riwayat peminjaman.

2. **Manajemen Buku**
   - Menambahkan, mengedit, dan menghapus data buku.

3. **Manajemen Kategori**
   - Mengelola kategori buku untuk mempermudah klasifikasi.

4. **Manajemen Anggota**
   - Menambahkan, mengedit, dan menghapus data anggota perpustakaan.

5. **Manajemen Peminjaman**
   - Mencatat transaksi peminjaman dan pengembalian buku.
   - Menampilkan riwayat peminjaman dengan informasi lengkap.

6. **Informasi Aturan Peminjaman**
   - Menampilkan informasi terkait aturan peminjaman seperti batas waktu, jumlah maksimal buku, dan denda.
7. **Fitur Cetak Laporan**
    Laporan riwayat peminjaman dapat diekspor ke format PDF untuk pencetakan atau penyimpanan arsip.

## Teknologi yang Digunakan
- **Frontend**: Blade Template Engine (Laravel)
- **Backend**: Laravel Framework
- **Database**: MySQL
- **Server**: Laragon (Local Development Server)

## Fungsi CRUD
Berikut implementasi CRUD (Create, Read, Update, Delete):

### Buku
- **Create**: Menambahkan buku baru dengan data seperti judul, kode buku, kategori, dan lainnya.
- **Read**: Melihat daftar buku lengkap.
- **Update**: Mengedit data buku yang ada.
- **Delete**: Menghapus data buku.

### Kategori
- **Create**: Menambahkan kategori baru.
- **Read**: Menampilkan daftar kategori yang tersedia.
- **Update**: Mengedit data kategori.
- **Delete**: Menghapus kategori.

### Anggota
- **Create**: Menambahkan anggota baru.
- **Read**: Menampilkan daftar anggota perpustakaan.
- **Update**: Mengedit data anggota.
- **Delete**: Menghapus data anggota.

## Cara Instalasi

1. **Persiapan Lingkungan**
   - Pastikan Laragon terinstal di sistem Anda.
   - Install Composer dan Node.js.

2. **Clone Repository**
   ```bash
   git clone <repository-url>
   cd akasha-library
   ```

3. **Install Dependencies**
   ```bash
   composer install
   npm install
   npm run dev
   ```

4. **Konfigurasi Environment**
   - Salin file `.env.example` menjadi `.env`:
     ```bash
     cp .env.example .env
     ```
   - Konfigurasikan database di file `.env`:
     ```env
     DB_CONNECTION=mysql
     DB_HOST=127.0.0.1
     DB_PORT=3306
     DB_DATABASE=akasha_library
     DB_USERNAME=root
     DB_PASSWORD=
     ```

5. **Migrasi Database**
   Jalankan perintah berikut untuk membuat tabel di database:
   ```bash
   php artisan migrate
   ```

6. **Menjalankan Aplikasi**
   ```bash
   php artisan serve
   ```
   Akses aplikasi melalui browser di [http://127.0.0.1:8000](http://127.0.0.1:8000).

7. **Login Awal**
   - Default Admin:
     - Email: `admin@admin.com`
     - Password: `admin123`
   - Default Anggota :
     - Email: `rani@gmail.com`
     - Password: `12345678`

## Screenshots
1. **Dashboard Admin**
   ![Dashboard Admin](path-to-your-screenshot1)

2. **Dashboard Anggota**
   ![Dashboard Anggota](path-to-your-screenshot2)
