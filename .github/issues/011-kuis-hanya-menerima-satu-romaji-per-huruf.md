---
title: "Kuis hanya menerima satu romaji per huruf"
labels: type: bug, area: quiz, priority: high
milestone: v2.1
state: open
---

**Konteks**
`checkAnswer()` membandingkan input dengan `item.romaji` persis. Jawaban sah lain dianggap salah, misalnya `si`, `ti`, `tu`, `hu`, `sya`, `zya`, `tya`, `nn` untuk ん, dan `o` untuk を.

**Usulan**
Tambah peta alias (Hepburn + Kunrei-shiki + Nihon-shiki umum) di data, lalu cocokkan terhadap daftar jawaban valid. Tampilkan bentuk utama saat salah.

**Kriteria selesai**
- [ ] `si`, `ti`, `tu`, `hu`, `sya`, `tya`, `zya` diterima
- [ ] Alias hidup di data, bukan di kode kuis
- [ ] Test unit untuk 208 huruf
