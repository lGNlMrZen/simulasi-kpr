# Tabel KPR Bulanan

Halaman KPR berupa satu file HTML, bisa dipakai **tanpa internet**, dengan jadwal **per bulan**, pilihan warna **pastel**, dan status **Sudah dibayar / Belum dibayar**.

## Fitur
- Hitung angsuran metode **Anuitas** atau **Flat** dari pokok, bunga per tahun, dan tenor dalam **bulan**.
- Tabel per bulan: pokok, bunga, angsuran, nominal yang dibayar, sisa pokok, status, dan catatan.
- Kolom **Dibayar (Rp)** dan **Catatan** bisa diedit langsung; centang **Sudah dibayar** untuk menandai lunas.
- Progres pembayaran dan tombol: tandai s.d. bulan ini, tandai yang dibayar, semua lunas, batalkan semua.
- 7 pilihan warna pastel + warna aksen kustom.
- Data tersimpan otomatis di `localStorage` browser (perangkat & browser yang sama).
- Ekspor CSV, cadangan/impor JSON, dan cetak.
- Service worker menyimpan halaman agar tetap bisa dibuka setelah pertama kali diakses online.

## Pakai di lokal
Buka `index.html` langsung di browser. Tidak perlu server, tidak perlu koneksi internet.

## Pindah perangkat / browser
Karena data disimpan lokal di browser, gunakan **Cadangkan JSON** di perangkat lama, lalu **Impor JSON** di perangkat baru.
