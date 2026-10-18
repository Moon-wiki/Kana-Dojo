---
title: "PWA, offline, dan font self-host"
labels: type: enhancement, area: infra, priority: medium
milestone: v3.0
state: open
---

**Konteks**
Font dimuat dari Google Fonts (`Shippori Mincho`, `Zen Kaku Gothic New`, `JetBrains Mono`, `Noto Sans JP`). Tanpa jaringan, tampilan jatuh ke font bawaan dan bayangan di papan tulis bisa berbeda. Ada juga isu privasi pihak ketiga.

**Usulan**
Self-host subset font (cukup glyph kana), tambah `manifest.webmanifest` dan service worker.

**Kriteria selesai**
- [ ] Berjalan penuh saat offline
- [ ] Bisa di-install di Android/iOS
