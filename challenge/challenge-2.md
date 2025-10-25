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
