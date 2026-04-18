---
id: indeks-ayat-quran
title: "Indeks Ayat Al-Quran"
chapter: indeks
order: 2
level: lintas
personas: [peneliti, pembaca-mandiri, murabbi]
reading_time_min: 3
tags: [indeks, ayat, quran, hermeneutik]
outcomes:
  - "Menemukan file yang mengutip ayat tertentu"
prerequisites: []
related: [indeks-readme, indeks-tema]
last_reviewed: 2026-04-18
---

# Indeks Ayat Al-Quran

> *"Dan sesungguhnya telah Kami jadikan Al-Quran itu mudah untuk pelajaran, maka adakah orang yang mengambil pelajaran?"*
> — QS. Al-Qamar [54]: 17

Indeks ini memetakan **ayat Al-Quran → file yang mengutipnya**. Repo mengutip 370+ ayat; indeks ini dibangun bertahap oleh komunitas.

**Format entri**:

```markdown
### QS. <Nama Surah> [nomor]: <ayat>
- [`<file-id>`](../<path>.md) — <konteks kutipan 1 kalimat>
```

---

## Al-Fatihah [1]

### QS. Al-Fatihah [1]: 1-7
- _Menunggu entri._ Kontributor: tambahkan file yang mengutip ayat ini.

## Al-Baqarah [2]

### QS. Al-Baqarah [2]: 30 — Penciptaan Khalifah
- [`kur-l1-s1-mengenal-jati-diri`](../kurikulum/level-1-tamhidi/sesi-01-mengenal-jati-diri.md) — konteks identitas manusia sebagai khalifah.
- [`ch0-visi-kebangkitan`](../00-mukadimah/03-visi-kebangkitan.md) — dasar visi kebangkitan.

### QS. Al-Baqarah [2]: 83 — Berkata yang Baik
- [`indeks-tema`](./tema.md) — epigraf.

### QS. Al-Baqarah [2]: 255 — Ayat Kursi
- _Menunggu entri._

## An-Nahl [16]

### QS. An-Nahl [16]: 36 — Perintah Menjauhi Thaghut
- [`ch1-tauhid-sebagai-pembebasan`](../01-fondasi-aqidah/01-tauhid-sebagai-pembebasan.md) — epigraf pembuka.

### QS. An-Nahl [16]: 120 — Ibrahim sebagai Imam
- [`ch1-readme`](../01-fondasi-aqidah/README.md) — epigraf pembuka bab.

### QS. An-Nahl [16]: 125 — Metode Dakwah (Hikmah, Mauizhah, Mujadalah)
- [`ch4-readme`](../04-strategi-dakwah/README.md) — epigraf pembuka bab.
- [`ch4-prinsip-dakwah-qurani`](../04-strategi-dakwah/01-prinsip-dakwah-qurani.md) — pembahasan utama prinsip dakwah.
- [`esai-dakwah-bukan-partisan`](../esai/dakwah-bukan-partisan.md) — penerapan lintas manhaj.

## Al-Isra' [17]

### QS. Al-Isra' [17]: 70 — Pemuliaan Manusia
- [`testimoni-readme`](../testimoni/README.md) — epigraf.

## Maryam [19]

### QS. Maryam [19]: 64 — Tuhanmu Tidak Melupakan
- [`meta-peta-konsep`](../peta-konsep.md) — penutup.

## Thaha [20]

### QS. Thaha [20]: 25-28 — Doa Kelapangan Dada
- [`meta-skema`](../META-SKEMA.md) — epigraf.

## Al-Anbiya [21]

### QS. Al-Anbiya [21]: 105 — Bumi Diwariskan Hamba Saleh
- [`meta-skema`](../META-SKEMA.md) — penutup.

## Al-Furqan [25]

### QS. Al-Furqan [25]: 33 — Datang dengan Kebenaran
- [`indeks-readme`](./README.md) — epigraf.

## As-Sajdah [32]

### QS. As-Sajdah [32]: 24 — Pemimpin yang Sabar & Yakin
- [`meta-peta-konsep`](../peta-konsep.md) — epigraf.

## Fussilat [41]

### QS. Fussilat [41]: 33 — Siapa Lebih Baik Perkataannya
- [`meta-dampak`](../DAMPAK.md) — epigraf.

## As-Saff [61]

### QS. As-Saff [61]: 4 — Barisan yang Kokoh
- [`jalur-ketua-ldk`](../jalur/ketua-ldk.md) — epigraf.

## Az-Zumar [39]

### QS. Az-Zumar [39]: 9 — Orang yang Tahu vs Tidak Tahu
- [`jalur-peneliti`](../jalur/peneliti.md) — epigraf.

## Al-'Alaq [96]

### QS. Al-'Alaq [96]: 1 — Perintah Membaca
- [`jalur-pembaca-mandiri`](../jalur/pembaca-mandiri.md) — epigraf.

## Ibrahim [14]

### QS. Ibrahim [14]: 4 — Bahasa Kaumnya
- [`meta-gaya-penulisan`](../GAYA-PENULISAN.md) — epigraf.
- [`jalur-readme`](../jalur/README.md) — epigraf.

## Adz-Dzariyat [51]

### QS. Adz-Dzariyat [51]: 56 — Tujuan Penciptaan
- [`kur-l1-s1-mengenal-jati-diri`](../kurikulum/level-1-tamhidi/sesi-01-mengenal-jati-diri.md) — rantai logika tauhid.

---

## Cara Melengkapi Indeks Ini

Indeks ini **sebagian besar kosong** — tugas komunitas mengisinya secara bertahap.

**Prioritas pengisian**:

1. Ayat yang dikutip di lebih dari 1 file (menunjukkan tema lintas bab).
2. Ayat kunci dalam Mental Model, Rantai Logika, atau Titik Refleksi.
3. Epigraf pembuka file dan bab.
4. Ayat yang dikutip dalam kurikulum halaqah.

**Cara berkontribusi**:

1. Pilih satu file. Scan semua kutipan `QS. <Surah> [nomor]: <ayat>`.
2. Untuk tiap ayat, cari heading `## <Nama Surah> [<nomor>]` di file ini. Tambah jika belum ada.
3. Di bawahnya, tambah `### QS. ... <deskripsi singkat>` dan daftar file.
4. Buka PR.

**Format deskripsi ayat**: singkat, deskriptif, bukan terjemahan penuh. Contoh: "Perintah Menjauhi Thaghut", bukan "Ayat tentang rasul disuruh menyeru sembah Allah".

**Verifikasi**: reviewer memastikan nomor ayat akurat dengan merujuk mushaf Kemenag.

---

## 📚 Bacaan Terkait

- [`indeks/hadis.md`](./hadis.md) — analog untuk hadis.
- [`indeks/tema.md`](./tema.md) — navigasi tematis.
- [`referensi/glosarium.md`](../referensi/glosarium.md) — istilah terkait.
