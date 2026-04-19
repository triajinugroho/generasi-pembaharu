---
id: indeks-readme
title: "Indeks — Temu Cepat Lintas Repo"
chapter: indeks
order: 0
level: lintas
personas: [pembaca-mandiri, peneliti, murabbi]
reading_time_min: 2
tags: [indeks, navigasi, referensi, temu-cepat]
outcomes:
  - "Menemukan ayat, hadis, tokoh, tema, atau istilah dengan cepat"
prerequisites: []
related: [root-readme, daftar-isi, ref-glosarium]
last_reviewed: 2026-04-18
---

# Indeks — Temu Cepat Lintas Repo

> *"Dan tidaklah mereka datang kepadamu dengan sesuatu yang aneh, melainkan Kami datangkan kepadamu dengan kebenaran dan penjelasan yang paling baik."*
> — QS. Al-Furqan [25]: 33

Direktori ini membantu **navigasi tematis** untuk pembaca yang tidak ingin membaca berurutan.

Bagi pembaca yang mencari **jawaban atas pertanyaan spesifik** ("Bab mana yang membahas kolaborasi lintas gerakan?", "Di mana ayat Al-Kahfi 13 dikutip?", "Siapa tokoh yang dibahas di Bab 2?"), indeks ini adalah pintu masuk tercepat.

---

## Lima Indeks

| Indeks | Isi | File |
|--------|-----|------|
| 📖 **Ayat Al-Quran** | Sura:ayah → file yang mengutip | [`ayat-quran.md`](./ayat-quran.md) |
| 📜 **Hadis** | Hadis → derajat + file yang mengutip | [`hadis.md`](./hadis.md) |
| 👥 **Tokoh** | Sahabat → tokoh kontemporer → file yang membahas | [`tokoh.md`](./tokoh.md) |
| 🎯 **Tema** | Tema kunci → file terkait | [`tema.md`](./tema.md) |
| 📚 **Istilah** | Istilah tarbiyah → glosarium + file terkait | [`istilah.md`](./istilah.md) |

---

## Catatan Metodologis

Indeks ini **dimulai sebagai scaffold** — belum lengkap untuk seluruh 82 file. Kontributor mengisi secara bertahap via PR.

**Prioritas pengisian**:

1. `tema.md` — paling berguna bagi pembaca umum.
2. `tokoh.md` — berguna untuk peneliti.
3. `istilah.md` — pintu masuk untuk pemula.
4. `ayat-quran.md` dan `hadis.md` — paling padat kerja, butuh review ulama untuk derajat hadis.

Editor akan menandai tiap file indeks dengan `last_reviewed` di frontmatter — supaya pembaca tahu sejauh mana indeks telah lengkap.

---

## Bagaimana Berkontribusi ke Indeks

1. Pilih file yang ingin Anda indeks (mis. `02-sirah-dan-sejarah/02-generasi-sahabat.md`).
2. Scan setiap kutipan ayat/hadis, tokoh yang disebut, tema yang diangkat.
3. Tambahkan entri di file indeks yang sesuai.
4. Buka PR dengan judul `indeks: <file sumber>`.
5. Reviewer memverifikasi akurasi.

**Contoh entri di `tokoh.md`**:

```markdown
### Abdurrahman bin Auf
- [`ch2-generasi-sahabat`](../02-sirah-dan-sejarah/02-generasi-sahabat.md) — profil singkat + etos wirausaha.
- [`ch3-karakter-pembaharu-sejati`](../03-pembangunan-diri/05-karakter-pembaharu-sejati.md) — contoh sifat zuhud dalam kekayaan.
```

Sederhana: nama tokoh sebagai heading `###`, lalu daftar file beserta catatan tematik.

---

## Hubungan dengan Glosarium

- Glosarium ([`referensi/glosarium.md`](../referensi/glosarium.md)) = **definisi** istilah.
- Indeks istilah ([`istilah.md`](./istilah.md)) = **kemana istilah itu muncul** di repo.

Keduanya saling melengkapi. Kalau Anda kontribusi, pastikan entri di kedua tempat konsisten.

---

## 📚 Bacaan Terkait

- [DAFTAR_ISI.md](../DAFTAR_ISI.md) — navigasi by struktur bab.
- [peta-konsep.md](../peta-konsep.md) — navigasi visual antar tema.
- [referensi/glosarium.md](../referensi/glosarium.md) — definisi istilah.
