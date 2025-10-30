# Lab6Web
#### Nama   : Dzaki Arif Rahman  
#### NIM    : 312410312  
#### Kelas  : TI.24.A4  
#### Mata Kuliah : Pemrograman Web 1  


## LATIHAN 1 – Mengenal Struktur Dasar Bootstrap

### Step 1: Membuat File Dasar HTML

Pertama, saya membuat file `index.html` dan menambahkan link **Bootstrap CSS** dari CDN.

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Praktikum 6 - Bootstrap</title>
  <!-- Link Bootstrap -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>
  <div class="container">
    <h1 class="text-center mt-4">Selamat Datang di Praktikum Bootstrap</h1>
    <p class="text-center text-muted">Belajar layout dan komponen menggunakan framework Bootstrap 5</p>
  </div>
</body>
</html>


⸻

Penjelasan
	1.	Container
Saya menggunakan <div class="container"> sebagai pembungkus utama agar konten memiliki margin otomatis dan tampilan teratur di tengah halaman.
	2.	Class text-center
Digunakan untuk meratakan teks ke tengah tanpa perlu menulis CSS manual.
	3.	Class mt-4 dan text-muted
	•	mt-4 menambahkan margin atas.
	•	text-muted membuat warna teks menjadi abu-abu lembut agar tampilan lebih estetik.

⸻

Screenshot hasil dan codingannya

(Tambahkan gambar hasil tampilannya di sini)

⸻

LATIHAN 2 – Sistem Grid Bootstrap

Step 1: Membuat Layout Grid

Saya menambahkan struktur grid untuk membagi halaman menjadi beberapa kolom.

<div class="container mt-5">
  <div class="row">
    <div class="col-md-4 bg-primary text-white p-3">Kolom 1</div>
    <div class="col-md-4 bg-success text-white p-3">Kolom 2</div>
    <div class="col-md-4 bg-warning text-dark p-3">Kolom 3</div>
  </div>
</div>


⸻

Penjelasan
	1.	Grid System
Bootstrap menggunakan sistem 12 kolom. Dalam contoh di atas, setiap kolom (col-md-4) mengambil 4 bagian dari total 12 kolom, sehingga 3 kolom sejajar sempurna.
	2.	Kelas Responsif
	•	col-md-4: berarti lebar kolom 4 pada layar sedang (medium) ke atas.
	•	Saat di layar kecil, kolom otomatis turun ke bawah (stack).
	3.	Warna dan Padding
	•	bg-primary, bg-success, dan bg-warning memberikan warna latar berbeda.
	•	p-3 menambahkan padding di dalam kolom.

⸻

Screenshot hasil dan codingannya

(Tambahkan gambar hasil tampilannya di sini)

⸻

LATIHAN 3 – Menambahkan Navbar dan Footer

Step 1: Membuat Navbar

Saya menambahkan navigasi di bagian atas halaman.

<nav class="navbar navbar-expand-lg navbar-dark bg-dark">
  <div class="container-fluid">
    <a class="navbar-brand" href="#">Zaki Bootstrap</a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarNav">
      <ul class="navbar-nav ms-auto">
        <li class="nav-item"><a class="nav-link active" href="#">Home</a></li>
        <li class="nav-item"><a class="nav-link" href="#">About</a></li>
        <li class="nav-item"><a class="nav-link" href="#">Contact</a></li>
      </ul>
    </div>
  </div>
</nav>


⸻

Penjelasan
	1.	Navbar Bootstrap
Navbar ini otomatis responsif. Saat tampilan kecil, menu akan berubah menjadi tombol (hamburger icon).
	2.	Kelas penting
	•	navbar-expand-lg → navbar melebar penuh di layar besar.
	•	bg-dark dan navbar-dark → kombinasi warna gelap dan teks terang.
	•	ms-auto → memindahkan menu ke sisi kanan.

⸻

Step 2: Menambahkan Footer

<footer class="bg-dark text-white text-center p-3 mt-5">
  <p>&copy; 2025 - Dzaki Arif Rahman | Universitas Pelita Bangsa</p>
</footer>

Penjelasan:
Footer diberi warna gelap dengan teks putih (text-white) dan posisi tengah (text-center). Padding (p-3) membuat ruang di dalam footer lebih lega.

⸻

Screenshot hasil dan codingannya

(Tambahkan gambar navbar dan footernya di sini)

⸻

LATIHAN 4 – Komponen Card dan Button

Step 1: Membuat Card

<div class="container my-5">
  <div class="row">
    <div class="col-md-4">
      <div class="card">
        <img src="img/profile.jpg" class="card-img-top" alt="Profil">
        <div class="card-body">
          <h5 class="card-title">Dzaki Arif Rahman</h5>
          <p class="card-text">Mahasiswa Universitas Pelita Bangsa, kelas TI.24.A4</p>
          <a href="#" class="btn btn-primary">Lihat Profil</a>
        </div>
      </div>
    </div>
  </div>
</div>


⸻

Penjelasan
	1.	Card Bootstrap
Komponen ini digunakan untuk menampilkan konten seperti profil, produk, atau artikel secara terstruktur.
	2.	Elemen dalam Card
	•	card-img-top: menampilkan gambar di bagian atas card.
	•	card-body: berisi teks dan tombol.
	•	btn btn-primary: menambahkan tombol bergaya biru khas Bootstrap.
	3.	Kelas my-5
Memberikan jarak vertikal (margin atas dan bawah).

⸻

Screenshot hasil dan codingannya

(Tambahkan gambar hasil tampilannya di sini)

⸻

TUGAS PRAKTIKUM – Membuat Halaman Portfolio Sederhana

Deskripsi

Buat halaman web portfolio menggunakan Bootstrap dengan komponen:
	•	Navbar
	•	Hero section
	•	Grid (3 kolom)
	•	Card (untuk menampilkan data proyek)
	•	Footer

⸻

Contoh Struktur File

/lab6web
 ├── index.html
 ├── img/
 └── css/


⸻

Contoh Potongan Kode

<section class="bg-light text-center py-5">
  <h2>My Portfolio</h2>
  <p>Beberapa proyek yang telah saya buat menggunakan HTML, CSS, dan Bootstrap.</p>
</section>

<div class="container my-5">
  <div class="row">
    <div class="col-md-4">
      <div class="card shadow">
        <img src="img/project1.jpg" class="card-img-top" alt="Project 1">
        <div class="card-body">
          <h5 class="card-title">Website Personal</h5>
          <p class="card-text">Desain web pribadi menggunakan HTML, CSS, dan Bootstrap.</p>
        </div>
      </div>
    </div>
    <!-- Tambahkan card lainnya -->
  </div>
</div>


⸻

Screenshot hasil dan codingannya

(Tambahkan screenshot hasil portfolio di sini)

⸻

Kesimpulan

Dari praktikum ini saya memahami bahwa:
	1.	Bootstrap sangat membantu dalam membuat tampilan web responsif dan menarik tanpa menulis CSS panjang.
	2.	Sistem grid 12 kolom memungkinkan layout yang fleksibel di berbagai ukuran layar.
	3.	Komponen seperti navbar, card, dan button membuat desain web terlihat profesional.
	4.	Penggunaan class utility (seperti p-3, mt-5, text-center) mempercepat proses styling.

Dengan penguasaan dasar Bootstrap ini, saya dapat membuat website yang modern, rapi, dan kompatibel di semua perangkat dengan lebih efisien.

⸻
