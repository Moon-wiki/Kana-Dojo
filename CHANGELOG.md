# Changelog

Format mengikuti [Keep a Changelog](https://keepachangelog.com/).

## [2.0.0]
### Ditambahkan
- Tab **kuis** romaji dengan skor dan umpan balik benar/salah
- **Mode adaptif** (pembobotan huruf belum dikuasai dan sering salah)
- **Persistensi** progres lewat `localStorage` (`kanaDojoData_v2`)
- **Streak harian** dan strip statistik
- **Contoh kata** (kata, bacaan, arti) di flashcard, papan tulis, dan kuis
- Dialog konfirmasi saat reset progres

## [1.0.0]
### Ditambahkan
- Navigasi multi-view: flashcard, **papan tulis**, **tabel**
- Papan tulis canvas: bayangan huruf, grid, undo, hapus, kunci papan
- **Audio** pelafalan (Web Speech API, `ja-JP`)
- Jumlah goresan per huruf
- Tabel evaluasi gojūon/dakuten/yōon
### Diubah
- Kunci progres disederhanakan: `script:kana:romaji` → `script:kana`
- Istilah "hafal" → "dikuasai" di sebagian UI

## [0.1.0]
- Prototipe flashcard hiragana/katakana/campur, filter baris, acak, tandai hafal (hanya di memori)
