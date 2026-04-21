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


---

### 5. 💊 Manajemen Obat

* CRUD obat
* Stok obat

---

### 6. 🧾 Resep Obat

* Input resep dari rekam medis
* Banyak obat dalam satu transaksi

---

### 7. 📊 Dashboard Sederhana

* Jumlah pasien
* Jumlah kunjungan
* Stok obat

---

## 🗂️ Struktur Database

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

## 🚀 Teknologi yang Digunakan

* Backend: CodeIgniter 4
* Database: MySQL
* Frontend: HTML, CSS

---

## 🎯 Output yang Diharapkan

* Aplikasi web berjalan
* Login multi-role
* CRUD lengkap
* Relasi data berjalan
* Query kompleks berhasil

---