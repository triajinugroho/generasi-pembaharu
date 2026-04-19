---
id: ringkasan-visual-readme
title: "Ringkasan Visual per Bab (Mermaid Diagrams)"
chapter: ringkasan
order: 3
level: lintas
personas: [aktivis-baru, pembaca-mandiri, murabbi, ketua-ldk]
reading_time_min: 1
tags: [ringkasan, visual, mermaid, diagram, story, infografik]
outcomes:
  - "Mendapat diagram padat yang merangkum satu bab"
prerequisites: []
related: [ringkasan-readme, meta-peta-konsep]
last_reviewed: 2026-04-18
---

# Ringkasan Visual per Bab

Satu Mermaid diagram per bab. Dirender langsung oleh github.com. Screenshot untuk status WhatsApp / IG story / slide pendek.

## Contoh: Bab 1 — Tauhid sebagai Pembebasan

```mermaid
flowchart TD
    T((Tauhid<br/>La ilaha illallah))
    T --> P[Pembebasan dari Thaghut]
    P --> T1[Materialisme]
    P --> T2[Opini Publik]
    P --> T3[Hawa Nafsu]
    P --> T4[Ideologi Dominan]
    T --> A[Aksi Sosial]
    A --> A1[Menegakkan Keadilan]
    A --> A2[Melawan Tirani]
    A --> A3[Membongkar Penindasan]
    classDef hub fill:#0a4d3f,stroke:#0a4d3f,color:#fff
    class T hub
```

Ambil screenshot, post dengan caption: *"Tauhid bukan dogma — ia pembebasan. Baca [link bab]."*

## Contoh: Bab 5 — Titik Temu

```mermaid
flowchart LR
    NU[NU]
    MUH[Muhammadiyah]
    PSS[Persis]
    SALAFI[Salafi]
    TAR[Tarbiyah / LDK]
    HIJ[Hijrah Populer]

    NU & MUH & PSS & SALAFI & TAR & HIJ --> TT[Titik Temu]
    TT --> T1[Aqidah Tauhid]
    TT --> T2[Akhlak Nabawi]
    TT --> T3[Misi Umat]
    classDef hub fill:#7d4f00,stroke:#7d4f00,color:#fff
    class TT hub
```

---

## Status per Bab

| Bab | Status |
|-----|--------|
| 0 | menunggu draf |
| 1 | contoh di atas |
| 2 | menunggu draf |
| 3 | menunggu draf |
| 4 | menunggu draf |
| 5 | contoh di atas |
| 6 | menunggu draf |
| 7 | menunggu draf |

## Cara Kontribusi

1. Baca bab asli. Identifikasi 1 konsep inti yang bisa divisualisasikan.
2. Gambar di Mermaid Live Editor (mermaid.live) — gratis, no login.
3. Simpan sebagai `ch<N>.md` dengan blok ```` ```mermaid ```` di dalam.
4. Buka PR.

**Tips**:
- Pakai `flowchart` untuk konsep statis, `timeline` untuk sirah, `pie` untuk distribusi.
- Maksimum 8-10 node per diagram — lebih dari itu sulit screenshot.
- Label dalam Indonesia.
- Pakai `classDef` untuk highlight node utama dengan warna.

## 📚 Bacaan Terkait

- [`peta-konsep.md`](../../peta-konsep.md) — diagram lintas-bab.
- [`GAYA-PENULISAN.md §6`](../../GAYA-PENULISAN.md) — aturan Mermaid di repo.
