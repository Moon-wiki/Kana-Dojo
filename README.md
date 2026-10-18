# 五十音 Kana Dojo

Aplikasi web satu-file untuk belajar **hiragana & katakana** (208 huruf: gojūon, dakuten, handakuten, yōon). Tanpa build step, tanpa backend. Buka `index.html` dan langsung jalan.

## Fitur (v2)

| Latihan | Isi |
|---|---|
| 🗂️ Flashcard | Balik kartu, audio pelafalan, contoh kata di sisi belakang |
| ✍️ Papan tulis | Canvas dengan bayangan huruf, grid, undo/hapus, kunci papan anti-scroll |
| 🧪 Kuis | Ketik romaji, skor, riwayat salah |
| 📊 Tabel | Tabel gojūon/dakuten/yōon, ketuk untuk tandai dikuasai |
| 🎯 Adaptif | Huruf yang sering salah / belum dikuasai muncul lebih sering |
| 🔥 Streak | Hari beruntun & statistik, tersimpan di `localStorage` |

## Menjalankan

```bash
# cukup buka file-nya, atau:
python3 -m http.server 8000   # lalu buka http://localhost:8000
```

## Struktur repo

```
index.html              # versi terkini (v2)
versions/
  v0-flashcard/         # prototipe: flashcard saja
  v1-multi-view/        # + papan tulis, tabel, audio
  v2-quiz/              # + kuis, adaptif, persistensi, streak (snapshot)
docs/
  EVOLUTION.md          # analisis perbedaan v0 → v1 → v2
  ROADMAP.md            # rencana v2.1 dan v3.0
.github/
  issues/               # draf issue (dibuat otomatis oleh scripts/create_issues.py)
  labels.yml
scripts/create_issues.py
```

## Riwayat versi

Baca [docs/EVOLUTION.md](docs/EVOLUTION.md) untuk perbandingan lengkap, dan [CHANGELOG.md](CHANGELOG.md) untuk ringkasan.

## Kontribusi

Lihat tab **Issues**. Issue berlabel `good first issue` cocok untuk mulai. Gunakan template yang tersedia.

## Lisensi

MIT. Font dimuat dari Google Fonts (lihat issue tentang self-hosting).
