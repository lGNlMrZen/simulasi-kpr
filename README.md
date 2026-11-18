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

## Lokasi penyimpanan default
File hasil (termasuk `kpr-bulanan.zip`) disimpan di **`/sdcard/Download`**. Di Android, unduhan browser juga biasanya masuk ke folder ini.

## Pakai di lokal
Buka `index.html` langsung di browser. Tidak perlu server, tidak perlu koneksi internet.

> Catatan: service worker hanya aktif lewat `http(s)`, jadi kalau dibuka dengan `file://`, halaman tetap berfungsi normal, hanya cache offline-nya yang tidak aktif.

## Pasang ke GitHub Pages
1. Buat repository baru di GitHub, misalnya `kpr-bulanan`.
2. Upload tiga file: `index.html`, `sw.js`, dan `README.md` ke root repository.
3. Buka **Settings → Pages**.
4. Di **Build and deployment**, pilih **Deploy from a branch**, branch `main`, folder `/ (root)`, lalu **Save**.
5. Tunggu beberapa menit, lalu buka `https://NAMA-USER.github.io/kpr-bulanan/`.

Lewat terminal (setelah `git init` dan remote disiapkan):

```bash
git add .
git commit -m "Tambah tabel KPR bulanan"
git push -u origin main
```

## Pindah perangkat / browser
Karena data disimpan lokal di browser, gunakan **Cadangkan JSON** di perangkat lama, lalu **Impor JSON** di perangkat baru.
