# Pengujian SauceDemo (saucedemo.com)

## Deskripsi
Pengujian manual (black box) pada SauceDemo, situs e-commerce demo yang disediakan untuk latihan testing. Proyek ini menunjukkan kemampuan menguji aplikasi pihak lain, menemukan defect, dan mendokumentasikannya dalam bug report.

## Ruang Lingkup Pengujian
- Autentikasi (login valid, akun terkunci, password salah, kolom kosong)
- Daftar produk, sort, dan halaman detail produk
- Keranjang (tambah, hapus, isi keranjang saat pindah halaman)
- Checkout (data valid, validasi kolom kosong, perhitungan total)
- Logout
- Perilaku akun khusus: problem_user dan error_user

## Metode dan Environment
- **Metode:** Manual testing (black box)
- **Browser:** Chrome 155, Windows 10
- **Tanggal pengujian:** 9 Oktober 2026 (pengujian awal), 10 dan 11 Oktober 2026 (pengujian ulang)
- **Praktik:** setiap bug diulang dari kondisi bersih (data situs dihapus), dan dibandingkan dengan perilaku standard_user

## Ringkasan Hasil

| Keterangan | Jumlah |
|---|---|
| Test case | 21 |
| Pass | 19 |
| Fail | 2 (TC-020 dan TC-021) |
| Bug terkonfirmasi | 7 |

| Severity | Jumlah |
|---|---|
| Critical | 1 |
| High | 3 |
| Medium | 3 |

## Dokumen
- [Daftar test case lengkap](test-cases.md)
- [Ringkasan dan detail bug report](bug-reports/README.md)

## Catatan
Beberapa temuan awal dibatalkan atau digabung setelah diuji ulang dari kondisi bersih (lihat tabel di ringkasan bug). Hanya bug yang dapat direproduksi yang dilaporkan.
