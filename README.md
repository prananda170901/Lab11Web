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
