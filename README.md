# Pemrograman Web

Kumpulan tugas mata kuliah **Pemrograman Web** (Web Programming) yang mencakup berbagai teknologi web dari frontend hingga backend.

## Deskripsi

Repository ini berisi 3 tugas utama yang dikerjakan selama perkuliahan:

---

### 1. Quiz 1 — Static Website (`Quiz1/`)

Website statis menggunakan HTML dan CSS murni dengan template Vertex.

**Tech Stack:** HTML5, CSS3, FontAwesome, Magnific Popup

---

### 2. UTS — Gigs Event Management (`UTS/gigs-am/`)

Aplikasi web manajemen event menggunakan framework Laravel.

**Fitur:**
- Autentikasi pengguna (Login, Register, Reset Password)
- CRUD Event — Membuat, melihat, mengubah, dan menghapus event
- Halaman utama dengan daftar event
- Manajemen pengguna

**Tech Stack:** PHP, Laravel, MySQL, Bootstrap, Vite

**Cara Menjalankan:**
```bash
cd UTS/gigs-am
composer install
npm install
cp .env.example .env
php artisan key:generate
php artisan migrate
php artisan serve
```

---

### 3. EAS — Bus Booking System (`EAS/`)

Sistem pemesanan tiket bus berbasis web menggunakan ASP.NET Web Forms.

**Fitur:**
- Login & registrasi pengguna
- Pencarian rute bus
- Pemesanan tiket dengan detail penumpang
- Laporan pemesanan (Booking Report)
- Halaman About Us
- Dockerized deployment

**Tech Stack:** ASP.NET Web Forms, C#, SQL Server, Docker

**Cara Menjalankan:**
```bash
cd EAS
# Menggunakan Docker
docker build -t bus-booking .
docker run -p 8080:80 bus-booking

# Atau menggunakan Visual Studio
# Buka BusBookingProject.sln dan jalankan
```

---

## Struktur Proyek

```
PemrogramanWeb/
├── Quiz1/                  # Website statis
│   ├── index.html
│   ├── css/
│   └── fontawesome/
├── UTS/                    # Laravel app
│   └── gigs-am/
│       ├── app/
│       ├── resources/
│       ├── routes/
│       └── ...
└── EAS/                    # ASP.NET Web Forms
    ├── BusBookingProject/
    ├── BusBookingProject.sln
    └── Dockerfile
```

## Penulis

**Marco Marcello Hugo** — 5025221102  
Teknik Informatika, Institut Teknologi Sepuluh Nopember
