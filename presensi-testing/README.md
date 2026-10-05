# Pengujian Website Presensi Karyawan

## Deskripsi
Website presensi untuk mencatat kehadiran karyawan kontrak, dikembangkan pada Praktik Kerja Lapangan (PKL) di Pusjar SKTAN LAN RI Jatinangor. Dokumen ini berisi temuan bug yang ditemukan saat pengujian fungsional.

## Ruang Lingkup Pengujian
- Manajemen data karyawan (peran admin)
- Absensi masuk dan pulang (peran karyawan)
- Absensi shift (peran karyawan)
- Konsistensi data riwayat absensi antara admin dan karyawan

## Metode
Black box testing (pengujian fungsional dari sisi pengguna).

## Ringkasan Temuan

| ID | Judul | Severity | Status |
|---|---|---|---|
| [BUG-001](bug-reports/BUG-001.md) | Perubahan data karyawan oleh admin tidak tersimpan | High | Fixed |
| [BUG-002](bug-reports/BUG-002.md) | Riwayat absensi admin tidak sama dengan halaman karyawan | High | Fixed |
| [BUG-003](bug-reports/BUG-003.md) | Batas waktu absensi masuk dan pulang tidak berlaku | High | Fixed |
| [BUG-004](bug-reports/BUG-004.md) | Tombol "Absen Masuk" tidak bisa diklik | Critical | Fixed |
| [BUG-005](bug-reports/BUG-005.md) | Tombol absen shift tidak berfungsi | High | Fixed |

## Catatan
Bug report ini ditulis ulang dari temuan saat pengembangan, bukan dari dokumen pengujian formal.
