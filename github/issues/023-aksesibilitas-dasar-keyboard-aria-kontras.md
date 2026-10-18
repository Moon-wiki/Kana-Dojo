---
title: "Aksesibilitas dasar: keyboard, ARIA, kontras"
labels: type: enhancement, area: a11y, priority: high
milestone: v2.1
state: open
---

**Konteks**
- Kartu flashcard adalah `div` dengan `click`, tidak fokus dan tidak punya role
- Tab (`home-tab`, `tab`, `row-chip`) tanpa `role="tablist"` / `aria-selected`
- Hasil kuis tidak diumumkan ke pembaca layar (`aria-live`)
- `prefers-reduced-motion` hanya ditangani di v0

**Usulan**
Jadikan kartu `button` atau beri `tabindex`, `role`, dan tangani Enter/Spasi. Tambah ARIA untuk tab. Tambah `aria-live="polite"` pada umpan balik kuis. Pulihkan dukungan reduced-motion. Cek kontras teks abu pada latar washi.

**Kriteria selesai**
- [ ] Seluruh alur bisa dipakai tanpa mouse
- [ ] Lulus audit Lighthouse a11y ≥ 95
