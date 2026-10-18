# KasirLokal

Aplikasi kasir gratis untuk booth dan UMKM kecil. Jalan di browser, bisa dipasang ke layar utama HP atau tablet, dan tetap bisa dipakai tanpa internet. Semua data tersimpan di perangkat. Tidak ada akun, tidak ada server, tidak ada biaya.

**Pakai sekarang:** https://akunsyarif-rgb.github.io/KasirLokal/

## Yang bisa dilakukan

- Kasir: produk, keranjang, bayar tunai (uang pas, kembalian otomatis)
- QRIS dan transfer manual dengan status Pending sampai Anda verifikasi sendiri
- Foto bukti pembayaran (opsional, otomatis dikecilkan, hanya catatan)
- Riwayat, pembatalan transaksi (tercatat, tidak dihapus), laporan harian
- Ekspor CSV untuk Excel atau Google Sheets
- Backup ke berkas `.json` dan pemulihan dari berkas itu

## Memasang

- **Android (Chrome):** menu ⋮, lalu Pasang aplikasi.
- **iPhone/iPad (Safari):** Bagikan, lalu Tambah ke Layar Utama. Pasang sebelum mulai mencatat penjualan, karena data di tab Safari terpisah dari app yang terpasang.

## Batasan yang perlu diketahui

- Data hanya ada di satu perangkat. Tidak sinkron antar HP.
- Kalau perangkat hilang atau data browser terhapus, data hilang. **Backup seminggu sekali** (Setelan, Buat backup sekarang) dan simpan berkasnya di tempat lain.
- Pemulihan hanya menambah data. Data yang sudah ada di perangkat tidak dihapus atau ditimpa.
- Foto bukan bukti pembayaran. Cek uang masuk di aplikasi bank atau e-wallet Anda.
- Gratis dan tanpa jaminan.

## Untuk pengembang

Satu berkas `index.html` (HTML, CSS, JavaScript), tanpa build. Data di IndexedDB. `sw.js` menyimpan aset untuk mode offline; naikkan `V` di `sw.js` setiap rilis. Hosting statis (GitHub Pages).
