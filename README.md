# 🌋 Simulasi Gunung Meletus 3D — Versi 2 (Three.js)

Media pembelajaran IPA — simulasi **3D interaktif** gunung meletus berbasis **Three.js**.
Ini versi 2 dari project [`simulasi-gunung-meletus`](https://simulasi-gunung-meletus-two.vercel.app) (versi 1 = 2D canvas).

## Fitur
- 3D volcano scene: lava fountain, kolom abu, hujan abu, aliran lava, uap panas
- Level status gunung api Indonesia (Normal → Waspada → Siaga → Awas), visual berubah tiap level
- Zona bahaya tampil sesuai level (radius kawah → siaga → evakuasi)
- Skenario erupsi otomatis (Level 2 → 3 → 4 → turun lagi)
- Panel materi edukasi: penyebab, tanda-tanda, level status, mitigasi
- Kamera orbit 3D: geser = putar, scroll = zoom; auto-rotate saat idle
- Mobile-friendly (HUD responsif, touch control)

## Teknis
- Static site tanpa backend. Three.js via CDN importmap (unpkg).
- Deploy Vercel: `vercel --prod --yes`

## Struktur
```
├── index.html    # seluruh aplikasi (HTML + CSS + Three.js)
├── vercel.json   # cleanUrls
└── README.md
```