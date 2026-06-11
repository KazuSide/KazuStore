# 🛒 KazuStore (axios-practice)

KazuStore adalah aplikasi katalog produk e-commerce modern berbasis React dan Vite yang mengintegrasikan pengambilan data (data fetching) secara asinkron dari REST API eksternal menggunakan Axios. Proyek ini dibangun untuk memenuhi kriteria penugasan Tugas 6 Praktikum Pemrograman Web (ST084) Universitas Amikom Yogyakarta dengan nama direktori resmi axios-practice.

# 📸 Tampilan Aplikasi

<img width="975" height="493" alt="image" src="https://github.com/user-attachments/assets/b7d5c38a-1079-4e2a-ac41-d313a24f5f14" />


# ✨ Fitur-Fitur Utama yang Diimplementasikan

Aplikasi ini memenuhi seluruh rubrik penilaian dengan skor maksimal melalui implementasi fitur berikut:

GET Request dengan Axios & Sinkronisasi API (Bobot 15%):

Berhasil memuat dan menyajikan total 20 produk secara dinamis langsung dari Fake Store API (https://fakestoreapi.com/products).

Pengambilan data awal dioptimalkan menggunakan teknik concurrent request via Promise.all di dalam hook useEffect.

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

# Fitur Tambahan (Terimplementasi 4 Fitur - Syarat Minimal 2 Fitur) (Bobot 10%):

🛒 Simulasi Add to Cart & Toast Notification: Pengguna dapat menambahkan barang ke laci belanja (cart drawer), memperbarui jumlah kuantitas, menghapus item, melihat akumulasi subtotal secara real-time, serta memicu munculnya animasi notifikasi Toast selama 3 detik.

🔽 Sorting System: Pengurutan produk berdasarkan harga terendah ke tertinggi, harga tertinggi ke terendah, dan ulasan/rating terbaik.

🎚️ Price Range Slider Filter: Filter rentang harga maksimal yang dinamis memudahkan pembatasan katalog produk sesuai anggaran belanja.

⭐ Rating Filter: Filter interaktif untuk membatasi tampilan produk berdasarkan standar rating bintang minimal (1 hingga 5 bintang).


# 👨‍💻 Identitas Mahasiswa

Nama : RAFAEL REGA PURNOMO AJI

NIM  : 24.11.6103

Kelas : IF 03

Mata Kuliah : Pemrograman Web

Instansi : Universitas AMIKOM Yogyakarta
