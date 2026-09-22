# Praktikum Pemrograman Mobile - Aplikasi Jualan

Aplikasi **Jualan** adalah platform berbasis **Android (Jetpack Compose / Kotlin)** yang dirancang untuk mempromosikan dan memadahi produk-produk lokal UMKM di wilayah Kabupaten Purbalingga, Jawa Tengah.

---

## 👤 Data Diri

| Informasi | Detail |
| :--- | :--- |
| **Nama** | Zahwa Nafiza Azzahra |
| **NIM** | H1D024015 |
| **Shift KRS** | H |
| **Shift Sekarang** | F |

---

## 📱 Fitur dan Halaman Aplikasi

### 1. Halaman Tentang Jualan (`BasicInfoScreen`)
* **Logo Aplikasi**: Menampilkan logo resmi platform Jualan.
* **Informasi & Misi**: Card deskripsi profil aplikasi dan komitmen memajukan UMKM lokal Purbalingga.
* **Navigasi**: Tombol *"Hubungi Kami"* untuk berpindah ke halaman formulir kontak.

### 2. Halaman Hubungi Kami (`HubungiKamiScreen`)
* **Top App Bar**: Dilengkapi tombol *Back* untuk kembali ke halaman utama.
* **Formulir Kontak**: Field input Email dan Pesan menggunakan `OutlinedTextField`.
* **Kirim Pesan & Feedback**: Tombol kirim interaktif yang memicu tampilan notifikasi **Snackbar** (*"Pesan Terkirim"*).

### 3. Halaman Daftar Produk UMKM (`DaftarProductScreen`) — *Tugas Pertemuan 2*
* **Filter Kategori (`LazyRow`)**: Menampilkan daftar kategori interaktif (*Makanan*, *Minuman*, *Kerajinan*) untuk memfilter produk secara real-time.
* **Grid Produk (`LazyVerticalGrid`)**: Layout grid 2 kolom menampilkan `ProductItemCard` berisi gambar, badge kategori, nama produk, dan harga.
* **Event Handling (Toast)**: Klik pada kartu produk memunculkan notifikasi **Toast** sesuai produk yang dipilih (contoh: *"Clicked: Sandal Bandol"*).
* **Dukungan Dual Theme**: Antarmuka mendukung tampilan **Light Theme** maupun **Dark Theme** secara responsif dan konsisten.
* **Modular Preview**: Preview komponen terpisah (`ProductItemCard`, `CategoryItem`) serta preview layar penuh untuk tema terang dan gelap.

---

## 📸 Hasil Implementasi (Screenshot)

### 📌 Pertemuan 1: Layar Informasi & Formulir Kontak

| 1. Halaman Tentang Jualan | 2. Halaman Hubungi Kami |
| :---: | :---: |
| <img src="img/tentang_jualan.png" width="280" alt="Tentang Jualan" /> | <img src="img/hubungi_kami.png" width="280" alt="Hubungi Kami" /> |

---

### 📌 Pertemuan 2: Daftar Produk UMKM (Light Mode)

| Filter Makanan | Filter Minuman | Filter Kerajinan | Interaksi Click (Toast) |
| :---: | :---: | :---: | :---: |
| <img src="img/daftar_produk_makanan.png" width="220" alt="Filter Makanan" /> | <img src="img/daftar_produk_minuman.png" width="220" alt="Filter Minuman" /> | <img src="img/daftar_produk_kerajinan.png" width="220" alt="Filter Kerajinan" /> | <img src="img/daftar_produk_toast.png" width="220" alt="Toast Sandal Bandol" /> |

---

### 📌 Pertemuan 2: Daftar Produk UMKM (Dark Mode)

| Filter Makanan (Dark) | Filter Minuman (Dark) | Filter Kerajinan (Dark) | Interaksi Click (Dark) |
| :---: | :---: | :---: | :---: |
| <img src="img/dark_makanan.png" width="220" alt="Dark Makanan" /> | <img src="img/dark_minuman.png" width="220" alt="Dark Minuman" /> | <img src="img/dark_kerajinan.png" width="220" alt="Dark Kerajinan" /> | <img src="img/dark_toast.png" width="220" alt="Dark Toast" /> |

---

### 📌 Component & Layout Preview

| Preview `ProductItemCard` | Preview `CategoryItem` |
| :---: | :---: |
| <img src="img/preview_product_card.png" width="250" alt="Preview ProductItemCard" /> | <img src="img/preview_category_item.png" width="250" alt="Preview CategoryItem" /> |

---

## 🛠️ Teknologi & Komponen yang Digunakan

* **Bahasa**: Kotlin
* **UI Framework**: Jetpack Compose (Material3)
* **Navigasi**: Jetpack Navigation Compose
* **Komponen Compose**: `Scaffold`, `TopAppBar`, `LazyRow`, `LazyVerticalGrid`, `Card`, `OutlinedTextField`, `Toast`, `Snackbar`