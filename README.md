# PERIODT — Website Merchandise Custom

Website untuk **PERIODT**, brand merchandise custom handmade asal Jakarta (tote bag, tumbler, sticker, keychain, pin, dan t-shirt custom).

## Struktur Halaman

| File | Fungsi |
|---|---|
| `index.html` | Halaman utama / toko — katalog produk, filter kategori, video behind-the-scenes, dan bagian about |
| `personal-work.html` | Galeri portofolio — koleksi hasil kerja, carousel "archives", dan bagian about |

## Fitur Utama

**index.html (Toko)**
- Marquee berjalan di atas (pengumuman promo)
- Hero section dengan judul brand & CTA (Shop Now / Customize Yours)
- Filter kategori produk (All, Tote Bag, Tumbler, Sticker, Keychain, PIN, Custom) — filtering dilakukan dengan JavaScript, tanpa reload halaman
- Grid produk dengan badge (New, Bestseller, Sold Out), harga, dan tombol order langsung ke WhatsApp
- Showcase carousel hasil kerja (auto-scroll)
- Video section dengan player custom (play/pause, mute, progress bar)
- About section dengan foto, hover-reveal image, dan social media links (Instagram, TikTok, WhatsApp)
- Custom cursor berbentuk hati

**personal-work.html (Galeri)**
- Hero judul "Personal Work"
- Galeri 3 kolom dengan efek parallax scroll (kecepatan tiap kolom berbeda)
- Marquee divider di tengah halaman
- Section "Archives" bergaya catatan robek (notepad) + carousel foto proses kerja (dengan auto-slide, dot navigation, swipe di mobile)
- About section (sama seperti index.html)

## Teknologi

- **HTML5 + CSS3** murni (tanpa framework)
- **Vanilla JavaScript** untuk semua interaktivitas (filter, carousel, video player, parallax, animasi scroll)
- Font: Google Fonts — `Instrument Serif`, `DM Sans`, `Caveat`, `Playfair Display`
- Font custom: `Socafe` (di-load dari folder `assets/`)

## Kebutuhan Folder `assets/`

Semua gambar, video, dan logo di-refer dari folder `assets/` yang harus berada satu level dengan file HTML, contoh:
```
/assets/logo design.png
/assets/logoo.png
/assets/TOTE.png, STIKER.png, TUMBLER.png, KEYCHAIN.png, PIN.png, T-SHIRT.png
/assets/PIDIO.MOV, cushion.webp
/assets/Bag.jpg, t-shirt.jpg, tumbler.jpg, keychain.jpg, stickers.jpg, dst.
```
Jika ada gambar yang hilang, beberapa elemen (foto About) punya fallback emoji lewat `onerror`.

## Kontak Order

Semua tombol "Order" mengarah ke WhatsApp: `https://wa.me/6281292526073`

## Responsif

Sudah ada media query untuk breakpoint `900px` dan `520px` (tablet & mobile) — nav disembunyikan di layar kecil, grid produk & galeri menyesuaikan jumlah kolom.

## Catatan Pengembangan

- Belum ada backend/database — semua data produk dan galeri masih hardcode di HTML
- Filter produk & carousel hanya jalan dengan JavaScript aktif (tidak ada fallback no-JS)
- Custom cursor menyembunyikan cursor asli browser (`cursor: none !important`) — pastikan ini disengaja untuk semua perangkat
