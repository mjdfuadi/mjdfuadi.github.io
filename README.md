# mjdfuadi.github.io
Portofolio Studi Kasus: Yayasan Tausiyah Harian Indonesia

Ini adalah berkas README.md untuk proyek website portofolio studi kasus "Yayasan Tausiyah Harian Indonesia". Website ini dirancang sebagai portofolio multi-halaman untuk memamerkan proses desain dan pengembangan.

Ringkasan Proyek

Website ini adalah portofolio online yang mendokumentasikan proses pembuatan ulang (desain dan pengembangan) website untuk Yayasan Tausiyah Harian Indonesia, serta menampilkan proyek-proyek lainnya.

Teknologi yang Digunakan

Proyek ini dibuat sebagai serangkaian berkas HTML mandiri untuk portabilitas maksimum dan kemudahan pratinjau.

HTML5: Untuk struktur semantik konten.

Tailwind CSS (via CDN): Untuk seluruh styling dan layout responsif. Konfigurasi kustom disematkan langsung di dalam tag <script> di <head>.

JavaScript (Vanilla): Untuk fungsionalitas interaktif, termasuk:

Animasi "Reveal on Scroll" menggunakan IntersectionObserver (di tausiyahharian.html).

Tombol "Back to Top" (di tausiyahharian.html).

Struktur Berkas

Proyek ini sekarang terdiri dari beberapa berkas HTML:

/
├── index.html           (Halaman utama pemilihan proyek)
├── tausiyahharian.html  (Studi kasus website)
└── tausiyahplus.html    (Studi kasus mobile app - placeholder)


Semua CSS kustom, konfigurasi Tailwind, dan JavaScript sudah termasuk di dalam berkas HTML masing-masing.

Kustomisasi

Berikut adalah cara untuk mengkustomisasi atau memperbarui portofolio ini:

1. Mengubah Palet Warna

Anda dapat dengan mudah mengubah skema warna utama (#0863da, #35a7e9, #f7ffff) langsung di dalam konfigurasi Tailwind di <head> pada setiap berkas HTML.

<script>
    tailwind.config = {
        theme: {
            extend: {
                colors: {
                    'brand-primary': '#0863da',   // Ganti warna ini
                    'brand-secondary': '#35a7e9', // Ganti warna ini
                    'brand-bg': '#f7ffff',       // Ganti warna ini
                    'brand-accent': '#35a7e9',    
                }
            }
        }
    }
</script>


2. Mengganti Gambar Placeholder

Di berkas tausiyahharian.html, semua gambar menggunakan layanan placehold.co. Untuk menggantinya dengan gambar Anda, cari tag <img> dan ganti atribut src="".

Contoh:

<!-- SEBELUM -->
<img src="[https://placehold.co/1024x640/f7ffff/333?text=Tampilan+Website+Desktop](https://placehold.co/1024x640/f7ffff/333?text=Tampilan+Website+Desktop)" 
     alt="Tampilan website Tausiyah Harian di laptop" 
     class="rounded-lg shadow-2xl w-full">

<!-- SESUDAH (Contoh) -->
<img src="./assets/gambar-desktop-anda.jpg" 
     alt="Tampilan website Tausiyah Harian di laptop" 
     class="rounded-lg shadow-2xl w-full">


3. Memperbarui Tautan Sosial Media

Tautan sosial media ada di bagian <footer> pada setiap berkas HTML. Cari bagian "Want to work with me?" dan perbarui atribut href="".

Contoh untuk LinkedIn:

<!-- Ganti '#' dengan URL LinkedIn Anda -->
<a href="#" title="LinkedIn" class="...">
    <svg>...</svg>
</a>


Contoh untuk WhatsApp:

<!-- Ganti '6281234567890' dengan nomor Anda -->
<a href="[https://wa.me/6281234567890](https://wa.me/6281234567890)" title="WhatsApp" ...>
    <svg>...</svg>
</a>


4. Memperbarui Teks

Semua konten teks dapat diubah langsung di dalam berkas HTML yang relevan.
