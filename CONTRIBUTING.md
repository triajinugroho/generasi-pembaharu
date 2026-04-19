---
id: meta-contributing
title: "Panduan Berkontribusi"
chapter: meta
order: 0
level: lintas
personas: [aktivis-baru, murabbi, ketua-ldk, pembaca-mandiri, peneliti]
reading_time_min: 7
tags: [kontribusi, governance, alur-kerja, editorial, kode-etik]
outcomes:
  - "Memahami alur kontribusi dari fork sampai merge"
  - "Memenuhi standar metadata, gaya, dan isi yang diharapkan"
prerequisites: []
related: [meta-skema, meta-gaya-penulisan, root-readme, dampak, testimoni-readme]
last_reviewed: 2026-04-18
---

# Panduan Berkontribusi

> *"Barangsiapa menunjukkan pada kebaikan, maka ia mendapatkan pahala seperti pelakunya."*
> — HR. Muslim no. 1893

Terima kasih atas niat berkontribusi ke **Generasi Pembaharu**. Repo ini adalah amanah komunitas — kontribusi Anda, insya Allah, menjadi amal jariyah.

---

## Model: Kurated Community

Repo ini bukan open-source bebas.

- Siapa pun boleh mengajukan kontribusi.
- Setiap kontribusi melewati **editorial review**.
- Standar utama: **kualitas, kedalaman, keseimbangan manhaj, disiplin metadata**.

Editor berhak menolak atau meminta revisi kontribusi yang tidak memenuhi standar — dengan adab dan penjelasan yang jelas.

---

## Jenis Kontribusi yang Diterima

### 1. Konten
- **Perbaikan**: koreksi ayat/hadis/referensi, tata bahasa, ejaan, link rusak.
- **Penambahan**: esai baru, pendalaman topik, studi kasus kontekstual Indonesia.
- **Terjemahan/adaptasi**: ke bahasa daerah atau konteks lokal.

### 2. Metadata & Struktural
- Melengkapi frontmatter sesuai [`META-SKEMA.md`](./META-SKEMA.md).
- Menambah entri di [`indeks/`](./indeks/).
- Menulis [`ringkasan/`](./ringkasan/), [`kartu-halaqah/`](./kartu-halaqah/), atau [`flashcards/`](./flashcards/).

### 3. Pengalaman Lapangan
- Menulis [`testimoni/`](./testimoni/) dari adopsi nyata.
- Mendaftarkan LDK/organisasi di [`DAMPAK.md`](./DAMPAK.md).
- Melaporkan isu yang muncul di lapangan via GitHub Issue.

### 4. Diskusi
- Mengajukan pertanyaan di GitHub Discussions (kalau aktif).
- Membuka Issue untuk saran struktural atau kritik konstruktif.

---

## Prinsip Penulisan

Sebelum menulis, pahami:

1. **Berbasis dalil** — setiap klaim bisa dirujuk ke Al-Quran, hadis shahih, atau karya ulama muktabar.
2. **Lintas manhaj** — jangan menyerang organisasi atau manhaj tertentu. Ambil hikmah; tinggalkan khilafiyah yang memecah.
3. **Bahasa hidup** — tulis menggugah, tidak akademis kering atau populer dangkal.
4. **Kontekstual Indonesia 2026+** — membumi di realitas pemuda Muslim Indonesia.
5. **Actionable** — akhiri dengan Titik Refleksi atau langkah aksi nyata.
6. **Pure markdown** — tidak menambah tooling (no `package.json`, no CI, no scripts).

Detail gaya dan komponen pedagogis: lihat [`GAYA-PENULISAN.md`](./GAYA-PENULISAN.md).

---

## Cara Berkontribusi

### Langkah 1: Fork & Clone

1. Fork repo di GitHub.
2. Clone fork Anda.

### Langkah 2: Buat Branch Deskriptif

```bash
git checkout -b <tipe>/<topik-anda>
```

Contoh prefix `tipe`:
- `konten/` — kontribusi isi (esai, bab, ringkasan).
- `metadata/` — frontmatter, indeks, kartu.
- `fix/` — perbaikan kecil (link, typo).
- `terjemahan/` — terjemahan ke bahasa lain.
- `testimoni/` — cerita lapangan.

### Langkah 3: Tulis Kontribusi

- Ikuti struktur file yang sudah ada (lihat contoh di bab yang terdekat dengan kontribusi Anda).
- Untuk **file baru**: wajib menyertakan frontmatter lengkap sesuai [`META-SKEMA.md`](./META-SKEMA.md).
- Untuk **edit file lama**: update field `last_reviewed: <YYYY-MM-DD>` di frontmatter.
- Patuhi [`GAYA-PENULISAN.md`](./GAYA-PENULISAN.md) — termasuk komponen pedagogis (Mental Model, Rantai Logika, Titik Refleksi).

### Langkah 4: Verifikasi Sendiri

Sebelum PR, lakukan self-check:

- [ ] Frontmatter valid (paste ke yamllint.com).
- [ ] H1 sama dengan `title:` di frontmatter.
- [ ] Ada epigraf (ayat/hadis/syair) di awal.
- [ ] Ada Titik Refleksi di akhir (untuk file konten pelajaran).
- [ ] Ada bagian "Bacaan Terkait" kalau relevan.
- [ ] Semua link internal berfungsi (klik test di preview GitHub).
- [ ] Tidak ada serangan manhaj atau organisasi.
- [ ] Dalil punya sumber valid dengan format standar (`QS. X [n]: m`, `HR. X no. n`).
- [ ] Jika file >400 baris: sudah dipecah atau ada justifikasi.
- [ ] Tidak ada tooling baru (no `package.json`, no `.github/workflows/`, no scripts).

### Langkah 5: Submit Pull Request

- Judul PR deskriptif — mulai dengan prefix tipe seperti di branch.
- Deskripsi PR jelaskan: **apa** yang diubah/ditambah, **mengapa**, dan **referensi apa** yang diacu.
- Kalau PR besar (>500 baris berubah), pecah jadi beberapa PR yang lebih kecil.

---

## Proses Review

| Tahap | Fokus | Waktu Standar |
|-------|-------|---------------|
| 1. Review Teknis | Format markdown, link, frontmatter, metadata | 1-3 hari |
| 2. Review Konten | Keakuratan dalil, kedalaman, kontekstualitas | 3-14 hari |
| 3. Review Manhaj | Keseimbangan, inklusivitas, tidak partisan | 3-14 hari |
| 4. Review Bahasa | Keterbacaan, kekuatan narasi, adab | 1-7 hari |

Total waktu review rata-rata: **1-4 minggu** tergantung kompleksitas.

> [!TIP]
> PR kecil + fokus + self-checked = cepat lolos review. PR besar + banyak topik bercampur = lama atau diminta dipecah.

Editor berhak menolak dengan alasan jelas. Penolakan bukan penolakan pribadi — seringkali sekadar tidak cocok arah repo saat ini, atau butuh revisi.

---

## Disiplin Metadata

Ini bagian yang paling sering terlupakan. Wajib dibaca sekali.

### Semua File Markdown Konten Wajib

```yaml
---
id: <slug-stabil>
title: <sama dengan H1>
chapter: <0-7 | kurikulum | esai | referensi | lampiran | indeks | ringkasan | kartu-halaqah | flashcards | jalur | meta | testimoni>
order: <int, 0 untuk README direktori>
level: <tamhidi | muayyid | muntasib | lintas>
personas: [<min 1 persona>]
reading_time_min: <int>
tags: [<min 2 tag>]
outcomes:
  - "<verb-led kalimat outcome>"
prerequisites: []
related: []
last_reviewed: <YYYY-MM-DD>
---
```

### Field yang Sering Keliru

- **`id`**: **permanen**. Kalau Anda mengganti nama file, `id` **tidak boleh** berubah. Reviewer akan menolak PR yang mengganti `id` tanpa justifikasi kuat.
- **`outcomes`**: mulai dengan kata kerja aktif (mengartikulasikan, mengidentifikasi, menerapkan, dll). Bukan "Memberi pemahaman tentang X" (pasif, vague), tapi "Memahami tiga pilar X dan menerapkannya di konteks Y".
- **`personas`**: pilih hanya dari enum tertutup di [`META-SKEMA.md`](./META-SKEMA.md). Tidak boleh menambah persona baru dalam PR biasa.
- **`related`**: gunakan `id` lain, bukan path. Graf kanonik hidup di frontmatter, bukan di prosa.
- **`last_reviewed`**: update saat PR.

Detail lengkap: [`META-SKEMA.md`](./META-SKEMA.md).

---

## Kontribusi Khusus

### Untuk Terjemahan

1. Fork, buat repo terpisah dengan nama `generasi-pembaharu-<bahasa>`.
2. Terjemahkan semua file `.md`, termasuk frontmatter.
3. Pertahankan `id:` sama dengan repo asli — supaya cross-referensi lintas bahasa tetap bisa.
4. Ayat Al-Quran gunakan terjemahan resmi bahasa target (untuk Indonesia: Kemenag).
5. Laporkan ke [`DAMPAK.md`](./DAMPAK.md) repo asli via PR.

### Untuk Testimoni

Lihat [`testimoni/README.md`](./testimoni/README.md) dan [`testimoni/TEMPLATE.md`](./testimoni/TEMPLATE.md). Editor akan verifikasi via kontak sebelum merge.

### Untuk Indeks

1. Pilih satu file sumber untuk di-indeks.
2. Scan ayat/hadis/tokoh/tema/istilah yang relevan.
3. Tambahkan entri ke file indeks yang sesuai di [`indeks/`](./indeks/).
4. PR dengan judul `indeks: <file sumber>`.

### Untuk Splitting File Panjang

Beberapa file masih >400 baris (lihat catatan di [`DAMPAK.md`](./DAMPAK.md)). Kalau Anda ingin membantu memecah:

1. File induk tetap dengan nama sama, jadi **index** dengan 2-3 paragraf + link ke sub-file.
2. Sub-file baru di folder sama, dengan prefix yang konsisten.
3. Jaga `id:` induk tetap; sub-file dapat `id:` baru.
4. Update `related:` di file lain yang menautkan ke induk — jangan sampai broken link.
5. PR dengan judul `split: <file-id>`.

---

## Kode Etik Kontributor

1. **Niatkan sebagai ibadah**. Bukan untuk popularitas atau portofolio akademis.
2. **Hormati perbedaan manhaj dan organisasi**. Kalau Anda anggota organisasi tertentu, tahan diri untuk tidak menyelipkan promosi halus.
3. **Kritik ide, bukan pribadi atau kelompok**. Kritik konten itu sah; serangan personal tidak.
4. **Jaga adab dalam diskusi & review**. Tidak sarkastik, tidak kondescending.
5. **Utamakan persatuan di atas perbedaan minor**. Perbedaan fiqih kecil jangan jadi alasan menolak PR yang jelas bermanfaat.
6. **Jujur tentang keterbatasan Anda**. Kalau Anda bukan ahli di satu bidang, kontribusi Anda tetap berharga — sebut saja "saran editorial" dan biarkan ahli verifikasi.

Pelanggaran kode etik bisa berujung pembatalan akses kontribusi.

---

## Yang TIDAK Diterima

- ❌ Kontribusi yang menyerang manhaj atau tokoh secara personal.
- ❌ Kontribusi promosi organisasi, produk, atau caleg.
- ❌ Kontribusi yang menambahkan tooling (npm, pip, workflows, scripts).
- ❌ Dalil palsu atau tanpa sumber.
- ❌ Plagiat dari karya berhak cipta tanpa izin.
- ❌ Materi yang tidak sesuai dengan prinsip lintas-manhaj repo.

---

## Kontak

- **GitHub Issues** — diskusi terbuka, pertanyaan, saran.
- **GitHub Discussions** (kalau aktif) — diskusi non-issue.
- **Kontak pengelola** — via akun GitHub `triajinugroho` atau channel yang disebut di landing page.

---

> *"Barakallahu fiikum. Semoga Allah menjadikan kontribusi kita sebagai timbangan kebaikan di hari akhir."*

## 📚 Bacaan Terkait

- [`META-SKEMA.md`](./META-SKEMA.md) — kontrak frontmatter.
- [`GAYA-PENULISAN.md`](./GAYA-PENULISAN.md) — panduan gaya & komponen pedagogis.
- [`DELIVERY.md`](./DELIVERY.md) — opsi distribusi eksternal.
- [`DAMPAK.md`](./DAMPAK.md) — log adopsi & impact.
- [`testimoni/`](./testimoni/) — cerita lapangan.
