# Generator Susunan Ibadah GMAHK Sepanjang 🌿

Aplikasi berbasis web (*Single Page Application*) yang elegan, interaktif, dan responsif. Digunakan untuk menghasilkan (*men-generate*) susunan acara ibadah secara cepat dan seragam, lalu menyalin format akhirnya secara otomatis ke *Clipboard* agar siap di-*Paste* ke aplikasi WhatsApp / Media Sosial Jemaat.

**Versi App:** v1.6.0

## Apa yang baru di v1.6.0 🎉
- **Aksi Hapus Data Admin:** Penambahan tombol **Hapus** pada baris tabel admin dengan konfirmasi *SweetAlert2* untuk menghapus data langsung dari database Supabase secara aman.
- **Majukan & Mundurkan Jadwal:** Tombol baru **"Majukan 1 Minggu"** dan **"Mundurkan 1 Minggu"** untuk menggeser tanggal seluruh jadwal di tabel aktif secara massal (paralel) dengan sekali klik.
- **Tampilan Tabel Full-Screen & Responsif:** Halaman dashboard admin kini otomatis melebar hingga **95%** layar dan sel tabel diatur melipat teks secara rapi (*word-wrap*) untuk mengeliminasi scrollbar horizontal pada desktop.
- **Refactoring Komentar Kode:** Pembersihan dan pembaruan seluruh komentar di dalam kode sumber (`index.html`, `style.css`, `script.js`) agar lebih akurat menerangkan alur logika, penanganan zona waktu, dan integrasi kolom database Supabase.

## Fitur Inti
- **Dashboard Admin Aman & Interaktif:** Panel manajemen data di dalam aplikasi untuk mempermudah edit data, dilindungi oleh autentikasi login terenkripsi berbasis ekosistem *Supabase Auth & Row Level Security* (RLS), serta ditenagai interaksi pop-up mulus dari *SweetAlert2*. Tabel PA dan Sabat Raya terintegrasi penuh ke dalam *Manager* Dasbor.
- **Integrasi Ekosistem Multi-Tab & Rapat Virtual:** Form Ibadah dipecah dalam tab-tab fungsional (Sabat Raya, Pemuda Advent, dan Rabu Malam) tanpa proses *reload* antarklik, lengkap dengan template undangan rapat Zoom otomatis yang ditenagai tautan & ID Zoom terbaru.
- **Integrasi Database Serverless (Supabase):** Ditenagai database *real-time* dengan fitur *Auto-Fill* cerdas. Jadwal Sabat (termasuk kelengkapan petugas *Soundman*) dan Jadwal PA terdekat akan terisi secara otomatis, memotong waktu input manual hingga 90%.
- **Smart Song Autocomplete & Nyanyian Sambutan:** Pencarian judul lagu Sion (LSEL) dan lagu Pemuda Advent (AYS) yang cerdas dan cepat dari *database* (cukup ketik 3 huruf) dengan *dropdown list* rekomendasi, serta penempatan otomatis lagu sambutan tetap (LSEL No. 523) setelah Doa Tutup dan Doa Berkat Sabat Raya.
- **Logika Validasi & Deteksi Otomatis Pintar:** Kalkulasi otomatis untuk penentuan angka "Sabat Ke" dan rentang "Triwulan" sesuai kalender berjalan, serta normalisasi penulisan nama petugas (fuzzy match untuk "Sdr" vs "Sdra.") untuk mencegah jabatan eksklusif ganda secara transparan.
- **Otomatisasi Doa Syafaat Rabu Malam:** Pengisian otomatis kolom Doa Syafaat untuk ibadah Rabu Malam dengan nama default ("Pdt. Benny Lumbantobing") yang ditempatkan secara tepat sebelum bagian Pujian.
- **Live Preview & 1-Click Copy WA:** Teks *WhatsApp* pratinjau seketika terbangun bersamaan dengan input ketikan (bebas spasi ganda untuk kenyamanan visual), siap disalin dalam sekali klik (dilengkapi notifikasi aksi).
- **Desain Responsif, Fleksibel, & Estetis:** Estetika UI modern berwarna *Maroon* elegan (mendukung *Dark/Light mode* permanen) yang otomatis menyesuaikan visual peranti ponsel, tablet, atau laptop. Navigasi tab didesain menggunakan tata letak flex agar meregang secara proporsional.
- **Refactoring & Struktur Bersih:** Kode HTML, CSS, dan JavaScript telah di-refactor secara rapi dengan pengelompokan yang jelas, penggunaan kelas utilitas CSS (seperti `.btn-success`), serta dokumentasi logika aplikasi yang sangat mendetail.

## Cara Penggunaan
1. Buka Tautan [Susunan Ibadah GMAHK Sepanjang](https://meakhelg.github.io/Susunan-Ibadah-GMAHK-Sepanjang/)
2. Tunggu 1 hingga 2 detik untuk inisialisasi Database Data Serverless **Supabase**. *Voila!* Anda akan mendapati jadwal otomatis tertarik ke form-form kosong Anda.
3. Ketik dan poles sedikit kekosongan sisa yang belum terakomodasi di sistem untuk melengkapi alur peribadatan hari itu.
4. Klik tombol "Salin ke Clipboard", buka Whatsapp jemaat, dan tekan CTRL+V (*Paste*). 

---

## 🛠 Dikembangkan Oleh
**Meakhel Gunawan**  
&copy; 2026 - Semua Hak Cipta Dilindungi (All rights reserved).


## 🚀 Roadmap (Rencana Fitur Mendatang)
Aplikasi ini direncanakan akan terus berekspansi ke depannya untuk menampung seluruh alur peribadatan jemaat:
- [x] Susunan Ibadah PA (Pemuda Advent) - *Selesai di v1.1.0*
- [x] Susunan Ibadah Rabu Malam - *Selesai di v1.2.0*
- [x] Transformasi Serverless via Integrasi Supabase - *Selesai di v1.3.0*
- [x] Secured Admin Dashboard & Authentication - *Selesai di v1.4.0*
- [ ] Susunan Jadwal Vesper / Buka Sabat

*Note: Mengingat fondasi database solid berteknologi pintar sudah diletakkan, ekspansi otomatisasi untuk jadwal-jadwal baru di gereja kini adalah hal yang sangat mudah direalisasikan!*