---
title: "Beri tahu pengguna jika penyimpanan gagal"
labels: type: bug, area: storage, priority: high
milestone: v2.1
state: open
---

**Konteks**
`saveState()` menelan error `localStorage` secara diam-diam (mode privat, penyimpanan penuh, cookie diblokir). Pengguna mengira progres tersimpan padahal hilang saat ditutup.

**Usulan**
Deteksi saat load. Jika tidak bisa, tampilkan banner kecil "progres tidak akan tersimpan di mode ini". Fallback ke memori.

**Kriteria selesai**
- [ ] Banner muncul di mode privat Safari / Firefox
- [ ] Tidak ada exception tak tertangani
