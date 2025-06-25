<p align="center">
  <a href="https://laravel.com" target="_blank">
    <img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo">
  </a>
</p>

<p align="center">
  <a href="https://github.com/laravel/framework/actions">
    <img src="https://github.com/laravel/framework/workflows/tests/badge.svg" alt="Build Status">
  </a>
  <a href="https://packagist.org/packages/laravel/framework">
    <img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads">
  </a>
  <a href="https://packagist.org/packages/laravel/framework">
    <img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version">
  </a>
  <a href="https://packagist.org/packages/laravel/framework">
    <img src="https://img.shields.io/packagist/l/laravel/framework" alt="License">
  </a>
</p>

---

# Sistem Project Monitoring 

Repositori ini berisi aplikasi berbasis Laravel yang digunakan untuk mengelola dan memantau proyek. Fitur utamanya meliputi input data proyek seperti judul, nama project leader, tanggal mulai dan berakhir, nama klien, progress, serta upload foto proyek.

## 👩‍💻 Dibuat oleh

**Ridhawati**  
D3 Teknik Informatika  
Politeknik Hasnur  

## 📌 Fitur
- CRUD (Create, Read, Update, Delete) data proyek
- Upload foto proyek
- Tampilan monitoring menggunakan tabel
- Desain responsif menggunakan Tailwind CSS
- Akses langsung tanpa login (open access)

## 🛠️ Teknologi yang Digunakan
- **Laravel 10**
- **MySQL**
- **Tailwind CSS**
- **Laravel File Storage (storage:link)**

## 📷 Screenshot Tampilan

> Pastikan folder `public/screenshots/` berisi file gambar berikut:

### 📋 Daftar Project
![Daftar Project](screenshots/daftar.png)

### ➕ Tambah Project
![Tambah Project](screenshots/tambah.png)

### ✏️ Edit Project
![Edit Project](screenshots/edit.png)

## 🚀 Cara Menjalankan Project (Lokal)

```bash
# Clone repository
git clone https://github.com/Ridhaawati/Sistem-Monitoring.git
cd sistem-monitoring-idha

# Install dependency Laravel
composer install

# Salin file .env dan generate key
cp .env.example .env
php artisan key:generate

# Konfigurasi database (di file .env)
# DB_DATABASE=your_db
# DB_USERNAME=your_username
# DB_PASSWORD=your_password

# Migrasi tabel ke database
php artisan migrate

# Buat symbolic link untuk file upload
php artisan storage:link

# Jalankan server
php artisan serve
