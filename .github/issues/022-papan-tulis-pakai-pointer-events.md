---
title: "Papan tulis: pakai Pointer Events"
labels: type: enhancement, area: board, priority: medium
milestone: v2.1
state: open
---

**Konteks**
Input memakai `mousedown/mousemove` dan `touchstart/touchmove` terpisah, dan `getPos` hanya membaca `touches[0]`. Stylus dan multi-touch tidak optimal, dan palm rejection tidak ada.

**Usulan**
Ganti dengan `pointerdown/move/up` + `setPointerCapture`, dan abaikan pointer kedua. Opsional: ketebalan garis dari `pressure`.

**Kriteria selesai**
- [ ] Berfungsi di Chrome, Safari iOS, Firefox
- [ ] Scroll vertikal tetap jalan saat papan terkunci
