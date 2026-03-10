# PERTEMUAN 4

## Latihan

### Soal 1
Cobalah urutan perintah berikut

`$ cd`
![](img/20260347-224739.png)

```$ pwd```
![](img/20260348-224805.png)

```$ ls –al```
![](img/20260348-224846.png)

```$ cd .```
![](img/20260348-224859.png)

```$ pwd```
![](img/20260349-224911.png)

```$ cd ..```
![](img/20260349-224928.png)

```$ pwd```
![](img/20260349-224943.png)

```$ ls -al```
![](img/20260349-224952.png)

```$ cd ..```
![](img/20260350-225009.png)

```$ pwd```
![](img/20260350-225033.png)

```$ ls -al```
![](img/20260350-225043.png)

```$ cd /etc```
![](img/20260350-225054.png)

```$ ls –al | more```
![](img/20260351-225114.png)

```$ cat passwd```
![](img/20260352-225207.png)

```$ cd –```
![](img/20260352-225220.png)

```$ pwd```
![](img/20260352-225230.png)

### Soal 2
Lanjutkan penelusuran pohon pada sistem file menggunakan `cd`, `ls`, `pwd` dan `cat`. Telusuri directory `/bin`, `/usr/bin`, `/sbin`, `/tmp` dan `/boot`.

```/bin```
![](img/20260355-225532.png)

```/usr/bin```
![](img/20260358-225809.png)

```/sbin```
![](img/20260358-225823.png)

```/tmp```
![](img/20260359-225904.png)

```/boot```
![](img/20260301-230106.png)

### Soal 3
Telusuri directory `/dev`. Identifikasi perangkat yang tersedia. Identifikasi `tty` (terminal) Anda (ketik `who am i`); siapa pemilih tty Anda (gunakan `ls –l`).
![](img/20260335-233517.png)

### Soal 4
Telusuri directory `/proc`. Tampilkan isi file `interrupts`, `devices`, `cpuinfo`, `meminfo` dan `uptime` menggunakan perintah `cat`. Dapatkah Anda melihat mengapa directory `/proc` disebut pseudo -filesystem yang memungkinkan akses ke struktur data kernel ?

`interrupts`
![](img/20260341-234117.png)

`devices`
![](img/20260341-234138.png)

`cpuinfo`
![](img/20260342-234206.png)

`meminfo`
![](img/20260342-234221.png)

`uptime`
![](img/20260342-234236.png)

#### Mengapa disebut pseudo-filesystem?
Karena isinya berubah-ubah secara real-time mengikuti kondisi hardware, sehingga data ini tidak memakan tempat di penyimpanan.

### Soal 5
Ubah lah directory home ke user lain secara langsung menggunakan `cd ~username`.
![](img/20260345-234547.png)
di linux ku hanya ada user ku sendiri, jadi aku tidak bisa pindah ke directory user lain, namun perintah `cd ~username` digunakan untuk pindah secara langsung ke directory user tertentu

### Soal 6
Ubah kembali ke directory home Anda.
![](img/20260347-234759.png)
seperti yang aku jelaskan sebelumnya, di linux ku hanya ada user ku saja, jadi aku tetap di directory `/home` milikku

### Soal 7
Buat subdirectory `work` dan `play`.
![](img/20260352-235231.png)

### Soal 8
Hapus subdirectory `work`.
![](img/20260352-235257.png)

### Soal 9
Copy file `/etc/passwd` ke directory home Anda.
![](img/20260355-235509.png)

### Soal 10
Pindahkan ke subdirectory `play`.
![](img/20260355-235533.png)

### Soal 11
Ubah lah ke subdirectory `play` dan buat symbolic link dengan nama `terminal` yang menunjuk ke perangkat tty. Apa yang terjadi jika melakukan hard link ke perangkat tty ?
![](img/20260357-235716.png)

### Soal 12
Buatlah file bernama `hello.txt` yang berisi kata ”`hello word`”. Dapatkah Anda gunakan `”cp”` menggunakan ”terminal” sebagai file asal untuk menghasilkan efek yang sama ?

### Soal 13
Copy `hello.txt` ke terminal. Apa yang terjadi ?

### Soal 14
Masih directory home, copy keseluruhan directory `play` ke directory bernama `work` menggunakan symbolic link.

### Soal 15
Hapus directory `work` dan isinya dengan satu perintah
