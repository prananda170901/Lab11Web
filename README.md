# Lab11Web

## Nama : Prananda Aditya

## NIM : 312010130

## Kelas : TI.20.A1

## Matkul : Pemoggraman Web

# Langkah-langkah Praktikum

## Persiapan

<br>Sebelum memulai menggunakan Framework Codeigniter, perlu dilakukan konfigur pada webserver. Beberapa ekstensi PHP perlu diaktifkan untuk kebutul penembangan Codengniter 4.

<br>Berikut beberapa ekstensi yang perlu diaktifkan
<br>> php-json ekstension untuk bekerja dengan JSON
<br>> php-mysqlnd native driver untuk MYSQL;
<br>> php-xml ekstension untuk bekerja dengan XML;
<br>> php-intl ekstensi untuk membuat aplikasi multibahasa;
<br>> libcurl (opsional), jika ingin pakai curl

<br>Untuk mengaktifkan ekstentsi tersebut, melalu XAMPP Control Panel, pada bagian
Apache klik Config -> PHP.ini
![p](img/SS1.png)
<br>Pada bagian extention, hilangkan tanda ; (titik koma) pada ekstensi yang akan
diaktifkan. Kemudian simpan kembali filenya dan restart Apache web server.
![P](img/SS2.png)

## Instalsasi Codeigniter 4

<br>Untuk melakukan instalasi Codeigniter 4 dapat dilakukan dengan 2 cara, yaitu cara manual dan menggunakan composer. pada praktikum ini kita menggunkan cara manual.
<br>> Unduh Codeigniter dari Website https://codeigniter.com/download
<br>> Ektak zip Codeigniter ke direktori htdoc/lab11_ci.
<br>> Ubah nama direktory framework-4.x.xx maenjadi ci4.
<br>> Buka browser dengan alamat http://localhost/lab11_ci/ci4/public/
![p](img/SS3.png)

## Menjalankan CLI(Command line Interface)

<br>Codeigniter 4 menyediakan CLI untuk mempermudah proses development. Untuk mengakses CLI buka terminal/Command prompt.
![p](img/SS4.png)
<br>Arahkan lokasi direktori sesuai dengan direktori kerja project dibuat(xampp/htdocs/lab11_ci/ci4)

<br>Perintah yang dapat dijalankan untuk memanggil CLI Codeigniter adalah :

```
php spark
```

![p](img/SS5.png)

## Mengaktifkan Mode Debugging

<br>Codeigniter 4 menyediakan fitur debugging untuk memudahkan developer untuk
mengetahui pesan error apabila terjadi kesalahan dalam membuat kode program.
<br>Secara default fitur ini belum aktif. Ketika terjadi error pada aplikasi akan ditampilkan
pesan kesalahan seperti berikut.
![p](img/SS6.png)
<br>Semua jenis error akan ditampilkan sama. Untuk memudahkan mengetahui jenis
errornya, maka perlu diaktifkan mode debugging dengan mengubah nilai konfigurasi
pada environment variable CI_ENVIRINMENT menjadi development.
![p](img/SS7.png)
<br>Ubah nama file env menjadi .env kemudian buka file tersebut dan ubah nilai variable CI_ENVIRINMENT menjadi development.
<br>Contoh error yang terjadi. Untuk mencoba error tersebut, ubah kode pada file app/Controller/Home.php hilangkan titik koma pada akhir kode.
![p](img/SS8.png)

## Struktur Direktori

<br>Untuk lebih memahami Framework Codeigniter 4 perlu mengetahui struktur direktori dan file yang ada. Buka pada Windows Explorer atau dari Visual Studio Code -> Open Folder.
<br> Terdapat beberapa direktori dan file yang perlu dipahami fungsi dan kegunaannya.
<br>• .github folder ini kita butuhkan untuk konfigurasi repo github, seperti konfigurasi untuk build dengan github action;
<br>• app folder ini akan berisi kode dari aplikasi yang kita kembangkan;
<br>• public folder ini berisi file yang bisa diakses oleh publik, seperti file index.php, robots.txt, favicon.ico, ads.txt, dll;
<br>• tests folder ini berisi kode untuk melakukan testing dengna PHPunit;
<br>• vendor folder ini berisi library yang dibutuhkan oleh aplikasi, isinya juga termasuk kode core dari system CI.
<br>• writable folder ini berisi file yang ditulis oleh aplikasi. Nantinya, kita bisa pakai untuk menyimpan file yang di-upload, logs, session, dll.

<br>Sedangkan file - file yang berada pada root direktori CI sebagai Berikut
<br>.env adalah file yang berisi variable environment yang dibutuhkan oleh aplikasi.
<br>.gitignore adalah file yang berisi daftar nama file dan folder yang akan diabaikan oleh git.
<br>build adalah script untuk mengubah versi codeigniter yang digunakan ada versi release (stabil) dan development (labil).
