# GorontaloKita — Blog Niche Gorontalo

Portal wisata, kuliner, budaya & info terkini dari Gorontalo.  
Dibangun dengan Jekyll + GitHub Pages. Gratis hosting, cukup tulis artikel dalam Markdown.

---

## 🚀 Cara Deploy ke GitHub Pages

### Langkah 1: Buat Repository GitHub
1. Buka https://github.com/new
2. Nama repo: `gorontalokita` (atau `username.github.io` untuk domain utama)
3. Set ke **Public**
4. Klik **Create repository**

### Langkah 2: Upload Semua File
```bash
# Clone repo kosong
git clone https://github.com/USERNAME/gorontalokita.git
cd gorontalokita

# Salin semua file dari folder ini ke dalam repo
# (atau langsung push jika sudah di folder ini)

git add .
git commit -m "Initial blog setup"
git push origin main
```

### Langkah 3: Aktifkan GitHub Pages
1. Buka repo di GitHub → **Settings** → **Pages**
2. Source: pilih **GitHub Actions** 
3. Atau pilih branch `main` dan folder `/ (root)`
4. Klik Save
5. Tunggu beberapa menit, blog Anda live di: `https://USERNAME.github.io/gorontalokita/`

### Langkah 4: (Opsional) Pasang Domain Kustom
1. Beli domain (misal: gorontalokita.com) — sekitar Rp 100-150rb/tahun
2. Di GitHub Pages settings, masukkan domain Anda
3. Di DNS domain, tambahkan:
   - CNAME record: `www` → `USERNAME.github.io`
   - A record: `@` → `185.199.108.153` (IP GitHub Pages)
4. Centang "Enforce HTTPS"

---

## ✍️ Cara Menulis Artikel Baru

Cukup buat file baru di folder `_posts/` dengan format:

**Nama file**: `YYYY-MM-DD-judul-artikel.md`

**Contoh**: `2026-04-01-wisata-baru-di-gorontalo.md`

**Template artikel**:
```markdown
---
title: "Judul Artikel Anda di Sini"
date: 2026-04-01
categories: [wisata]
tags: [Tag1, Tag2, Tag3]
author: Nama Penulis
excerpt: "Ringkasan singkat artikel yang akan muncul di halaman utama."
---

Paragraf pembuka artikel Anda di sini. Tulis dengan gaya yang menarik
dan informatif.

## Sub Judul

Konten artikel lanjutan...

> Ini adalah blockquote untuk tips atau kutipan penting.

- Item list 1
- Item list 2
- Item list 3

![Deskripsi gambar](/assets/img/nama-gambar.jpg)
```

### Kategori yang Tersedia
| Kategori | Kode | Warna |
|----------|------|-------|
| Wisata | `[wisata]` | Teal |
| Kuliner | `[kuliner]` | Coral |
| Budaya | `[budaya]` | Emas |
| Bisnis | `[bisnis]` | Biru |
| Info Lokal | `[info]` | Hijau |

### Menambah Gambar
1. Taruh gambar di folder `assets/img/`
2. Referensikan di artikel: `![alt text](/assets/img/foto.jpg)`
3. Untuk cover artikel, tambahkan di front matter:
   ```
   cover: /assets/img/cover-artikel.jpg
   ```

---

## 💰 Cara Monetisasi

### Google AdSense (bulan ke 4-6)
1. Pastikan blog sudah punya 30+ artikel berkualitas
2. Daftar di https://adsense.google.com
3. Setelah disetujui, buka `_layouts/default.html`
4. Ganti placeholder komentar AdSense dengan kode asli Anda

### Affiliate Marketing
- Daftar program affiliate Tokopedia/Shopee
- Sisipkan link affiliate di artikel review produk/tempat

### Sponsored Content
- Setelah traffic naik, tawarkan paket artikel sponsor ke bisnis lokal Gorontalo

---

## 📁 Struktur Folder

```
gorontalokita/
├── _config.yml          ← Pengaturan blog
├── _layouts/            ← Template halaman
│   ├── default.html     ← Layout utama
│   ├── post.html        ← Layout artikel
│   └── page.html        ← Layout halaman statis
├── _includes/           ← Komponen yang bisa dipakai ulang
│   ├── header.html
│   ├── footer.html
│   └── sidebar.html
├── _posts/              ← ARTIKEL BLOG (tulis di sini!)
│   ├── 2026-03-28-judul.md
│   └── ...
├── assets/
│   ├── css/style.css    ← Stylesheet utama
│   └── img/             ← Folder gambar (buat sendiri)
├── pages/               ← Halaman statis
│   └── tentang.md
├── index.html           ← Halaman utama
└── README.md            ← File ini
```

---

## 🎯 Target & Milestone

| Bulan | Target | Aksi |
|-------|--------|------|
| 1 | 30 artikel | Tulis 1-2 artikel/hari |
| 2 | 60 artikel | Mulai share di medsos |
| 3 | 90 artikel, 1000 visitor/bulan | Optimasi SEO |
| 4-6 | Daftar AdSense | Mulai monetisasi |
| 6+ | Scale ke portal berita | Tambah penulis freelance |

---

Dibuat dengan ❤️ dari Gorontalo
