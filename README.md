#latihan1


## Menambahkan Global Config ##
- Pada saat pertama kali menggunakan git, perlu dilakukan konfigurasi
user.name dan user.email
- konfigurasi ini bisa dilakukan untuk global repostiry atau individual
repository.
- apabila belum dilakukan konfigurasi, akan mengakibatkan terjadi
kegagalan saat menjalankan perintah git commit
- Config Global Repository

	>> $ git config --global user.name �nama_user�

	![GitHub Logo](g.png)
	>> $ git config --global user.email �email_user�

	![GitHub Logo](h.png)
## Perintah Dasar Git ##
- git init, perintah untuk membuat repository local
- git add, perintah untuk menambahkan file baru, atau perubahan
pada file pada staging sebelum proses commit.
- git commit, perintah untuk menyimpan perubahan kedalam database
git.
- git push -u origin master, perintah untuk mengirim perubahan pada
repository local menuju server repository.
- git clone [url], perintah untuk membuat working directory yang
diambil dari repositry sever.
- git remote add origin [url], perintah untuk menambahkan remote
server/reopsitory server pada local repositry (working directory)
Membuat Reposiory Local
- Buka direktory aktif, misal: d:\labs_pemrograman1 (buka
menggunakan Windows Explorer)
- klik kanan pada direktory aktif tersebut, dan pilih menu Git Bash,
sehingga muncul git bash commad
- Buat direktory project praktikum pertama dengan nama latihan1
- Sehingga terbentuk satu direktori baru dibawahnya, selanjutnya
masuk kedalam direktori tersebut dengan perintah cd (change
directory)
- direktory aktif menjadi: d:\labs_pemrograman1\latihan1

	>> $ mkdir latihan1

	>> $ cd latihan1

	![GitHub Logo](a.png)

## Membuat Repository Local ##
- Jalankan perintah git init, untuk membuat repository local.
- Repository baru berhasil di inisialisasi, dengan terbentuknya satu
direktori hidden dengan nama .git
- Pada direktori tersebut, semua perubahan pada working directory
akan disimpan.

	>> $ git init
	
	![GitHub Logo](c.png)

## Menambahkan File baru pada repository ##
- Untuk membuat file dapat menggunakan text editor, lalu menyimpan
filenya pada direktori aktif (repository)
- disini kita akan coba buat satu file bernama README.md (text file)
- File README.md berhasil dibuat.

	>> $ echo �#Latihan 1� >> README.md

	![GitHub Logo](b.png)
## Menambahkan File baru pada repository ##
- Untuk menambahkan file yang baru saja dibuat tersebut gunakan
perintah git add.
- File README.md berhasil ditambahkan.

	>> $ git add README.md

	![GitHub Logo](f.png)
## Commit (Menyimpan perubahan ke database) ##
- Untuk menyimpan perubahan yang ada kedalam database repository
local, gunakan perintah git commit -m �komentar commit�
- Perubahan berhasil disimpan.

	>> $ git commit -m �File pertama saya�

	![GitHub Logo](d.png)
## Membuat repository server ##
- Server reopsitory yang akan kita gunakan adalah http://github.com
- Anda harus membuat akun terlebih dahulu.
- Pada laman github, klik tombol start a project, atau
- Dari menu (icon +) klik New Repository

## Membuat repository server ##
- Isi nama repositorynya, misal: labpy1.
- lalu klik tombol Create repository

## Menambahkan Remote Repository ##
- Remote Repository merupakan repository server yang akan
digunakan untuk menyimpan setiap perubahan pada local repository,
sehingga dapat diakses oleh banyak user.
- Untuk menambahkan remote repository server, gunakan perintah
git remote add origin [url]

	>> $ git remote add origin https://github.com/..../....git

	![GitHub Logo](e.png)
## Push (Mengirim perubahan ke server) ##
- Untuk mengirim perubahan pada local repository ke server gunakan
perintah git push.
- Perintah ini akan meminta memasukkan username dan password
pada akun github.com

	>> $ git push -u origin master

	![GitHub Logo](i.png)

## Melihat hasilnya pada server repository ##
- Buka laman github.com,
arahkan pada repositorinya.
- Maka perubahan akan
terlihat pada laman
tersebut.

## Clone Repository ##
- Clone repository, pada dasarnya adalah meng-copy repository server
dan secara otomatis membuat satu direktory sesuai dengan nama
repositorynya (working directory).
- Untuk melakukan cloning, gunakan perintah git clone [url]
Kegunaan file README.md
- Apabila kita menggunakan github, untuk memberikan penjelasan
awal pada project yang kita buat, maka dapat menggunakan sebuah
file yang bernama README.md
- Pada file tersebut kita dapat membuat dokumentasi awal dari setiap
project yang kita buat untuk memberikan penjelasan atau sekedar
cara penggunaan dari aplikasi yang kita kembangkan.
- Penulisan file README.md berbasis teks, dan untuk pemformatannya
menggunakan Markdown format.
- untuk lebih jelasnya, dapat anda pelajari cara penggunaan markdown
pada url berikut: https://guides.github.com/features/masteringmarkdown/
Latihan
- Buatlah satu repository Latihan1
- Buat file README.md, lalu isi file tersebut dengan penjelasan
(tutorial) cara penggunaan git, dan langkah-langkahnya lengkapi juga
dengan screenshot prosesnya.