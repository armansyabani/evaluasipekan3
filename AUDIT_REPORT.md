1. banyak file yang tidak teratur pada tempat nya 
2<link rel="stylesheet" href="style.sss"> kesalahan nya berada di penulisan link nya karna salah link css maka tidak bisa menyambung pada css nya dan seharus nya begini  <link rel="stylesheet" href="style.css"> nah baru bener

3. commit a3f1c2d
   Author: Arman
   Date:   Mon Oct 21 10:00 2025

    add debug.log for testing
     Audit Keamanan & Riwayat
- File `debug.log` pertama kali ditambahkan di commit `a3f1c2d`.
- Ditemukan baris sensitif:
- File ini seharusnya dimasukkan ke `.gitignore` agar tidak ikut diunggah ke Git.
4. =
 1. Analisis Struktur Aset
- File `logo.png` ditemukan di folder utama (root) → seharusnya berada di `assets/images/`
- File `style.css` sudah berada di `assets/css/` (benar)
- File `main.js` sudah berada di `assets/js/` (benar)

---

 2. Perburuan Bug Visual (CSS)
- Masalah: Tampilan halaman tidak memiliki gaya (CSS tidak muncul)
- Penyebab: Path file CSS salah di file `index.html`
- Sebelumnya:
  ```html
  <link rel="stylesheet" href="style.css">
 3. File debug.log pertama kali ditambahkan di commit a3f1c2d.
     Commit message: add debug.log for testing
     Di dalam debug.log, ditemukan baris sensitif berisi API Key:
     API_KEY = "sk-12345abcde"
     singkat nya = Struktur folder sebagian besar benar, bug CSS disebabkan   oleh path yang salah,
dan ditemukan masalah keamanan karena file debug.log berisi data sensitif (API Key).