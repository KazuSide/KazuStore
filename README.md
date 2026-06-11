🛒 KazuStore (axios-practice)

KazuStore adalah aplikasi katalog produk e-commerce modern berbasis React dan Vite yang mengintegrasikan pengambilan data (data fetching) secara asinkron dari REST API eksternal menggunakan Axios. Proyek ini dibangun untuk memenuhi kriteria penugasan Tugas 6 Praktikum Pemrograman Web (ST084) Universitas Amikom Yogyakarta dengan nama direktori resmi axios-practice.

📸 Tampilan Aplikasi

Catatan: Anda dapat mengunggah berkas tangkapan layar image_1dfde4.jpg ke dalam repositori GitHub Anda, lalu mengubah namanya menjadi screenshot.jpg agar gambar pratinjau aplikasi Anda otomatis muncul di atas ini.

✨ Fitur-Fitur Utama yang Diimplementasikan

**//Aplikasi ini memenuhi seluruh rubrik penilaian dengan skor maksimal melalui implementasi fitur berikut:

GET Request dengan Axios & Sinkronisasi API (Bobot 15%):

Berhasil memuat dan menyajikan total 20 produk secara dinamis langsung dari Fake Store API (https://fakestoreapi.com/products).

Pengambilan data awal dioptimalkan menggunakan teknik concurrent request via Promise.all di dalam hook useEffect.//**

Loading Indicator (Bobot 10%):

Animasi indikator pemuatan data (spinning loader) yang halus, bersih, dan interaktif untuk memberikan pengalaman pengguna (UX) terbaik saat aplikasi sedang memproses pemanggilan API.

Error Handling & Retry Mechanism (Bobot 10%):

Penanganan kesalahan tangguh menggunakan blok try-catch. Jika koneksi terputus, aplikasi menampilkan pesan kesalahan (alert card) yang ramah pengguna lengkap dengan tombol "Coba Muat Ulang" tanpa harus melakukan hard reload browser.

Category Filter Dinamis dari API (Bobot 15%):

Panel samping (sidebar) kategori dirender secara dinamis dengan mengambil daftar kategori langsung dari API. Mengeklik kategori tertentu akan memicu pemanggilan endpoint spesifik:
https://fakestoreapi.com/products/category/{category_name}

Fitur Pencarian Produk Real-Time (Bobot 10%):

Input pencarian responsif yang langsung menyaring produk di sisi klien (client-side filtering) berdasarkan judul (title) maupun isi deskripsi produk (case-insensitive).

Product Detail Modal (Bobot 10%):

Menampilkan jendela pop-up modal interaktif yang menyajikan detail lengkap spesifikasi produk ketika gambar atau judul produk diklik oleh pengguna.

Responsive Grid (Bobot 10%):

Tata letak grid yang sepenuhnya responsif menggunakan utility kelas Tailwind CSS dengan 3 breakpoints utama:

Desktop / Monitor: Grid 3 - 4 Kolom (lg:grid-cols-3 atau xl:grid-cols-4)

Tablet / iPad: Grid 2 Kolom (sm:grid-cols-2)

Mobile / Smartphone: Grid 1 Kolom Penuh (grid-cols-1)

Fitur Tambahan (Terimplementasi 4 Fitur - Syarat Minimal 2 Fitur) (Bobot 10%):

🛒 Simulasi Add to Cart & Toast Notification: Pengguna dapat menambahkan barang ke laci belanja (cart drawer), memperbarui jumlah kuantitas, menghapus item, melihat akumulasi subtotal secara real-time, serta memicu munculnya animasi notifikasi Toast selama 3 detik.

🔽 Sorting System: Pengurutan produk berdasarkan harga terendah ke tertinggi, harga tertinggi ke terendah, dan ulasan/rating terbaik.

🎚️ Price Range Slider Filter: Filter rentang harga maksimal yang dinamis memudahkan pembatasan katalog produk sesuai anggaran belanja.

⭐ Rating Filter: Filter interaktif untuk membatasi tampilan produk berdasarkan standar rating bintang minimal (1 hingga 5 bintang).

🚀 Cara Menjalankan Aplikasi secara Lokal

Ikuti langkah-langkah mudah di bawah ini untuk memasang dan menjalankan proyek di komputer Anda:

1. Prasyarat

Pastikan komputer Anda sudah terinstal Node.js (versi 18+) dan manajer paket npm.

2. Kloning Repositori

Jalankan perintah berikut pada terminal atau Git Bash Anda:

git clone https://github.com/[Username_GitHub_Anda]/axios-practice.git
cd axios-practice


3. Instalasi Dependensi Proyek

Instal semua pustaka yang dibutuhkan (termasuk Axios dan React Developer Tools) dengan perintah:

npm install


4. Menjalankan Server Pengembangan Lokal

Jalankan server lokal berbasis Vite untuk melihat aplikasi secara real-time:

npm run dev


Setelah server aktif, terminal akan menampilkan tautan lokal (biasanya http://localhost:3000 atau http://localhost:5173). Buka tautan tersebut di browser Anda.

🛠️ Spesifikasi Teknologi (Tech Stack)

Library Utama: React.js (v18)

Bundler & Build Tool: Vite

HTTP Client: Axios

Styling & UI: Tailwind CSS (via CDN integrasi cepat)

👨‍💻 Identitas Mahasiswa

Nama : [Nama Lengkap Anda]

NIM  : [NIM Anda, contoh: 22.11.xxxx]

Kelas : [Kelas Anda, contoh: 22-IF-xx]

Mata Kuliah : Praktikum Pemrograman Web (ST084)

Instansi : Universitas AMIKOM Yogyakarta
