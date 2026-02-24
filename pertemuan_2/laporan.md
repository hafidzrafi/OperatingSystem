# PERTEMUAN 2

## Praktikum 2.1

### 1. Menampilkan informasi CPU
![](img/20260249-194934.png)

### 2. Menampilkan ringkasan memori
![](img/20260250-195032.png)

### 3. Mengecek informasi hardware dari DMI/BIOS
![](img/20260251-195115.png)

## Latihan 2.1

### Soal
Catat: (1) jumlah CPU(s), core/thread, (2) total RAM, (3) total swap. Jelaskan perbedaan RAM vs swap dalam 2–3 kalimat.

### Jawaban
| Komponen | Detail Konfigurasi |
| --- | --- |
| Jumlah CPU(s) | 8 CPU(s) |
| Core/Thread   | 4 core/2 thread |
| Total RAM     | 8 GB |
| Total Swap    | 1 GB |

RAM adalah memori yang digunakan untuk menyimpan data program yang sedang berjalan saat ini. Sedangkan Swap adalah memori cadangan yang diambil dari SSD. Swap digunakan ketika RAM penuh dan tidak dapat menampung data dari program yang sedang berjalan, maka data tersebut disimpan di dalam Swap.

## Praktikum 2.2

### 1. Melihat daftar perangkat PCI
![](img/20260238-033830.png)

### 2. Melihat perangkat PCI beserta driver kernel yang digunakan
![](img/20260245-034501.png)

### 3. Berfokus pada NIC (Ethernet) untuk mencari modul driver
![](img/20260248-034828.png)

### 4. Melihat perangkat USB
![](img/20260239-033938.png)

### 5. Melihat topologi USB (tree)
![](img/20260239-033956.png)

## Soal Latihan 2.2

### Soal
Temukan 1 perangkat PCI (misal NIC) dan tuliskan: Vendor:Device ID (angka
heksadesimal), nama driver/modul kernel, dan deskripsi singkat fungsinya.

### Jawaban
| Komponen | Detail Konfigurasi |
| --- | --- |
| Nama Perangkat | Microsoft Corporation Basic Render Driver |
| Vendor:Device ID | 1414:008e |
| Kernel Driver in Use | dxgkrnl (DirectX Graphics Kernel) |
| Deskripsi Fungsi | Perangkat ini berfungsi sebagai pengolah grafis virtual. Driver dxgkrnl memungkinkan lingkungan WSL untuk berkomunikasi langsung dengan kartu grafis (GPU) yang ada di Windows agar bisa digunakan untuk proses rendering atau perhitungan grafis di dalam Linux. |

## Praktikum 2.3

### 1. Melihat daftar disk/partisi
![](img/20260216-041650.png)

### 2. Menampilkan UUID dan tipe filesystem
![](img/20260217-041719.png)

### 3. Melihat mount point untuk root filesystem
![](img/20260217-041740.png)

## Praktikum 2.4

### 1. Mengecek versi kernel
![](img/20260218-041808.png)

### 2. Menampilkan daftar modul aktif
![](img/20260218-041824.png)

### 3. Memilih salah satu modul (contoh aman: loop) dan melihat detail nya
![](img/20260218-041859.png)

### 4. Memuat modul (jika belum aktif), lalu memverifikasi
![](img/20260220-042002.png)

### 5. Melihat pesan kernel terbaru
![](img/20260220-042031.png)

## Praktikum 2.5

### 1. Membuat file auto-load
![](img/20260220-042054.png)

### 2. Menyimulasikan verifikasi (tanpa reboot) dengan memastikan modul sudah aktif
![](img/20260221-042129.png)

## Praktikum 2.6

### 1. Melihat detail salah satu disk (misalnya sda)
![](img/20260222-042220.png)

### 2. Melihat detail device terminal
![](img/20260222-042249.png)

### 3. Melihat disk dan partisi untuk mengaitkan dengan /dev
![](img/20260223-042307.png)

## Soal Latihan 2.3

### Soal
Dari output `ls -l`, jelaskan perbedaan penanda file untuk block device dan
character device. (Hint: karakter pertama pada permission string)

### Jawaban
Dalam Linux, tipe file dapat diidentifikasi melalui karakter pertama pada string perizinan (permission string) yang muncul saat menjalankan perintah ls -l

**1. Character Device (c)**
| Komponen | Detail |
| --- | --- |
| Penanda | Karakter pertama adalah huruf c. |
| Penjelasan | Perangkat ini mengirimkan atau menerima data sebagai aliran karakter (byte demi byte) secara berurutan. Perangkat ini tidak memiliki mekanisme buffering internal yang kompleks. |
| Contoh | Terminal (/dev/tty), keyboard, dan mouse. |

**1. Block Device (b)**
| Komponen | Detail |
| --- | --- |
| Penanda | Karakter pertama adalah huruf b. |
| Penjelasan | Perangkat ini mengelola data dalam bentuk blok-blok (kumpulan byte) dengan ukuran tertentu. Perangkat ini memungkinkan akses data secara acak (random access) dan memiliki buffer untuk meningkatkan performa. |
| Contoh | Hard disk, SSD, dan partisi sistem (/dev/sda, /dev/nvme0n1). |

## Praktikum 2.7

### 1. Mengecek atribut udev untuk disk
![](img/20260233-043314.png)

### 2. Mengecek monitor event udev
![](img/20260251-045110.png)

## Praktikum 2.8

### 1. Membuat direktori praktikum dan masuk ke dalamnya
![](img/20260242-044244.png)

### 2. Membuat beberapa file contoh
![](img/20260243-044345.png)

### 3. Mengisi file log
![](img/20260245-044557.png)

### 4. Membaca file dengan less
![](img/20260248-044836.png)

## Praktikum 2.9

### 1. Mencari baris yang mengandung ERROR pada data.log
![](img/20260249-044932.png)

### 2. Mencari tanpa memperhatikan huruf besar/kecil
![](img/20260250-045009.png)

### 3. Menampilkan nomor baris
![](img/20260250-045032.png)

### 4. Menampilkan baris yang tidak cocok (invert match)
![](img/20260250-045053.png)

## Latihan 2.4

### Soal
Gunakan grep untuk menampilkan hanya baris yang mengandung INFO atau
WARN dari data.log. (Hint: gunakan grep -E dengan pola alternatif)

### Jawaban 
![](img/20260252-045230.png)

## Praktikum 2.10

### 1. Menyiapkan file konfigurasi latihan
![](img/20260259-045923.png)

### 2. Mengganti dev menjadi prod (tanpa mengubah file asli)
![](img/20260200-050020.png)

### 3. Menerapkan perubahan langsung ke file (-i)
![](img/20260201-050131.png)

### 4. Mengganti semua kemunculan kata (g untuk global), misalnya mengubah myserver menjadi node
![](img/20260202-050236.png)

## Praktikum 2.11

### 1. Melihat output df -h
![](img/20260202-050253.png)

### 2. Mengambil kolom filesystem dan presentase pemakaian
![](img/20260203-050337.png)

### 3. Memfilter hanya yang pemakaian disk di atas 80%
![](img/20260204-050407.png)

## Praktikum 2.12

### 1. Menampilkan semua proses (format BSD)
![](img/20260204-050425.png)

### 2. Mencari proses tertentu (misal sshd)
![](img/20260204-050447.png)

## Praktikum 2.13

### 1. Menjalankan top
![](img/20260205-050516.png)

### 2. Mengamati nilai load average, pemakaian CPU, dan proses teratas
![](img/20260206-050601.png)

## Praktikum 2.14

### 1. Menjalankan proses dummy di background
![](img/20260206-050623.png)

### 2. Mencari PID proses sleep
![](img/20260206-050649.png)

### 3. Menghentikan dengan SIGTERM
![](img/20260209-050930.png)

### 4. Memverifikasi proses berhenti
![](img/20260210-051000.png)

## Praktikum 2.15

### 1. Mengecek penggunaan disk
![](img/20260210-051050.png)

### 2. Mencari direktori yang besar (contoh pada /var)
![](img/20260212-051233.png)

### 3. Mengecek load dan uptime
![](img/20260212-051255.png)

### 4. Mengecek service yang gagal
![](img/20260213-051320.png)

### 5. Mengambil log error terbaru (jika ada indikasi masalah)
![](img/20260213-051343.png)

## Praktikum 2.16

### 1. Melihat interface dan IP
![](img/20260214-051406.png)

### 2. Melihat routing table
![](img/20260214-051421.png)

### 3. Melihat port yang sedang listening
![](img/20260214-051445.png)

## Latihan 2.5

### Soal
Pilih satu port yang listening dari output ss -tulpn(misal port 22), lalu
tuliskan service/proses yang membukanya. Jelaskan kegunaan port tersebut
secara singkat.

### Jawaban
![](img/20260221-052108.png)

| Komponen | Detail |
| --- | --- |
| Nomor Port | 53 |
| Protokol | TCP/UDP |
| Service/Proses yang membukanya | systemd-resolved (Layanan DNS lokal) |
| Kegunaan | Port 53 adalah port standar untuk layanan DNS (Domain Name System). Kegunaannya adalah untuk menerjemahkan nama domain yang mudah diingat manusia (seperti google.com) menjadi alamat IP yang dipahami oleh komputer. Tanpa port ini yang berfungsi sebagai listening, sistem tidak akan bisa mencari alamat server di internet. |

## Latihan 2.A

### Soal
Jalankan lspci -nnk. Pilih 1 perangkat PCI dan tuliskan: nama perangkat,
ID vendor:device, dan kernel driver in use.

### Jawaban
![](img/20260225-052546.png)

| Komponen | Detail |
| --- | --- |
| Komponen | Detail Informasi |
| Nama Perangkat | 3D controller: Microsoft Corporation Basic Render Driver |
| ID Vendor:Device | 1414:008e |
| Kernel Driver in Use | dxgkrnl |


## Latihan 2.B

### Soal
Tentukan device root filesystem dengan findmnt /. Lalu cocokkan dengan
lsblk -f dan tuliskan tipe filesystem serta UUID-nya.

### Jawaban
![](img/20260234-053428.png)

| Komponen | Detail |
| --- | --- |
| Device Root | /dev/sdf |
| Tipe Filesystem | ext4 |
| UUID | fc8bdcea-e6e5-4569-9a8c-d3697cc4c8f9 |


## Latihan 2.C

### Soal
Buat file server.log berisi minimal 10 baris dengan variasi kata: INFO,
WARN, ERROR. Gunakan grep untuk menampilkan hanya baris ERROR.

### Jawaban
![](img/20260237-053738.png)

Pertama, saya membuat file log menggunakan fitur Heredoc (EOF) untuk efisiensi. Kemudian, saya menggunakan perintah grep untuk memfilter (ERROR).

## Latihan 2.D

### Soal
Gunakan sed untuk mengganti semua kata server menjadi node pada file
latihan. Tunjukkan sebelum dan sesudah.

### Jawaban
![](img/20260243-054316.png)

## Latihan 2.E

### Soal
Gunakan df -h lalu awk untuk menampilkan filesystem yang penggunaan disk
di atas 70%.

### Jawaban
![](img/20260246-054636.png)

## Latihan 2.F

### Soal
Jalankan sleep 600 &. Temukan PID-nya dengan ps. Hentikan dengan
SIGTERM. Jelaskan beda SIGTERM vs SIGKILL.

### Jawaban
![](img/20260251-055121.png)
![](img/20260252-055222.png)

| Fitur | SIGTERM | SIGKILL |
| --- | --- | --- |
| Cara Kerja | Meminta program berhenti secara "sopan" | Memaksa program berhenti seketika |
| Proses | Program diberi kesempatan untuk menyimpan data dan menutup koneksi (bersih-bersih) | Program langsung dimatikan oleh kernel |
| Kapan Digunakan | Digunakan sebagai langkah pertama untuk mematikan program | Digunakan hanya jika program sudah benar-benar macet (hang) dan tidak bisa dimatikan dengan cara biasa |

## Latihan 2.G

### Soal
Gunakan systemctl –failed. Jika tidak ada yang gagal, pilih satu service
aktif (misal ssh) dan tampilkan status serta 30 baris log terakhirnya.

### Jawaban
![](img/20260258-055839.png)

Setelah menjalankan perintah systemctl --failed, ditemukan bahwa tidak ada layanan yang gagal pada sistem saya. Oleh karena itu, saya memilih layanan cron untuk dianalisis lebih lanjut.

1. Status Layanan `systemctl status cron`
![](img/20260258-055858.png)

1. Log Layanan `journalctl -u cron -n 30`:
![](img/20260259-055934.png)
