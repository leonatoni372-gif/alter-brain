# 🧠 Core Ilmu

> Satu simpul pusat semua pengetahuan. Setiap literature note menaut balik ke sini (`core: [[Core Ilmu]]`). Mulai eksplorasi dari tabel grup di bawah.

## 🗂️ Kelompok ilmu
```dataview
TABLE WITHOUT ID
  choice(domain = "amdal", "🏭 AMDAL", choice(domain = "k3", "🦺 K3",
  choice(domain = "arsitektur", "🏛️ Arsitektur", choice(domain = "bencana", "🌊 Bencana",
  choice(domain = "energi", "⚡ Energi", choice(domain = "air", "💧 Air",
  choice(domain = "material", "🧱 Material", choice(domain = "biologi", "🧬 Biologi",
  choice(domain = "fisika", "⚛️ Fisika", choice(domain = "matematika", "📐 Matematika",
  choice(domain = "pangan", "🌾 Pangan", choice(domain = "komputer", "💻 Komputer",
  choice(domain = "transportasi", "🚚 Transportasi", choice(domain = "coding", "🤖 Coding/AI",
  choice(domain = "sosial", "🧠 Sosial", choice(domain = "medical", "🏥 Medical",
  choice(domain = "economy", "💰 Ekonomi", choice(domain = "environmental", "🌱 Environmental",
  choice(domain = "process-engineering", "⚙️ Process-Eng",
  choice(domain = "iot", "📡 IoT", "🧪 " + domain)))))))))))))))))))) AS "Kelompok",
  length(rows) AS "Notes",
  sum(map(rows, (r) => r.sitasi)) AS "Total sitasi"
FROM "03-Riset/Literatur"
GROUP BY domain
SORT length(rows) DESC
```

## 🌟 Top cited per kelompok (pintu masuk tiap ilmu)
```dataview
TABLE WITHOUT ID domain AS "Grup", file.link AS "Paper", sitasi AS "Sit."
FROM "03-Riset/Literatur"
SORT sitasi DESC LIMIT 20
```

## 📖 Antrian baca global
```dataview
TABLE WITHOUT ID file.link AS "Paper", domain AS "Grup", sitasi AS "Sit."
FROM "03-Riset/Literatur"
WHERE status_baca = "belum"
SORT sitasi DESC LIMIT 15
```

## 📊 Progress
```dataview
TABLE WITHOUT ID status_baca AS "Status", length(rows) AS "Jumlah"
FROM "03-Riset/Literatur"
GROUP BY status_baca
```
