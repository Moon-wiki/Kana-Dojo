---
title: "Pecah `index.html` menjadi modul (css/js) dengan build opsional"
labels: type: refactor, area: infra, priority: medium
milestone: v2.1
state: open
---

**Konteks**
v2 sudah 972 baris dalam satu file dengan state global dan listener tersebar. Fitur v3 akan mempersulit.

**Usulan**
Struktur `src/` (`state`, `storage`, `deck`, `views/*`, `data`) dan Vite dengan plugin single-file agar rilis tetap satu `index.html`. Tanpa framework dulu.

**Kriteria selesai**
- [ ] `npm run build` menghasilkan satu `dist/index.html`
- [ ] Perilaku v2 tidak berubah (cek manual dengan daftar di PR)
