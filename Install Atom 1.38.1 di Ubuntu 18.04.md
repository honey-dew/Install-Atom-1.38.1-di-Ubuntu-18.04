---
title: "Install Atom 1.38.1 di Ubuntu 18.04"
output: github_document
---

## Prerequisite

Sebelum Menginstall Atom versi 1.38.1 pastikan hal-hal berikut ini:

- Ubuntu 18.04 LTS sudah terinstal
- Komputer dapat terkoneksi dengan internet, dan
- Bisa menggunakan perintah-perintah dasar pada terminal linux seperti cara untuk berpindah directory dan sebagainya.

## Install Atom versi 1.38.1

Atom merupakan salah satu teks editor yang bisa didownload secara gratis dan berikut ini adalah screenshot web untuk [mendownload](https://github.com/atom/atom/releases/tag/v1.38.1) Atom versi 1.38.1. Ada beberapa file yang bisa didownload, dan file yang akan didownload adalah file bernama **atom-amd64.tar.gz** yang berukuran 148 MB. Klik pada file tersebut untuk mendownloadnya.

<img src="Image/Download atom 1.38.1.png">

Setelah terdownload maka file akan berada di folder Download. Masuk ke folder Download tersebut untuk mengekstaknya.

- Buka terminal dengan menekan **Ctrl+Alt+T**.
- Ketikan **cd Downloads/** untuk masuk ke folder Download.
- Untuk mengecek apakah file yang sudah didownload berada di folder tersebut ketik **ls -la**.
- Ekstak file **atom-amd64.tar.gz**, dan kali ini file akan di ekstak di folder /opt.
- Ketik **cd /opt/** unuk masuk ke folder opt.
- Pada folder tersebut ketikan **sudo tar -xvf ~/Downloads/atom-amd64.tar.gz**.

<img src="Image/Ekstrak file atom 1.38.1.png">

File **atom-amd64.tar.gz** berahsil diekstrak dan sekarang pada folder opt terdapat folder **atom-1.38.1-amd64**. Ketik **ls -la** untuk mengecek kembali is folder opt. Selanjutnya folder **atom-1.38.1-amd64** akan dirubah kepemilikannya dengan mengetikan **sudo chown -R root:root atom-1.38.1-amd64/** menjadi milik user root dan merubah hak aksesnya dengan mengetikan **sudo chmod 755 atom-1.38.1-amd64/** agar tidak bisa sembarangan di rubah.

<img src="Image/Ganti owner dan hak akses.png">

Sampai dengan saat ini Atom versi 1.38.1 sudah berhasil diinstall.

## Membuat Launcher Atom versi 1.38.1

Untuk mempermudah di dalam menggunakan Atom yang sudah terinstall tersebut, langkah selanjutnya yaitu membuat launcher dengan cara berikut ini:

- Buka terminal dengan menekan **Ctrl+Alt+T**.
- Ketikan **cd /usr/share/applications**.
- Ketik **sudo nano atom.desktop** untuk membuat launcher.
- Isi file **atom.desktop** tersebut seperti gambar di bawah ini.

<img src="Image/Atom desktop.png">

- Simpan file tersebut dengan menekan **Ctrl+X** lalu tekan **Y** kemudian tekan **Enter**.

_note: untuk Icon pada file atom.desktop bisa dirubah sesuai gambar yang diinginkan, dan simpan gambar yang diinginkan pada folder atom-1.38.1-amd64_.

Launcher sudah berhasil dibuat, dan untuk mengeceknya tekan tombol windows pada keyboard lalu ketikan atom. Jika berhasil maka hasilnya seperti gambar di bawah ini.

<img src="Image/Atom launcher.png">

Atom versi 1.38.1 sudah siap untuk digunakan.