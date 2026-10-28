# Studi Ablasi RNN, LSTM, GRU vs ANN untuk Prediksi Trafik Seluler Milan

Tugas Workshop Deep Learning — Teknik Telekomunikasi ITERA.

<!-- Ganti seluruh isian bertanda [ ... ] di bawah. Hapus komentar ini. -->

## Kelompok

| Peran | Nama | NIM |
|---|---|---|
| Ketua | [Syarif Hidayatullah] | [124400082] |
| Anggota | [Aura Ikhwat Riharja] | [124400010] |
| Anggota | [Revana Tiara Oksanda] | [124400019] |

- **Kelas:** [RB]
- **Lokasi kelompok:** [0] — [Stazione Centrale] (digit terakhir NIM terkecil)
- **Laporan:** [`laporan-latex/main.pdf` atau `laporan-typst/main.pdf`]

## Cara Menjalankan

```bash
uv sync
uv run jupyter lab
```

Buka `tugas_ablasi.ipynb`, isi `LOKASI_KELOMPOK`, lalu jalankan semua sel. Semua run tercatat di `hasil/ablasi.csv`.

Perangkat yang kami pakai: [laptop CPU Ryzen 3 / Google Colab T4], total waktu training: [16.2] menit.

## Ringkasan Hasil

[File ablasi (D).csv memuat 360 catatan eksperimen: 90 catatan untuk masing-masing model ANN, RNN, LSTM, dan GRU. Dari seluruh catatan yang ada, nilai test MAE terendah yang tercatat adalah ANN sebesar 248,52, RNN sebesar 211,25, LSTM sebesar 223,09, dan GRU sebesar 203,82.]

## Struktur

```
tugas_ablasi.ipynb      notebook eksperimen (di-commit beserta output)
data/                   data trafik per jam (Duomo + 10 lokasi tugas)
hasil/                  CSV seluruh run, tabel, dan grafik
laporan-latex/ atau laporan-typst/   sumber laporan + PDF
```

## Data

Telecom Italia Big Data Challenge (Barlacchi dkk., 2015, *Scientific Data*, lisensi ODbL), versi per jam dari Zhang dkk. (INFOCOM 2021). Disiapkan oleh pengajar di repo [mctosima/dl-workshop](https://github.com/mctosima/dl-workshop).
