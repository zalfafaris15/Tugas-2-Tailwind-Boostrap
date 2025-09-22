# 📘 README – Tugas 2 Tailwind & Bootstrap

## Pertanyaan & Jawaban

### 1. Mengapa memilih konfigurasi col- tertentu untuk tiap breakpoint?  
Karena dengan **grid system Bootstrap** maupun **utility Tailwind**, setiap breakpoint (`sm`, `md`, `lg`, `xl`) membantu tampilan website menyesuaikan ukuran layar (responsive). Misalnya di layar HP hanya 1 kolom, di tablet 2 kolom, dan di laptop/PC bisa 3–4 kolom. Konfigurasi ini membuat user experience lebih baik di berbagai perangkat.

---

### 2. Bagaimana kamu merancang tombol *Follow* pada profil tetap mudah diklik walaupun di mobile?  
Saya menggunakan utility class seperti `px-4 py-2 rounded-md` (Tailwind) atau `btn btn-primary` (Bootstrap) agar tombol cukup besar, memiliki padding yang nyaman, dan border radius supaya terlihat modern. Di mobile tombol otomatis **full width (w-full)** sehingga lebih mudah diklik dengan jari.

---

### 3. Jelaskan penataan layout profil (foto, nama, bio, jumlah postingan, followers, following).  
Layout dibuat menggunakan grid/flex:  
- Foto profil ditaruh di sisi kiri (pada layar besar) dan di atas (pada layar kecil).  
- Nama, bio, dan tombol *Follow* diletakkan di samping/ bawah foto.  
- Statistik (posting, followers, following) menggunakan grid 3 kolom agar rata dan konsisten.  

---

### 4. Jika postingan bertambah jadi 50, apa potensi masalah dan bagaimana solusinya?  
Potensi masalah: halaman akan jadi panjang sekali dan berat saat loading.  
Solusi: tambahkan **pagination**, **infinite scroll**, atau fitur **lazy loading** untuk gambar supaya performa tetap optimal.

---

### 5. Jelaskan keputusan grid col-(x) apa di tiap breakpoint — kenapa begitu?  
- Mobile (`sm:`) → 1 kolom, agar konten mudah dibaca.  
- Tablet (`md:`) → 2 kolom, memanfaatkan layar lebih lebar.  
- Desktop (`lg:`/`xl:`) → 3 kolom atau lebih, supaya postingan banyak terlihat sekaligus.  

Keputusan ini mengikuti prinsip **responsive web design**.

---

### 6. Utility responsiveness lain yang kamu gunakan?  
Saya menggunakan utility seperti:  
- `max-w-screen-lg` → membatasi lebar konten di layar besar.  
- `p-4 md:p-6` → padding berbeda di layar kecil & besar.  
- `hidden md:block` → menyembunyikan elemen di HP tapi tampil di desktop.  

---

### 7. Jelaskan trade-off antara memakai banyak utility classes vs membuat component CSS tersendiri.  
- **Utility classes (Tailwind):** cepat, konsisten, langsung terlihat hasilnya, tapi kadang membuat HTML panjang.  
- **Component CSS tersendiri:** lebih rapi dan reusable, tapi butuh file CSS tambahan dan bisa memakan waktu lebih lama.  

Solusi terbaik biasanya **kombinasi**: gunakan utility untuk styling cepat, tapi jika pattern berulang, lebih baik dibuat component CSS.
