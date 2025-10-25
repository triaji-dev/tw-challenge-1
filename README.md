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

## Mini Challenge: "Form Pendaftaran dengan Interaktivitas & Dark Mode"

### Instruksi

Buat halaman HTML menggunakan **Tailwind CSS v4** dengan ketentuan berikut:

1. **Judul Halaman**
   - Tampilkan judul `Form Pendaftaran` di bagian atas, gunakan `text-2xl font-bold text-center`.
2. **Formulir**
   - Input **Nama Lengkap** (wajib diisi, gunakan efek fokus `focus:ring-2 focus:ring-blue-500`).
   - Input **Email** (validasi email dengan `invalid:border-red-500 invalid:text-red-600`).
   - Textarea **Pesan**.
   - Checkbox **Saya menyetujui syarat & ketentuan**.
   - Tombol **Daftar Sekarang** dengan efek `hover:bg-blue-700 focus:ring-2 focus:ring-blue-500 active:bg-blue-800 disabled:opacity-50`.
3. **Dark Mode**
   - Tambahkan dukungan **dark mode** menggunakan kelas `dark:` pada form.
   - Default: `bg-white text-black`, saat dark mode aktif → `dark:bg-gray-900 dark:text-white`.
   - Buat tombol toggle "Ganti Tema" untuk mengaktifkan dark mode.
4. **Layout**
   - Gunakan `max-w-md mx-auto` agar form terpusat.
   - Beri `shadow-md p-6 rounded-lg` untuk membuat card form.
5. **Bonus**
   - Tambahkan utilitas kustom `@layer components` untuk membuat kelas `.btn-primary` yang bisa dipakai ulang.

---

### Output yang Diharapkan

- Form responsif, rapi di tengah layar.
- Input dan tombol memiliki efek interaktif (`hover`, `focus`, `active`).
- Bisa switch ke **dark mode** dengan tombol toggle.
- Jika email tidak valid → border merah.
- Jika checkbox belum dicentang → tombol disabled.

---

## Setup Instructions for Tailwind CSS v4 CLI

### Installation

1. **Install dependencies:**

   ```bash
   npm install
   ```

2. **Build Tailwind CSS:**

   ```bash
   npm run build
   ```

   Or for development with watch mode:

   ```bash
   npm run watch
   ```

3. **Open the HTML files:**
   - Challenge 1: `pages/challenge-1.html` (uses CDN)
   - Challenge 2: `pages/challenge-2.html` (requires build step)

### Project Structure

```
tw-challenge-1/
├── src/
│   └── input.css          # Tailwind source with custom components
├── dist/
│   └── output.css         # Generated CSS (created after build)
├── pages/
│   ├── challenge-1.html   # Profile page with Tailwind CDN
│   └── challenge-2.html   # Registration form with Tailwind CLI
├── challenge/
│   ├── challenge-1.md
│   └── challenge-2.md
└── package.json
```

### Features

**Challenge 1 - Profile Page:**

- Responsive profile card
- Grid-based hobbies section
- Lucide icons
- Orange accent color with monochrome design

**Challenge 2 - Registration Form:**

- Interactive form validation
- Dark mode toggle with localStorage
- Custom button component (.btn-primary)
- Real-time validation feedback
- Disabled state until all requirements met
- Orange-700 accent color
- Lucide icons for visual enhancement

### Technologies Used

- Tailwind CSS v4 (CLI)
- Lucide Icons (CDN)
- Vanilla JavaScript for interactivity
