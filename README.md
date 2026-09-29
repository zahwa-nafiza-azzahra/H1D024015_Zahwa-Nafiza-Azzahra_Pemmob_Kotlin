# Praktikum Pemrograman Mobile - Aplikasi Jualan

Aplikasi **Jualan** adalah platform berbasis **Android (Jetpack Compose / Kotlin)** yang dirancang untuk mempromosikan dan memfasilitasi produk-produk lokal UMKM di wilayah Kabupaten Purbalingga, Jawa Tengah.

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

### 1. Halaman Tentang Jualan (`BasicInfoScreen`) — *Pertemuan 1*
* **Logo Aplikasi**: Menampilkan logo resmi platform Jualan.
* **Informasi & Misi**: Card deskripsi profil aplikasi dan komitmen memajukan UMKM lokal Purbalingga.
* **Navigasi**: Tombol *"Hubungi Kami"* untuk berpindah ke halaman formulir kontak.

### 2. Halaman Hubungi Kami (`HubungiKamiScreen`) — *Pertemuan 1 & Pertemuan 4 (State Hoisting & Form Validation)*
* **Top App Bar**: Dilengkapi tombol *Back* untuk kembali ke halaman utama.
* **Formulir Kontak Interaktif**: Input Email dengan validasi format email secara real-time.
* **Dropdown Tipe Pesan (`ExposedDropdownMenuBox`)**: Pilihan kategori pesan (*Pertanyaan*, *Keluhan*, *Saran*).
* **Validasi Pesan**: Field pesan dengan batasan minimal 10 karakter.
* **Upload Bukti (Photo Picker)**: Integrasi `PickVisualMedia` launcher untuk mengunggah screenshot/foto bukti.
* **Syarat & Ketentuan**: Checkbox persetujuan yang mengontrol keaktifan tombol submit.
* **Kirim Pesan & Feedback (Snackbar)**: State enablement tombol Submit jika seluruh form valid, serta notifikasi **Snackbar** (*"Pesan Terkirim!"*).

### 3. Halaman Daftar Produk UMKM (`DaftarProductScreen`) — *Pertemuan 2 & Pertemuan 4 (Recomposition & Search State)*
* **Pencarian Real-Time (`OutlinedTextField`)**: Fitur pencarian nama produk yang responsif memperbarui tampilan list secara real-time.
* **Filter Kategori (`LazyRow`)**: Menampilkan daftar kategori interaktif (*Makanan*, *Minuman*, *Kerajinan*) untuk memfilter produk secara instan.
* **Grid Produk (`LazyVerticalGrid`)**: Layout grid 2 kolom menampilkan `ProductItemCard` berisi gambar, badge kategori, nama produk, dan harga.
* **TopAppBar Overflow Menu**: Dropdown menu ikon titik tiga pada bagian kanan atas untuk navigasi cepat ke layar *Hubungi Kami*.
* **Dukungan Dual Theme**: Antarmuka mendukung tampilan **Light Theme** maupun **Dark Theme** secara responsif dan konsisten.

### 4. Halaman Detail Produk (`DetailProductScreen`) — *Pertemuan 4 (State & UI Lifecycle)*
* **UI Lifecycle Handling (`LaunchedEffect`)**: Simulasi pemuatan data produk (*loading delay*) dengan indikator `CircularProgressIndicator`.
* **State Management (`rememberSaveable`)**: Counter jumlah pembelian (tombol `+` / `-`) yang menjaga nilai state saat terjadi rotasi layar atau rekomposisi.
* **Informasi Produk Lengkap**: Menampilkan gambar produk, nama, harga, deskripsi, dan sisa stok.
* **Tombol Tambah ke Keranjang**: Interaksi `Button` dengan notifikasi Toast confirmation jumlah item yang dibeli.

---

## 📸 Hasil Implementasi (Screenshot)

### 📌 Pertemuan 1: Layar Informasi & Formulir Kontak Basic

| 1. Halaman Tentang Jualan | 2. Halaman Hubungi Kami |
| :---: | :---: |
| <img src="img/tentang_jualan.png" width="280" alt="Tentang Jualan" /> | <img src="img/hubungi_kami.png" width="280" alt="Hubungi Kami" /> |

---

### 📌 Pertemuan 2: Daftar Produk UMKM

#### Light Mode
| Filter Makanan | Filter Minuman | Filter Kerajinan | Interaksi Click (Toast) |
| :---: | :---: | :---: | :---: |
| <img src="img/daftar_produk_makanan.png" width="220" alt="Filter Makanan" /> | <img src="img/daftar_produk_minuman.png" width="220" alt="Filter Minuman" /> | <img src="img/daftar_produk_kerajinan.png" width="220" alt="Filter Kerajinan" /> | <img src="img/daftar_produk_toast.png" width="220" alt="Toast Sandal Bandol" /> |

#### Dark Mode
| Filter Makanan (Dark) | Filter Minuman (Dark) | Filter Kerajinan (Dark) | Interaksi Click (Dark) |
| :---: | :---: | :---: | :---: |
| <img src="img/dark_makanan.png" width="220" alt="Dark Makanan" /> | <img src="img/dark_minuman.png" width="220" alt="Dark Minuman" /> | <img src="img/dark_kerajinan.png" width="220" alt="Dark Kerajinan" /> | <img src="img/dark_toast.png" width="220" alt="Dark Toast" /> |

---

### 📌 Pertemuan 4: Recomposition, State Management & UI Lifecycle

#### 1. Navigasi Overflow & Detail Produk
| TopAppBar Overflow Menu | Halaman Detail Produk (Counter & State) |
| :---: | :---: |
| <img src="img/p4_navigasi_overflow.png" width="260" alt="Overflow Menu" /> | <img src="img/p4_detail_produk.png" width="260" alt="Detail Produk" /> |

#### 2. Formulir Hubungi Kami Interaktif (State Hoisting & Form Validation)
| Validasi Error Format Email | Form Valid & Siap Kirim | Feedback Kirim Pesan (Snackbar) |
| :---: | :---: | :---: |
| <img src="img/p4_form_validation_error.png" width="250" alt="Validasi Email Error" /> | <img src="img/p4_form_interaktif.png" width="250" alt="Form Valid" /> | <img src="img/p4_form_snackbar.png" width="250" alt="Snackbar Feedback" /> |

#### 3. Pencarian Produk Real-Time (Light Mode)
| Search Makanan ("kri") | Search Minuman ("k") | Search Kerajinan ("b") |
| :---: | :---: | :---: |
| <img src="img/p4_search_makanan.png" width="240" alt="Search Makanan" /> | <img src="img/p4_search_minuman.png" width="240" alt="Search Minuman" /> | <img src="img/p4_search_kerajinan.png" width="240" alt="Search Kerajinan" /> |

#### 4. Filter Kategori Produk Pertemuan 4 (Light Mode)
| Kategori Makanan | Kategori Minuman | Kategori Kerajinan |
| :---: | :---: | :---: |
| <img src="img/p4_filter_makanan.png" width="240" alt="Filter Makanan P4" /> | <img src="img/p4_filter_minuman.png" width="240" alt="Filter Minuman P4" /> | <img src="img/p4_filter_kerajinan.png" width="240" alt="Filter Kerajinan P4" /> |

#### 5. Filter Kategori Produk Pertemuan 4 (Dark Mode)
| Kategori Makanan (Dark) | Kategori Minuman (Dark) | Kategori Kerajinan (Dark) |
| :---: | :---: | :---: |
| <img src="img/p4_dark_makanan.png" width="240" alt="Dark Makanan P4" /> | <img src="img/p4_dark_minuman.png" width="240" alt="Dark Minuman P4" /> | <img src="img/p4_dark_kerajinan.png" width="240" alt="Dark Kerajinan P4" /> |

#### 6. Pencarian Produk Real-Time (Dark Mode)
| Search Makanan Dark ("kri") | Search Minuman Dark ("b") | Search Kerajinan Dark ("b") |
| :---: | :---: | :---: |
| <img src="img/p4_search_dark_makanan.png" width="240" alt="Search Dark Makanan" /> | <img src="img/p4_search_dark_minuman.png" width="240" alt="Search Dark Minuman" /> | <img src="img/p4_search_dark_kerajinan.png" width="240" alt="Search Dark Kerajinan" /> |

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
* **State & Lifecycle Management**: `remember`, `rememberSaveable`, `mutableStateOf`, `LaunchedEffect`
* **Media & Photo Picker**: `ActivityResultContracts.PickVisualMedia`
* **Komponen Compose**: `Scaffold`, `TopAppBar`, `ExposedDropdownMenuBox`, `LazyRow`, `LazyVerticalGrid`, `Card`, `OutlinedTextField`, `Button`, `OutlinedButton`, `Checkbox`, `CircularProgressIndicator`, `Toast`, `Snackbar`