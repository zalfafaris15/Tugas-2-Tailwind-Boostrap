# 📘 README – Tugas 2 Tailwind & Bootstrap

## Jawaban Pertanyaan README

1. **Kenapa pilih konfigurasi col di tiap breakpoint?**  
   Agar tampilan responsive: mobile 1 kolom, tablet 2 kolom, desktop 3–4 kolom. Ini membuat website mudah digunakan di semua perangkat.

2. **Tombol Follow tetap mudah di mobile?**  
   Tombol diberi padding besar (`px-4 py-2`), full width (`w-full`) di mobile, dan menggunakan utility `rounded` agar nyaman diklik.

3. **Jika postingan bertambah jadi 50, masalah & solusi?**  
   Masalah: halaman jadi panjang & berat.  
   Solusi: gunakan pagination, infinite scroll, atau lazy loading gambar.

4. **Keputusan grid-cols/gap di tiap breakpoint?**  
   - `sm:` → 1 kolom (mudah dibaca di HP).  
   - `md:` → 2 kolom (tablet).  
   - `lg:` → 3 kolom+ (desktop).  
   Gap diatur agar jarak antar posting tidak terlalu rapat.

5. **Utility responsive yang dipakai?**  
   - `p-4 md:p-6` → padding berbeda di HP & desktop.  
   - `hidden md:block` → sembunyikan elemen di HP.  
   - `max-w-screen-lg` → batasi lebar di layar besar.

6. **Trade-off utility classes vs component CSS?**  
   - Utility: cepat, konsisten, tapi HTML jadi panjang.  
   - Component CSS: rapi & reusable, tapi perlu file tambahan.  
   👉 Solusi: kombinasi keduanya.
