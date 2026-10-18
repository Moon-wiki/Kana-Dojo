---
title: "Spaced repetition sungguhan (Leitner atau SM-2)"
labels: type: enhancement, area: flashcard, priority: medium
milestone: v3.0
state: open
---

**Konteks**
Mode adaptif sekarang hanya pembobotan sesi, tanpa jadwal ulang. Huruf yang dikuasai tidak pernah kembali pada waktu yang tepat.

**Usulan**
Kotak Leitner 5 tingkat (atau SM-2 sederhana) dengan `dueAt` per huruf. Tampilan "ulang hari ini: N huruf". Gantikan `weightFor()`.

**Kriteria selesai**
- [ ] Data `dueAt` dan `box` tersimpan dan termigrasi
- [ ] Sesi harian berisi huruf jatuh tempo + beberapa huruf baru
