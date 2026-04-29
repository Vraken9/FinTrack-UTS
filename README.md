# UTS_Mobile_FinTrack 

Repositori ini dibuat untuk memenuhi tugas Ujian Tengah Semester (UTS) mata kuliah Pemrograman Mobile. Aplikasi yang dikembangkan adalah **FinTrack (Financial Tracker)**, sebuah aplikasi pelacak keuangan pribadi berbasis Android Native.

## Identitas Kelompok (Universitas Ma'arif Nahdlatul Ulama Kebumen)

| Nama Lengkap | NIM |
| :--- | :--- |
| **Akhyar Mualif** | TI1024137 |
| **Ahmad Fahrur Rozi** | TI1024028 |
| **Indi Wardatun Nafisah** | TI1024010 |
| **Alfiatu Zainil Ngaliah** | TI1024034 |
| **Lisa Sofiatuz Zahro** | TI1024027 |

---

##  Deskripsi Aplikasi
**FinTrack** adalah aplikasi *mobile native* yang dirancang untuk mengatasi masalah pencatatan keuangan pribadi yang seringkali tidak teratur. Dibangun dengan antarmuka "Clean UI" minimalis, aplikasi ini membantu mahasiswa dan pekerja muda untuk melacak arus kas (pemasukan, pengeluaran, dan transfer) dengan mudah, menganalisis pengeluaran melalui grafik visual, serta mengekspor data laporan secara praktis.

##  Fitur Utama (Fungsionalitas)

1. **Pencatatan Transaksi Dinamis (Multi-Type):**
   - Mendukung 3 tipe transaksi: Pemasukan, Pengeluaran, dan Transfer.
   - Form pintar: Kategori berubah otomatis sesuai tipe, dan opsi "Tunai" disembunyikan saat melakukan transaksi Transfer (diganti dengan input Nama Penerima/Bank).
   - Input tanggal dan waktu presisi menggunakan bawaan sistem Android (`DatePickerDialog` & `TimePickerDialog`).

2. **Dashboard & Analitik Visual:**
   - Menampilkan ringkasan total saldo, pemasukan, dan pengeluaran bulan berjalan.
   - **Daily Bar Chart:** Grafik batang pengeluaran harian dengan navigasi simulasi pergantian bulan.
   - **Analytics Distribution:** Menampilkan persentase distribusi kategori (misal: "Makanan: 45%") untuk memudahkan evaluasi keuangan.

3. **Manajemen Riwayat Transaksi (CRUD):**
   - Riwayat transaksi disajikan dalam daftar interaktif.
   - Pengguna dapat membaca rincian, mengubah data lama (**Edit**), atau menghapus baris transaksi (**Delete**) secara langsung.

4. **Pengaturan Lanjutan (Settings):**
   - **Mode Gelap/Terang (Theme Customization):** Pengguna dapat mengubah tema aplikasi sesuai kenyamanan mata, yang akan tersimpan dalam preferensi lokal.
   - **Export to CSV:** Fitur *generator* laporan yang memungkinkan pengguna mengekspor seluruh riwayat transaksi ke dalam format `.csv` dan membagikannya ke aplikasi lain (seperti WhatsApp, Email, atau Google Drive) melalui *FileProvider*.

##  Spesifikasi Teknis & Arsitektur

- **Bahasa Pemrograman:** Java
- **UI & Layout:** XML dengan pendekatan "Clean UI" (Warna solid elegan: Navy `#1E293B`, Hijau `#10B981`, Merah `#EF4444`, dan Radius 16dp).
- **Arsitektur:** Menggunakan kombinasi `Activity` untuk Container/Form Utama dan `Fragment` untuk navigasi antar halaman utama (Beranda, Analitik, Riwayat, Pengaturan).
- **Navigasi Utama:** Menggunakan `BottomNavigationView` dan pemisahan form spesifik menggunakan `Intent`.
- **Library Tambahan:** - `MPAndroidChart` (Untuk visualisasi grafik *Bar Chart*).

---
*Dibuat untuk keperluan evaluasi Ujian Tengah Semester (UTS) - 2026*
