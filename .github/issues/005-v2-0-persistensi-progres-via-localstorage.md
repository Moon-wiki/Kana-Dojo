---
title: "[v2.0] Persistensi progres via localStorage"
labels: shipped, type: enhancement, area: storage
milestone: v2.0
state: closed
---

**Dari:** v1 → v2

`saveState()` / `loadState()` dengan kunci `kanaDojoData_v2`. Tersimpan: `mastered`, `wrongCount`, `quizStats`, `adaptiveMode`, `streak`, `lastVisitDate`. Dibungkus `try/catch`.

Menutup kekurangan v0/v1 di mana progres hilang saat refresh (v0 hanya punya stub mati `loadKnown`).
