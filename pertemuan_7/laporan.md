# PERTEMUAN 7

## Praktikum 7.1 — Mengenali Bash dan Menyiapkan Workspace

### 1. Lihat shell login dan shell aktif saat ini:
![](img/20260448-114848.png)

### 2. Lihat proses shell yang sedang berjalan:
![](img/20260450-115027.png)

### 3. Buat workspace praktikum:
![](img/20260453-115351.png)

### 4. Buat beberapa file contoh yang akan dipakai pada praktikum berikutnya:
![](img/20260455-115506.png)

## Praktikum 7.2 — Membuat Ringkasan Sesi Terminal

### 1. Masuk ke workspace praktikum:
![](img/20260459-115912.png)

### 2. Simpan informasi sesi terminal ke file laporan:
![](img/20260458-115844.png)

### 3. Verifikasi isi file laporan:
![](img/20260458-115844.png)

## Praktikum 7.3 — Menambahkan Konfigurasi Aman pada .bashrc

### 1. Lihat file konfigurasi Bash pada home directory:
![](img/20260400-120026.png)

### 2. Buat backup .bashrc:
![](img/20260402-120208.png)

### 3. Tambahkan blok konfigurasi praktikum:
![](img/20260402-120247.png)

### 4. Terapkan konfigurasi tanpa logout:
![](img/20260405-120529.png)

## Praktikum 7.4 — Menyiapkan .bash_profile untuk Shell Login

### 1. Backup .bash_profile jika sudah ada:
![](img/20260406-120623.png)

### 2. Tambahkan konfigurasi login shell:
![](img/20260406-120623.png)

### 3. Uji dengan membuka login shell baru:
![](img/20260408-120839.png)

## Praktikum 7.5— Membedakan Variabel Shell dan Environment Variable

### 1. Buat variabel lokal:
![](img/20260409-120927.png)

### 2. Buka subshell dan cek apakah variabel masih ada:
![](img/20260411-121158.png)

### 3. Sekarang ubah menjadi environment variable:
![](img/20260412-121250.png)

### 4. Lihat isi PATH dan lokasi beberapa perintah:
![](img/20260413-121339.png)

## Praktikum 7.6 — Menambahkan Direktori Script Pribadi ke PATH

### 1. Pastikan direktori bin praktikum tersedia:
![](img/20260415-121539.png)

### 2. Tambahkan direktori tersebut ke PATH melalui .bashrc:
![](img/20260415-121539.png)

### 3. Buat script ringkasan sistem:
![](img/20260416-121647.png)

### 4. Jalankan script dari direktori yang berbeda:
![](img/20260417-121722.png)

## Praktikum 7.7 — Membuat Alias Produktivitas Dasar

### 1. Tambahkan alias ke .bashrc:
![](img/20260417-121758.png)

### 2. Uji alias:
![](img/20260418-121831.png)
![](img/20260420-122057.png)

## Praktikum 7.8 — Membuat Fungsi Backup Konfigurasi

### 1. Siapkan file konfigurasi contoh:
![](img/20260403-130342.png)

### 2. Tambahkan fungsi ke .bashrc:
![](img/20260404-130444.png)

### 3. Uji fungsi:
![](img/20260405-130559.png)

## Praktikum 7.9 — Menggunakan Completion Dasar dan Melihat History

### 1. Pastikan file contoh tersedia:
![](img/20260408-130847.png)

### 2. Uji completion file:
a. Ketik cat lap lalu tekan Tab dua kali.
![](img/20260410-131048.png)
Completion berhasil `cat lap` jadi `cat laporan-`

b. Amati daftar file yang memiliki prefix lap.

sudah

c. Ketik lebih spesifik, misalnya cat laporan-h lalu tekan Tab.
![](img/20260412-131230.png)
Completion berhasil `cat laporan-h` jadi `cat laporan-harian.log`

### 3. Jalankan beberapa perintah sederhana:
![](img/20260413-131354.png)

## Praktikum 7.10 — Menelusuri Perintah Diagnostik dengan History

### 1. Jalankan beberapa perintah diagnostik:
![](img/20260414-131435.png)

### 2. Cari ulang perintah diagnostik dari history:
![](img/20260416-131629.png)
![](img/20260416-131658.png)

### 3. Jalankan ulang salah satu perintah berdasarkan nomor history:
![](img/20260417-131742.png)

### 4. Simpan potongan history ke file dokumentasi:
![](img/20260419-131929.png)

## Praktikum 7.11 — Mencoba Wildcard Dasar

### 1. Masuk ke direktori sampel:
![](img/20260420-132054.png)

### 2. Coba beberapa pola wildcard:
![](img/20260421-132146.png)

### 3. Coba beberapa ekspansi lain:
![](img/20260422-132244.png)

## Praktikum 7.12 — Mengarsipkan Banyak Log Sekaligus

### 1. Siapkan file log tambahan:
![](img/20260423-132349.png)

### 2. Preview file yang akan diproses:
![](img/20260424-132419.png)

### 3. Pindahkan semua file log ke folder arsip:
![](img/20260425-132513.png)

### 4. Kompres folder arsip:
![](img/20260426-132615.png)

## Praktikum 7.13 — Membedakan Single Quote, Double Quote, dan Escape

### 1. Uji single quote dan double quote:
![](img/20260427-132738.png)

### 2. Uji escape karakter spasi:
![](img/20260439-133905.png)

### 3. Uji akses file yang sama dengan double quote:
![](img/20260439-133945.png)

## Praktikum 7.14 — Menangani File dengan Nama Sulit Secara Aman

### 1. Pastikan file target tersedia:
![](img/20260440-134030.png)

### 2. Salin file dengan nama kompleks ke folder backup:
![](img/20260442-134210.png)

### 3. Gunakan variabel untuk memproses path dengan aman:
![](img/20260444-134448.png)

### 4. Tampilkan daftar file hasil backup:
![](img/20260445-134548.png)

## Tugas Praktikum 1 — Toolkit Bash Administrator Pribadi

### Konteks riil: 
seorang administrator sering mengulang perintah yang sama setiap hari. Agar pekerjaan lebih efisien dan konsisten, ia perlu memiliki toolkit Bash pribadi yang otomatis aktif setiap login.

### Instruksi tugas:
1. Tambahkan konfigurasi pada .bashrc untuk:
- menambahkan direktori bin pribadi ke PATH,
- membuat minimal 2 alias yang membantu kerja harian 
- membuat minimal 1 fungsi shell yang berguna untuk administrasi.
1. Pastikan konfigurasi tersebut aktif kembali saat membuka shell login.
2. Buat satu script sederhana di direktori bin pribadi, misalnya script untuk
menampilkan ringkasan sistem.
1. Uji dari direktori yang berbeda untuk memastikan script dapat dipanggil tanpa
menuliskan path lengkap.
1. Simpan bukti pengujian ke file toolkit-bash-report.txt.

### Minimal luaran:
- isi blok konfigurasi yang ditambahkan ke .bashrc,
- output echo $PATH,
- output type untuk alias, fungsi, dan script,
- file laporan toolkit-bash-report.txt.

### Proses Pengerjaan Tugas
1. Persiapan Direktori Bin Pribadi
![](img/20260408-140853.png)

2. Menambahkan Konfigurasi ke `.bashrc`
![](img/20260400-140037.png)
![](img/20260402-140226.png)

3. Membuat Script Ringkasan Sistem
![](img/20260406-140633.png)
![](img/20260405-140533.png)
![](img/20260410-141054.png)

4. Aktivasi dan Pengujian
![](img/20260412-141212.png)

5. Menyimpan Bukti ke Laporan
![](img/20260414-141445.png)
![](img/20260415-141505.png)

## Tugas Praktikum 2 — Audit File Konfigurasi dan Logging Aman

### Konteks riil: 
saat troubleshooting, administrator sering perlu menginventarisasi file konfigurasi dan memisahkan output normal dari pesan error.

### Instruksi tugas:
1. Buat file laporan bernama audit-konfigurasi-$(date +%F).txt.
2. Cari file *.conf di dalam /etc dan simpan hasilnya ke file laporan.
3. Catat jumlah total file konfigurasi yang ditemukan.
4. Jika ada pesan error, simpan ke file terpisah, misalnya audit-error.log.
5. Tampilkan isi laporan ke terminal dan sekaligus simpan menggunakan tee.
6. Tambahkan ringkasan singkat 3–5 baris yang menjelaskan mengapa pemisahan stdout dan stderr penting dalam audit sistem.

### Syarat konsep yang harus muncul:
- redirection >, 2>, atau &>,
- pipeline,
- tee,
- penggunaan variabel atau command substitution.

### Minimal luaran:
- file laporan audit,
- file log error,
- perintah yang digunakan,
- analisis singkat hasil audit.

### Proses Pengerjaan Tugas
1. Menyiapkan Variabel Nama File
![](img/20260407-150747.png)

2. Proses Audit (Pencarian, Redirection, dan Tee)
![](img/20260410-151009.png)
![](img/20260410-151020.png)
![](img/20260410-151051.png)
![](img/20260411-151116.png)

3. Menghitung Total dan Menambahkan Ringkasan
![](img/20260413-151311.png)

4. File yang dibuat dan ringkasan analisis
- audit-konfigurasi-2026-04-12.txt
![](img/20260414-151443.png)
![](img/20260415-151501.png)
![](img/20260415-151514.png)
![](img/20260415-151534.png)
- audit-error.log
![](img/20260416-151647.png)

5. Perintah yang digunakan

| Komponen | Perintah/Karakter | Fungsi |
| - | - | - |
| Command Substitution | `$(date +%F)` | Membuat nama file unik berdasarkan tanggal otomatis. |
| Redirection Stdout | `>` | Membuat file laporan baru (diwakili oleh perintah tee). |
| Redirection Stderr | `2>` | Memisahkan pesan error ke audit-error.log. |
| Pipeline | `\|` | Menghubungkan output find ke input tee. |
| Tee | `tee` | Menampilkan hasil audit di layar agar bisa kamu lihat langsung sambil tetap menyimpannya ke file. |

## Tugas Praktikum 3 — Mini Health Check Harian Server

### Konteks riil:
administrator perlu membuat pemeriksaan cepat (health check) untuk mengetahui kondisi dasar server sebelum dan sesudah maintenance.

### Instruksi tugas:
1. Buat script Bash bernama daily-healthcheck pada direktori bin pribadi.
2. Script minimal harus menampilkan:
- tanggal dan waktu,
- hostname,
- user aktif,
- shell aktif,
- uptime,
- penggunaan memori,
- penggunaan filesystem root,
- 10 baris terakhir history command yang relevan dengan pengecekan.
3. Simpan hasil ke file log harian, misalnya healthcheck-$(date +%F).log.
4. Tampilkan hasil ke terminal dan ke file secara bersamaan.
5. Jika Anda menggunakan pipeline dengan tee, cek juga status exit command utama.

### Syarat konsep yang harus muncul:
- environment variable,
- PATH,
- alias atau fungsi pendukung,
- history,
- tee,
- penanganan error dasar.

### Minimal luaran:
- file script yang executable,
- contoh isi file log hasil eksekusi,
- penjelasan singkat fungsi tiap bagian script.

### Proses Pengerjaan Tugas
1. Membuat Script daily-healthcheck
![](img/20260427-152712.png)
![](img/20260430-153011.png)

2. Memberikan Izin Eksekusi
![](img/20260430-153035.png)

3. Pengujian dan Verifikasi
![](img/20260433-153314.png)

4. File yang berhasil di buat oleh Script
![](img/20260434-153447.png)

5. Penjelasan singkat fungsi tiap bagian script

| Bagian | Fungsi Teknis |
| - | - |
| `print_line()` | Sebuah fungsi internal untuk konsistensi tampilan (agar output tidak berantakan). |
| `$HOSTNAME, $USER` | Menggunakan Environment Variables bawaan Linux untuk mengambil info identitas. |
| `{ ... } \| tee` | Mengelompokkan semua perintah pengecekan agar outputnya bisa dialirkan secara bersamaan ke layar dan file log. |
| `tail ~/.bash_history` | Mengambil histori perintah langsung dari file penyimpanan Bash agar tetap muncul meskipun dijalankan dalam skrip. |
| `PIPESTATUS[0]` | "Cara cerdas untuk mengecek apakah proses pengumpulan data (di sisi kiri pipe) berhasil atau gagal, karena $? biasa hanya akan mengecek status tee." |

## Tugas Praktikum 4 — Penanganan File dengan Nama Kompleks dan Arsip Aman

### Konteks riil:
file hasil backup, ekspor, atau laporan sering memiliki nama yang mengandung spasi atau karakter khusus. Administrator harus tetap dapat memproses file-file tersebut tanpa salah target.

### Instruksi tugas:
1. Buat minimal 4 file contoh dengan nama yang bervariasi, termasuk:
- nama file yang mengandung spasi,
- nama file yang mengandung tanda kurung siku atau karakter khusus,
- file dengan pola nama serupa untuk diuji dengan wildcard.
2. Tunjukkan perbedaan hasil jika file diakses tanpa quoting dan dengan quoting
yang benar.
3. Lakukan preview wildcard dengan echo sebelum dipakai untuk operasi nyata.
4. Salin file-file tersebut ke direktori backup dengan nama yang aman.
5. Buat arsip tar.gz dari hasil backup.
6. Simpan riwayat perintah yang Anda gunakan ke file riwayat-arsip.txt.

### Syarat konsep yang harus muncul:
- single quote, double quote, dan escaping,
- wildcard,
- variabel path,
- history,
- operasi file lanjutan yang aman.

### Minimal luaran:
- daftar file awal,
- daftar file hasil backup,
- file arsip tar.gz,
- file riwayat-arsip.txt,
- refleksi singkat tentang pentingnya quoting di Bash.

### Proses Pengerjaan Tugas
1. Menyiapkan Workspace dan File Contoh
![](img/20260452-155252.png)

2. Demonstrasi Quoting
- Tanpa Quoting
![](img/20260453-155323.png)
- Dengan Quoting
![](img/20260453-155339.png)

3. Preview Wildcard dengan `echo`
![](img/20260454-155427.png)

4. Backup Menggunakan Variabel Path
![](img/20260455-155519.png)

5. Membuat Arsip Terkompresi
![](img/20260455-155534.png)

6. Menyimpan Riwayat dan Refleksi
![](img/20260456-155605.png)

### Hasil
1. Daftar file awal
![](img/20260457-155719.png)
2. Daftar file backup
![](img/20260457-155736.png)
3. File arsip
![](img/20260458-155859.png)
4. File riwayat
![](img/20260459-155924.png)
5. File refleksi
![](img/20260400-160010.png)
