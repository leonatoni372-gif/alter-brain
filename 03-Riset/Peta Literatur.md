# 🗺️ Peta Literatur (104 papers)

> Sumber: OpenAlex top-cited 2015+. Isi `💡 Insight-ku` tiap selesai baca satu paper. Ubah `status_baca: sudah` kalau tamat.

## Per domain
```dataview
TABLE WITHOUT ID domain AS "Domain", length(rows) AS "Jumlah", sum(map(rows, (r) => r.sitasi)) AS "Total sitasi"
FROM "03-Riset/Literatur"
GROUP BY domain
SORT length(rows) DESC
```

## 🎯 Antrian baca (sitasi tertinggi, belum dibaca)
```dataview
TABLE WITHOUT ID file.link AS "Paper", tahun AS "Thn", sitasi AS "Sit."
FROM "03-Riset/Literatur"
WHERE status_baca = "belum"
SORT sitasi DESC LIMIT 15
```

## ✅ Sudah dibaca
```dataview
TABLE WITHOUT ID file.link AS "Paper", sitasi AS "Sit."
FROM "03-Riset/Literatur"
WHERE status_baca = "sudah"
SORT sitasi DESC
```

## Per domain detail
- 🌱 Environmental: `domain = environmental`
- ⚙️ Process Engineering: `domain = process-engineering`
- 🧪 Chemical: `domain = chemical`
- 💻 Coding/AI: `domain = coding`
- 🧠 Sosial: `domain = sosial`
- 🏥 Medical: `domain = medical`
- 💰 Economy: `domain = economy`

```dataview
TABLE WITHOUT ID file.link AS "Paper", tahun AS "Thn", sitasi AS "Sit.", status_baca AS "Status"
FROM "03-Riset/Literatur"
SORT sitasi DESC LIMIT 30
```
