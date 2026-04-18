---
id: ringkasan-readme
title: "Ringkasan Shareable"
chapter: ringkasan
order: 0
level: lintas
personas: [aktivis-baru, pembaca-mandiri, murabbi, ketua-ldk]
reading_time_min: 2
tags: [ringkasan, shareable, whatsapp, telegram, mikro-konten]
outcomes:
  - "Mendapatkan konten ringkas yang siap dibagi di WhatsApp/Telegram"
  - "Memilih format sesuai platform (1-menit / 5-menit / visual)"
prerequisites: []
related: [root-readme, meta-delivery]
last_reviewed: 2026-04-18
---

# Ringkasan Shareable

> *"Sebarkanlah dariku walaupun satu ayat."*
> — HR. Bukhari no. 3461

Direktori ini berisi **versi ringkas** tiap bab repo, dirancang untuk dibagi di WhatsApp, Telegram, status Instagram, atau forum kampus.

## Tiga Format

| Format | Panjang | Platform ideal | Folder |
|--------|---------|----------------|--------|
| **1 menit** | ~150 kata | Status WhatsApp, caption IG | [`1-menit/`](./1-menit/) |
| **5 menit** | ~700 kata | Broadcast grup, newsletter | [`5-menit/`](./5-menit/) |
| **Visual** | 1 diagram Mermaid | Screenshot untuk status/story | [`visual/`](./visual/) |

## Satu File per Bab

Setiap format punya 8 file — satu per bab utama (0-7). Nama file: `chN.md` (mis. `ch1.md`).

## Aturan Penulisan Ringkasan

- **Tidak mengganti bab asli** — hanya ringkasan yang mengajak orang membaca utuh.
- **Selalu tutup dengan link** ke bab asli.
- **Dalil minimum** — tapi pastikan setiap yang dikutip benar.
- **Gaya WhatsApp** — paragraf pendek, tidak heading bertingkat, emoji hemat.
- **Copy-paste friendly** — tanpa markdown yang akan rusak saat dipaste (tidak pakai `#`, gunakan **bold** saja).

## Contoh Pemakaian

**Murabbi**: broadcast ringkasan 1-menit ke grup WhatsApp halaqah di pagi hari sebagai pengingat tema pekan ini.

**Ketua LDK**: pasang ringkasan visual ke akun IG LDK sebelum open recruitment, undang ngaji dalam.

**Pembaca mandiri**: simpan ringkasan 5-menit di Notes untuk refresh kalau lupa inti bab.

**Peneliti**: pakai ringkasan sebagai abstract saat mengutip repo dalam paper.

## Kontribusi

Ringkasan ini diisi bertahap. Tiap chapter punya kartu ringkasan template di `1-menit/TEMPLATE.md` dan `5-menit/TEMPLATE.md`.

1. Pilih bab dan format.
2. Salin template → isi.
3. Review: apakah esensi bab benar-benar tersampaikan? Apakah ada klaim di luar bab?
4. Buka PR dengan judul `ringkasan: chN <format>`.

Editor memastikan ringkasan tidak mengerdilkan nuansa bab asli.

## 📚 Bacaan Terkait

- [`kartu-halaqah/`](../kartu-halaqah/) — versi padat untuk fasilitator (bukan untuk di-share).
- [DELIVERY.md](../DELIVERY.md) — opsi distribusi lain.
