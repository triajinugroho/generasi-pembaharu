---
id: flashcards-readme
title: "Flashcards — Spaced Repetition per Bab"
chapter: flashcards
order: 0
level: lintas
personas: [aktivis-baru, pembaca-mandiri, murabbi]
reading_time_min: 2
tags: [flashcards, spaced-repetition, anki, mochi, latihan, mikro]
outcomes:
  - "Mendapat kartu Q&A untuk spaced repetition dari tiap bab"
  - "Mengimpor ke Anki/Mochi untuk review harian"
prerequisites: []
related: [root-readme, ringkasan-readme]
last_reviewed: 2026-04-18
---

# Flashcards — Spaced Repetition per Bab

> *"Ikatlah ilmu dengan menuliskannya."*
> — Atsar yang masyhur

Direktori ini menyimpan **flashcards Q&A** untuk tiap bab — dirancang untuk latihan harian 5-10 menit dengan metode [spaced repetition](https://en.wikipedia.org/wiki/Spaced_repetition).

## Mengapa Flashcards?

Membaca bab sekali tidak cukup. Bab 1 yang Anda baca bulan lalu — berapa banyak yang bisa Anda recall hari ini?

Flashcards mengatasi *forgetting curve*. Review 5 menit/hari bertahun-tahun lebih efektif daripada membaca ulang 1 jam sekali-sekali.

## Format

Setiap file `ch<N>.md` berisi ~10-20 kartu dalam format markdown sederhana:

```markdown
## Q: <pertanyaan>
A: <jawaban>

Sumber: [<file id>](<path>)
Tag: <bab>, <tema>
```

## Cara Pakai

### Di browser / GitHub

Baca langsung. Tutupi jawaban dengan tangan/kertas, coba jawab, buka cek.

### Di Anki (spaced repetition scheduler)

1. Install [Anki](https://apps.ankiweb.net/) (gratis, multi-platform).
2. Pakai add-on community **Markdown Import** atau tool CLI `md2anki`.
3. Import file `ch<N>.md`.
4. Review tiap hari. Anki otomatis jadwal ulang berdasarkan recall Anda.

### Di Mochi / RemNote / Obsidian

Format ini bisa dibaca oleh mayoritas tool knowledge management modern.

## Daftar Kartu

| Bab | File | Status |
|-----|------|--------|
| 0 | Mukadimah | _menunggu draf_ |
| 1 | Fondasi Aqidah | [`ch1.md`](./ch1.md) _contoh tersedia_ |
| 2 | Sirah & Sejarah | _menunggu draf_ |
| 3 | Pembangunan Diri | _menunggu draf_ |
| 4 | Strategi Dakwah | _menunggu draf_ |
| 5 | Titik Temu Gerakan | _menunggu draf_ |
| 6 | Tantangan Kontemporer | _menunggu draf_ |
| 7 | Penutup | _menunggu draf_ |

Template untuk kontributor: [`TEMPLATE.md`](./TEMPLATE.md).

## Prinsip Desain Kartu

- **Satu kartu = satu ide**. Jangan gabung 3 konsep dalam 1 kartu.
- **Pertanyaan spesifik**. Bukan *"Apa itu tauhid?"* (terlalu luas) tapi *"Apa 3 dimensi tauhid menurut Bab 1.1?"*.
- **Jawaban padat**. Maksimal 3 kalimat. Detail ada di bab asli.
- **Sumber wajib**. Link balik ke file sumber untuk verifikasi.
- **Hindari pertanyaan pengetahuan ensiklopedis murni** (tahun, nama, angka) kecuali kritis untuk pemahaman — lebih bagus pertanyaan konsep yang butuh penalaran.

## Peringatan

- Flashcards **bukan pengganti** pembacaan utuh. Ia pelengkap recall.
- Jangan belajar dari flashcards saja tanpa pernah baca sumber — pemahaman akan dangkal.
- Adab: materi dakwah dan aqidah perlu **dihayati**, bukan hanya dihafal. Flashcards membantu ingat; hati harus tetap disentuh oleh bab utuh.

## 📚 Bacaan Terkait

- [`TEMPLATE.md`](./TEMPLATE.md) — struktur kartu standar.
- [`ch1.md`](./ch1.md) — contoh siap pakai untuk Bab 1.
- [`ringkasan/`](../ringkasan/) — pelengkap untuk sharing.
