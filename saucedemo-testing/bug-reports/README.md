# Ringkasan Bug: SauceDemo (saucedemo.com)

Daftar bug yang ditemukan pada pengujian manual SauceDemo, dikelompokkan berdasarkan test case. Klik ID untuk melihat bug report lengkap.

**Environment:** Chrome 155, Windows 10
**Tanggal pengujian:** 9 Oktober 2026 (pengujian awal), 13 dan 14 Oktober 2026 (pengujian ulang)

## Bug Terkonfirmasi

### TC-020: Menambah produk dengan problem_user
Expected: perilaku sama seperti standard_user.

| ID | Judul | Severity | Status |
|---|---|---|---|
| [BUG-001](BUG-001.md) | Gambar produk di halaman Products tidak sesuai produknya (semua produk) | Medium | Open |
| [BUG-002](BUG-002.md) | Halaman detail menampilkan produk yang berbeda dari produk yang diklik | High | Open |
| [BUG-003](BUG-003.md) | Tombol "Add to cart" hanya berfungsi di 3 dari 6 produk | High | Open |
| [BUG-004](BUG-004.md) | Opsi sort selain Name (A to Z) tidak bisa dipilih | Medium | Open |
| [BUG-007](BUG-007.md) | Tombol "Remove" tidak berfungsi di halaman Products | Medium | Open |

### TC-021: Checkout dengan error_user
Expected: checkout berjalan normal.

| ID | Judul | Severity | Status |
|---|---|---|---|
| [BUG-005](BUG-005.md) | Kolom Last Name tidak bisa diisi dan checkout tetap bisa dilanjutkan | High | Open |
| [BUG-006](BUG-006.md) | Tombol "Finish" tidak bisa diklik pada halaman Overview | Critical | Open |

## Perlu Ditinjau (belum terbukti di kondisi bersih)

| ID | Temuan | Yang harus dibuktikan | Hasil |
|---|---|---|---|
| BUG-010 | Badge keranjang menunjukkan 1 padahal keranjang kosong | Ulangi dari profil bersih. Sempat muncul juga di standard_user pada profil lama, jadi kemungkinan sisa data | Ditunda |

## Temuan yang Digabung atau Dibatalkan

| ID | Alasan |
|---|---|
| BUG-008 | Tombol detail "Add to cart" ternyata sesuai produk yang tampil (Fleece Jacket). Digabung ke BUG-002 |
| BUG-009 | Tombol detail "Remove" ternyata sesuai produk yang tampil (Backpack). Digabung ke BUG-002 |
| BUG-011 | Tampilan "ITEM NOT FOUND" tidak muncul saat diuji ulang dari kondisi bersih. Dibatalkan, kemungkinan sisa data lama |
## Ringkasan Bug Terkonfirmasi

| Severity | Jumlah |
|---|---|
| Critical | 1 |
| High | 3 |
| Medium | 3 |
| **Total** | **7** |

## Panduan Severity yang Digunakan

| Level | Arti |
|---|---|
| Critical | Fitur inti tidak bisa dipakai sama sekali dan tidak ada jalan pintas |
| High | Fitur penting rusak atau hasilnya salah, tetapi sistem masih bisa dipakai sebagian |
| Medium | Fitur sekunder bermasalah, atau ada jalan pintas yang mudah |
| Low | Masalah tampilan atau teks kecil yang tidak mengganggu fungsi |

## Catatan
Status "Open" karena SauceDemo adalah aplikasi demo milik pihak lain dan bug tidak diperbaiki. Akun problem_user dan error_user memang dirancang berperilaku bermasalah untuk latihan testing.
