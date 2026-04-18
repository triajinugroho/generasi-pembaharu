---
id: meta-delivery
title: "DELIVERY — Opsi Distribusi Eksternal Tanpa Build Tool"
chapter: meta
order: 0
level: lintas
personas: [murabbi, ketua-ldk, pembaca-mandiri, peneliti]
reading_time_min: 6
tags: [delivery, distribusi, hosting, pdf, ebook, audio, web]
outcomes:
  - "Mengenali lima opsi distribusi repo tanpa menambah tooling ke repo itu sendiri"
  - "Memilih opsi yang sesuai dengan kebutuhan komunitas lokal"
prerequisites: []
related: [root-readme, meta-skema, dampak]
last_reviewed: 2026-04-18
---

# DELIVERY — Menyebarkan Repo Tanpa Mengotori Repo

> *"Sampaikanlah dariku walaupun hanya satu ayat."*
> — HR. Bukhari no. 3461

Repo ini sengaja **pure-markdown**, tanpa generator, CI/CD, atau build tool. Itu pilihan sadar: agar materinya tahan waktu, mudah di-fork, gampang diterjemahkan, dan tidak mati karena satu framework depresiasi.

Tapi pembaca 2026+ mengharapkan pengalaman lain selain "clone git lalu baca di editor". Dokumen ini mendaftar **opsi distribusi eksternal** yang bisa dijalankan komunitas mana pun tanpa mengotori repo utama.

**Prinsip panduan**:

1. Repo utama **tidak menyediakan** tooling distribusi. Tidak ada `package.json`, tidak ada GitHub Actions, tidak ada build scripts.
2. Siapa pun boleh menjalankan salah satu opsi ini **dari fork mereka sendiri** — hasil akhir adalah milik komunitas penerbitnya.
3. Kalau komunitas penerbit ingin link-back ke repo utama, silakan. Tidak wajib.
4. **Lisensi tetap berlaku**: CC BY-NC-SA 4.0. Non-komersial + atribusi + share-alike.

---

## Opsi 1: GitHub sebagai Situs (Nol Konfigurasi)

GitHub sudah merender markdown dengan:

- **Mermaid diagrams** (sejak 2022)
- **Admonitions** `> [!NOTE]`, `> [!TIP]`, dll. (sejak 2024)
- **Collapsible sections** (`<details>`)
- **Task lists** (`- [ ]`)
- **Dark mode** otomatis
- **Search** (pakai GitHub search + `repo:triajinugroho/generasi-pembaharu`)
- **Mobile-responsive** natif
- **Permalinks** ke line number
- **Frontmatter rendered as metadata table**

**Cocok untuk**: mayoritas pembaca. Ini default.

**Kelemahan**: perlu akun GitHub untuk interaksi penuh (fork, PR). Pencarian kurang canggih dibanding situs dedicated.

**Setup**: tidak ada. Sudah jalan.

---

## Opsi 2: Docsify (Runtime JS, Zero Build)

[Docsify](https://docsify.js.org) merender `.md` secara runtime. Satu file `index.html` + CDN JS. **Tidak butuh build step.**

**Cara pakai** (di fork Anda):

1. Buat `docs/index.html` di fork:
   ```html
   <!DOCTYPE html>
   <html>
   <head>
     <meta charset="UTF-8">
     <title>Generasi Pembaharu</title>
     <meta name="viewport" content="width=device-width,initial-scale=1.0">
     <link rel="stylesheet" href="//cdn.jsdelivr.net/npm/docsify@4/lib/themes/vue.css">
   </head>
   <body>
     <div id="app"></div>
     <script>
       window.$docsify = {
         name: 'Generasi Pembaharu',
         loadSidebar: true,
         subMaxLevel: 3,
         search: 'auto',
         basePath: '../'
       }
     </script>
     <script src="//cdn.jsdelivr.net/npm/docsify@4"></script>
     <script src="//cdn.jsdelivr.net/npm/docsify/lib/plugins/search.min.js"></script>
     <script src="//cdn.jsdelivr.net/npm/mermaid/dist/mermaid.min.js"></script>
   </body>
   </html>
   ```
2. Aktifkan **GitHub Pages** → Source: `main` branch `/docs` folder.
3. Situs hidup dalam 1 menit di `https://<user>.github.io/<fork>/`.

**Kelemahan**: SEO terbatas (JS-rendered). Tidak ada offline PWA tanpa plugin tambahan.

**Cocok untuk**: komunitas yang mau situs cepat dengan search tanpa belajar Astro/Docusaurus/Starlight.

---

## Opsi 3: GitBook Import

[GitBook](https://www.gitbook.com/) free tier mengimpor repo markdown dan merender sebagai buku digital dengan TOC kiri + konten + PDF export built-in.

**Cara pakai**:

1. Sign up di GitBook.
2. **Import from Git**: masukkan URL fork Anda.
3. GitBook otomatis membangun site + export PDF.

**Kelemahan**: free tier terbatas. Lock-in ke GitBook.

**Cocok untuk**: komunitas yang butuh PDF export siap pakai.

---

## Opsi 4: Obsidian Publish

[Obsidian](https://obsidian.md/) (gratis, desktop) membaca repo sebagai vault:

1. Buka folder repo sebagai vault di Obsidian.
2. Obsidian langsung memahami frontmatter YAML (sesuai `META-SKEMA.md`) dan menampilkan graph view, backlinks, properties panel.
3. Gunakan **Obsidian Publish** (berbayar, $8/bulan) untuk publish vault ke web dengan domain kustom.

**Kelemahan**: Obsidian Publish berbayar.

**Cocok untuk**: komunitas yang mau visualisasi graph knowledge base + willing to pay.

---

## Opsi 5: Ekspor PDF / EPUB Manual

Untuk distribusi offline (pesantren tanpa internet, tahanan, pengungsi, distribusi fisik):

**PDF dari GitHub**:
- Buka file di github.com → Print (Cmd/Ctrl+P) → Save as PDF. Satu file per halaman.
- Gabungkan dengan `pdftk` atau `qpdf` (alat offline, di komputer Anda — bukan di repo).

**EPUB dari Pandoc** (di komputer Anda):
```bash
pandoc -o generasi-pembaharu.epub \
  README.md \
  00-mukadimah/README.md 00-mukadimah/*.md \
  01-fondasi-aqidah/README.md 01-fondasi-aqidah/*.md \
  # ... dst
```

**Cetak buku**:
- Konversi seluruh repo ke LaTeX (Pandoc support), cetak via percetakan lokal.
- Beberapa penerbit dakwah kampus sudah menawarkan jasa ini — kontak [testimoni/](./testimoni/) untuk cerita mereka.

---

## Opsi 6: Audio (TTS + Arab Asli)

Untuk pembaca yang lebih suka mendengar — komuter, penglihatan terbatas:

- Gunakan TTS gratis: **Google Cloud TTS** (Indonesian voice), **Microsoft Edge Read Aloud**, **Eleven Labs** (berbayar, lebih natural).
- Untuk ayat Al-Quran yang dikutip: **sisipkan rekaman qari** yang Anda sukai (Mishary, Sudais, dll.) menggantikan pembacaan TTS.
- Hasil akhir: podcast MP3 per bab. Host di Spotify Podcasters (gratis) atau Anchor.fm.

**Template proses**:
1. Ekstrak teks markdown jadi teks polos (pakai Pandoc atau skrip Anda).
2. Pisahkan bagian "QS. ..." jadi cue untuk recorded audio.
3. Gabungkan dengan FFmpeg.

---

## Opsi 7: WhatsApp & Telegram Summaries

Paling viral di Indonesia 2026+.

- [`ringkasan/1-menit/`](./ringkasan/1-menit/) — sudah didesain untuk di-copas ke status WA (150 kata).
- [`ringkasan/5-menit/`](./ringkasan/5-menit/) — cocok untuk broadcast grup.
- [`ringkasan/visual/`](./ringkasan/visual/) — screenshot Mermaid untuk status WA/IG story.

**Tip**: buat bot Telegram yang setiap pagi kirim ringkasan 1 menit dari bab random. Butuh hosting ringan (Vercel free, Railway, fly.io) — di luar repo.

---

## Opsi 8: Terjemahan Komunitas

Lisensi CC BY-NC-SA 4.0 mengizinkan terjemahan. Fork repo → terjemahkan seluruh file `.md` → pertahankan frontmatter → publish sebagai repo baru dengan atribusi.

**Sudah / sedang dijajaki** (kalau ada, update di [DAMPAK.md](./DAMPAK.md)):
- [ ] Bahasa Melayu Malaysia
- [ ] Bahasa Jawa (ngoko & krama)
- [ ] Bahasa Sunda
- [ ] Bahasa Inggris
- [ ] Bahasa Arab

**Penting**: terjemahan bukan sekadar bahasa — ayat & hadis idealnya merujuk terjemahan resmi yang diakui di bahasa target.

---

## Opsi 9: AI Study Assistant (RAG Komunitas)

Komunitas mana pun bisa membangun asisten AI berbasis repo ini tanpa mengotori repo. Skema:

1. Clone repo.
2. Chunk per file (frontmatter jadi metadata filter).
3. Embed (OpenAI, Gemini, atau model lokal seperti Indonesian BERT).
4. Store di vector DB (Pinecone, Weaviate, pgvector).
5. Deploy bot Telegram/Discord/Web.

**Guardrails yang wajib** untuk konten dakwah:

- Selalu sertakan **sitasi ke file + `id:` frontmatter**.
- **Tolak menjawab** pertanyaan fiqh kontroversial tanpa menunjukkan dalil asli.
- Tekankan **bukan pengganti ustadz/mentor** — alat belajar tambahan.
- Log dan audit jawaban secara berkala.

Repo tidak menyediakan bot ini. Kalau komunitas Anda membangunnya, daftarkan di [DAMPAK.md](./DAMPAK.md).

---

## Opsi 10: Micro-Learning / Flashcards

- [`flashcards/`](./flashcards/) berisi Q&A per bab dalam format yang bisa diimpor ke:
  - **Anki** (via komunitas plugin markdown-to-Anki)
  - **Mochi**
  - **Quizlet** (paste manual)
- Durasi review: 5-10 menit per hari, review spaced-repetition.

---

## Apa yang TIDAK Boleh

Berikut adalah opsi distribusi yang **bertentangan dengan lisensi CC BY-NC-SA 4.0**:

- ❌ Menjual buku cetak untuk profit tanpa izin.
- ❌ Memasukkan konten repo ke platform berbayar sebagai paywall.
- ❌ Mengklaim sebagai karya sendiri.
- ❌ Merubah lisensi (turunan harus tetap BY-NC-SA 4.0).
- ❌ Menyisipkan iklan komersial atau sponsor politik di turunan publik.

Distribusi yang **diperbolehkan dengan atribusi**:

- ✅ Cetakan untuk dibagikan gratis (bukan dijual).
- ✅ Audio podcast gratis (boleh monetisasi non-iklan seperti donasi sukarela).
- ✅ Situs gratis dengan hosting berbayar dari donasi komunitas.
- ✅ Adaptasi & terjemahan dengan atribusi jelas + link balik.

---

## Titik Refleksi (Bagi yang Akan Menerbitkan Ulang)

1. **Motif saya** menerbitkan ulang ini — apakah betul-betul dakwah, atau ada motif lain (popularitas, branding organisasi)?
2. **Kualitas kurasi** di fork/turunan saya — apakah saya menambahkan nilai, atau sekadar menyalin?
3. **Umpan balik** dari pembaca turunan saya — apakah saya tampung dan forward ke repo utama?
4. **Keberlanjutan** hosting/distribusi saya — kalau saya berhenti, apakah pembaca punya jalur alternatif?

---

## 📚 Bacaan Terkait

- [README.md](./README.md) — landing page utama.
- [DAMPAK.md](./DAMPAK.md) — daftar adopsi & turunan publik.
- [CONTRIBUTING.md](./CONTRIBUTING.md) — alur kontribusi ke repo utama.
- [META-SKEMA.md](./META-SKEMA.md) — struktur yang memudahkan pipeline distribusi.
- [LICENSE / CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/) — aturan main.
