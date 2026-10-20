# 📘 PRAKTIKUM 1 — PEMROGRAMAN BERBASIS WEB

<p align="center">
  <b>Dokumentasi Praktikum Pemrograman Berbasis Web</b><br>
  Universitas Pancasila · Teknik Informatika
</p>

<p align="center">
  <img src="https://img.shields.io/badge/PHP-8.2%2B-777BB4?style=for-the-badge&logo=php&logoColor=white" alt="PHP">
  <img src="https://img.shields.io/badge/HTML5-Web%20Structure-E34F26?style=for-the-badge&logo=html5&logoColor=white" alt="HTML5">
  <img src="https://img.shields.io/badge/CSS3-Page%20Styling-1572B6?style=for-the-badge&logo=css3&logoColor=white" alt="CSS3">
</p>

---

## 👨‍🎓 Identitas Mahasiswa

| Informasi | Keterangan |
|---|---|
| Nama | Ridwan Odi Nugroho |
| NIM | 4524210089 |
| Program Studi | Teknik Informatika |
| Perguruan Tinggi | Universitas Pancasila |
| Mata Kuliah | Pemrograman Berbasis Web (PBW) |
| Praktikum | Pertemuan 1 |

## 📋 Daftar Isi

- [Tentang Praktikum](#-tentang-praktikum)
- [Tujuan Pembelajaran](#-tujuan-pembelajaran)
- [Daftar Program](#-daftar-program)
- [Teknologi yang Digunakan](#-teknologi-yang-digunakan)
- [Struktur Folder](#-struktur-folder)
- [Persyaratan Sistem](#-persyaratan-sistem)
- [Cara Menjalankan Program](#-cara-menjalankan-program)
- [Skenario Pengujian](#-skenario-pengujian)
- [Konsep yang Dipelajari](#-konsep-yang-dipelajari)
- [Pengembangan Selanjutnya](#-pengembangan-selanjutnya)
- [Penutup](#-penutup)

## 🎯 Tentang Praktikum

Praktikum ini merupakan latihan dasar pengembangan aplikasi web menggunakan PHP sebagai bahasa pemrograman sisi server, dengan HTML untuk membangun struktur halaman dan CSS untuk mengatur tampilan.

Program yang dibuat berfokus pada tiga penerapan utama, yaitu menampilkan informasi mahasiswa, mengolah data akademik menggunakan fungsi dan percabangan, serta melakukan operasi matematika melalui formulir interaktif.

Setiap program memiliki tujuan yang berbeda, tetapi saling berkaitan dalam memperkenalkan logika pemrograman dan penerapannya pada halaman web.

## 📚 Tujuan Pembelajaran

Praktikum ini bertujuan untuk:

1. Memahami struktur dasar dokumen PHP dan HTML.
2. Mempelajari penggunaan variabel dan array asosiatif.
3. Membuat fungsi untuk mengolah dan menentukan hasil berdasarkan kondisi tertentu.
4. Menggunakan percabangan `if` dan `switch`.
5. Memanfaatkan perulangan `foreach` untuk menampilkan data.
6. Memproses input pengguna melalui formulir HTML.
7. Menampilkan hasil pengolahan data secara dinamis pada browser.
8. Mengenal penggunaan CSS untuk memperbaiki tampilan halaman web.

## 🗂️ Daftar Program

### 1. Biodata Mahasiswa — `biodata.php`

Program ini menampilkan informasi mahasiswa yang tersimpan dalam array asosiatif. Data ditampilkan secara otomatis menggunakan perulangan sehingga setiap pasangan kunci dan nilai dapat ditampilkan tanpa menuliskan elemen HTML satu per satu.

Program juga menggunakan fungsi `statusKelulusan()` untuk menentukan predikat akademik berdasarkan nilai IPK.

**Fitur utama:**

- Menyimpan informasi mahasiswa dalam array.
- Menampilkan data menggunakan `foreach`.
- Menentukan predikat IPK melalui fungsi.
- Menggunakan percabangan untuk memilih hasil predikat.
- Menampilkan informasi melalui halaman HTML.

**Aturan predikat IPK:**

| Kondisi IPK | Predikat |
|---|---|
| IPK ≥ 3,50 | Sangat Memuaskan |
| IPK ≥ 3,00 dan < 3,50 | Memuaskan |
| IPK < 3,00 | Perlu Peningkatan |

**Konsep yang diterapkan:** array asosiatif, fungsi, percabangan, perulangan, dan output dinamis.

### 2. Biodata Mahasiswa yang Dikembangkan — `biodatatugas1.php`

Program ini merupakan pengembangan dari contoh biodata dengan penyesuaian informasi mahasiswa dan penambahan fungsi untuk menentukan status berdasarkan semester.

Selain menampilkan predikat IPK, halaman ini menampilkan status mahasiswa serta menggunakan CSS internal untuk memberikan tampilan yang lebih terstruktur.

**Fitur utama:**

- Menampilkan identitas mahasiswa.
- Mengolah data menggunakan array asosiatif.
- Menentukan predikat berdasarkan IPK.
- Menentukan status mahasiswa berdasarkan semester.
- Menggunakan CSS untuk mengatur tata letak dan tampilan.
- Menggunakan `htmlspecialchars()` ketika menampilkan data.

**Aturan status mahasiswa:**

| Kondisi Semester | Status |
|---|---|
| Semester 1–2 | Mahasiswa Baru |
| Semester 3–6 | Mahasiswa Aktif |
| Semester 7 ke atas | Mahasiswa Tingkat Akhir |

**Konsep yang diterapkan:** penggunaan kembali fungsi, percabangan, array, perulangan, HTML, CSS, dan pengamanan output.

### 3. Kalkulator Sederhana — `kalkulator.php`

Program kalkulator digunakan untuk melakukan perhitungan berdasarkan dua angka yang dimasukkan pengguna melalui formulir.

Setelah tombol **Hitung** ditekan, data dikirim menggunakan metode `POST`. PHP kemudian membaca input, memeriksa operator yang dipilih, dan menghitung hasil sesuai operasi yang diminta.

**Fitur utama:**

- Input dua angka.
- Pemilihan operator matematika.
- Pemrosesan formulir menggunakan metode `POST`.
- Pemilihan operasi menggunakan `switch`.
- Menampilkan hasil perhitungan.
- Menangani pembagian dengan nol.
- Menampilkan pesan untuk operator yang tidak valid.

**Operasi yang tersedia:**

| Operator | Fungsi | Contoh |
|---|---|---|
| `+` | Penjumlahan | 10 + 5 = 15 |
| `-` | Pengurangan | 10 - 5 = 5 |
| `*` | Perkalian | 10 × 5 = 50 |
| `/` | Pembagian | 10 ÷ 5 = 2 |

Contoh di atas merupakan ilustrasi cara kerja operasi, bukan hasil pengujian yang sudah dijalankan.

## 🛠️ Teknologi yang Digunakan

| Teknologi | Kegunaan |
|---|---|
| PHP | Mengolah data dan menjalankan logika aplikasi |
| HTML5 | Menyusun elemen halaman dan formulir |
| CSS3 | Mengatur tampilan halaman biodata tugas |
| Web Browser | Menampilkan halaman dan hasil program |
| PHP Development Server / XAMPP | Menjalankan aplikasi pada komputer lokal |

> Versi PHP yang digunakan sebaiknya disesuaikan dengan versi yang terpasang di komputer.

## 📁 Struktur Folder

Susunan folder yang disarankan untuk Praktikum 1:

```text
Praktikum 1/
├── README.md
├── biodata.php
├── biodatatugas1.php
└── kalkulator.php
```

**Keterangan file:**

- `README.md` — dokumentasi proyek dan petunjuk penggunaan.
- `biodata.php` — program untuk menampilkan biodata dan predikat IPK.
- `biodatatugas1.php` — pengembangan biodata dengan status semester dan CSS.
- `kalkulator.php` — program perhitungan aritmetika menggunakan formulir.

## 💻 Persyaratan Sistem

Sebelum menjalankan program, siapkan perangkat lunak berikut:

- PHP yang sudah terpasang, atau XAMPP yang menyertakan PHP.
- Browser seperti Google Chrome, Microsoft Edge, atau Firefox.
- Editor kode seperti Visual Studio Code.

Untuk memeriksa apakah PHP sudah tersedia, jalankan perintah berikut di terminal:

```bash
php -v
```

Jika versi PHP ditampilkan, PHP dapat dipanggil melalui terminal.

## 🚀 Cara Menjalankan Program

### Metode 1 — Menggunakan PHP Development Server

**Langkah 1.** Pastikan ketiga file PHP berada di folder yang sama.

**Langkah 2.** Buka terminal pada folder Praktikum 1.

**Langkah 3.** Jalankan server lokal:

```bash
php -S localhost:8000
```

**Langkah 4.** Buka browser dan akses program yang diinginkan.

| Program | URL Lokal |
|---|---|
| Biodata | `http://localhost:8000/biodata.php` |
| Biodata Tugas | `http://localhost:8000/biodatatugas1.php` |
| Kalkulator | `http://localhost:8000/kalkulator.php` |

**Langkah 5.** Untuk kalkulator, masukkan dua angka, pilih operator, kemudian tekan tombol **Hitung**.

Untuk menghentikan server, kembali ke terminal dan tekan `Ctrl + C`.

### Metode 2 — Menggunakan XAMPP

1. Pindahkan folder Praktikum 1 ke direktori `htdocs`.
2. Buka XAMPP Control Panel.
3. Jalankan layanan Apache.
4. Buka browser.
5. Akses `http://localhost/Praktikum%201/biodata.php` atau file lain sesuai nama program.

Pastikan nama folder pada URL sesuai dengan nama folder yang sebenarnya.

## 🧪 Skenario Pengujian

Pengujian berikut dapat dilakukan untuk memeriksa perilaku dasar program.

### Pengujian Biodata

| No. | Skenario | Hasil yang Diharapkan |
|---|---|---|
| 1 | Membuka `biodata.php` | Data mahasiswa ditampilkan |
| 2 | Memeriksa predikat IPK 3,50 | Predikat Sangat Memuaskan |
| 3 | Membuka `biodatatugas1.php` | Biodata tampil dengan CSS |
| 4 | Memeriksa status semester 5 | Status Mahasiswa Aktif |

### Pengujian Kalkulator

| No. | Input | Operator | Hasil yang Diharapkan |
|---|---|---|---|
| 1 | 10 dan 5 | `+` | 15 |
| 2 | 10 dan 5 | `-` | 5 |
| 3 | 10 dan 5 | `*` | 50 |
| 4 | 10 dan 5 | `/` | 2 |
| 5 | 10 dan 0 | `/` | Pesan pembagian dengan nol |

Tabel tersebut berisi skenario dan hasil yang diharapkan. Hasil aktual perlu diperiksa dengan menjalankan setiap program.

## 🧠 Konsep yang Dipelajari

Beberapa konsep pemrograman yang diterapkan dalam praktikum ini meliputi:

- **Array asosiatif:** menyimpan informasi dalam pasangan kunci dan nilai.
- **Fungsi:** memisahkan proses tertentu agar dapat digunakan sesuai kebutuhan.
- **Percabangan:** menentukan keluaran berdasarkan kondisi.
- **Perulangan:** menampilkan sejumlah data secara otomatis.
- **Formulir HTML:** menerima input dari pengguna.
- **Metode POST:** mengirim data formulir untuk diproses oleh PHP.
- **Switch-case:** menentukan operasi berdasarkan operator yang dipilih.
- **CSS:** mengatur tampilan dan tata letak halaman.
- **Validasi sederhana:** menangani kondisi pembagian dengan nol.

## 🔧 Pengembangan Selanjutnya

Beberapa pengembangan yang dapat dipertimbangkan untuk latihan berikutnya:

- Menambahkan validasi input yang lebih lengkap.
- Memperbaiki tampilan kalkulator menggunakan CSS.
- Menambahkan tombol untuk menghapus atau mengulang input.
- Memisahkan CSS ke dalam file tersendiri.
- Mengembangkan biodata agar menerima data dari formulir.
- Menghubungkan aplikasi dengan database jika materi praktikum sudah mencakup pengelolaan data.

Pengembangan tersebut merupakan ide lanjutan, bukan fitur yang diklaim sudah tersedia pada program saat ini.

## 📌 Penutup

Praktikum 1 memberikan latihan awal dalam memahami hubungan antara PHP dan HTML untuk membangun halaman web dinamis. Melalui program biodata, pengolahan status mahasiswa, dan kalkulator sederhana, konsep dasar seperti array, fungsi, percabangan, perulangan, serta pemrosesan formulir dapat dipelajari melalui contoh yang mudah dipahami.

Dokumentasi ini diharapkan dapat membantu menjelaskan isi program dan mempermudah proses menjalankan serta memeriksa hasil praktikum.

---

<p align="center">
  <i>Praktikum 1 · Pemrograman Berbasis Web</i><br>
  <b>Ridwan Odi Nugroho · 4524210089</b>
</p>
