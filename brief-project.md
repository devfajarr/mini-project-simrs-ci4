# 🏥 PROJECT BRIEF

## Sistem Informasi Manajemen Rumah Sakit (Mini SIMRS)

### 📌 Nama Proyek

**SIMRS – Rumah Sakit Sejahtera Medika**

---

## 🏢 Profil Klien

**Rumah Sakit Sejahtera Medika** adalah rumah sakit umum swasta skala menengah yang berlokasi di Yogyakarta.

Saat ini:

* Masih menggunakan pencatatan manual + Excel
* Data pasien sering duplikat
* Rekam medis sulit dilacak
* Proses pelayanan lambat

---

## 🚨 Permasalahan Utama

1. **Data pasien tidak terpusat**

   * Sering terjadi duplikasi data
   * Sulit mencari riwayat pasien

2. **Rekam medis tidak terstruktur**

   * Dokter mencatat manual
   * Tidak ada histori yang rapi

3. **Manajemen obat tidak terkontrol**

   * Stok tidak akurat
   * Tidak ada riwayat penggunaan obat

4. **Tidak ada sistem login & hak akses**

   * Semua orang bisa akses data
   * Tidak aman

---

## 🎯 Tujuan Proyek

Membangun sistem berbasis web untuk:

* Mengelola data pasien secara terpusat
* Mencatat rekam medis digital
* Mengontrol stok obat
* Menerapkan sistem login berbasis role

---

## 👥 Target Pengguna

1. **Admin**
2. **Dokter**
3. **Petugas (Staff)**

---

## 🔐 Role & Hak Akses

| Role   | Akses                              |
| ------ | ---------------------------------- |
| Admin  | Full akses semua data              |
| Dokter | Melihat pasien + input rekam medis |
| Staff  | Input data pasien & pendaftaran    |

---

## ⚙️ Fitur Utama

### 1. 🔑 Autentikasi

* Login
* Logout
* Session
* Filter (role-based access)

👉 Ini akan melatih:

* Session handling
* Filter di CodeIgniter 4

---

### 2. 👤 Manajemen Pasien

* Tambah pasien
* Edit data pasien
* Hapus pasien
* List pasien

Field:

* Nama
* NIK
* Alamat
* Tanggal lahir
* No HP

👉 Latihan:

* CRUD
* Validasi
* Query dasar

---

### 3. 🩺 Manajemen Dokter

* CRUD dokter
* Spesialisasi

---

### 4. 📋 Rekam Medis

* Input rekam medis
* Relasi:

  * Pasien
  * Dokter
* Data:

  * Keluhan
  * Diagnosa
  * Tanggal periksa

👉 Ini bagian PALING PENTING:

* JOIN query
* Relasi tabel

---

### 5. 💊 Manajemen Obat

* CRUD obat
* Stok obat

---

### 6. 🧾 Resep Obat

* Input resep dari rekam medis
* Banyak obat dalam satu transaksi

👉 Latihan:

* One-to-many relationship
* Insert multiple data

---

### 7. 📊 Dashboard Sederhana

* Jumlah pasien
* Jumlah kunjungan
* Stok obat

👉 Latihan:

* COUNT
* SUM
* Query agregasi

---

## 🗂️ Struktur Database (Simplified)

### Tabel:

* users
* patients
* doctors
* medical_records
* medicines
* prescriptions
* prescription_details

---

### Relasi:

* patients → medical_records (1:N)
* doctors → medical_records (1:N)
* medical_records → prescriptions (1:1)
* prescriptions → prescription_details (1:N)

---

## 🔄 Contoh Flow Sistem

### Flow 1: Login

1. User login
2. Validasi ke database
3. Simpan session
4. Redirect sesuai role

---

### Flow 2: Input Rekam Medis

1. Pilih pasien
2. Pilih dokter
3. Input diagnosa
4. Simpan ke database

---

### Flow 3: Lihat Riwayat Pasien

* Ambil data:

  * pasien
  * rekam medis
  * dokter

👉 Wajib pakai JOIN

---

## 🧠 Tantangan Teknis (Wajib Dikerjakan)

* Query JOIN manual
* Validasi form
* Session login manual
* Filter (auth & role)
* Pagination (opsional tapi bagus)

---

## 🚀 Teknologi yang Digunakan

* Backend: CodeIgniter 4
* Database: MySQL
* Frontend: HTML, CSS (boleh pakai Bootstrap)

---

## 📈 Scope Batasan (biar tidak overkill)

TIDAK perlu:

* API kompleks
* UI mewah
* Realtime system

Fokus:

> **logic, query, dan arsitektur**

---

## 🎯 Output yang Diharapkan

* Aplikasi web berjalan
* Login multi-role
* CRUD lengkap
* Relasi data berjalan
* Query kompleks berhasil

---