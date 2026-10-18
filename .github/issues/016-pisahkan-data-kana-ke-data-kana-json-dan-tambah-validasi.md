---
title: "Pisahkan data kana ke `data/kana.json` dan tambah validasi"
labels: type: refactor, area: data, priority: high
milestone: v2.1
state: open
---

**Konteks**
Data hiragana/katakana (104 huruf masing-masing) tertanam di tuple array dan disalin tiga kali di v0, v1, v2. Struktur tuple (`x[3]`, `x[4]`…) rapuh dan sulit dibaca.

**Usulan**
- Satu sumber: `data/kana.json` dengan objek bernama (`kana`, `romaji`, `aliases`, `group`, `strokes`, `example`)
- Skrip validasi: jumlah 104 per skrip, tidak ada kana duplikat, katakana sejajar dengan hiragana, semua `group` ada di `ROW_ORDER`
- Tuple lama dimigrasi otomatis

**Kriteria selesai**
- [ ] `node scripts/validate-data.mjs` lulus
- [ ] Aplikasi membaca dari JSON (inline saat build jika tetap single-file)
