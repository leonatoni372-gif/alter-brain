# 💰 Keuangan

Laporan otomatis dari **agen-keuangan** (cron tiap 2 jam WIB, rekap di 06/12/16/20). File per jam: `laporan-YYYY-MM-DD-HH00.md`. Daily note hari terkait juga ditempeli ringkasan + link ke sini.

```dataview
TABLE WITHOUT ID file.link AS "Laporan", jam_wib AS "Jam", jumlah_baris AS "Baris"
FROM "04-Keuangan"
WHERE file.name != "Keuangan"
SORT file.name DESC LIMIT 20
```

> Datang dari GitHub (agen push) → Obsidian Git yang pull. Jangan edit manual file `laporan-*`.
