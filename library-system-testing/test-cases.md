# Test Case: Sistem Informasi Perpustakaan Berbasis Web

**Metode:** Black box testing
**Aplikasi:** Sistem Informasi Manajemen Perpustakaan (Laravel), SMK Negeri 1 Bojongpicung
**Peran pengguna:** Siswa, Petugas

| ID | Skenario | Langkah | Expected Result | Status |
|---|---|---|---|---|
| TC-001 | Pendaftaran anggota dengan data valid | Siswa mengisi form pendaftaran lengkap dengan NISN miliknya sendiri | Akun berhasil dibuat dan diarahkan ke dashboard siswa | Pass |
| TC-002 | Pendaftaran dengan NISN yang sudah terdaftar | Mendaftar menggunakan NISN yang sudah ada di sistem | Muncul pesan validasi bahwa NISN sudah terdaftar | Pass |
| TC-003 | Login siswa dengan data valid | Masukkan NISN dan password yang benar | Berhasil masuk ke dashboard siswa | Pass |
| TC-004 | Login petugas dengan data valid | Masukkan username dan password yang benar di halaman login admin | Berhasil masuk ke dashboard petugas | Pass |
| TC-005 | Login dengan password salah | Masukkan username benar dan password salah | Muncul pesan "Password salah" | Pass |
| TC-006 | Pencarian buku dengan kata kunci valid | Siswa mengetik kata kunci pada kolom pencarian | Sistem menampilkan buku sesuai kata kunci | Pass |
| TC-007 | Pencarian buku yang tidak ada | Siswa mengetik kata kunci buku yang tidak tersedia | Hasil pencarian kosong | Pass |
| TC-008 | Booking peminjaman buku | Siswa memilih buku, menentukan tanggal (maksimal 2 hari kerja), klik Pinjam | Notifikasi booking berhasil, data tersimpan berstatus "Menunggu", stok berkurang, notifikasi terkirim ke petugas | Pass |
| TC-009 | Booking melebihi batas peminjaman | Siswa yang masih meminjam 3 buku mengajukan booking baru | Muncul pesan "Anda sudah mencapai batas maksimal peminjaman 3 buku" | Pass |
| TC-010 | Pengembalian buku dalam kondisi baik | Petugas mengecek fisik buku dan menginput kondisi "baik" | Status peminjaman berubah menjadi "Selesai" | Pass |
| TC-011 | Pengembalian buku dalam kondisi rusak | Petugas mengecek fisik buku dan menginput kondisi "rusak" | Status menjadi "Sanksi Buku Rusak" dan notifikasi sanksi terkirim ke siswa | Pass |
| TC-012 | Siswa mengunggah bukti sanksi | Siswa mengunggah foto bukti di menu Sanksi | Bukti tersimpan, status menjadi "Menunggu Verifikasi", foto tampil di halaman sanksi petugas | Pass |
| TC-013 | Petugas menolak bukti sanksi | Petugas menolak bukti yang diunggah siswa | Notifikasi terkirim ke siswa: bukti ditolak, harap unggah ulang bukti yang valid | Pass |
| TC-014 | Menambah buku dengan data lengkap | Petugas mengisi seluruh form tambah buku, klik Simpan | Data buku tersimpan ke database | Pass |
| TC-015 | Menambah buku tanpa judul | Petugas mengosongkan kolom "Judul Buku", klik Simpan | Penambahan gagal dan muncul tulisan "Wajib diisi" di bawah kolom judul | Pass |
| TC-016 | Menampilkan laporan per bulan | Petugas memilih filter "Per Bulan", klik Tampilkan | Tampil rekap kunjungan, peminjaman, pengembalian, dan koleksi buku sesuai bulan beserta grafik | Pass |
| TC-017 | Mengirim laporan tanpa file | Petugas mengirim laporan tanpa mengunggah file PDF | Muncul pesan validasi agar mengunggah laporan PDF | Pass |

## Catatan
Test case disusun dari tabel hasil pengujian pada dokumen skripsi, lalu dirapikan ke format test case standar.
