---
id: jalur-peneliti
title: "Jalur Peneliti — Navigasi Tematik untuk Riset"
chapter: jalur
order: 5
level: muntasib
personas: [peneliti]
reading_time_min: 4
tags: [jalur, peneliti, riset, akademik, tematik]
outcomes:
  - "Memanfaatkan repo sebagai sumber primer terstruktur untuk riset gerakan dakwah"
  - "Menavigasi tematik melalui indeks, glosarium, dan frontmatter"
prerequisites: []
related:
  - indeks-tema
  - indeks-tokoh
  - ref-glosarium
  - ref-tokoh-inspirasi
  - ref-kitab-wajib
last_reviewed: 2026-04-18
---

# 🔬 Jalur Peneliti — Navigasi Tematik

> *"Katakanlah: 'Adakah sama orang-orang yang mengetahui dengan orang-orang yang tidak mengetahui?'"*
> — QS. Az-Zumar [39]: 9

Anda sedang menulis skripsi, tesis, disertasi, atau artikel akademik tentang gerakan dakwah Indonesia kontemporer, pedagogi tarbiyah, epistemologi aqidah, atau respons Islam terhadap tantangan modern. Jalur ini memberi Anda **peta navigasi tematik** — bukan peta baca naratif.

Repo ini bukan jurnal peer-reviewed. Ia adalah **kumpulan materi kurikulum kurasi komunitas** yang bisa jadi: (a) objek studi tentang bentuk kurikulum dakwah kampus generasi 2026+, (b) sumber sekunder tentang sintesis lintas-manhaj, (c) contoh lapangan tentang tarbiyah digital.

---

## Fitur yang Berguna untuk Peneliti

### 1. Frontmatter Terstruktur

Setiap file `.md` punya YAML frontmatter dengan: `id`, `tags`, `personas`, `outcomes`, `related`, `last_reviewed`. Lihat [`META-SKEMA.md`](../META-SKEMA.md).

**Untuk peneliti**: Anda bisa memakai pipeline RAG sederhana (mis. Obsidian + plugin Dataview, Logseq, atau skrip Python dengan `python-frontmatter`) untuk:

- Memfilter semua file dengan `tags: [tauhid]`.
- Memetakan graf `related:` antar file.
- Mengumpulkan seluruh `outcomes:` untuk analisis kurikulum.

Repo tidak menyediakan tooling ini — Anda bangun sendiri atau pakai Obsidian. Ini konsekuensi dari disiplin pure-markdown.

### 2. Indeks Tematis

- [ ] [`indeks/ayat-quran.md`](../indeks/ayat-quran.md) — 370+ ayat → file pengutip. Berguna untuk analisis hermeneutik kurikulum.
- [ ] [`indeks/hadis.md`](../indeks/hadis.md) — 470+ hadis dengan derajat.
- [ ] [`indeks/tokoh.md`](../indeks/tokoh.md) — sahabat → tokoh kontemporer.
- [ ] [`indeks/tema.md`](../indeks/tema.md) — tema → file terkait.
- [ ] [`indeks/istilah.md`](../indeks/istilah.md) — istilah → glosarium.

### 3. Glosarium & Tokoh

- [ ] [`referensi/glosarium.md`](../referensi/glosarium.md) — 100+ istilah dengan definisi terstruktur.
- [ ] [`referensi/tokoh-inspirasi.md`](../referensi/tokoh-inspirasi.md) — Setelah split menjadi klasik/pertengahan/modern/Nusantara.
- [ ] [`referensi/kitab-wajib.md`](../referensi/kitab-wajib.md) — bibliografi kanonik lintas manhaj.

---

## Peta Navigasi per Topik Riset

### Riset: Epistemologi Dakwah Kampus Kontemporer

- [ ] [Bab 4: Strategi Dakwah](../04-strategi-dakwah/) — keseluruhan sebagai korpus.
- [ ] [Prinsip Dakwah Qurani](../04-strategi-dakwah/01-prinsip-dakwah-qurani.md) — metodologi hermeneutik.
- [ ] [Fiqh Dakwah Kontemporer](../04-strategi-dakwah/02-fiqh-dakwah-kontemporer.md) — ijtihad operasional.
- [ ] Esai [Dakwah Bukan Partisan](../esai/dakwah-bukan-partisan.md) — debat intra-gerakan.

### Riset: Sejarah & Tipologi Gerakan Islam Indonesia

- [ ] [Sejarah Pergerakan Islam Indonesia](../02-sirah-dan-sejarah/05-sejarah-pergerakan-islam-indonesia.md) — narasi historis.
- [ ] [Peta Gerakan Dakwah Indonesia](../05-titik-temu-gerakan/01-peta-gerakan-dakwah-indonesia.md) — tipologi kontemporer.
- [ ] [Titik Temu Lintas Manhaj](../05-titik-temu-gerakan/02-titik-temu-lintas-manhaj.md) — sintesis yang diajukan.
- [ ] Esai [Kritik Diri Gerakan Dakwah](../esai/kritik-diri-gerakan-dakwah.md) — kritik internal.

### Riset: Pedagogi Tarbiyah Kontemporer

- [ ] [kurikulum/](../kurikulum/) — seluruh 18 sesi sebagai korpus kurikulum.
- [ ] [GAYA-PENULISAN.md §3](../GAYA-PENULISAN.md) — komponen pedagogis (Mental Model, Rantai Logika, Titik Refleksi).
- [ ] [Panduan Fasilitator](../lampiran/panduan-fasilitator.md) — metodologi fasilitasi.
- [ ] [kartu-halaqah/](../kartu-halaqah/) — bentuk padat pedagogi.
- [ ] Esai [Dari Halaqah ke Peradaban](../esai/dari-halaqah-ke-peradaban.md).

### Riset: Gender & Perempuan dalam Dakwah

- [ ] Esai [Perempuan Pembaharu](../esai/perempuan-pembaharu.md) — posisi eksplisit repo.
- [ ] [referensi/tokoh-inspirasi.md](../referensi/tokoh-inspirasi.md) — representasi tokoh perempuan dalam daftar.
- [ ] Diskursus implisit: lihat file yang *tidak* menggunakan figur perempuan sebagai teladan — metodologi kritis.

### Riset: Islam, Ekonomi, Kemandirian

- [ ] Esai [Ekonomi Umat dan Kemandirian](../esai/ekonomi-umat-dan-kemandirian.md).
- [ ] [Dakwah Struktural dan Kultural](../04-strategi-dakwah/04-dakwah-struktural-dan-kultural.md).
- [ ] [Membangun Ekosistem Dakwah](../04-strategi-dakwah/05-membangun-ekosistem-dakwah.md).

### Riset: Respons Islam atas Modernitas (Post-truth, AI, Liberalisme)

- [ ] [Bab 6: Tantangan Kontemporer](../06-tantangan-kontemporer/) — seluruh bab.
- [ ] Esai [Spiritualitas di Era Digital](../esai/spiritualitas-di-era-digital.md).
- [ ] [Intelektualitas dan Wawasan](../03-pembangunan-diri/03-intelektualitas-dan-wawasan.md) — model Ibnu Rushd.

---

## Metodologi yang Disarankan

1. **Sebut repo sebagai**: "Tim Kurasi Generasi Pembaharu (2026). *Generasi Pembaharu: Fondasi, Strategi, dan Peta Jalan bagi Pemuda Muslim Indonesia yang Rindu Memperbaharui Umat*. Repositori kurikulum kurasi komunitas. Tersedia di: [URL repo]. Lisensi: CC BY-NC-SA 4.0."
2. **Kutip file spesifik** dengan `id:` frontmatter, bukan hanya path. `id` permanen; path bisa berubah.
3. **Catat `last_reviewed`** dalam kutipan — repo ini hidup, isi bisa berubah.
4. **Akses via git clone** untuk snapshot permanen — `git log --oneline` menampilkan sejarah perubahan.

---

## Data yang Bisa Ditambang

| Aset | Ukuran | Analisis yang Relevan |
|------|--------|-----------------------|
| 82 file markdown | ~18.000 baris | Corpus linguistics, content analysis |
| 370+ kutipan ayat | Indeks tersedia | Hermeneutik kurikuler, frekuensi surah |
| 470+ kutipan hadis | Indeks tersedia | Distribusi kutubussittah, derajat hadis |
| 600+ istilah tarbiyah | Pencarian mudah | Etnolinguistik kurikulum dakwah |
| Frontmatter terstruktur | 82 file | Topic modeling, graf semantik |
| Git log | 40+ commit | Evolusi kurikulum |

---

## Kontribusi Balik

- [ ] Kalau riset Anda menghasilkan insight yang berguna, pertimbangkan kontribusi ke [testimoni/](../testimoni/) atau buka PR dengan catatan kritik.
- [ ] Repo ini lintas-manhaj — kritik akademik yang tajam tapi adil adalah kontribusi paling berharga.
- [ ] Kalau Anda menerbitkan paper yang mereferensikan repo, sampaikan ke editor via issue — akan dicatat di [DAMPAK.md](../DAMPAK.md).

---

## Keterbatasan yang Perlu Dicatat

Jujurlah tentang ini di bagian metodologi paper Anda:

- Repo ini **bukan riset akademik**. Ia kurikulum kurasi komunitas.
- Frontmatter (termasuk `outcomes:`) sebagian diisi otomatis oleh editor, bukan hasil desain instruksional formal.
- `last_reviewed` adalah tanda editorial, bukan peer review.
- Kutipan dalil belum diverifikasi silang oleh ahli hadis di semua file.
- Repo condong ke sensibilitas tarbiyah-harakah meski berusaha lintas-manhaj — patut diakui.

---

## Titik Refleksi (Peneliti)

1. Repo ini adalah **subjek riset** atau **rekan pemikir** bagi saya? Bagaimana saya menempatkannya?
2. Bias metodologis apa yang saya bawa ke pembacaan repo ini?
3. Apa **gap** di repo ini yang justru jadi titik masuk paper saya?
4. Kalau saya menulis kritik publik, apakah kritik saya **adil, dibaca oleh objek kritik, dan niat ilmiah**?

---

## 📚 Bacaan Terkait

- [Daftar Isi Lengkap](../DAFTAR_ISI.md) — navigasi menyeluruh.
- [Peta Konsep](../peta-konsep.md) — graf konseptual.
- [Indeks](../indeks/) — lima pintu indeksasi.
- [CONTRIBUTING.md](../CONTRIBUTING.md) — alur kontribusi & kode etik.
