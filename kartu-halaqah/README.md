---
id: kartu-halaqah-readme
title: "Kartu Halaqah — One-Pager Fasilitator"
chapter: kartu-halaqah
order: 0
level: muayyid
personas: [murabbi, ketua-ldk]
reading_time_min: 2
tags: [kartu, halaqah, fasilitator, one-pager, ringkas]
outcomes:
  - "Menjalankan sesi halaqah dengan kartu satu-halaman, bukan dokumen panjang"
prerequisites: [jalur-murabbi, kurikulum-readme]
related: [kurikulum-readme, lamp-panduan-fasilitator]
last_reviewed: 2026-04-18
---

# Kartu Halaqah — One-Pager untuk Fasilitator

> *"Sebaik-baik petunjuk adalah petunjuk Muhammad ﷺ, dan sebaik-baik urusan adalah pertengahannya."*

Kartu halaqah adalah **versi padat** file kurikulum penuh. Satu kartu = satu halaman = satu sesi.

## Mengapa Ada?

File kurikulum di [`kurikulum/level-N-xxx/sesi-N-xxx.md`](../kurikulum/) kaya konten — antara 150-350 baris per sesi. Itu **referensi lengkap**.

Tapi saat Anda memfasilitasi di ruangan, Anda butuh:
- **Satu lembar** yang bisa di-print.
- **Ringkasan waktu** per segmen.
- **Prompt pertanyaan** yang siap diucap.
- **Tidak perlu scroll** sambil bicara.

Itu fungsi kartu halaqah.

## Struktur Standar Kartu

```
Header: Level, Sesi, Durasi, Tujuan 1 kalimat
----
Menit 0-10  : Pembukaan — 1 cerita/pertanyaan pemicu
Menit 10-70 : 3 pokok bahasan, masing-masing dengan:
              - inti 2 kalimat
              - 1 dalil kunci
              - 1 pertanyaan pemancing diskusi
Menit 70-90 : Diskusi kelompok — 3 pertanyaan
Menit 90-105: Refleksi — 3 prompt jurnal
Menit 105-120: Penutup — doa + tugas pekan depan
----
Catatan Adab: 3 poin pengingat murabbi
```

## Daftar Kartu (18 Sesi)

### Level 1 — Tamhidi

- [Sesi 1: Mengenal Jati Diri](./l1-s1-jati-diri.md) · _contoh siap_
- Sesi 2: Dasar Aqidah Gerakan · _menunggu kontributor_
- Sesi 3: Teladan Rasulullah · _menunggu kontributor_
- Sesi 4: Adab dan Akhlak Da'i · _menunggu kontributor_
- Sesi 5: Dasar Dakwah Fardiyah · _menunggu kontributor_
- Sesi 6: Evaluasi dan Komitmen · _menunggu kontributor_

### Level 2 — Muayyid
- 6 sesi · _menunggu kontributor_

### Level 3 — Muntasib
- 6 sesi · _menunggu kontributor_

## Cara Bikin Kartu Baru

1. Baca file kurikulum asli secara utuh.
2. Salin [`TEMPLATE.md`](./TEMPLATE.md) menjadi `l<level>-s<sesi>-<slug>.md`.
3. Isi dari file asli — hanya inti, tidak semua.
4. Test dengan diri sendiri: **bisakah saya memfasilitasi sesi hanya dengan kartu ini di tangan?** Kalau tidak, revisi.
5. Buka PR.

## Prinsip Kartu Halaqah

- **Satu halaman cetak** (A4 landscape / portrait). Kalau lebih panjang, berarti terlalu banyak.
- **Bukan pengganti** file kurikulum utuh — hanya panduan ringkas di ruangan.
- **Bahasa operasional** — apa yang murabbi katakan dan lakukan, bukan teori.
- **Ukuran font nyaman cetak** — jangan terlalu kecil.

## 📚 Bacaan Terkait

- [`kurikulum/`](../kurikulum/) — materi utuh.
- [`lamp-panduan-fasilitator`](../lampiran/panduan-fasilitator.md) — panduan fasilitasi umum.
- [`jalur-murabbi`](../jalur/murabbi.md) — onboarding untuk murabbi baru.
- [`lamp-template-evaluasi`](../lampiran/template-evaluasi.md) — evaluasi pasca-sesi.
