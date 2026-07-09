# Generator Website PPI Cabang

Aplikasi pembuat website statis responsif satu halaman untuk PPI Cabang di Jerman secara instan tanpa perlu coding.

## Fitur Utama

- **Penyunting Visual & Pratinjau Langsung**: Edit konten dan langsung lihat hasilnya di panel pratinjau (mendukung mode Desktop & Ponsel).
- **Struktur Halaman Dinamis**: Aktifkan, nonaktifkan, dan ubah urutan bagian sesuka Anda (Hero, Galeri, Tentang Kami, Sejarah, Visi Misi, Pengurus, Sosial Media, & Tautan Lain).
- **Multi-bahasa**: Mendukung Bahasa Indonesia (utama), Inggris, dan Jerman secara bersamaan dengan tombol pengalih bahasa otomatis.
- **Kustomisasi Tampilan**: Pilih kombinasi warna primer & aksen, jenis huruf (Plus Jakarta Sans, Inter, Poppins, dll.), atau ekstrak warna secara otomatis dari logo yang Anda unggah.
- **Halaman Impressum Otomatis**: Memenuhi regulasi hukum Jerman (§ 5 DDG) dengan opsi pembuatan halaman `impressum.html` yang terhubung ke badan hukum induk.
- **Integrasi Decap CMS**: Opsi menyertakan CMS berbasis Git agar pengurus cabang berikutnya bisa mengedit konten langsung tanpa menyentuh kode program.
- **Tanpa Database / Server**: Seluruh konfigurasi disimpan di browser Anda (`localStorage`) dan diunduh dalam format ZIP yang siap dideploy langsung ke hosting statis (GitHub Pages, Cloudflare Pages, Netlify, dll.).

## Cara Menggunakan

1. **Jalankan Aplikasi**: Cukup buka file `index.html` di browser Anda (atau jalankan server lokal sederhana).
2. **Isi Informasi Cabang**: Masukkan nama cabang, kota, kontak, logo, serta favicon.
3. **Pilih Bagian & Konten**: Masukkan teks visi-misi, daftar pengurus, galeri foto, dan tautan sosial media.
4. **Unduh ZIP**: Klik tombol **Unduh ZIP Website** di bagian bawah.
5. **Hosting**: Ekstrak berkas ZIP tersebut lalu unggah filenya ke penyedia hosting statis pilihan Anda.

## Struktur File Hasil Unduhan

Berkas ZIP yang dihasilkan berisi berkas mandiri dengan struktur berikut:

```text
├── index.html          # Halaman utama website Anda
├── impressum.html      # Halaman Impressum (jika diaktifkan)
├── README.md           # Panduan penggunaan dan hosting website hasil generate
├── content/
│   └── site.json       # Seluruh data konten & konfigurasi website
├── assets/             # Direktori logo dan favicon
└── admin/              # Berkas konfigurasi Decap CMS (jika diaktifkan)
```

## Pengembangan & Kontribusi

Proyek ini dibangun menggunakan HTML, CSS (Vanilla), dan JavaScript tanpa framework eksternal untuk memastikan kecepatan muat yang maksimal dan kesederhanaan pemeliharaan.

### Cara Menjalankan Secara Lokal untuk Pengembangan

Jika Anda ingin melakukan pengembangan atau modifikasi pada generator ini:

1. Clone repositori ini:
   ```bash
   git clone https://github.com/unbopsingsegalanya/webgenppij.git
   ```
2. Jalankan server lokal menggunakan Python atau perkakas lain:
   ```bash
   python3 -m http.server 8000
   ```
3. Buka `http://localhost:8000` di peramban Anda.

## Penafian (Disclaimer)

Proyek ini dikembangkan secara **independen** dan **tidak memiliki hubungan afiliasi resmi** dengan **PPI Jerman (PPIJ)**. Seluruh tanggung jawab atas konten, hukum (termasuk kepatuhan Impressum), dan pengelolaan website hasil generator ini berada sepenuhnya pada masing-masing pengurus PPI Cabang yang menggunakannya.

