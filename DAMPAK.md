---
id: meta-dampak
title: "DAMPAK — Log Terbuka Pemakaian Repo di Lapangan"
chapter: meta
order: 0
level: lintas
personas: [aktivis-baru, murabbi, ketua-ldk, pembaca-mandiri, peneliti]
reading_time_min: 3
tags: [dampak, impact, testimoni, adopsi, transparansi]
outcomes:
  - "Memetakan jangkauan aktual repo di lapangan secara transparan"
  - "Memberi ruang komunitas untuk mendaftarkan adopsi, terjemahan, dan turunan"
prerequisites: []
related: [testimoni, meta-delivery, root-readme]
last_reviewed: 2026-04-18
---

# DAMPAK — Log Terbuka Pemakaian Repo

> *"Dan siapakah yang lebih baik perkataannya daripada orang yang menyeru kepada Allah, mengerjakan amal yang saleh, dan berkata: 'Sesungguhnya aku termasuk orang-orang yang berserah diri.'"*
> — QS. Fussilat [41]: 33

Dokumen ini adalah **log transparan** pemakaian repo Generasi Pembaharu di lapangan.

Tujuannya **bukan memuji diri**. Tujuannya:

1. **Akuntabilitas** — setiap angka yang diklaim harus bisa diverifikasi (link, kontak, foto).
2. **Pelajaran** — pola apa yang muncul dari adopsi di berbagai konteks.
3. **Undangan** — komunitas yang belum adopsi bisa melihat siapa yang sudah, lalu menghubungi mereka untuk belajar.

Log ini diisi **sendiri oleh komunitas** via Pull Request ke file ini. Editor repo memverifikasi basic dengan cara menghubungi kontak yang didaftarkan. Tidak ada angka yang dipublish tanpa verifikasi.

---

## Cara Mendaftarkan Adopsi

1. Fork repo.
2. Edit file ini — tambahkan baris di tabel relevan.
3. Buka PR dengan judul `dampak: <LDK / organisasi / proyek> adopsi repo`.
4. Editor akan menghubungi kontak yang Anda sertakan untuk konfirmasi.
5. Setelah konfirmasi, PR di-merge.

**Data minimum**:
- Nama organisasi / LDK / komunitas
- Kota, kampus, atau konteks
- Periode pemakaian
- Jumlah peserta (approx ok)
- Skop pemakaian (bab apa, kurikulum level berapa, dll)
- Kontak (email atau nomor WA, akan diverifikasi, bisa disembunyikan di versi publik)

---

## LDK & Rohis yang Mengadopsi (Adopters)

_Tabel di bawah diisi oleh komunitas via PR. Kalau belum ada entri, berarti belum ada yang mendaftar — bukan berarti tidak ada adopsi._

| # | Nama LDK/Rohis | Kampus/Kota | Periode | Peserta | Skop | Kontak (terverifikasi) |
|---|----------------|-------------|---------|---------|------|------------------------|
| 1 | _Belum ada entri._ Daftarkan LDK Anda. | — | — | — | — | — |

---

## Fasilitator Halaqah Terdaftar

Kalau Anda seorang murabbi/fasilitator yang memakai kurikulum di sini — daftarkan diri. Tujuannya: membentuk **jaringan peer-to-peer** fasilitator lintas kota/kampus. Editor tidak mempublikasikan nama lengkap tanpa izin — Anda bisa pakai inisial + kota + kontak kanal diskusi.

| # | Inisial | Kota | Level yang difasilitasi | Periode aktif | Kanal kontak |
|---|---------|------|-------------------------|---------------|--------------|
| 1 | _Belum ada entri._ | — | — | — | — |

---

## Terjemahan Aktif

| # | Bahasa | Penerjemah/Tim | URL | Status | Lisensi |
|---|--------|----------------|-----|--------|---------|
| 1 | _Belum ada entri._ | — | — | — | — |

---

## Turunan Publik (Situs, PDF, Audio, Bot)

Daftarkan kalau Anda telah menerbitkan ulang repo dalam format lain.

| # | Jenis | Judul/URL | Pengelola | Catatan |
|---|-------|-----------|-----------|---------|
| 1 | _Belum ada entri._ | — | — | — |

---

## Referensi Akademik

Paper, skripsi, tesis, atau disertasi yang mereferensikan repo ini.

| # | Judul | Penulis | Institusi | Tahun | Link |
|---|-------|---------|-----------|-------|------|
| 1 | _Belum ada entri._ | — | — | — | — |

---

## Testimoni Tersinopsis

Log ringkas. Cerita lengkap ada di [`testimoni/`](./testimoni/).

- _Belum ada entri._

---

## Pekerjaan Berjalan (Open Work)

Pekerjaan yang sudah dimulai tapi belum tuntas — terbuka untuk kontribusi komunitas:

### Split File Panjang (>400 baris)

File-file ini menampung dua atau lebih tesis dalam satu halaman scroll — memecahnya jadi sub-file dengan file induk sebagai index akan memudahkan pembaca. Gaya pecahan mengikuti panduan di [`CONTRIBUTING.md`](./CONTRIBUTING.md) bagian "Untuk Splitting File Panjang".

- [ ] [`referensi/tokoh-inspirasi.md`](./referensi/tokoh-inspirasi.md) (~556 baris) → pisah ke `tokoh-klasik.md`, `tokoh-pertengahan.md`, `tokoh-modern.md`, `tokoh-nusantara.md`.
- [ ] [`02-sirah-dan-sejarah/01-blueprint-nabawi.md`](./02-sirah-dan-sejarah/01-blueprint-nabawi.md) (~473 baris) → Makkah / Madinah / Sintesis.
- [ ] [`01-fondasi-aqidah/04-falsafah-tauhid-pergerakan.md`](./01-fondasi-aqidah/04-falsafah-tauhid-pergerakan.md) (~432 baris) → Teori / Implikasi / Kritik Kontemporer.
- [ ] [`05-titik-temu-gerakan/04-blueprint-persatuan-umat.md`](./05-titik-temu-gerakan/04-blueprint-persatuan-umat.md) (~421 baris) → Diagnosa / Prinsip / Praktik.
- [ ] [`01-fondasi-aqidah/02-aqidah-yang-menggerakkan.md`](./01-fondasi-aqidah/02-aqidah-yang-menggerakkan.md) (~415 baris) → Konsep / Sejarah / Latihan.

### Pengisian Indeks

Berkas indeks di [`indeks/`](./indeks/) masih scaffold. Kontributor mengisi bertahap: ayat/hadis/tokoh/tema/istilah → file pengutip. Lihat [`indeks/README.md`](./indeks/README.md).

### Ringkasan 5-Menit & Visual

`ringkasan/5-menit/` dan `ringkasan/visual/` masih berisi hanya README + template. Tiap bab (0-7) butuh satu draf 700 kata + satu diagram.

### Kartu Halaqah 17 Sesi Lagi

`kartu-halaqah/` baru berisi 1 contoh siap (`l1-s1-jati-diri.md`). Masih 17 sesi tersisa — distilasi dari file `kurikulum/level-N-xxx/sesi-N-xxx.md`.

### Flashcards 7 Bab Lagi

`flashcards/` baru berisi 1 deck lengkap (`ch1.md`). 7 bab tersisa (0, 2-7).

### Frontmatter Outcomes untuk File Kurikulum

Sebagian file kurikulum (sesi-*.md) memiliki `outcomes: []  # TODO: editorial review` — butuh editorial pass untuk mengisi outcome yang verb-led.

---

## Metrik yang Kami Sengaja TIDAK Lacak

Repo ini **tidak memasang analytics**, tidak melacak IP, tidak punya account wall. Itu disengaja:

- ❌ Pageview count
- ❌ Unique visitors
- ❌ Dwell time
- ❌ A/B testing copy
- ❌ Conversion funnels
- ❌ Session recording

Yang kami dengar adalah **yang Anda ceritakan** via `testimoni/` atau PR ke file ini. Kualitas > kuantitas.

---

## Catatan Pengelola

- **Verifikasi**: setiap entri diverifikasi via kontak balik. Editor boleh menolak entri tanpa kontak verifikasi.
- **Privasi**: kontak personal tidak dipublish tanpa izin. Bisa dipakai alias/inisial.
- **Kejujuran**: lebih baik daftar kosong yang jujur daripada daftar ramai yang dipalsukan.
- **Anti-klaim**: editor tidak membiarkan klaim berlebihan ("mengubah hidup 10.000 orang") tanpa bukti.
- **Sensitif**: untuk konteks yang sensitif secara politis (mis. LDK di wilayah rentan), entri bisa pakai pseudonim dengan verifikasi tertutup.

---

## Target Impact yang Kami Doakan (Bukan Janji)

Ini bukan KPI. Ini doa:

- 100 LDK/Rohis di Indonesia yang menggunakan kurikulum ini dalam 2 tahun pertama.
- 1.000 murabbi yang terhubung dalam jaringan peer-to-peer.
- 5 terjemahan aktif.
- 1 turunan PDF siap cetak yang didistribusikan gratis di pesantren dan lapas.
- 10 paper akademik yang merujuk repo ini secara kritis.
- 1 ekosistem turunan (bot, audio, cetak, flashcard) yang otonom dari repo utama.

Kalau tidak tercapai — tidak apa-apa. Amal dinilai dari niat dan kesungguhan, bukan volumenya.

Kalau tercapai — itu karunia Allah, bukan jerih payah kami.

---

## Titik Refleksi (Untuk Yang Akan Daftarkan)

1. Apa **dampak konkret** yang saya saksikan — bukan yang saya harapkan?
2. Apakah saya akan **mendaftarkan** ini kalau tidak ada imbalan branding apa pun?
3. Apakah saya **siap dihubungi** editor untuk verifikasi, termasuk diminta menunjukkan peserta atau dokumentasi?
4. Apa pelajaran yang akan saya **bagikan** ke komunitas lain yang baru akan memulai?

---

## 📚 Bacaan Terkait

- [testimoni/](./testimoni/) — cerita lengkap dari lapangan.
- [DELIVERY.md](./DELIVERY.md) — opsi distribusi yang dipakai turunan.
- [CONTRIBUTING.md](./CONTRIBUTING.md) — alur kontribusi.
- [jalur/ketua-ldk.md](./jalur/ketua-ldk.md) — salah satu pintu masuk untuk LDK yang akan adopsi.
