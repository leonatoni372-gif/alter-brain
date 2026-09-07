# 📓 Jurnal

Ringkasan otomatis dari **agen-jurnal** (tiap 22:05 WIB dari daily note hari itu). File: `ringkasan-YYYY-MM-DD.md`.

```dataview
TABLE WITHOUT ID file.link AS "Ringkasan", selesai AS "Selesai", sisa AS "Sisa"
FROM "05-Jurnal"
WHERE file.name != "Jurnal"
SORT file.name DESC LIMIT 14
```

> Dibuat agen, jangan edit manual file `ringkasan-*`.
