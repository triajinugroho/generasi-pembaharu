---
id: indeks-hadis
title: "Indeks Hadis"
chapter: indeks
order: 3
level: lintas
personas: [peneliti, pembaca-mandiri, murabbi]
reading_time_min: 3
tags: [indeks, hadis, sunnah]
outcomes:
  - "Menemukan file yang mengutip hadis tertentu"
prerequisites: []
related: [indeks-readme, indeks-ayat-quran]
last_reviewed: 2026-04-18
---

# Indeks Hadis

> *"Barangsiapa menyampaikan satu hadis yang dipakai orang, maka ia mendapatkan pahalanya dan pahala orang yang mengamalkannya."*
> — makna dari HR. Muslim no. 1893

Indeks **hadis → file yang mengutipnya**. Repo mengutip 470+ hadis; indeks dibangun bertahap.

**Format entri**:

```markdown
### HR. <Periwayat> no. <nomor> — <tema singkat>
Derajat: <shahih/hasan/dha'if/etc>
- [`<file-id>`](../<path>.md) — <konteks kutipan>
```

---

## Catatan Metodologi

- **Derajat hadis** harus mengacu pada pendapat ulama yang dikenal. Kalau tidak yakin, tandai `_perlu verifikasi_`.
- Hadis dalam **Kutub as-Sittah** (Bukhari, Muslim, Abu Dawud, Tirmidzi, Nasa'i, Ibn Majah) adalah prioritas entri awal.
- Kalau satu hadis ada di beberapa periwayat, daftar semuanya — pembaca mencari dari periwayat mana pun.

---

## Bukhari

### HR. Bukhari no. 1 — Niat
Derajat: shahih (muttafaq 'alaih dengan Muslim no. 1907).
- [`meta-gaya-penulisan`](../GAYA-PENULISAN.md) — contoh format kutipan.

### HR. Bukhari no. 3461 — Sampaikan Walaupun Satu Ayat
Derajat: shahih.
- [`meta-delivery`](../DELIVERY.md) — epigraf.

## Muslim

### HR. Muslim no. 1893 — Penunjuk pada Kebaikan
Derajat: shahih.
- [`meta-gaya-penulisan`](../GAYA-PENULISAN.md) — penutup.
- [`testimoni-template`](../testimoni/TEMPLATE.md) — penutup.

### HR. Muslim no. 1907 — Niat (lihat juga HR. Bukhari no. 1)
Derajat: shahih.
- _Cross-reference._

## Abu Dawud

### HR. Abu Dawud no. 4291 — Mujaddid Setiap 100 Tahun
Derajat: shahih (dishahihkan al-Albani).
- [`root-readme`](../README.md) — epigraf landing page.
- [`ch0-manifesto-generasi-pembaharu`](../00-mukadimah/01-manifesto-generasi-pembaharu.md) — dasar manifesto.
- [`ref-tokoh-inspirasi`](../referensi/tokoh-inspirasi.md) — pengantar bab tokoh.

## Tirmidzi

### HR. Tirmidzi no. 2516 — Jagalah Allah
Derajat: hasan shahih.
- [`jalur-aktivis-baru`](../jalur/aktivis-baru.md) — epigraf.

## Ahmad

### HR. Ahmad — Sebaik-baik Manusia
Derajat: hasan (lihat pendapat ulama hadis kontemporer).
- [`jalur-readme`](../jalur/README.md) — penutup.

---

## Cara Melengkapi Indeks Ini

Indeks ini **sebagian besar kosong**. Prioritas pengisian:

1. Hadis yang dikutip di lebih dari 1 file.
2. Hadis dalam Mental Model, Rantai Logika, atau Titik Refleksi.
3. Hadis dalam kurikulum halaqah (prioritas ulama untuk verifikasi derajat).

**Langkah**:

1. Pilih file.
2. Scan kutipan `HR. <periwayat> no. <n>`.
3. Tambahkan entri di section periwayat yang sesuai.
4. Periksa derajat dari sumber tepercaya (mis. *Jami' al-Uhul* Ibn al-Atsir, kitab syarh, atau database Dorar.net).
5. Buka PR.

**Kalau derajat meragukan**: tandai `_perlu verifikasi ulama_` dan sebutkan kemungkinan status. Editor akan meneruskan ke reviewer bersertifikasi.

---

## 📚 Bacaan Terkait

- [`indeks/ayat-quran.md`](./ayat-quran.md)
- [`indeks/tema.md`](./tema.md)
- [`referensi/kitab-wajib.md`](../referensi/kitab-wajib.md) — bibliografi kitab hadis.
