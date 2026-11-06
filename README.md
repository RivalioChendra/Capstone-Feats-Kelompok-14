<div align="center">

# 🥖 FEAST

### Sistem Informasi Pengelolaan Stok Bahan Baku, Produksi, dan Distribusi Produk Jadi Berbasis Java

*Produse Roti Kemasan*

</div>

---
 
## 📚 Daftar Isi
 
1. [Deskripsi Singkat](#1--deskripsi-singkat)
2. [Fitur Utama Program](#2--fitur-utama-program)
3. [Tech Stack](#3--tech-stack)
4. [Perancangan Sistem](#4--perancangan-sistem)
5. [Struktur Folder/Package](#5--struktur-folderpackage)
6. [Penerapan 4 Pilar OOP](#6--penerapan-4-pilar-oop)
7. [Cara Penggunaan Program](#7--cara-penggunaan-program)
8. [Kontributor](#8--kontributor)
---

## 1. 📌 Deskripsi Singkat
 
Bagi produsen roti kemasan seperti PT Feast, pengelolaan bahan baku, produksi, dan distribusi yang rapi sangat menentukan kelancaran usaha. Namun, ketika stok bahan, hasil produksi, dan pengiriman masih dicatat terpisah, data mudah tidak sinkron, kecukupan bahan sulit dipastikan sebelum produksi, dan roti yang mendekati kedaluwarsa baru disadari ketika sudah terlambat.
 
Sebagai solusi, dikembangkanlah Sistem Informasi Pengelolaan Stok Bahan Baku, Produksi, dan Distribusi Produk Jadi berbasis aplikasi desktop. Seluruh data bahan baku, resep, produksi, dan pengiriman tersimpan terpusat, sehingga stok selalu terbarui dan riwayat setiap kegiatan dapat ditelusuri.
 
Sistem ini dilengkapi dengan:
- Pencatatan batch produksi, yaitu satu kelompok roti yang dibuat bersamaan, lengkap dengan tanggal produksi dan tanggal kedaluwarsanya.
- Validasi stok otomatis, sehingga produksi atau pengiriman tidak dapat diproses jika bahan atau produk tidak mencukupi.
- Penerapan metode FEFO (First Expired, First Out), yaitu produk yang paling cepat kedaluwarsa dikirim lebih dulu dan produk yang sudah kedaluwarsa tidak ikut terkirim, sehingga pemborosan dapat ditekan.
- Peringatan stok menipis dan produk mendekati kedaluwarsa, serta laporan untuk membantu pengambilan keputusan.
- Pembagian peran Admin (mengelola data master) dan Staff (menjalankan produksi dan distribusi).

---
 
## 2. ⚙️ Fitur Utama Program
 
### 🧑‍💼 Admin
| Fitur | Keterangan |
|---|---|
| Login & Logout | Autentikasi username/password dan penentuan peran |
| Kelola Data Bahan Baku | CRUD bahan baku |
| Kelola Data Produk Jadi | CRUD produk |
| Kelola Data Resep | CRUD komposisi bahan baku per produk |
| Kelola Data Distributor | Mengelola distributor tujuan pengiriman |
| Kelola Akun Staff | Mendaftarkan dan mengelola akun staf beserta shift kerja |
| Dashboard | Ringkasan stok, peringatan, dan riwayat produksi |

 
### 👷 Staff Khusus
| Fitur | Keterangan |
|---|---|
| Login & Logout | Masuk sesuai hak akses staf |
| Kelola Produksi & Batch | Hitung kebutuhan bahan, validasi stok bahan baku, simpan batch (tanggal produksi & kedaluwarsa), perbarui stok produk jadi |
| Pemantauan Stok & Kedaluwarsa | Peringatan tanggal kedaluwarsa dan peringatan stok minimum |
| Menu Distribusi Produk | Validasi stok produk, pilih batch dengan FEFO, kurangi stok produk jadi |
 
---

## 3. 🧰 Tech Stack
  
| Kategori | Teknologi |
|---|---|
| **Bahasa Pemrograman** | Java |
| **GUI Framework** | Java Swing |
| **Database** | MySQL (via Laragon) |
| **IDE** | NetBeans |

     
**Library yang digunakan:**
 
| Library | Fungsi |
|---|---|
| `flatlaf-3.8.jar` | Tema tampilan modern untuk antarmuka |
| `AbsoluteLayout-RELEASE180.jar` | Pengaturan tata letak komponen GUI |
| `mysql-connector-j-8.3.0.jar` | Koneksi aplikasi Java ke database MySQL (JDBC) |
| `protobuf-java-3.25.1.jar` | Pendukung MySQL Connector/J untuk pertukaran data dengan database |
 
---
