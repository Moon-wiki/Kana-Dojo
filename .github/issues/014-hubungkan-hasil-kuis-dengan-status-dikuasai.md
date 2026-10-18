---
title: "Hubungkan hasil kuis dengan status dikuasai"
labels: type: enhancement, area: quiz, priority: medium
milestone: v2.1
state: open
---

**Konteks**
Kuis mengubah `wrongCount` dan `quizStats` tetapi tidak menyentuh `mastered`. Ada dua sistem progres paralel: yang ditandai manual dan yang terukur lewat kuis.

**Usulan**
Opsional dan bisa dimatikan: N jawaban benar beruntun menyarankan "tandai dikuasai". Jawaban salah pada huruf yang sudah dikuasai menurunkan statusnya atau menandainya "perlu diulang".

**Kriteria selesai**
- [ ] Aturan ambang terdokumentasi
- [ ] Pengguna bisa menolak saran
- [ ] Strip statistik tetap konsisten
