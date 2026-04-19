---
id: meta-skema
title: "META-SKEMA — Kontrak Frontmatter"
chapter: meta
order: 0
level: lintas
personas: [aktivis-baru, murabbi, ketua-ldk, pembaca-mandiri, peneliti]
reading_time_min: 6
tags: [meta, skema, frontmatter, yaml, kontribusi]
outcomes:
  - "Menulis frontmatter yang valid dan konsisten untuk setiap file konten"
  - "Memahami aturan id, prefix, persona, tags, dan graf cross-reference"
prerequisites: []
related: [meta-gaya-penulisan, meta-contributing, root-readme]
last_reviewed: 2026-04-18
---

# META-SKEMA — Kontrak Frontmatter Repo Generasi Pembaharu

> *"Tuhanku, lapangkanlah dadaku, dan mudahkanlah urusanku, dan lepaskanlah kekakuan dari lidahku agar mereka mengerti perkataanku."*
> — QS. Thaha [20]: 25–28

Dokumen ini mendefinisikan **skema metadata (YAML frontmatter)** yang wajib dipasang di bagian paling atas setiap file `.md` di repo ini.

Tujuannya bukan untuk membangun tooling — repo ini tetap **murni markdown, tanpa build step**. Skema ini adalah:

1. **Janji semantik** antar kontributor — setiap file mendeklarasikan siapa dia, untuk siapa, dan apa tujuannya.
2. **Siap-konsumsi** untuk alat baca komunitas: Obsidian, Logseq, Dataview, RAG, dan alat apa pun yang bisa membaca YAML — tanpa mengunci repo ini ke satu alat tertentu.
3. **Graf yang stabil**: field `id` dan `related` memungkinkan lintas-referensi tetap valid meski file dipindah atau diganti nama.

---

## Lokasi Frontmatter

Blok YAML di baris 1–N file, diapit oleh `---` di atas dan bawah:

```markdown
---
id: ch1-tauhid-pembebasan
title: Tauhid sebagai Pembebasan
...
---

# Tauhid sebagai Pembebasan

> *Epigraf Quran / Hadis / Syair...*
```

GitHub merender frontmatter sebagai tabel metadata di bagian atas halaman — tidak mengganggu isi.

---

## Skema Wajib

| Field | Tipe | Wajib | Contoh | Catatan |
|-------|------|-------|--------|---------|
| `id` | string | Ya | `ch1-tauhid-sebagai-pembebasan` | Slug permanen. Tidak berubah setelah publish. Format: `ch<N>-<slug>` untuk bab utama (slug = filename tanpa prefix `NN-`), `kur-l<N>-s<N>-<slug>` untuk kurikulum, `esai-<slug>`, `ref-<slug>`, `lamp-<slug>`, `indeks-<slug>`, `ringkas-<durasi>-ch<N>`, `kartu-l<N>-s<N>-<slug>`, `flash-ch<N>`, `jalur-<slug>`. |
| `title` | string | Ya | `Tauhid sebagai Pembebasan` | Judul penuh. Sama dengan H1 di badan file. |
| `chapter` | enum | Ya | `1` | `0`–`7` untuk bab utama; `kurikulum`, `esai`, `referensi`, `lampiran`, `indeks`, `ringkasan`, `kartu-halaqah`, `flashcards`, `jalur`, `meta` untuk lainnya. |
| `order` | int | Ya | `1` | Urutan dalam direktori. `0` untuk README direktori. |
| `level` | enum | Ya | `tamhidi` | `tamhidi` (dasar) \| `muayyid` (menengah) \| `muntasib` (lanjut) \| `lintas` (semua tingkat). |
| `personas` | list | Ya | `[aktivis-baru, murabbi]` | Subset dari: `aktivis-baru`, `murabbi`, `ketua-ldk`, `pembaca-mandiri`, `peneliti`. |
| `reading_time_min` | int | Ya | `12` | Heuristik: `ceil(baris / 40)`. |
| `tags` | list | Ya | `[tauhid, pembebasan, dakwah]` | Minimal 2, maksimal 7 tag. Gunakan lowercase-dengan-strip. |
| `outcomes` | list | Ya | `["Mengartikulasikan makna tauhid sebagai pembebasan", ...]` | 2–5 butir. Mulai dengan kata kerja aktif: *mengartikulasikan, mengidentifikasi, menghayati, menerapkan, mengevaluasi*. |
| `prerequisites` | list | Tidak | `[ch0-manifesto]` | Daftar `id` yang disarankan dibaca lebih dulu. Kosongkan `[]` kalau tidak ada. |
| `related` | list | Tidak | `[ch1-aqidah-menggerakkan, ch4-prinsip-dakwah-qurani]` | Daftar `id` untuk cross-reference. **Graf kanonik** hidup di sini. |
| `last_reviewed` | date | Tidak | `2026-04-18` | ISO 8601. Kontributor update saat melakukan editorial review. |

---

## Contoh Lengkap

### File bab utama

```yaml
---
id: ch1-tauhid-pembebasan
title: Tauhid sebagai Pembebasan
chapter: 1
order: 1
level: tamhidi
personas: [aktivis-baru, murabbi, pembaca-mandiri]
reading_time_min: 9
tags: [tauhid, aqidah, pembebasan, revolusi-kesadaran]
outcomes:
  - Mengartikulasikan makna tauhid sebagai pembebasan dari tirani selain Allah
  - Mengidentifikasi bentuk-bentuk penghambaan modern (materialisme, konsumerisme, opini publik)
  - Menerapkan La ilaha illallah sebagai lensa pembebasan harian
prerequisites: [ch0-manifesto]
related:
  - ch1-aqidah-menggerakkan
  - ch1-tauhid-sosial-keadilan
  - ch3-kepemimpinan-profetik
  - ch4-prinsip-dakwah-qurani
last_reviewed: 2026-04-18
---
```

### File kurikulum sesi

```yaml
---
id: kur-l1-s1-jati-diri
title: "Sesi 01: Mengenal Jati Diri — Siapakah Aku?"
chapter: kurikulum
order: 1
level: tamhidi
personas: [murabbi, aktivis-baru]
reading_time_min: 4
tags: [jati-diri, tauhid, pembukaan, halaqah]
outcomes:
  - Memfasilitasi sesi 120 menit tentang identitas mahasiswa muslim
  - Menghantarkan peserta pada kesadaran misi ilahiah
prerequisites: []
related:
  - ch0-manifesto
  - ch1-tauhid-pembebasan
  - kartu-l1-s1-jati-diri
last_reviewed: 2026-04-18
---
```

### File esai

```yaml
---
id: esai-mengapa-pemuda
title: Mengapa Pemuda?
chapter: esai
order: 1
level: lintas
personas: [aktivis-baru, pembaca-mandiri]
reading_time_min: 5
tags: [pemuda, tajdid, generasi]
outcomes:
  - Menjawab pertanyaan "mengapa justru pemuda yang dipanggil menjadi pembaharu?"
prerequisites: []
related: [ch0-manifesto, ch0-peta-krisis]
last_reviewed: 2026-04-18
---
```

---

## Aturan Penulisan `id`

1. **Permanen**: sekali dipublish, `id` tidak boleh diganti. Kalau file harus diganti nama, `id` ikut di frontmatter file baru — referensi di file lain tetap valid.
2. **Deterministik**: dihasilkan dari path + judul. Tim reviewer harus menolak PR dengan `id` duplikat.
3. **Hierarkis tapi ringkas**: `ch1-tauhid-pembebasan` lebih baik daripada `bab-1-fondasi-aqidah-01-tauhid-sebagai-pembebasan`.
4. **ASCII + tanda strip**: `[a-z0-9-]+`. Tidak ada spasi, tidak ada huruf kapital, tidak ada tanda baca.

---

## Prefix `id` Per Kategori

| Kategori | Prefix | Contoh |
|----------|--------|--------|
| Bab utama 0–7 | `ch<N>-` | `ch0-manifesto`, `ch1-tauhid-pembebasan`, `ch6-post-truth` |
| README direktori | `ch<N>-readme` atau `<kat>-readme` | `ch1-readme`, `kurikulum-readme`, `esai-readme` |
| Kurikulum | `kur-l<N>-s<N>-` | `kur-l1-s1-jati-diri`, `kur-l3-s6-visi-aksi` |
| Esai | `esai-` | `esai-mengapa-pemuda`, `esai-perempuan-pembaharu` |
| Referensi | `ref-` | `ref-glosarium`, `ref-tokoh-klasik` |
| Lampiran | `lamp-` | `lamp-panduan-fasilitator`, `lamp-peta-bacaan` |
| Indeks | `indeks-` | `indeks-ayat-quran`, `indeks-hadis` |
| Ringkasan | `ringkas-<durasi>-ch<N>` | `ringkas-1m-ch1`, `ringkas-5m-ch4` |
| Kartu halaqah | `kartu-l<N>-s<N>-` | `kartu-l1-s1-jati-diri` |
| Flashcards | `flash-ch<N>` | `flash-ch1`, `flash-ch4` |
| Jalur persona | `jalur-` | `jalur-aktivis-baru`, `jalur-murabbi` |
| Meta (skema, gaya, dll) | `meta-` | `meta-skema`, `meta-gaya-penulisan` |

---

## Personas (Enum Tertutup)

| Persona | Arti | Sumber |
|---------|------|--------|
| `aktivis-baru` | Mahasiswa/pelajar baru bergabung LDK/Rohis | `CARA-MENGGUNAKAN.md` |
| `murabbi` | Pembina/pementor halaqah, fasilitator tarbiyah | `CARA-MENGGUNAKAN.md` |
| `ketua-ldk` | Pengurus inti atau ketua LDK/Rohis | `CARA-MENGGUNAKAN.md` |
| `pembaca-mandiri` | Pembaca umum tidak terikat organisasi | `CARA-MENGGUNAKAN.md` |
| `peneliti` | Akademisi atau peneliti gerakan dakwah | `CARA-MENGGUNAKAN.md` |

Jangan menambah persona baru tanpa revisi skema ini.

---

## Tags (Terbuka, Tapi Terkurasi)

Tags bersifat terbuka, namun PR reviewer menjaga konsistensi:

- **Tema teologis**: `tauhid`, `aqidah`, `dakwah`, `ukhuwah`, `tarbiyah`, `manhaj`
- **Tema historis**: `sirah`, `sahabat`, `tabiin`, `pembaharu`, `pergerakan-indonesia`
- **Tema pengembangan diri**: `muraqabah`, `muhasabah`, `adab`, `akhlak`, `kepemimpinan`, `intelektual`
- **Tema strategi**: `metodologi-dakwah`, `dakwah-digital`, `manajemen-organisasi`, `komunikasi`
- **Tema kontemporer**: `post-truth`, `ai`, `gender`, `ekonomi`, `kebangsaan`, `liberalisme`
- **Tema operasional**: `halaqah`, `kurikulum`, `evaluasi`, `fasilitator`, `rekrutmen`

Hindari tag yang terlalu generik (`islam`, `dakwah-kampus`) atau terlalu spesifik (`hadith-no-4291`).

---

## Hubungan dengan Cross-Reference Prosa

File tetap boleh memuat bagian `### 📚 Bacaan Terkait dalam Buku Ini` di badan prosa (dengan link relatif), **namun graf kanonik hidup di `related:` frontmatter**. Kalau dua sumber tidak sinkron, `related:` yang menang.

Aturan saat file dipindah atau dipecah:

1. `id` tetap; update `title`, `order`, dan path di file lain yang menautkannya.
2. Jalankan pencarian global atas `id` yang dipindah — tidak perlu update karena `id` stabil.
3. Link relatif di prosa (hard-coded paths) perlu di-update manual. Reviewer memeriksa setiap PR pemindahan.

---

## Validasi Manual (Tanpa Tooling)

Karena repo ini pure-markdown:

1. **Copy-paste frontmatter ke linter YAML online** (mis. yamllint.com) saat menulis file baru.
2. **Buka repo di Obsidian** (gratis, tanpa build) — frontmatter muncul di panel *Properties*; field kosong atau salah tipe akan terlihat jelas.
3. **Spot-check reviewer**: dalam editorial review, pastikan `id` unik, `outcomes` verb-led, `personas` dan `level` enum valid, `related` merujuk `id` yang ada.

---

## FAQ

**T: Kenapa tidak pakai JSON Schema atau tool validasi?**
J: Repo ini pure-markdown — zero tooling. Skema ini adalah *disiplin manusia*, bukan kontrak yang di-enforce mesin. Reviewer PR adalah validator.

**T: Apakah boleh menambah field?**
J: Tidak dalam PR biasa. Perubahan skema melalui PR terpisah yang meng-update dokumen ini + alasan.

**T: Bagaimana kalau saya tidak tahu `reading_time_min` persisnya?**
J: Gunakan heuristik `ceil(baris / 40)`. Lebih penting konsisten daripada akurat.

**T: Mengapa `id` terpisah dari filename?**
J: Filename bisa berubah (tipo, restrukturisasi). `id` adalah alamat permanen yang mengikat cross-reference meski file dipindah.

---

> *"Dan Kami telah tulis dalam Zabur sesudah (Kami tulis dalam) Lauh Mahfuzh, bahwasanya bumi ini dipusakai hamba-hamba-Ku yang saleh."*
> — QS. Al-Anbiya [21]: 105

Skema ini adalah upaya kecil agar repo yang memuat amanah besar ini tetap mudah dirujuk, dijaga, dan diteruskan.
