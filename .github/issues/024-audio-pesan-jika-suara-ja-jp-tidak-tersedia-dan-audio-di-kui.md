---
title: "Audio: pesan jika suara ja-JP tidak tersedia, dan audio di kuis"
labels: type: enhancement, area: flashcard, priority: medium
milestone: v2.1
state: open
---

**Konteks**
`speakCurrent()` langsung keluar jika `speechSynthesis` tidak ada, dan tidak memeriksa apakah ada suara Jepang terpasang. Tombol 🔊 terlihat rusak di perangkat tanpa suara itu. Kuis tidak punya audio.

**Usulan**
Cek `getVoices()` (tunggu `voiceschanged`). Jika tidak ada suara `ja`, nonaktifkan tombol dengan tooltip jelas. Tambah 🔊 di kuis setelah menjawab.

**Kriteria selesai**
- [ ] Tombol nonaktif + penjelasan saat tidak didukung
- [ ] Audio tersedia di kuis
