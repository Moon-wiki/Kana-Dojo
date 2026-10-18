---
title: "Streak naik hanya karena halaman dibuka"
labels: type: bug, area: storage, priority: low
milestone: v2.1
state: open
---

**Konteks**
`updateStreak()` jalan saat init dan memakai `toDateString()` (bergantung locale/zona waktu). Membuka tab tanpa belajar tetap menambah streak.

**Usulan**
Hitung streak hanya jika ada aktivitas bermakna (mis. ≥ 5 kartu dilihat atau ≥ 1 jawaban kuis). Simpan tanggal sebagai `YYYY-MM-DD` lokal.

**Kriteria selesai**
- [ ] Aktivitas minimum terdokumentasi
- [ ] Test untuk pergantian hari dan DST
