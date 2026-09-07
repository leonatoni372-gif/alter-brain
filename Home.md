# 🧠 ALTER BRAIN

> Semua yang belum ada tempatnya → [[00-Inbox/]] dulu, sortir tiap weekend.

## 📥 Tugas terbuka (semua vault)
```dataview
TASK WHERE !completed SORT file.mtime DESC LIMIT 20
```

## 📅 7 hari terakhir
```dataview
TABLE WITHOUT ID file.link AS "Daily", length(filter(file.tasks, (t) => !t.completed)) AS "Todo sisa"
FROM "01-Daily"
SORT file.name DESC LIMIT 7
```

## 📚 Kuliah terakhir disentuh
```dataview
TABLE WITHOUT ID file.link AS "Catatan", matkul AS "Matkul"
FROM "02-Kuliah"
SORT file.mtime DESC LIMIT 10
```

## 🔬 Riset aktif
```dataview
TABLE WITHOUT ID file.link AS "Topik", status AS "Status"
FROM "03-Riset"
SORT file.mtime DESC LIMIT 10
```

## 💰 Keuangan terakhir
```dataview
TABLE WITHOUT ID file.link AS "Laporan", jam_wib AS "Jam", jumlah_baris AS "Baris"
FROM "04-Keuangan"
WHERE file.name != "Keuangan"
SORT file.name DESC LIMIT 5
```
