KazuStore - Katalog Produk Premium (Modul 6 Pemrograman Web)

Aplikasi web katalog produk modern berbasis React dan Vite yang mengintegrasikan pengambilan data (data fetching) real-time dari REST API eksternal menggunakan Axios. Proyek ini dibuat untuk memenuhi tugas praktikum Modul 6 Pemrograman Web (ST084) Universitas Amikom Yogyakarta dengan nama proyek resmi axios-practice.

🚀 Cara Menjalankan Aplikasi

Ikuti langkah-langkah di bawah ini untuk menjalankan proyek ini di lingkungan lokal Anda:

Prasyarat

Pastikan komputer Anda sudah terinstal Node.js (versi 18 atau yang lebih baru direkomendasikan) dan npm.

Langkah Instalasi

Unduh atau Kloning Repositori:
Jika menggunakan Git, jalankan perintah berikut di terminal:

git clone <url-repository-anda>
cd axios-practice


Atau jika Anda mengunduh berkas ZIP, ekstrak terlebih dahulu lalu buka terminal di dalam folder axios-practice tersebut.

Instal Dependensi:
Pasang semua pustaka yang diperlukan (React, Vite, Axios) dengan menjalankan perintah:

npm install


Jalankan Server Pengembangan (Local Dev Server):
Mulai server lokal dengan perintah berikut:

npm run dev


Buka Aplikasi di Browser:
Setelah server berhasil berjalan, buka browser Anda dan akses tautan berikut:

http://localhost:3000


(Atau sesuaikan dengan port yang tampil pada terminal Anda, contohnya http://localhost:5173)

✨ Fitur-Fitur yang Diimplementasikan

Aplikasi KazuStore ini dilengkapi dengan berbagai fitur interaktif yang memenuhi seluruh komponen penilaian praktikum pada Modul 6:

GET Request dengan Axios & Sinkronisasi API:

Melakukan pengambilan data produk secara real-time dari Fake Store API (https://fakestoreapi.com/products).

Menggunakan concurrent request (Promise.all) untuk mengambil daftar produk dan kategori sekaligus saat komponen pertama kali dimuat (component did mount via useEffect).

Loading Indicator & State Management:

Menampilkan indikator animasi pemuatan (loading spinner) yang halus dan informatif selama proses pengambilan data berlangsung untuk menjaga kenyamanan pengalaman pengguna (UX).

Error Handling yang User-Friendly:

Menyediakan mekanisme penanganan kesalahan jika koneksi internet terputus atau API gagal diakses, lengkap dengan tombol "Coba Muat Ulang" untuk memicu pengambilan data kembali tanpa harus me-refresh seluruh halaman.

Category Filter Dinamis:

Mengimplementasikan penyaringan produk berdasarkan kategori yang datanya diambil langsung dari API secara dinamis. Mengubah kategori akan memicu request Axios baru sesuai endpoint kategori terpilih (https://fakestoreapi.com/products/category/{category}).

Sistem Pencarian Produk Real-Time:

Fitur pencarian interaktif yang menyaring produk berdasarkan kecocokan judul (title) secara langsung saat pengguna mengetik pada kolom pencarian.

Filter Lanjutan (Harga & Rating):

Slider Harga Maksimal: Membatasi tampilan produk berdasarkan budget maksimal secara dinamis.

Penyaring Rating Minimal: Memfilter produk berdasarkan batas minimal rating bintang (1-5 bintang).

Sistem Keranjang Belanja (Simulasi):

Menambah produk ke keranjang, menambah/mengurangi kuantitas produk, menghapus item tertentu, serta mengosongkan seluruh isi keranjang belanja.

Menghitung subtotal belanjaan secara otomatis dan real-time.

Modal Detail Produk & Notifikasi Toast:

Menyediakan jendela pop-up (Modal) untuk melihat detail info deskripsi lengkap produk secara mendalam ketika salah satu kartu produk diklik.

Dilengkapi sistem notifikasi instan (Toast) berdurasi 3 detik yang muncul setiap kali pengguna sukses menambahkan atau menghapus produk dari keranjang belanja.

🛠️ Teknologi yang Digunakan

Framework / Bundler: React (v18) + Vite

HTTP Client: Axios

Styling Framework: Tailwind CSS
