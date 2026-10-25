# STATUS — KasirLokal

_Disusun 25 Oktober 2026 dari isi repo (commit terakhir 18 Okt 2026, "v0.4"). Hanya fakta yang tertulis di repo; yang tidak bisa diverifikasi dari repo ditandai._

## Ringkasan
Aplikasi kasir gratis untuk booth dan UMKM kecil. Berjalan di browser, bisa dipasang ke layar utama HP atau tablet, tetap bisa dipakai tanpa internet. Semua data tersimpan di perangkat; tanpa akun dan tanpa server. Versi **v0.4** (cache service worker `kasirlokal-v4`). Repo public. Alamat pakai: https://akunsyarif-rgb.github.io/KasirLokal/ (dari README, belum saya buka).

## Stack
Satu berkas `index.html` (HTML, CSS, JavaScript; sekitar 1.100 baris) tanpa build. Data di IndexedDB. `sw.js` menyimpan aset untuk mode offline. Hosting statis GitHub Pages. Seluruh riwayat commit ada di tanggal 18 Okt (v0.1 sampai v0.4).

## Sudah ada
- Kasir: produk, keranjang, bayar tunai (uang pas, kembalian otomatis).
- QRIS dan transfer manual dengan status Pending sampai diverifikasi sendiri.
- Foto bukti pembayaran opsional (otomatis dikecilkan, hanya catatan).
- Riwayat, pembatalan transaksi (tercatat, tidak dihapus), laporan harian.
- Ekspor CSV untuk Excel atau Google Sheets.
- Backup ke berkas `.json` dan pemulihan dari berkas itu (pemulihan hanya menambah data).
- Petunjuk pasang, panduan singkat, teks backup khusus iPad, banner versi baru (v0.3–v0.4).

## Belum / terbuka
- Data hanya ada di satu perangkat; tidak sinkron antar HP.
- Tidak ada tes otomatis dan tidak ada CI.
- Belum ada catatan pengujian di perangkat nyata atau pemakaian oleh pedagang sungguhan.
- Tidak ada rencana atau roadmap tertulis di repo.

## Hal yang perlu diwaspadai
- Naikkan konstanta `V` di `sw.js` setiap rilis; kalau tidak, pengguna tidak mendapat versi baru.
- Data di tab Safari terpisah dari app yang terpasang di iPhone/iPad. Pasang dulu sebelum mulai mencatat penjualan.
- Data hilang bila perangkat hilang atau data browser dihapus. README menyarankan backup seminggu sekali.
- Foto bukan bukti pembayaran; uang masuk harus dicek di aplikasi bank atau e-wallet.

## Dokumen penting
`README.md`.

## Langkah berikutnya (usulan, bukan dari repo)
Uji alur lengkap (jual, batalkan, backup, pulihkan) di satu HP Android dan satu iPhone/iPad, lalu catat hasilnya di sini.

---
Perbarui file ini di akhir tiap sesi kerja: tanggal, apa yang selesai, apa yang terbuka.
