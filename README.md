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
