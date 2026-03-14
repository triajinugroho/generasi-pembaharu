# STRATEGIC PLAN: Penuntasan Buku Generasi Pembaharu

*Dokumen perencanaan komprehensif — berisi analisis, target, dan paket prompt eksekusi*

---

## STATUS SAAT INI

### Inventaris Konten

| Komponen | File | Lines | Avg/File | Kondisi |
|----------|------|-------|----------|---------|
| Mukadimah (Bab 0) | 3 + README | 342 | ~100 | Cukup solid |
| Fondasi Aqidah (Bab 1) | 4 + README | 361 | ~80 | Sedang, perlu pengayaan |
| Sirah & Sejarah (Bab 2) | 5 + README | 305 | ~56 | **Tipis — outline** |
| Pembangunan Diri (Bab 3) | 5 + README | 469 | ~84 | Sedang, 1 file sudah kuat |
| Strategi Dakwah (Bab 4) | 5 + README | 316 | ~60 | **Tipis — outline** |
| Titik Temu (Bab 5) | 4 + README | 250 | ~58 | **Tipis — outline** |
| Tantangan Kontemporer (Bab 6) | 4 + README | 243 | ~57 | **Tipis — outline** |
| Kurikulum L1 | 6 | 830 | ~138 | Kuat (sudah enriched) |
| Kurikulum L2 | 6 | 856 | ~143 | Kuat (sudah enriched) |
| Kurikulum L3 | 6 | 1,053 | ~176 | Kuat (sudah enriched) |
| Esai | 4 | 406 | ~101 | Baik |
| Referensi | 3 | 538 | ~179 | Baik |
| **TOTAL** | **67 file** | **~5,562** | | |

### Diagnosis Utama

1. **Ketimpangan kritis**: Bab buku utama (Bab 2-6) rata-rata hanya 55-60 baris — masih berupa **kerangka/outline dengan bullet points**, bukan narasi bab buku yang utuh
2. **Kurikulum sudah kuat**: 18 file kurikulum sudah diperkaya dengan Mental Model Box dan Rantai Logika Tauhid
3. **Bab buku utama belum punya elemen pedagogis**: Tidak ada Mental Model Box, Rantai Logika Tauhid, atau kotak refleksi terstruktur
4. **Belum ada penutup/epilog** buku
5. **Esai bisa ditambah** untuk memperkaya perspektif
6. **Referensi silang** antar-bab belum ada

---

## TARGET AKHIR

| Metrik | Sekarang | Target | Kenaikan |
|--------|----------|--------|----------|
| Total lines | ~5,562 | ~14,000-16,000 | ~3x |
| Avg lines/bab buku | ~65 | ~250-350 | ~4-5x |
| File buku utama | 25 | 25 (sama) | — |
| File kurikulum | 18 | 18 (sama) | — |
| Esai | 4 | 8-10 | +4-6 |
| File baru (epilog, lampiran) | 0 | 5-7 | +5-7 |
| Mental Model Box di buku | 0 | ~50+ | +50 |
| Rantai Logika Tauhid di buku | 0 | ~25+ | +25 |

---

## ARSITEKTUR PHASE

```
Phase 1: DEEPENING (Prioritas Tertinggi)
  └── Expand 22 file bab buku utama dari ~60 → ~250-350 baris
  └── 5 batch prompt (per bab)

Phase 2: ENRICHMENT
  └── Tambah Mental Model Box + Rantai Logika Tauhid ke semua bab buku
  └── 5 batch prompt (per bab)

Phase 3: EXPANSION
  └── Esai baru + Lampiran praktis + Epilog
  └── 3 batch prompt

Phase 4: COHERENCE
  └── Cross-referencing + konsistensi format + update navigasi
  └── 2 batch prompt

Phase 5: POLISH
  └── Final review + bibliografi + glosarium update
  └── 1 batch prompt
```

**Total: ~16 batch prompt**

---

## PHASE 1: DEEPENING — Pendalaman Bab Buku Utama

### Prinsip Pendalaman

Setiap file bab buku harus ditransformasi dari **outline bullet-point** menjadi **narasi bab buku** dengan struktur:

1. **Pembukaan naratif** — paragraf pembuka yang menarik, kontekstual, membawa pembaca masuk
2. **Isi substantif** — setiap sub-bab dikembangkan menjadi narasi lengkap dengan:
   - Argumen yang dibangun secara logis
   - Dalil Al-Quran dan Hadits yang relevan (dengan konteks, bukan sekadar kutipan)
   - Contoh historis dan kontemporer
   - Analisis kritis, bukan sekadar deskripsi
3. **Refleksi & Aksi** — dipertahankan dan diperkuat

**Target per file: 250-350 baris (naik dari ~55-65)**

---

### Prompt 1A: Deepening Bab 2 — Sirah & Sejarah (5 file)

```
KONTEKS:
Kamu sedang mengerjakan buku "Generasi Pembaharu" — buku referensi untuk aktivis dakwah kampus
Islam Indonesia. File-file di bab 02-sirah-dan-sejarah/ saat ini masih berupa OUTLINE (55-60
baris). Tugasmu: expand setiap file menjadi BAB BUKU NARATIF yang utuh (250-350 baris).

INSTRUKSI:
Baca kelima file berikut, lalu EDIT masing-masing (jangan write ulang, gunakan Edit tool):
1. 02-sirah-dan-sejarah/01-blueprint-nabawi.md
2. 02-sirah-dan-sejarah/02-generasi-sahabat.md
3. 02-sirah-dan-sejarah/03-para-pembaharu-klasik.md
4. 02-sirah-dan-sejarah/04-pembaharu-modern.md
5. 02-sirah-dan-sejarah/05-sejarah-pergerakan-islam-indonesia.md

PANDUAN PENGEMBANGAN:
- Pertahankan struktur heading yang sudah ada
- Kembangkan setiap bullet point menjadi 2-4 paragraf naratif
- Tambahkan dalil Al-Quran/Hadits yang relevan dengan konteks penjelasan
- Tambahkan contoh historis konkret (nama, tahun, peristiwa spesifik)
- Tambahkan analisis — "mengapa ini penting bagi aktivis dakwah kampus hari ini?"
- Pertahankan tone: serius tapi accessible, ilmiah tapi menggerakkan
- Jangan ubah judul atau struktur heading level 1 dan 2
- Kembangkan bagian "Refleksi & Aksi" menjadi lebih substansial

CONTOH TRANSFORMASI (dari outline ke narasi):
SEBELUM:
"- Dar al-Arqam sebagai model halaqah pertama"

SESUDAH:
"Rumah Al-Arqam bin Abi Al-Arqam di kaki bukit Shafa menjadi markas rahasia pertama.
Di sinilah Rasulullah ﷺ membina generasi pertama — tidak lebih dari 40 orang selama
tiga tahun. Bayangkan: gerakan yang akan mengubah wajah dunia dimulai di sebuah rumah
kecil dengan segelintir orang yang beriman. Dar Al-Arqam adalah prototipe halaqah:
ruang kecil, jamaah terpilih, materi langsung dari sumber, ikatan personal yang kuat.
Setiap LDK yang memulai halaqah kecil di pojok masjid kampus sedang mengulangi
sunnatullah yang sama."

TARGET: Masing-masing file menjadi 250-350 baris. Total ~1,500 baris baru.
Setelah selesai, commit dengan pesan yang jelas dan push.
```

---

### Prompt 1B: Deepening Bab 4 — Strategi Dakwah (5 file)

```
KONTEKS:
Buku "Generasi Pembaharu" — buku referensi aktivis dakwah kampus Islam Indonesia.
File-file di bab 04-strategi-dakwah/ masih OUTLINE (55-65 baris).
Expand menjadi BAB BUKU NARATIF (250-350 baris per file).

INSTRUKSI:
Baca dan EDIT (bukan write ulang) kelima file:
1. 04-strategi-dakwah/01-prinsip-dakwah-qurani.md
2. 04-strategi-dakwah/02-fiqh-dakwah-kontemporer.md
3. 04-strategi-dakwah/03-dakwah-digital-dan-media.md
4. 04-strategi-dakwah/04-dakwah-struktural-dan-kultural.md
5. 04-strategi-dakwah/05-membangun-ekosistem-dakwah.md

PANDUAN:
- Pertahankan heading yang ada, kembangkan bullet → narasi (2-4 paragraf per sub-bab)
- Untuk 01 (Prinsip Qurani): analisis mendalam metode dakwah para nabi dalam Al-Quran
  (Nuh, Ibrahim, Musa, Yusuf, Muhammad ﷺ) — pola, konteks, pelajaran
- Untuk 02 (Fiqh Kontemporer): masukkan pembahasan tentang fiqh prioritas (Al-Qaradhawi),
  fiqh muwazanat, dan bagaimana menerapkannya di konteks kampus Indonesia
- Untuk 03 (Digital): data dan tren terkini, studi kasus akun dakwah yang berhasil,
  strategi konten, etika digital dari perspektif Islam
- Untuk 04 (Struktural-Kultural): analisis mendalam model dakwah Muhammadiyah (struktural)
  vs NU (kultural) vs Tarbiyah (sel/halaqah) — kelebihan dan kekurangan masing-masing
- Untuk 05 (Ekosistem): framework konkret bagaimana membangun ekosistem dakwah kampus
  yang sustainable — dari halaqah sampai lembaga, dari individual sampai institutional

TONE: Praktis, aplikatif, berbasis pengalaman nyata gerakan dakwah Indonesia.
TARGET: 250-350 baris per file. Total ~1,500 baris baru.
Commit dan push setelah selesai.
```

---

### Prompt 1C: Deepening Bab 5 — Titik Temu Gerakan (4 file)

```
KONTEKS:
Buku "Generasi Pembaharu". Bab 05-titik-temu-gerakan/ adalah bab paling UNIK dan
SENSITIF — membahas upaya menyatukan gerakan dakwah yang terpecah.
File masih OUTLINE (53-62 baris). Expand ke 250-350 baris per file.

INSTRUKSI:
Baca dan EDIT keempat file:
1. 05-titik-temu-gerakan/01-peta-gerakan-dakwah-indonesia.md
2. 05-titik-temu-gerakan/02-titik-temu-lintas-manhaj.md
3. 05-titik-temu-gerakan/03-kolaborasi-strategis.md
4. 05-titik-temu-gerakan/04-blueprint-persatuan-umat.md

PANDUAN:
- KRITIS: Jaga keseimbangan dan keadilan. Jangan memihak satu gerakan.
  Buku ini lintas manhaj — semua gerakan diapresiasi.
- Untuk 01 (Peta Gerakan): profil mendalam setiap gerakan besar:
  Muhammadiyah, NU, Tarbiyah/PKS, Salafi, PERSIS, Al-Irsyad, HTI (historis),
  KAMMI, LDK — sejarah, manhaj, kontribusi, karakteristik. Fair & balanced.
- Untuk 02 (Titik Temu): elaborasi mendalam setiap titik temu — ushul aqidah,
  maqashid syariah, musuh bersama, teladan ikhtilaf sahabat & ulama klasik
- Untuk 03 (Kolaborasi): studi kasus kolaborasi yang BERHASIL antar gerakan,
  framework kolaborasi praktis, mengatasi hambatan psikologis & organisasional
- Untuk 04 (Blueprint): visi konkret persatuan umat — bukan utopis tapi
  pragmatis. Model federasi, platform bersama, mekanisme konsultasi.

PRINSIP PENULISAN:
- Deskriptif, bukan judgmental
- Mengakui perbedaan tanpa mempertajamnya
- Fokus pada "apa yang bisa kita bangun bersama"
- Dalil tentang persatuan umat yang kuat

TARGET: 250-350 baris per file. Total ~1,200 baris baru.
Commit dan push setelah selesai.
```

---

### Prompt 1D: Deepening Bab 6 — Tantangan Kontemporer (4 file)

```
KONTEKS:
Buku "Generasi Pembaharu". Bab 06-tantangan-kontemporer/ membahas isu-isu terkini
yang dihadapi pemuda Muslim Indonesia. Masih OUTLINE (56-58 baris).
Expand ke 250-350 baris per file.

INSTRUKSI:
Baca dan EDIT keempat file:
1. 06-tantangan-kontemporer/01-liberalisme-dan-identitas.md
2. 06-tantangan-kontemporer/02-era-post-truth-dan-media-sosial.md
3. 06-tantangan-kontemporer/03-ai-teknologi-dan-masa-depan.md
4. 06-tantangan-kontemporer/04-islam-dan-kebangsaan-indonesia.md

PANDUAN:
- Untuk 01 (Liberalisme): analisis kritis tapi fair tentang liberalisme —
  apa yang benar, apa yang bertentangan dengan Islam, bagaimana merespons
  secara cerdas (bukan reaktif). Bedakan liberalisme politik vs liberalisme
  moral vs liberalisme keagamaan. Perspektif Syed Muhammad Naquib Al-Attas.
- Untuk 02 (Post-Truth): fenomena hoax, echo chamber, polarisasi digital,
  cancel culture. Bagaimana Islam menjawab: etika tabayyun (QS. Al-Hujurat:6),
  larangan ghibah, kritik membangun. Literasi media dari perspektif Islam.
- Untuk 03 (AI & Teknologi): update terkini tentang AI generatif, implikasi
  etis, peluang dakwah, Muslim di industri tech. Perspektif maqashid syariah
  terhadap teknologi. Studi kasus konkret.
- Untuk 04 (Kebangsaan): relasi Islam dan NKRI — dari perspektif historis
  (peran ulama dalam kemerdekaan), teologis (konsep ummah dan wathan),
  dan pragmatis (dakwah dalam kerangka negara bangsa). Posisi moderat yang
  tidak sekuler tapi juga tidak anti-negara.

TONE: Intelektual, kritis, kontekstual Indonesia, berbasis dalil.
TARGET: 250-350 baris per file. Total ~1,200 baris baru.
Commit dan push setelah selesai.
```

---

### Prompt 1E: Deepening Bab 1 & 3 — Fondasi Aqidah & Pembangunan Diri (7 file)

```
KONTEKS:
Buku "Generasi Pembaharu". Dua bab ini sudah lebih baik dari Bab 2/4/5/6,
tapi masih perlu pendalaman. Bab 1 rata-rata ~80 baris (kecuali 01 yang 129),
Bab 3 rata-rata ~84 baris (kecuali 01 yang 164).

INSTRUKSI:
Baca dan EDIT file-file berikut yang BELUM kuat (skip file yang sudah 120+ baris):

Bab 1 (3 file yang perlu deepening):
1. 01-fondasi-aqidah/02-aqidah-yang-menggerakkan.md (68 baris → target 200-250)
2. 01-fondasi-aqidah/03-tauhid-sosial-dan-keadilan.md (55 baris → target 200-250)
3. 01-fondasi-aqidah/04-falsafah-tauhid-pergerakan.md (68 baris → target 200-250)

Bab 3 (4 file yang perlu deepening):
4. 03-pembangunan-diri/02-manajemen-ruhani-dai.md (65 baris → target 200-250)
5. 03-pembangunan-diri/03-intelektualitas-dan-wawasan.md (58 baris → target 200-250)
6. 03-pembangunan-diri/04-kepemimpinan-profetik.md (56 baris → target 200-250)
7. 03-pembangunan-diri/05-karakter-pembaharu-sejati.md (78 baris → target 200-250)

PANDUAN BAB 1 (Aqidah):
- Kembangkan argumentasi tauhid secara filosofis dan praktis
- Hubungkan tauhid dengan gerakan sosial dan keadilan
- Referensi pemikir: Al-Attas, Sayyid Qutb (Fi Zhilal), Hasan Al-Banna, Ibnu Taimiyah
- Tunjukkan bahwa tauhid bukan sekadar teologi — ia worldview yang menggerakkan

PANDUAN BAB 3 (Pembangunan Diri):
- Buat panduan tarbiyah dzatiyah yang praktis dan mendalam
- Gabungkan wisdom klasik (Imam Ghazali, Ibnu Qayyim) dengan aplikasi modern
- Untuk kepemimpinan: model servant leadership Nabawi dengan contoh konkret
- Untuk intelektualitas: tradisi ilmu dalam Islam, adab menuntut ilmu,
  reading list terstruktur

TARGET: 200-250 baris per file. Total ~1,200 baris baru.
Commit dan push setelah selesai.
```

---

## PHASE 2: ENRICHMENT — Elemen Pedagogis di Buku Utama

### Prinsip Enrichment

Setelah bab-bab buku diperdalam (Phase 1), tambahkan elemen pedagogis yang sudah
terbukti efektif di kurikulum:
- **Mental Model Box**: framework berpikir dari tokoh Islam
- **Rantai Logika Tauhid**: argumentasi berantai dari prinsip tauhid
- **Kotak Refleksi Terstruktur**: pertanyaan mendalam untuk internalisasi

---

### Prompt 2A: Enrichment Bab 1 — Fondasi Aqidah (4 file)

```
KONTEKS:
File-file bab 01-fondasi-aqidah/ sudah diperdalam (Phase 1). Sekarang tambahkan
elemen pedagogis. Baca dulu file kurikulum level-1-mubtadi/sesi-02-dasar-aqidah-gerakan.md
sebagai CONTOH format Mental Model Box dan Rantai Logika Tauhid.

INSTRUKSI:
Untuk setiap file di 01-fondasi-aqidah/ (4 file, skip README):
1. Tambahkan 2-3 Mental Model Box yang relevan dengan topik
2. Tambahkan 1 Rantai Logika Tauhid per file
3. Tambahkan 1 kotak "Titik Refleksi" (pertanyaan mendalam, 3-5 pertanyaan)
4. Sisipkan di lokasi yang tepat secara natural (jangan clump di akhir)

TOKOH UNTUK MENTAL MODEL:
- 01 (Tauhid Pembebasan): Ibrahim AS, Ali Syariati, Frantz Fanon (perspektif Islam)
- 02 (Aqidah Menggerakkan): Hasan Al-Banna, Sayyid Qutb, Imam Ghazali
- 03 (Tauhid Sosial): Umar bin Khattab, Abu Dzar Al-Ghifari, Ibnu Khaldun
- 04 (Falsafah Tauhid): Al-Attas, Muhammad Iqbal, Ismail Raji Al-Faruqi

FORMAT Mental Model Box:
> **Mental Model: [Nama Tokoh] — [Judul Konsep]**
> 1. [Langkah/prinsip 1]
> 2. [Langkah/prinsip 2]
> 3. [Langkah/prinsip 3]
> 4. [Langkah/prinsip 4]
> *Aplikasi: [bagaimana menerapkan di konteks aktivis dakwah kampus]*

FORMAT Rantai Logika Tauhid:
**Rantai Logika Tauhid: [Judul]**
- [Premis 1 + dalil] →
- [Premis 2] →
- [Premis 3] →
- [Kesimpulan praktis]

Commit dan push setelah selesai.
```

---

### Prompt 2B: Enrichment Bab 2 — Sirah & Sejarah (5 file)

```
KONTEKS:
Sama seperti Prompt 2A, tapi untuk bab 02-sirah-dan-sejarah/ (5 file).

TOKOH UNTUK MENTAL MODEL:
- 01 (Blueprint Nabawi): Rasulullah ﷺ (Tadarruj), Khadijah (Support System)
- 02 (Generasi Sahabat): Abu Bakar (Keberanian Iman), Umar (Ketegasan Adil),
  Salman Al-Farisi (Pencari Kebenaran Lintas Budaya)
- 03 (Pembaharu Klasik): Umar bin Abdul Aziz, Al-Ghazali, Ibnu Taimiyah,
  Shalahuddin Al-Ayyubi
- 04 (Pembaharu Modern): Jamaluddin Al-Afghani, Muhammad Abduh,
  Hasan Al-Banna, Badiuzzaman Said Nursi
- 05 (Indonesia): KH Ahmad Dahlan, KH Hasyim Asy'ari, HOS Tjokroaminoto,
  Mohammad Natsir, Buya Hamka

2-3 Mental Model Box + 1 Rantai Logika Tauhid + 1 Titik Refleksi per file.
Commit dan push setelah selesai.
```

---

### Prompt 2C: Enrichment Bab 3 — Pembangunan Diri (5 file)

```
KONTEKS:
Sama seperti 2A, untuk bab 03-pembangunan-diri/ (5 file).

TOKOH UNTUK MENTAL MODEL:
- 01 (Muraqabah): Hasan Al-Bashri, Imam Ghazali (Ihya Ulumiddin)
- 02 (Manajemen Ruhani): Ibnu Qayyim (Madarij As-Salikin), Ibnu Atha'illah
- 03 (Intelektualitas): Ibnu Rushd, Al-Biruni, Ibnu Khaldun
- 04 (Kepemimpinan): Umar bin Khattab, Shalahuddin, modern: Alija Izetbegovic
- 05 (Karakter Pembaharu): Muhammad Iqbal (Khudi), Malik Bennabi (Peradaban)

2-3 Mental Model Box + 1 Rantai Logika Tauhid + 1 Titik Refleksi per file.
Commit dan push setelah selesai.
```

---

### Prompt 2D: Enrichment Bab 4 — Strategi Dakwah (5 file)

```
KONTEKS:
Sama seperti 2A, untuk bab 04-strategi-dakwah/ (5 file).

TOKOH UNTUK MENTAL MODEL:
- 01 (Prinsip Qurani): Nuh AS (Persistensi), Yusuf AS (Dakwah dalam Sistem)
- 02 (Fiqh Kontemporer): Al-Qaradhawi (Fiqh Prioritas), Wahbah Az-Zuhaili
- 03 (Digital): Hamza Yusuf, Omar Suleiman (model konten), Nouman Ali Khan
- 04 (Struktural-Kultural): Walisongo, KH Ahmad Dahlan, Hasan Al-Banna
- 05 (Ekosistem): Rasulullah ﷺ (Ekosistem Madinah), Said Hawwa (Jundullah)

2-3 Mental Model Box + 1 Rantai Logika Tauhid + 1 Titik Refleksi per file.
Commit dan push setelah selesai.
```

---

### Prompt 2E: Enrichment Bab 5 & 6 (8 file)

```
KONTEKS:
Sama seperti 2A, untuk bab 05-titik-temu-gerakan/ (4 file) dan
06-tantangan-kontemporer/ (4 file).

TOKOH UNTUK MENTAL MODEL BAB 5:
- 01 (Peta Gerakan): KH Wahid Hasyim, Buya Hamka (MASYUMI)
- 02 (Titik Temu): Imam Syafi'i (Adab Ikhtilaf), Ibnu Taimiyah (Ushul vs Furu')
- 03 (Kolaborasi): Rasulullah ﷺ (Piagam Madinah), Soekarno-Hatta-ulama
- 04 (Blueprint): Muhammad Iqbal (Rekonstruksi), Alija Izetbegovic

TOKOH UNTUK MENTAL MODEL BAB 6:
- 01 (Liberalisme): Al-Attas (De-Westernisasi), Taha Abdurrahman
- 02 (Post-Truth): Ibnu Khaldun (Analisis Sosial), Al-Quran (Tabayyun)
- 03 (AI & Teknologi): Al-Khawarizmi (Algoritmika), Ibnu Haitham (Metode Ilmiah)
- 04 (Kebangsaan): Mohammad Natsir (Negarawan-Dai), KH Wahid Hasyim

2-3 Mental Model Box + 1 Rantai Logika Tauhid + 1 Titik Refleksi per file.
Commit dan push setelah selesai.
```

---

## PHASE 3: EXPANSION — Konten Baru

### Prompt 3A: Esai Baru (4-6 file baru)

```
KONTEKS:
Buku "Generasi Pembaharu" sudah memiliki 4 esai. Tambahkan 5 esai baru yang
memperkaya perspektif. Baca esai yang ada dulu (folder esai/) untuk memahami
tone dan format, lalu buat esai baru dengan kualitas setara atau lebih baik.

ESAI BARU YANG PERLU DITULIS:

1. esai/perempuan-pembaharu.md
   "Perempuan Pembaharu: Dari Khadijah hingga Kampus"
   - Peran perempuan dalam sejarah pergerakan Islam
   - Bias gender dalam gerakan dakwah kampus
   - Model pemberdayaan perempuan yang Islami dan progresif
   - ~100-130 baris

2. esai/ekonomi-umat-dan-kemandirian.md
   "Ekonomi Umat dan Kemandirian"
   - Mengapa gerakan dakwah harus peduli ekonomi
   - Model ekonomi Islam: dari BMT hingga startup
   - Kemandirian finansial sebagai prasyarat kemandirian dakwah
   - ~100-130 baris

3. esai/spiritualitas-di-era-digital.md
   "Spiritualitas di Era Digital: Menjaga Hati di Tengah Algoritma"
   - Dampak teknologi terhadap kehidupan ruhani
   - Digital detox dari perspektif Islam
   - Membangun kebiasaan spiritual di era smartphone
   - ~100-130 baris

4. esai/dari-halaqah-ke-peradaban.md
   "Dari Halaqah ke Peradaban: Peta Jalan yang Hilang"
   - Gap antara tarbiyah individual dan dampak peradaban
   - Mengapa banyak alumni halaqah "menguap" setelah lulus
   - Framework: halaqah → organisasi → institusi → peradaban
   - ~100-130 baris

5. esai/kritik-diri-gerakan-dakwah.md
   "Kritik Diri Gerakan Dakwah: Keberanian Melihat Cermin"
   - Kelemahan-kelemahan internal gerakan dakwah kampus
   - Kultus tokoh, eksklusivisme, anti-intelektualisme
   - Jalan keluar: reform dari dalam
   - ~100-130 baris

FORMAT: Ikuti format esai yang sudah ada — naratif, personal, provokatif tapi konstruktif.
TONE: Seperti surat dari kakak senior yang jujur dan peduli.
Commit dan push setelah selesai. Update juga esai/README.md.
```

---

### Prompt 3B: Lampiran Praktis (3 file baru)

```
KONTEKS:
Buku "Generasi Pembaharu" membutuhkan lampiran praktis yang bisa langsung
digunakan oleh fasilitator dan aktivis dakwah kampus.

FILE BARU:

1. lampiran/panduan-fasilitator.md
   "Panduan Fasilitator: Cara Menggunakan Kurikulum Ini"
   - Prinsip fasilitasi halaqah yang efektif
   - Tips mengelola diskusi kelompok
   - Cara menggunakan Mental Model Box dan Rantai Logika Tauhid
   - Template rundown sesi (120 menit)
   - Do's and Don'ts
   - ~150-200 baris

2. lampiran/template-evaluasi.md
   "Template Evaluasi Peserta dan Program"
   - Rubrik penilaian per level (Mubtadi, Mutawassith, Mutaqaddim)
   - Format evaluasi diri peserta
   - Format evaluasi program oleh peserta
   - Indikator keberhasilan tarbiyah
   - ~120-150 baris

3. lampiran/peta-bacaan-bertahap.md
   "Peta Bacaan Bertahap: Dari Pemula hingga Lanjutan"
   - Kurikulum bacaan terstruktur per level
   - Level 1: 5 buku foundational
   - Level 2: 10 buku intermediate
   - Level 3: 15 buku advanced
   - Cara membaca buku secara kritis
   - Format: resensi mini + alasan kenapa penting
   - ~150-200 baris

Buat juga lampiran/README.md sebagai pengantar.
Commit dan push setelah selesai. Update DAFTAR_ISI.md.
```

---

### Prompt 3C: Epilog & Penutup

```
KONTEKS:
Buku "Generasi Pembaharu" membutuhkan penutup yang powerful.

FILE BARU:

1. 07-penutup/01-epilog-surat-untuk-generasi-mendatang.md
   "Epilog: Surat untuk Generasi Mendatang"
   - Ditulis sebagai surat dari generasi pembaharu hari ini kepada
     generasi 50 tahun yang akan datang
   - Refleksi tentang apa yang kita wariskan
   - Harapan, doa, dan amanah
   - Emosional, personal, menggerakkan
   - Ditutup dengan doa Qurani
   - ~150-200 baris

2. 07-penutup/02-doa-penutup.md
   "Doa Penutup: Ya Allah, Jadikan Kami Pembaharu"
   - Kompilasi doa-doa dari Al-Quran dan Sunnah yang relevan
   - Doa untuk ilmu, istiqamah, persatuan, dan kebangkitan umat
   - Format: Arab + transliterasi + terjemahan + konteks
   - ~80-100 baris

Buat juga 07-penutup/README.md.
Commit dan push. Update DAFTAR_ISI.md dan README.md.
```

---

## PHASE 4: COHERENCE — Konsistensi & Interkoneksi

### Prompt 4A: Cross-Referencing & Navigasi

```
KONTEKS:
Semua konten sudah ditulis. Sekarang buat koneksi antar-bagian.

INSTRUKSI:
1. Baca semua file bab buku (00-06 + 07-penutup)
2. Tambahkan "Bacaan Terkait" box di akhir setiap file bab buku:

   > **Bacaan Terkait dalam Buku Ini:**
   > - [Judul bab terkait 1](../path/to/file.md) — relevansi singkat
   > - [Judul bab terkait 2](../path/to/file.md) — relevansi singkat
   > - [Sesi kurikulum terkait](../kurikulum/path.md) — untuk pendalaman

3. Minimal 2-3 cross-reference per file, maksimal 5
4. Pastikan referensi bi-directional (jika A referensi B, B juga referensi A)
5. Update semua README.md di setiap folder untuk mencerminkan konten terbaru

Commit dan push setelah selesai.
```

---

### Prompt 4B: Konsistensi Format & Final DAFTAR_ISI

```
KONTEKS:
Final pass untuk konsistensi.

INSTRUKSI:
1. Pastikan semua file bab buku punya:
   - Quote pembuka (ayat atau hadits)
   - Penanda level: [F] Foundational, [I] Intermediate, [A] Advanced
   - Bagian "Refleksi & Aksi" di akhir
   - Link "Selanjutnya: [...]" di akhir

2. Update DAFTAR_ISI.md untuk mencakup SEMUA file termasuk yang baru:
   - Esai baru
   - Lampiran
   - Epilog/Penutup

3. Update README.md utama:
   - Tambahkan baris untuk Bab 7 (Penutup) di tabel
   - Tambahkan section Lampiran
   - Update jumlah esai

4. Pastikan tidak ada broken link di seluruh repo

Commit dan push setelah selesai.
```

---

## PHASE 5: POLISH — Final Review

### Prompt 5A: Glosarium, Bibliografi & Final Review

```
KONTEKS:
Tahap akhir penuntasan buku.

INSTRUKSI:

1. UPDATE GLOSARIUM (referensi/glosarium.md):
   - Grep semua istilah Arab/teknis yang muncul di seluruh buku
   - Pastikan SEMUA istilah yang digunakan ada di glosarium
   - Tambahkan istilah baru yang belum tercakup
   - Urutkan secara alfabetis

2. UPDATE KITAB WAJIB (referensi/kitab-wajib.md):
   - Pastikan semua buku yang direferensi di bab-bab masuk ke daftar
   - Tambahkan buku baru yang belum tercakup

3. UPDATE TOKOH INSPIRASI (referensi/tokoh-inspirasi.md):
   - Pastikan semua tokoh yang disebut di Mental Model Box tercantum
   - Tambahkan bio singkat tokoh baru

4. FINAL REVIEW:
   - Baca sekilas setiap file — cari inkonsistensi tone atau format
   - Pastikan tidak ada TODO, placeholder, atau catatan draft
   - Pastikan semua link berfungsi

Commit dan push setelah selesai.
```

---

## RINGKASAN EKSEKUSI

| Phase | Prompt | Target File | Estimasi Lines Baru | Prioritas |
|-------|--------|-------------|---------------------|-----------|
| 1A | Deepening Bab 2 | 5 file | +1,500 | **CRITICAL** |
| 1B | Deepening Bab 4 | 5 file | +1,500 | **CRITICAL** |
| 1C | Deepening Bab 5 | 4 file | +1,200 | **CRITICAL** |
| 1D | Deepening Bab 6 | 4 file | +1,200 | **CRITICAL** |
| 1E | Deepening Bab 1 & 3 | 7 file | +1,200 | HIGH |
| 2A | Enrichment Bab 1 | 4 file | +300 | HIGH |
| 2B | Enrichment Bab 2 | 5 file | +400 | HIGH |
| 2C | Enrichment Bab 3 | 5 file | +400 | HIGH |
| 2D | Enrichment Bab 4 | 5 file | +400 | HIGH |
| 2E | Enrichment Bab 5 & 6 | 8 file | +600 | HIGH |
| 3A | Esai Baru | 5 file baru | +550 | MEDIUM |
| 3B | Lampiran Praktis | 4 file baru | +500 | MEDIUM |
| 3C | Epilog & Penutup | 3 file baru | +400 | MEDIUM |
| 4A | Cross-Referencing | 25+ file | +300 | MEDIUM |
| 4B | Konsistensi Format | 30+ file | +200 | LOW |
| 5A | Glosarium & Final | 3+ file | +300 | LOW |
| | **TOTAL** | | **~10,450** | |

### Proyeksi Akhir

| Metrik | Sekarang | Setelah Selesai |
|--------|----------|-----------------|
| Total lines | ~5,562 | **~16,000** |
| Total files | 67 | **~79** |
| Bab buku utama avg | ~65 lines | **~300 lines** |
| Mental Model Box total | 36 (kurikulum only) | **~90+** |
| Rantai Logika Tauhid total | 18 (kurikulum only) | **~45+** |
| Esai | 4 | **9** |

---

## CATATAN EKSEKUSI

1. **Phase 1 bisa diparalelkan**: Prompt 1A-1D bisa dijalankan secara paralel (4 agent)
2. **Phase 2 bergantung pada Phase 1**: Jangan mulai enrichment sebelum deepening selesai
3. **Phase 3 independen**: Bisa dijalankan paralel dengan Phase 2
4. **Phase 4-5 harus sequential**: Harus dikerjakan terakhir setelah semua konten final
5. **Setiap prompt = 1 sesi Claude**: Dirancang agar cukup untuk satu context window

---

*Dokumen ini adalah peta jalan. Setiap prompt di atas sudah siap copy-paste untuk eksekusi.*
