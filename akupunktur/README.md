# Navigasi 12 Meridian Akupunktur

Aplikasi web ringan untuk navigasi 12 meridian utama + database 244 penyakit dengan saran titik akupunktur.

## Ukuran (perbandingan)

| Versi | Ukuran |
|-------|--------|
| Asli (base64 + list statis) | **1.06 MB** (1 file) |
| Optimasi sebelumnya (gambar dipisah) | ~590 KB |
| **Versi ini (JSON + gambar)** | **~590 KB total** |
| → `index.html` saja | **37 KB** |
| → Data JSON | ~102 KB |
| → Gambar | ~451 KB |

Saat di-host di GitHub Pages, file otomatis dikompres (gzip/brotli).

## Struktur folder

```
.
├── index.html          # UI + logika (37 KB)
├── data/
│   ├── meridians.json  # 12 meridian + titik
│   ├── diseases.json   # 244 penyakit
│   └── meta.json       # sistem tubuh + kelas
├── img/                # 30 diagram meridian
└── README.md
```

## Perbaikan yang dilakukan

- Data dipisah ke file JSON (lebih mudah diedit & di-maintain)
- Banyak kesalahan penulisan nama penyakit diperbaiki (OCR error dari buku)
- Gambar dioptimasi
- List penyakit statis dihapus (dibangun ulang oleh JS)

## Cara deploy ke GitHub Pages

1. Buat repository baru di GitHub.
2. Upload **seluruh isi folder** ini.
3. Settings → Pages → Source: branch `main` / root.
4. Akses: `https://USERNAME.github.io/NAMA-REPO/`

## Catatan

Sumber data: buku *Akupunktur Medik* (Kiswojo, 2013).
Beberapa nama penyakit & ICD masih bisa diperbaiki lebih lanjut jika ada referensi asli yang lebih jelas.
