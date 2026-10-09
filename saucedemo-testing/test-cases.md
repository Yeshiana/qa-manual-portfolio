# Test Case: SauceDemo (saucedemo.com)

**Metode:** Manual testing (black box)
**Aplikasi:** SauceDemo, situs e-commerce demo untuk latihan testing
**Browser:** (isi, contoh: Chrome versi xxx, Windows 11)
**Tanggal pengujian:** (isi)

**Akun uji** (tertera di halaman login): standard_user, locked_out_user, problem_user, performance_glitch_user, error_user, visual_user

| ID | Skenario | Langkah | Expected Result | Status |
|---|---|---|---|---|
| TC-001 | Login dengan akun valid | Login sebagai standard_user | Masuk ke halaman daftar produk | Pass |
| TC-002 | Login dengan akun terkunci | Login sebagai locked_out_user | Muncul pesan bahwa akun terkunci | Pass |
| TC-003 | Login dengan password salah | Isi username valid dan password salah | Muncul pesan error, login ditolak | Pass |
| TC-004 | Login dengan username kosong | Kosongkan username, isi password, klik Login | Muncul pesan "Username is required" | Pass |
| TC-005 | Login dengan password kosong | Isi username, kosongkan password, klik Login | Muncul pesan "Password is required" | Pass |
| TC-006 | Tampilan daftar produk | Login, lihat halaman produk | Semua produk tampil lengkap dengan gambar, nama, dan harga | Pass |
| TC-007 | Urutkan nama A-Z dan Z-A | Pilih opsi sort nama | Produk terurut sesuai pilihan | Belum dijalankan |
| TC-008 | Urutkan harga rendah ke tinggi dan sebaliknya | Pilih opsi sort harga | Produk terurut sesuai harga | Belum dijalankan |
| TC-009 | Membuka detail produk | Klik nama produk | Halaman detail menampilkan produk yang benar | Belum dijalankan |
| TC-010 | Menambah satu produk ke keranjang | Klik Add to cart pada satu produk | Tombol berubah menjadi Remove, angka di ikon keranjang bertambah | Belum dijalankan |
| TC-011 | Menambah beberapa produk | Tambahkan 3 produk berbeda | Jumlah di ikon keranjang sesuai, ketiganya ada di keranjang | Belum dijalankan |
| TC-012 | Menghapus produk dari keranjang | Buka keranjang, klik Remove | Produk hilang, jumlah keranjang berkurang | Belum dijalankan |
| TC-013 | Isi keranjang tetap ada saat pindah halaman | Tambah produk, buka halaman lain, kembali | Isi keranjang tidak berubah | Belum dijalankan |
| TC-014 | Checkout dengan data valid | Isi nama depan, nama belakang, kode pos, lanjutkan sampai selesai | Muncul halaman konfirmasi pesanan berhasil | Belum dijalankan |
| TC-015 | Checkout dengan nama depan kosong | Kosongkan First Name, klik Continue | Muncul pesan wajib diisi | Belum dijalankan |
| TC-016 | Checkout dengan nama belakang kosong | Kosongkan Last Name, klik Continue | Muncul pesan wajib diisi | Belum dijalankan |
| TC-017 | Checkout dengan kode pos kosong | Kosongkan Postal Code, klik Continue | Muncul pesan wajib diisi | Belum dijalankan |
| TC-018 | Perhitungan total di halaman Overview | Cek Item total, Tax, dan Total | Total = harga item + pajak, hitungannya benar | Belum dijalankan |
| TC-019 | Logout | Buka menu, klik Logout | Kembali ke halaman login | Belum dijalankan |
| TC-020 | Menambah produk dengan problem_user | Login problem_user, tambah dan hapus produk, cek gambar dan sort | Perilaku sama seperti standard_user | Belum dijalankan |
| TC-021 | Checkout dengan error_user | Login error_user, lakukan checkout lengkap | Checkout berjalan normal | Belum dijalankan |
