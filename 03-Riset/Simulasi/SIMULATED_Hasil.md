---
tags: [simulasi, riset]
---

# Hasil Simulasi (SYNTHETIC — BUKAN data eksperimen)

> Model benar: Langmuir qmax=25.0 mg/g, KL=0.08 L/mg; noise 5%.
> Pipeline fitting di bawah ini SAMA yang dipakai untuk data real nanti.

## Isotherm (V=50 mL, m=3 g, pH 5)

| C₀ (mg/L) | Ce (mg/L) | qe (mg/g) | Removal (%) |
|---|---|---|---|
| 5 | 1.059 | 1.97 | 78.8 |
| 10 | 2.262 | 3.869 | 77.4 |
| 20 | 5.208 | 7.396 | 74.0 |
| 40 | 14.265 | 12.868 | 64.3 |
| 60 | 25.998 | 17.001 | 56.7 |
| 80 | 38.449 | 20.775 | 51.9 |
| 100 | 59.746 | 20.127 | 40.3 |

**Fitting Langmuir (Ce/qe vs Ce):** qmax = 25.1 mg/g | KL = 0.082 L/mg | R² = 0.9910
→ recovery qmax 100.2% dari nilai benar (validasi pipeline OK).

## Kinetika PSO (C0=20 mg/L)

| t (min) | qt (mg/g) |
|---|---|
| 10 | 4.3653 |
| 20 | 5.4781 |
| 30 | 6.0428 |
| 40 | 6.3565 |
| 60 | 6.8642 |
| 90 | 7.0 |
| 120 | 7.0102 |

**Fitting PSO (t/qt vs t):** qe = 7.474 mg/g (benar 7.381) | R² = 0.9995

## Cara pakai untuk data real
1. Ganti isi CSV dengan angka lab (hapus kolom NOTE).
2. Set `SIMULATE=False`, jalankan ulang → tabel + R² langsung jadi.
3. Plot grafik di Excel dari CSV (Ce/qe vs Ce; t/qt vs t).
