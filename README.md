# Kalkulator Modal Recovery (PWA)

Aplikasi web yang bisa di-install di HP dan dipakai offline.

## Isi folder

- `index.html` : kalkulatornya
- `manifest.webmanifest` : nama, ikon, dan tampilan aplikasi
- `sw.js` : service worker, menyimpan file di HP supaya bisa offline
- `icons/` : ikon aplikasi
- `fonts/` : font Barlow (lisensi SIL OFL, lihat `fonts/OFL.txt`)

## Upload ke GitHub Pages (dari laptop)

1. Login ke github.com, klik **New repository**. Beri nama, misalnya `kalkulator-modal`, pilih **Public**, lalu **Create repository**.
2. Di halaman repo, klik **uploading an existing file** (atau **Add file > Upload files**).
3. Ekstrak zip, buka foldernya, lalu seret **isi** folder (index.html, sw.js, manifest.webmanifest, folder icons, folder fonts) ke halaman upload. `index.html` harus berada di level paling atas repo, bukan di dalam subfolder.
4. Klik **Commit changes**.
5. Buka **Settings > Pages**. Di bagian Source pilih **Deploy from a branch**, branch **main**, folder **/ (root)**, lalu **Save**.
6. Tunggu 1 sampai 2 menit. Alamat aplikasi muncul di halaman yang sama, formatnya `https://NAMA-AKUN.github.io/kalkulator-modal/`.

## Install di HP

- **Android (Chrome):** buka alamatnya, ketuk menu titik tiga, pilih **Install app** atau **Add to Home screen**.
- **iPhone (Safari):** buka alamatnya, ketuk tombol **Share**, pilih **Add to Home Screen**.

Buka sekali saat online. Setelah itu aplikasi bisa dipakai tanpa internet.

## Memperbarui aplikasi

1. Ganti file yang berubah di GitHub (upload ulang dengan nama yang sama).
2. Di `sw.js`, naikkan versi cache, misalnya `modal-recovery-v1` menjadi `modal-recovery-v2`.
3. Buka aplikasi di HP saat online, tutup, lalu buka lagi. Versi baru akan terpakai.

## Catatan

- Repo publik berarti kode kalkulator bisa dilihat orang lain. Angka yang Anda isi hanya tersimpan di HP Anda, tidak dikirim ke mana pun.
- Gambaran matematis, bukan rekomendasi keuangan.
