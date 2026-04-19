---
id: meta-peta-konsep
title: Peta Konsep Generasi Pembaharu
chapter: meta
order: 0
level: lintas
personas: [aktivis-baru, murabbi, ketua-ldk, pembaca-mandiri, peneliti]
reading_time_min: 4
tags: [peta-konsep, navigasi, diagram, graf]
outcomes:
  - "Memvisualisasikan hubungan antar bab dan tema dalam repo"
  - "Memilih titik masuk yang sesuai dengan profil dan kebutuhan pembaca"
prerequisites: []
related: [root-readme, meta-cara-menggunakan]
last_reviewed: 2026-04-18
---

# Peta Konsep Generasi Pembaharu

> *"Dan Kami jadikan di antara mereka itu pemimpin-pemimpin yang memberi petunjuk dengan perintah Kami ketika mereka sabar. Dan mereka meyakini ayat-ayat Kami."*
> — QS. As-Sajdah [32]: 24

File ini memetakan **hubungan antar konsep** di repo ini secara visual. Tujuannya bukan menggantikan bacaan isi, tapi memberi peta agar pembaca tahu ia sedang berada di mana dan hendak ke mana.

Semua diagram di sini memakai Mermaid — dirender langsung oleh github.com tanpa build tool.

---

## 1. Peta Buku Utama: Tauhid sebagai Poros

Semua bab berpusar pada tauhid. Tidak ada bab yang berdiri sendiri.

```mermaid
flowchart TB
    T((Tauhid))
    B0[Bab 0<br/>Mukadimah]
    B1[Bab 1<br/>Fondasi Aqidah]
    B2[Bab 2<br/>Sirah &amp; Sejarah]
    B3[Bab 3<br/>Pembangunan Diri]
    B4[Bab 4<br/>Strategi Dakwah]
    B5[Bab 5<br/>Titik Temu]
    B6[Bab 6<br/>Tantangan Kontemporer]
    B7[Bab 7<br/>Penutup]

    B0 -->|mengapa| T
    T -->|diinternalisasi| B1
    T -->|diwujudkan| B3
    B1 -->|diverifikasi| B2
    B2 -->|diterjemahkan| B4
    B3 -->|dibentuk| B4
    B4 -->|dikolaborasikan| B5
    B5 -->|diuji| B6
    B6 -->|dirangkum| B7

    classDef hub fill:#0a4d3f,stroke:#0a4d3f,color:#fff,stroke-width:2
    class T hub
```

- **B0 → T**: Mukadimah menjelaskan mengapa tauhid harus dihidupkan kembali.
- **T → B1**: Aqidah adalah pembebasan dari tirani selain Allah.
- **T → B3**: Pembangunan diri = mengikat diri pada tauhid setiap hari.
- **B1 → B2**: Sirah memverifikasi bahwa tauhid pernah melahirkan peradaban.
- **B2 → B4**: Metode Nabawi jadi sumber strategi dakwah.
- **B3 ⊕ B4 → B5**: Diri yang matang + strategi yang tajam → kolaborasi yang sehat.
- **B5 → B6**: Kolaborasi teruji oleh tantangan zaman.
- **B6 → B7**: Penutup menyerahkan estafet ke generasi berikutnya.

---

## 2. Peta Persona: 5 Jalur Baca

```mermaid
flowchart LR
    P([Saya siapa?])
    P --> A[🌱 Aktivis Baru]
    P --> M[🕯️ Murabbi / Fasilitator]
    P --> K[🧭 Ketua LDK]
    P --> S[📖 Pembaca Mandiri]
    P --> R[🔬 Peneliti]

    A --> A1[Mukadimah] --> A2[Kurikulum L1 Tamhidi]
    M --> M1[Panduan Fasilitator] --> M2[Kartu Halaqah] --> M3[Kurikulum L1-L3]
    K --> K1[Bab 4 Strategi] --> K2[Bab 5 Titik Temu] --> K3[Bab 6 Kontemporer]
    S --> S1[Mukadimah] --> S2[Bab 1-7 berurutan]
    R --> R1[Daftar Isi] --> R2[Indeks] --> R3[Glosarium + Tokoh]
```

Detail setiap jalur: [`jalur/`](./jalur/).

---

## 3. Sirah Nabawi: Fase dan Prinsip

```mermaid
timeline
    title Blueprint Dakwah Nabawi (23 Tahun)
    610 : Wahyu pertama
        : Dakwah sirriyyah (rahasia, 3 tahun)
    613 : Dakwah jahriyyah (terbuka)
        : Boikot, intimidasi, penyiksaan
    619 : Tahun Kesedihan
        : Khadijah &amp; Abu Thalib wafat
    620 : Bai'at Aqabah I
    622 : Bai'at Aqabah II
        : Hijrah ke Madinah
        : Piagam Madinah
    624 : Perang Badar
    628 : Perjanjian Hudaibiyah
    630 : Fathu Makkah
    632 : Haji Wada'
        : Nabi ﷺ wafat
```

Baca: [`02-sirah-dan-sejarah/01-blueprint-nabawi.md`](./02-sirah-dan-sejarah/01-blueprint-nabawi.md).

---

## 4. Lanskap Gerakan Islam Indonesia

```mermaid
flowchart TB
    subgraph Tradisional[Tradisional]
        NU[Nahdlatul Ulama]
        PBH[Pesantren &amp; Thoriqoh]
    end
    subgraph Modernis[Modernis]
        MUH[Muhammadiyah]
        Persis[Persis]
    end
    subgraph Salafi[Salafi / Dakwah Sunnah]
        SLF[Yayasan &amp; pesantren salafi]
    end
    subgraph Tarbiyah[Tarbiyah / Harakah]
        LDK[LDK kampus]
        PKS[Gerakan tarbiyah]
    end
    subgraph HijrahPop[Hijrah Populer]
        HJR[Komunitas hijrah<br/>media sosial]
    end

    Tradisional & Modernis & Salafi & Tarbiyah & HijrahPop --> TT[(Titik Temu: Aqidah, Akhlak, Misi Umat)]
```

Detail: [`05-titik-temu-gerakan/01-peta-gerakan-dakwah-indonesia.md`](./05-titik-temu-gerakan/01-peta-gerakan-dakwah-indonesia.md).

---

## 5. Alur Tarbiyah Dzatiyah (Pembangunan Diri)

```mermaid
flowchart LR
    subgraph Harian[Harian]
        Mur[Muraqabah<br/>kesadaran]
        Muh[Muhasabah<br/>evaluasi]
    end
    subgraph Pekanan[Pekanan]
        Hal[Halaqah<br/>liqo']
        Baca[Bacaan terstruktur]
    end
    subgraph Bulanan[Bulanan]
        Khi[Khidmah pada umat]
        Prj[Proyek dakwah]
    end
    subgraph Tahunan[Tahunan]
        Eval[Evaluasi jalan]
        Visi[Revisi visi 5 tahun]
    end

    Harian --> Pekanan --> Bulanan --> Tahunan --> Harian
```

Baca: [`03-pembangunan-diri/`](./03-pembangunan-diri/).

---

## 6. Progresi Kurikulum Halaqah

```mermaid
flowchart LR
    T1[L1 Tamhidi<br/>6 sesi x 120 mnt<br/>Persiapan] --> T2[L2 Muayyid<br/>6 sesi x 120 mnt<br/>Pendukung]
    T2 --> T3[L3 Muntasib<br/>6 sesi x 120 mnt<br/>Anggota Penuh]
    T1 -.outcome.-> O1[Identitas<br/>+ komitmen awal]
    T2 -.outcome.-> O2[Kepemimpinan<br/>+ proyek dakwah]
    T3 -.outcome.-> O3[Visi makro<br/>+ institusi]
```

Baca: [`kurikulum/`](./kurikulum/). Kartu ringkas: [`kartu-halaqah/`](./kartu-halaqah/).

---

## 7. Peta Tantangan Kontemporer → Jawaban Repo

```mermaid
flowchart LR
    L[Liberalisme &amp;<br/>krisis identitas] --> J1[Bab 1 Tauhid<br/>+ Bab 6.1]
    P[Post-truth &amp;<br/>banjir informasi] --> J2[Bab 3.3 Intelektualitas<br/>+ Bab 4.3 Digital<br/>+ Bab 6.2]
    A[AI &amp; disrupsi<br/>pekerjaan] --> J3[Bab 6.3<br/>+ Esai Ekonomi Umat]
    G[Gender &amp;<br/>krisis keluarga] --> J4[Esai Perempuan Pembaharu<br/>+ Bab 3]
    K[Kebangsaan &amp;<br/>krisis kepemilikan] --> J5[Bab 6.4<br/>+ Bab 2.5 Sejarah Indonesia]
    F[Fragmentasi<br/>gerakan] --> J6[Bab 5 Titik Temu<br/>+ Esai Dakwah Bukan Partisan]
```

---

## 8. Rantai Logika Utama Repo

```mermaid
flowchart TD
    P1[Pemuda adalah penggerak<br/>perubahan dalam sirah]
    P2[Pemuda Indonesia hari ini<br/>menghadapi 3 krisis besar]
    P3[Krisis bukan karena kurang semangat<br/>tapi kurang fondasi + strategi + ukhuwah]
    P4[Maka dibutuhkan tarbiyah yang mengakar:<br/>aqidah + sirah + diri + strategi + kolaborasi]
    P5[Ini bukan milik satu manhaj<br/>ia milik umat]
    P6[Jadi repo ini lintas-manhaj,<br/>kurasi komunitas, bebas dipakai]

    P1 --> P2 --> P3 --> P4 --> P5 --> P6
```

---

## 9. Graf Cross-Reference (Contoh)

Setiap bab mereferensikan bab lain. Berikut contoh rajutan Bab 1 → seluruh buku.

```mermaid
flowchart LR
    C1[ch1-tauhid-pembebasan]
    C1 --> A1[ch1-aqidah-menggerakkan]
    C1 --> A3[ch1-tauhid-sosial-keadilan]
    C1 --> C3[ch3-kepemimpinan-profetik]
    C1 --> C4[ch4-prinsip-dakwah-qurani]
    C1 --> C6[ch6-liberalisme-identitas]
    C1 --> E1[esai-dakwah-bukan-partisan]
```

Graf kanonik hidup di field `related:` di frontmatter setiap file (lihat [`META-SKEMA.md`](./META-SKEMA.md)).

---

## 10. Navigasi Cepat dari Halaman Ini

- Cari **tema** → [`indeks/tema.md`](./indeks/tema.md)
- Cari **ayat atau hadis** → [`indeks/ayat-quran.md`](./indeks/ayat-quran.md) · [`indeks/hadis.md`](./indeks/hadis.md)
- Cari **tokoh** → [`indeks/tokoh.md`](./indeks/tokoh.md)
- Cari **istilah** → [`referensi/glosarium.md`](./referensi/glosarium.md) via [`indeks/istilah.md`](./indeks/istilah.md)
- Cari **sesi halaqah** → [`kurikulum/`](./kurikulum/) + [`kartu-halaqah/`](./kartu-halaqah/)
- Mau **share di grup** → [`ringkasan/1-menit/`](./ringkasan/1-menit/)

---

> *"Dan Tuhanmu tidak melupakan."* — QS. Maryam [19]: 64

Peta ini insya Allah hidup. Kalau ada konsep yang belum terwakili, buka PR.
