## Mini Challenge: "Buat Halaman Profil Responsif dengan Tailwind CSS"

### Instruksi

Buat sebuah halaman HTML sederhana menggunakan **Tailwind CSS** (via CDN atau CLI). Halaman harus berisi:

1. **Header**
    - Judul "My Profile"
    - Subjudul kecil di bawahnya (gunakan utilitas typography: font size, font weight, text color).
    - Gunakan alignment `text-center`.
2. **Profile Card**
    - Kotak berisi foto profil (gunakan `aspect-ratio` dan `object-cover`).
    - Nama pengguna (gunakan `text-2xl font-bold text-blue-600`).
    - Deskripsi singkat (gunakan `text-gray-600 leading-tight tracking-tight`).
    - Tambahkan **shadow**, **rounded corner**, dan **padding**.
3. **Layout Bagian Hobi**
    - Buat **grid** yang responsif:
        - `grid-cols-1` di layar kecil.
        - `grid-cols-2` di layar medium.
        - `grid-cols-3` di layar besar.
    - Setiap item hobi ditampilkan dalam kotak dengan background berwarna berbeda (gunakan utilities warna Tailwind).
4. **Responsiveness**
    - Atur agar **foto profil** tampil di atas teks di layar kecil (`flex-col`), dan sejajar di layar medium ke atas (`flex-row`).
    - Pastikan padding/margin menyesuaikan ukuran layar (`sm:`, `md:`, `lg:`).
5. **Bonus (opsional)**
    - Tambahkan **tombol** dengan hover effect (`hover:bg-blue-700`).
    - Gunakan **plugin typography** (`prose`) untuk menampilkan 1 paragraf artikel pendek tentang dirimu.

---

### Output yang Diharapkan

- Di layar kecil: elemen tampil rapi secara vertikal.
- Di layar besar: layout menjadi lebih kompleks (grid, flex).
- Styling konsisten dan memanfaatkan **utility classes** dari Tailwind, bukan CSS manual.