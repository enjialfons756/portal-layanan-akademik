# Portal Layanan Akademik

Tugas Pertemuan 5 – Responsive & Accessible Web Client.
Halaman web responsif dan aksesibel dengan HTML semantik, CSS mobile-first, form valid, tanpa JavaScript.

## Struktur proyek
```
index.html
css/styles.css
img/        (aset gambar, bila ada)
evidence/   (screenshot bukti DevTools)
README.md
```

## Link
- Aplikasi: https://enjialfons756.github.io/portal-layananankademik/
- Repository: https://github.com/enjialfons756/portal-layananankademik

## Keputusan desain
- **Semantik:** `header`, `nav`, `main` (2 `section`), `footer`; satu `h1`, `h2` per section, `h3` per kartu.
- **Mobile-first:** gaya dasar satu kolom; breakpoint 768px (kartu 2 kolom, tipografi lebih besar) dan 1280px (kartu 3 kolom) dipilih karena konten mulai lebar/renggang, bukan karena nama perangkat.
- **Layout:** Flexbox untuk nav dan kartu, Grid untuk daftar kartu dan intro desktop.
- **Form:** label terasosiasi (`for`/`id`), `fieldset`+`legend` untuk radio jenis layanan, `required`, `type="email"`, `<button type="submit">`.
- **Aksesibilitas:** skip link, `:focus-visible` jelas, kontras teks ≥ 4.5:1, target sentuh ≥ 44px, `alt` bermakna pada gambar, `prefers-reduced-motion`.

## Hasil pengujian DevTools
Isi sesuai hasil pengujianmu, simpan screenshot di folder `evidence/`.

| No | Pemeriksaan | Alat | Temuan / Perbaikan | Bukti |
|----|-------------|------|--------------------|-------|
| 1 | Viewport 360px | Responsive Mode | Tidak ada horizontal scroll, 1 kolom | evidence/360.png |
| 2 | Viewport 768px | Responsive Mode | Kartu 2 kolom | evidence/768.png |
| 3 | Viewport 1280px | Responsive Mode | Kartu 3 kolom | evidence/1280.png |
| 4 | Reload halaman | Network | Semua resource (HTML, CSS) status 200, tidak ada yang gagal | evidence/network.png |
| 5 | Struktur DOM & CSS | Elements/Inspector | Landmark dan heading hierarchy sesuai | evidence/elements.png |
| 6 | Aksesibilitas | Accessibility tree / Lighthouse | Label form terbaca, kontras lolos | evidence/a11y.png |
| 7 | Keyboard | Tab manual | Semua kontrol terjangkau, fokus terlihat | evidence/keyboard.png |
