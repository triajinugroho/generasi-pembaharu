---
id: flashcards-template
title: "TEMPLATE — Flashcards per Bab"
chapter: flashcards
order: 99
level: lintas
personas: [pembaca-mandiri, murabbi]
reading_time_min: 1
tags: [template, flashcards]
outcomes:
  - "Menulis set flashcards yang konsisten untuk 1 bab"
prerequisites: []
related: [flashcards-readme]
last_reviewed: 2026-04-18
---

# TEMPLATE — Flashcards per Bab

Copy file ini sebagai `ch<N>.md` (N = 0-7). Isi 10-20 kartu.

Frontmatter:

```yaml
---
id: flash-ch<N>
title: "Flashcards — Bab <N>: <Judul>"
chapter: flashcards
order: <N>
level: lintas
personas: [aktivis-baru, pembaca-mandiri, murabbi]
reading_time_min: <kira-kira>
tags: [flashcards, ch<N>, <tema>]
outcomes:
  - "Memperkuat recall tentang Bab <N> dengan spaced repetition"
prerequisites: []
related: [ch<N>-readme]
last_reviewed: <YYYY-MM-DD>
---
```

---

# Flashcards — Bab <N>: <Judul>

> 10-20 kartu. Urut dari konsep fundamental ke detail spesifik.

---

## Q: <pertanyaan konsep inti>
A: <jawaban padat maks 3 kalimat>

Sumber: [`<file-id>`](../<path>.md)
Tag: ch<N>, <tema-spesifik>

---

## Q: <pertanyaan>
A: <jawaban>

Sumber: [`<file-id>`](../<path>.md)
Tag: ch<N>, <tema>

---

<!-- Ulangi untuk 10-20 kartu -->

---

## Prinsip per Kartu

- [ ] Pertanyaan spesifik (bukan "Apa itu X")
- [ ] Jawaban ≤3 kalimat
- [ ] Sumber + link file
- [ ] Tag minimal 2 (ch<N> + tema)
- [ ] Tidak ada hafalan trivia murni

## Checklist Sebelum PR

- [ ] 10-20 kartu.
- [ ] Semua kartu punya Sumber valid.
- [ ] Format konsisten (Q:/A: + Sumber + Tag).
- [ ] Tidak duplikat antar kartu.
- [ ] Uji coba dengan tool favorit Anda (Anki, Obsidian, dll).
