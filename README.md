# Tugas Rutin 4 — Konversi CSS ke SCSS (7-1 Pattern)

Aplikasi web portofolio pribadi hasil *refactoring* dari **Tugas Pertemuan 2** menggunakan **SCSS (SASS)** dengan arsitektur modular **7-1 Pattern**.

## 📌 Pemenuhan Requirements

1. **Konversi CSS Existing ke SCSS:** Seluruh gaya CSS dikonversi penuh ke format SCSS.
2. **Variables:** Deklarasi warna, font, spacing, dan shadow menggunakan variabel SASS di `scss/abstracts/_variables.scss`.
3. **Nesting:** Penerapan nesting bersarang maksimal 3 level (pada komponen `.card` dan `.form`).
4. **Minimal 3 Mixins Reusable:**
   - `@mixin flex-layout` — Helper flexbox.
   - `@mixin card-base` — Styling dasar kontainer/kartu.
   - `@mixin respond-to` — Media query responsif berdasarkan breakpoint map.
5. **Struktur 7-1 Pattern (Partials):** Pembagian folder terstruktur (`abstracts/`, `base/`, `components/`, `layout/`).
6. **Sintaks `@use`:** Mengimpor modul partials menggunakan `@use` (tanpa `@import`).
7. **Control Directives (`@each` Loop):** Penggunaan `@each` loop pada `scss/components/_badges.scss` untuk memproduksi *utility classes* `.badge-*` dari `$status-colors` map.
8. **Kompilasi SASS:** Dikompilasi menggunakan Dart SASS menghasilkan `css/main.css`.

## 🛠️ Arsitektur Folder 7-1 Pattern

```text
TugasWeb-Pertemuan4-SCSS/
├── index.html
├── README.md
├── css/
│   ├── main.css
│   └── main.css.map
└── scss/
    ├── abstracts/
    │   ├── _mixins.scss
    │   └── _variables.scss
    ├── base/
    │   ├── _reset.scss
    │   └── _typography.scss
    ├── components/
    │   ├── _badges.scss
    │   ├── _buttons.scss
    │   ├── _cards.scss
    │   └── _forms.scss
    ├── layout/
    │   ├── _dark-mode.scss
    │   ├── _footer.scss
    │   ├── _grid.scss
    │   ├── _header.scss
    │   └── _sidebar.scss
    └── main.scss
```
 
## 👤 Informasi Mahasiswa

- **Nama:** Tengku Fahreza (4252550005)
- **Class:** PSIK 25B
- **Program Studi:** S1 Ilmu Komputer
- **Mata Kuliah:** Pemrograman Web
- **Instansi:** Universitas Negeri Medan (UNIMED)