# PERTEMUAN 9

## Praktikum 9.1 — Script Pertama: Laporan Sistem

### 1. Buat workspace praktikum:
![](img/20260442-124214.png)

### 2. Buat script dengan nano:
![](img/20260443-124340.png)

### 3. Ketik isi berikut, simpan (`Ctrl+O` `Enter`), lalu keluar (`Ctrl+X`):
![](img/20260445-124512.png)

### 4. Beri izin dan jalankan:
![](img/20260446-124633.png)

## Latihan 9.1
**Modifikasi laporan-sistem.sh agar menyimpan output ke file laporan-YYYY-MM-DD.txt sekaligus menampilkannya di terminal. Petunjuk: gunakan tee yang sudah dipelajari di bab sebelumnya.**
![](img/20260454-125435.png)
![](img/20260455-125529.png)

## Praktikum 9.2 — Script Info Sistem dengan Argumen

### 1. Buat script:
![](img/20260458-125811.png)

### 2. Ketik isi berikut:
![](img/20260457-125717.png)

### 3. Simpan, beri izin, uji dengan berbagai kombinasi argumen:
![](img/20260400-130033.png)

## Latihan 9.2
**Buat script kalkulator.sh yang menerima tiga argumen: <angka1> <operator> <angka2> dengan operator +, -, *, atau /. Contoh: ./kalkulator.sh 20 + 5 menghasilkan 25. Gunakan case untuk memilih operasi, dan validasi jika argumen tidak lengkap.**
![](img/20260403-130351.png)
![](img/20260406-130641.png)

## Praktikum 9.3 — Script Grading dan Menu Interaktif

### 1. Buat script grading (menggunakan if dan for):
![](img/20260410-131058.png)

### 2. Ketik isi berikut:
![](img/20260410-131015.png)

### 3. Simpan, beri izin, dan jalankan:
![](img/20260412-131235.png)

### 4. Buat script menu interaktif (`while` + `case`):
![](img/20260413-131352.png)

### 5. Ketik isi berikut:
![](img/20260419-131900.png)

### 6. Beri izin dan jalankan, coba setiap opsi:
![](img/20260420-132058.png)
![](img/20260421-132117.png)

## Latihan 9.3
**Tambahkan ke script grading-batch.sh sebuah ringkasan di bagian bawah yang menampilkan: jumlah mahasiswa per grade (A, B, C, D, E) menggunakan perulangan for kedua yang mengiterasi array MAHASISWA.**
![](img/20260432-133253.png)
![](img/20260436-133644.png)

## Praktikum 9.4 — Library Fungsi Validasi

### 1. Buat file library:
![](img/20260448-134852.png)

### 2. Ketik isi berikut:
![](img/20260451-135131.png)

### 3. Buat script yang menggunakan library:
![](img/20260452-135217.png)

### 4. Ketik isi berikut:
![](img/20260455-135513.png)

### 5. Beri izin dan uji semua skenario:
![](img/20260459-135911.png)

## Latihan 9.4
**Tambahkan fungsi konfirmasi() ke lib-validasi.sh. Fungsi ini menampilkan pertanyaan, membaca input Y/N dari user, mengembalikan 0 jika Y dan 1 jika N. Buat script demo yang memanggil fungsi ini sebelum menghapus sebuah file.**
![](img/20260402-140219.png)
![](img/20260403-140334.png)
![](img/20260405-140557.png)

## Praktikum 9.5 — Script Backup dengan Opsi

### 1. Buat script:
![](img/20260407-140715.png)

### 2. Ketik isi berikut:
![](img/20260410-141034.png)
![](img/20260410-141052.png)

### 3. Beri izin dan uji
![](img/20260413-141329.png)

## Praktikum 9.6 — Debugging Script

### 1. Buat script untuk dianalisis:
![](img/20260425-142520.png)

### 2. Ketik isi berikut:
![](img/20260427-142756.png)

### 3. cek sintak, lalu jalankan dengan tracing:
![](img/20260444-144448.png)
![](img/20260445-144508.png)
![](img/20260435-113512.png)

## Latihan 9.6
**Script debug-latihan.sh tidak menangani direktori yang tidak ada. Perbaiki dengan menambahkan:**

- **set -e di baris kedua**
- **Pengecekan -d "$DIREKTORI" sebelum memanggil du**
- **Pesan error yang informatif jika direktori tidak ditemukan**

**Uji dengan direktori yang tidak ada.**

**Jawaban:**
![](img/20260452-115255.png)
![](img/20260408-120850.png)

## Tugas Praktikum 1 — Script Absensi Kelas

### Konteks: 
instruktur mencatat kehadiran mahasiswa dari command line.

### Instruksi:
1. Buat script `absensi.sh` yang:
- Menerima argumen nama mahasiswa dan status (hadir/izin/alpha)
- Menyimpan entri ke absensi-YYYY-MM-DD.txt dengan format [HH:MM] NAMA - STATUS
- Opsi `-r`: tampilkan rekapitulasi (jumlah per status)
- Opsi `-h`: tampilkan bantuan
2. Rekam minimal 5 entri dan tampilkan rekapitulasi nya.

### Konsep wajib:
variabel, parameter posisional, getopts, if, for, fungsi, dan
redirection ke file.

### Proses Pengerjaan Tugas
1. Persiapan Variabel & Fungsi Bantuan
![](img/20260415-121507.png)

2. Fungsi Rekapitulasi (Menggunakan for & if)
![](img/20260416-121652.png)

3. Parsing Opsi dengan getopts
![](img/20260419-121949.png)

4. Logika Pencatatan & Redirection
![](img/20260420-122034.png)

5. Pengujian Sesuai Syarat Tugas
![](img/20260428-122814.png)

## Tugas Praktikum 2 — Script Health Check Sistem

### Konteks: 
administrator membuat pemeriksaan kondisi server sebelum maintenance.

### Instruksi:
1. Buat script healthcheck.sh menggunakan template profesional dari bagian Best Practices.
2. Script menampilkan: tanggal/waktu, hostname, uptime, penggunaan CPU, memori, dan disk untuk setiap filesystem yang terpasang.
3. Jika penggunaan disk mana pun melebihi 80%, tampilkan peringatan.
4. Simpan hasil ke healthcheck-YYYY-MM-DD.log dan tampilkan ke terminal sekaligus menggunakan tee.
5. Opsi -t <persen> mengubah batas peringatan disk (default 80).

### Konsep wajib:
set -euo pipefail, trap, getopts, fungsi dengan local,
for, if, dan tee.

### Proses Pengerjaan Tugas
1. Best Practices & Penanganan Opsi (getopts)
![](img/20260435-123541.png)

2. Membuat Fungsi Pemeriksaan Sistem
![](img/20260436-123656.png)

3. Fungsi Pemeriksaan Disk (Perulangan for & if)
![](img/20260438-123824.png)

4. Eksekusi Utama & Redirection (tee)
![](img/20260438-123856.png)

5. Pengujian
![](img/20260440-124029.png)
![](img/20260440-124041.png)
