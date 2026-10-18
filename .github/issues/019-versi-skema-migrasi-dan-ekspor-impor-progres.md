---
title: "Versi skema, migrasi, dan ekspor/impor progres"
labels: type: enhancement, area: storage, priority: medium
milestone: v2.1
state: open
---

**Konteks**
Kunci `kanaDojoData_v2` tidak membawa nomor skema internal. Perubahan bentuk data (mis. alias, SRS) akan memutus progres lama. Pengguna juga tidak bisa memindahkan progres antar perangkat.

**Usulan**
- Tambah `schemaVersion` dan fungsi migrasi berurutan
- Tombol "ekspor JSON" dan "impor JSON" (dengan validasi)

**Kriteria selesai**
- [ ] Data v2 tetap terbaca setelah upgrade
- [ ] Impor menolak berkas rusak dengan pesan jelas
