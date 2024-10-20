
veGETables Website

Selamat datang di veGETables Website. Ini adalah website untuk menjual produk sayuran, buah-buahan, dan herbal secara online. Website ini dirancang untuk mempermudah pengguna dalam berbelanja bahan makanan sehat langsung dari petani atau supplier lokal.

## Fitur
- Daftar produk termasuk sayuran, buah-buahan, dan herbal.
- Wishlist: Pengguna dapat menyimpan produk favorit mereka.
- Keranjang belanja: Pengguna dapat menambahkan produk ke dalam keranjang untuk pembelian.
- Checkout: Proses pembayaran mudah dan aman.
- Pengguna dapat mendaftar dan login untuk mengelola akun dan pesanan mereka.

## Struktur Database
Website ini menggunakan database MySQL untuk menyimpan data pengguna, produk, kategori, wishlist, pesanan, dan item pesanan.

### Tabel
1. **users**
   - id: ID pengguna
   - username: Nama pengguna
   - email: Email pengguna
   - password: Kata sandi pengguna
   - created_at: Tanggal pembuatan
   - updated_at: Tanggal pembaruan

2. **categories**
   - id: ID kategori
   - category_name: Nama kategori
   - created_at: Tanggal pembuatan

3. **products**
   - id: ID produk
   - product_name: Nama produk
   - price: Harga produk
   - description: Deskripsi produk
   - image_url: URL gambar produk
   - category_id: ID kategori produk
   - created_at: Tanggal pembuatan
   - updated_at: Tanggal pembaruan

4. **wishlist**
   - id: ID wishlist
   - user_id: ID pengguna
   - product_id: ID produk
   - added_date: Tanggal ditambahkan ke wishlist

5. **orders**
   - id: ID pesanan
   - user_id: ID pengguna
   - order_date: Tanggal pesanan
   - status: Status pesanan (pending, completed, cancelled)

6. **order_items**
   - id: ID item pesanan
   - order_id: ID pesanan
   - product_id: ID produk
   - quantity: Kuantitas produk
   - price: Harga produk

## Instalasi dan Penggunaan
1. Clone repository ini:
   ```
   git clone https://github.com/Danielle024/veGETables-Website.git
   ```
   
2. Buka project di code editor pilihan Anda.

3. Atur koneksi database MySQL di file konfigurasi untuk menghubungkan website dengan database.

4. Import file SQL untuk membuat tabel dan menyimpan data awal:
   ```
   mysql -u root -p vegetables_website < vegetables_integrasidata.sql
   ```

5. Jalankan server lokal menggunakan XAMPP atau platform server lainnya.

6. Akses website di browser dengan alamat:
   ```
   http://localhost/veGETables-Website
   ```

## Kontribusi
Jika Anda ingin berkontribusi pada proyek ini, silakan lakukan langkah berikut:
1. Fork repository ini.
2. Buat branch baru untuk perubahan Anda.
3. Lakukan commit perubahan.
4. Kirim pull request.

## Lisensi
Proyek ini dilisensikan di bawah MIT License.

## Form Login Responsif

Proyek ini juga mencakup form login responsif yang dirancang untuk bekerja dengan lancar di berbagai perangkat. Form ini memungkinkan pengguna untuk login dengan antarmuka yang bersih dan modern.

### Fitur:
- **Desain Responsif**: Form login ini dioptimalkan untuk tampilan di perangkat seluler, tablet, dan desktop.
- **Antarmuka yang Mudah Digunakan**: Desainnya memprioritaskan kemudahan penggunaan dan aksesibilitas untuk pengalaman login yang lancar.
- **Aset yang Dapat Disesuaikan**: Folder assets berisi file CSS dan JavaScript yang dapat Anda modifikasi untuk menyesuaikan tema website.

### Cara Menggunakan:
1. Buka file `index.html` yang terletak di dalam folder `responsive-login-form-main`.
2. Sesuaikan aset (CSS, JS) jika diperlukan untuk penyesuaian gaya atau fungsionalitas.
3. Integrasikan form ini ke bagian manapun dari website veGETables di mana fungsi login diperlukan.
4. Lihat pratinjau desain form menggunakan file `preview.png`.

Untuk detail lebih lanjut, silakan lihat `README.md` di dalam folder `responsive-login-form-main`.
