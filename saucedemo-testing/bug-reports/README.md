# Ringkasan Bug: SauceDemo (saucedemo.com)

Daftar bug yang ditemukan pada pengujian manual SauceDemo, dikelompokkan berdasarkan test case. Klik ID untuk melihat bug report lengkap.

**Environment:** Chrome 155, Windows 10
**Tanggal pengujian:** 9 Oktober 2026 (pengujian awal), 13 Oktober 2026 (pengujian ulang)

## Bug Terkonfirmasi

### TC-020: Menambah produk dengan problem_user
Expected: perilaku sama seperti standard_user.

| ID | Judul | Severity | Status |
|---|---|---|---|
| [BUG-001](BUG-001.md) | Gambar produk di halaman Products tidak sesuai produknya (semua produk) | Medium | Open |
| [BUG-002](BUG-002.md) | Gambar dan keterangan di halaman detail tidak sesuai produk yang diklik | High | Open |
| [BUG-004](BUG-004.md) | Opsi sort selain Name (A to Z) tidak bisa dipilih | Medium | Open |

### TC-021: Checkout dengan error_user
Expected: checkout berjalan normal.

| ID | Judul | Severity | Status |
|---|---|---|---|
| [BUG-005](BUG-005.md) | Kolom Last Name tidak bisa diisi dan checkout tetap bisa dilanjutkan | High | Open |
| [BUG-006](BUG-006.md) | Tombol "Finish" tidak bisa diklik pada halaman Overview | Critical | Open |

## Perlu Ditinjau (belum terbukti di kondisi bersih)

Temuan di bawah ini belum diulang dari kondisi bersih (data situs dihapus atau Incognito, badge keranjang kosong sebelum mulai). Jangan dianggap bug resmi sebelum terbukti.

### TC-020: problem_user

| ID | Temuan | Yang harus dibuktikan | Hasil |
|---|---|---|---|
| BUG-003 | Add to cart hanya berfungsi di 3 dari 6 produk | Klik Add to cart satu per satu di tiap produk, catat tombol dan badge setiap kali | Belum diuji ulang |
| BUG-007 | Tombol Remove tidak berfungsi di halaman Products | Setelah Add to cart berhasil, klik Remove, cek tombol dan badge | Belum diuji ulang |
| BUG-008 | Tombol di detail masih "Add to cart" padahal produk sudah ditambahkan (contoh: Backpack) | Tambah satu produk di Products, buka detailnya | Belum diuji ulang |
| BUG-009 | Tombol "Remove" muncul di detail untuk produk yang belum ditambahkan (contoh: Test.allTheThings() T-Shirt (Red)) | Dari keranjang bersih, tambah satu produk saja, buka detail produk lain | Belum diuji ulang |
| BUG-010 | Badge keranjang menunjukkan 1 padahal keranjang kosong | Ulangi dari profil bersih. Sempat muncul juga di standard_user pada profil lama, jadi kemungkinan sisa data | Ditunda |
| BUG-011 | Detail Sauce Labs Fleece Jacket menampilkan "ITEM NOT FOUND" dan harga tidak valid | Buka detail Fleece Jacket dari kondisi bersih | Belum diuji ulang |

## Ringkasan Bug Terkonfirmasi

| Severity | Jumlah |
|---|---|
| Critical | 1 |
| High | 2 |
| Medium | 2 |
| **Total** | **5** |

## Panduan Severity yang Digunakan

| Level | Arti |
|---|---|
| Critical | Fitur inti tidak bisa dipakai sama sekali dan tidak ada jalan pintas |
| High | Fitur penting rusak atau hasilnya salah, tetapi sistem masih bisa dipakai sebagian |
| Medium | Fitur sekunder bermasalah, atau ada jalan pintas yang mudah |
| Low | Masalah tampilan atau teks kecil yang tidak mengganggu fungsi |

## Catatan
Status "Open" karena SauceDemo adalah aplikasi demo milik pihak lain dan bug tidak diperbaiki. Akun problem_user dan error_user memang dirancang berperilaku bermasalah untuk latihan testing.
