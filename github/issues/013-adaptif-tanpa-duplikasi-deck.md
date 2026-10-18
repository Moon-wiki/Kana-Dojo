---
title: "Adaptif tanpa duplikasi deck"
labels: type: bug, area: flashcard, priority: high
milestone: v2.1
state: open
---

**Konteks**
`buildDeckList()` memperluas deck dengan mengulang objek sesuai bobot. Akibatnya:
- Counter menunjukkan jumlah palsu (mis. "huruf 1 / 150" padahal 46 huruf)
- Huruf yang sama bisa muncul berurutan
- Bar progres dan deck tidak lagi satu skala

**Usulan**
Pertahankan deck asli. Pilih kartu berikutnya dengan *weighted random sampling*, dengan aturan tidak mengulang kartu yang baru saja muncul. Counter menghitung kartu unik yang sudah dilihat di sesi ini.

**Kriteria selesai**
- [ ] Counter menunjukkan jumlah huruf asli
- [ ] Tidak ada pengulangan berurutan
- [ ] Bobot tetap mengikuti `wrongCount` dan `mastered`
