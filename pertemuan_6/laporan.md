# PERTEMUAN 6

## Praktikum 6.1

### Tampilkan semua proses yang berjalan:
![](img/20260459-165944.png)

### Tampilkan proses beserta thread-nya, dapat dilihat pada kolom LWP (Light-Weight Process ID):
![](img/20260400-170022.png)

### Lihat PID shell aktif dan detail prosesnya:
![](img/20260401-170113.png)

### Lihat hierarki proses secara visual:
![](img/20260401-170134.png)

## Latihan 6.1
**Jalankan ps aux dan amati output nya:**

1. Berapa total proses yang berjalan? Proses apa yang memiliki PID terkecil?

2. Jalankan pstree -p dan temukan proses bash Anda. Proses apa yang menjadi induk (PPID) dari bash tersebut?

3. Bandingkan output ps aux dan ps aux -L. Apa perbedaan yang Anda lihat?

## Praktikum 6.2

### Buat proses di background dan amati kondisinya:
![](img/20260402-170236.png)

### Amati perubahan exit code dari perintah yang berhasil dan gagal:
![](img/20260403-170327.png)

## Latihan 6.2
1. Jalankan sleep 120 & dan amati kolom STAT pada ps aux. Kondisi
apa yang ditampilkan? Mengapa proses sleep berada di kondisi tersebut?

1. Jalankan beberapa perintah yang berhasil dan yang gagal, lalu catat exit
code masing-masing. Pola apa yang Anda temukan?

## Praktikum 6.3

### Jalankan proses dengan prioritas rendah:
![](img/20260403-170349.png)

### Verifikasi nilai nice pada kolom NI:
![](img/20260404-170405.png)

### Ubah nilai nice proses yang sudah berjalan:
![](img/20260408-170835.png)

### Bersihkan proses percobaan:
![](img/20260409-170909.png)

## Latihan 6.3
1. Jalankan nice -n 5 sleep 200 & dan verifikasi nilai NI-nya dengan ps.

2. Coba ubah nilai nice menjadi -5 tanpa sudo. Apa yang terjadi? Mengapa

3. Ubah nilai nice menjadi 10 menggunakan renice, lalu verifikasi kembali. Linux membatasi hal ini untuk user biasa?

## Praktikum 6.4

### Buat proses percobaan:
![](img/20260409-170954.png)

### Hentikan satu proses dengan SIGTERM dan verifikasi:
![](img/20260412-171204.png)

### Jeda dan lanjutkan proses dengan SIGSTOP/SIGCONT:
![](img/20260413-171335.png)

### Hentikan semua proses sleep sekaligus:
![](img/20260413-171358.png)

## Latihan 6.4
1. Jalankan sleep 400 &, kirim SIGSTOP, dan amati perubahan kolom STAT. Kondisi apa yang muncul?

2. Kirim SIGCONT dan verifikasi proses kembali berjalan.

3. Hentikan proses dengan SIGTERM lalu verifikasi sudah tidak ada. Kapan Anda memilih SIGKILL daripada SIGTERM?

## Praktikum 6.5

### Jalankan tiga job di background:
![](img/20260414-171432.png)

### Bawa job pertama ke foreground, jeda, lalu kembalikan ke background:
![](img/20260415-171522.png)

### Hentikan semua job:
![](img/20260416-171607.png)

## Latihan 6.5
1. Jalankan top di foreground. Apa yang terjadi di terminal?

2. Tekan Ctrl+Z dan cek statusnya dengan jobs. Kondisi apa yang ditampilkan?

3. Pindahkan ke background dengan bg. Apakah top dapat berjalan dengan baik di background? Mengapa?

4. Kembalikan ke foreground dengan fg, lalu keluar dengan q .

## Praktikum 6.6

### Temukan proses dengan penggunaan CPU dan memori tertinggi:
![](img/20260418-171842.png)

### Jalankan top dan eksplorasi shortcut-nya:
![](img/20260420-172022.png)

#### M
![](img/20260420-172054.png)
![](img/20260421-172114.png)
![](img/20260421-172130.png)

#### p (unknown command)
![](img/20260421-172157.png)

#### 1
![](img/20260423-172318.png)

#### u
![](img/20260423-172347.png)

#### q
![](img/20260424-172425.png)

### Instal dan jalankan htop:
![](img/20260425-172515.png)

## Latihan 6.6
1. Gunakan ps aux –sort=%mem untuk menemukan proses yang menggu- nakan memori paling banyak di VM Anda. Proses apa itu?

2. Di dalam top, tekan 1 . Apa yang berubah pada tampilan? Mengapa informasi ini berguna?

3. Di dalam htop, navigasikan ke proses sshd menggunakan tombol panah. Tekan F9 dan amati opsi sinyal yang tersedia.

## Latihan

### Latihan 6.A
**Eksplorasi Proses Sistem**
1. Jalankan ps aux –forest dan temukan proses dengan PID 1. Apa nama dan fungsi proses tersebut dalam sistem Linux modern?

2. Hitung berapa proses yang dimiliki oleh user root dan berapa yang dimiliki oleh user Anda. Mengapa root memiliki lebih banyak proses?

3. Temukan semua proses yang berada dalam kondisi S. Mengapa sebagian besar proses di sistem berada dalam kondisi ini?
 
### Latihan 6.B
**Simulasi Manajemen Job**
1. Jalankan tiga perintah sleep dengan durasi 100, 200, dan 300 detik di background. Verifikasi ketiganya dengan jobs.

2. Bawa job kedua ke foreground, jeda dengan Ctrl+Z , lalu kembalikan ke background dengan bg.

3. Hentikan job pertama dengan kill %1. Tampilkan kembali daftar job. Berapa job yang tersisa?
 
### Latihan 6.C
**Prioritas dan Sinyal**
1. Jalankan dua proses sleep: satu dengan nice +5 dan satu dengan nice +15. Verifikasi nilai NI keduanya dengan ps.

2. Gunakan renice untuk mengubah nice proses pertama menjadi +10. Proses mana yang kini lebih diprioritaskan scheduler?

3. Kirim SIGSTOP ke salah satu proses, verifikasi kondisi T-nya, lalu kirim SIGCONT. Akhiri semua proses percobaan dengan pkill sleep.

 