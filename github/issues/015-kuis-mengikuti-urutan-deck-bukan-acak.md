---
title: "Kuis mengikuti urutan deck, bukan acak"
labels: type: bug, area: quiz, priority: medium, good first issue
milestone: v2.1
state: open
---

**Konteks**
Kuis memakai `state.deck` dan `next()` yang sama dengan flashcard. Pada mode non-adaptif urutannya a, i, u, e, o, ka, ki… sehingga jawaban bisa ditebak dari pola.

**Usulan**
Kuis punya antrean sendiri yang diacak per ronde, dengan opsi "ronde = semua huruf terpilih" dan ringkasan di akhir ronde.

**Kriteria selesai**
- [ ] Urutan acak per ronde
- [ ] Ringkasan akhir ronde (benar/salah, huruf yang meleset)
