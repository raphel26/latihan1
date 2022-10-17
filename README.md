Install Git
Download Git,buka website resminya Git git-scm.com My_Image
Kemudian Unduh git sesuai dengan arsitektur komputer anda kalau menggunakan 64 bit, unduh yang 64bit, Begitu juga kalau menggunakan 32bit.
Lalu di install
Untuk memcobanya, silahkan bukan CMD atau PowerShell kemudian ketik perintah git --version My Image
Menambah Global Config
Pada saat pertama kali menggunakan git, perlu dilakukan konfigurasi "user.name" dan "user.email"

konfigurasi inin bisa dilakukan untuk global reposity atau individual repository

Apabila belum dilakukan konfigurasi , akan mengakibatkan terjadi kegagalan saat menjadikan perintah git commit

Config Global Repository git config --global user.name "name_user My Image

git config --global user.email "email_anda"

My Image

Membuat Reposiory Local
Buka derektory aktif misal " C:/Document/LatihanVCS " buka menggunakan Windowns Expoler
Klik kanan pada direktory aktif tersebut , dan pilih menu " Git Bash " , sehingga muncul git bash command
Buat direktory project praktikum pertama dengan Latihan VCS " mkdir Latihan VCS " " Latihan VCS "
direktory aktif menjadi " C:/Document/LatihanVCS " My Image
Membuat Reposiory Local
Jalankan perintah git init, untuk membuat repository local.
Repository baru berhasil di inisialisasi, dengan terbentuknya satu direktori hidden dengan nama .git
Pada direktori tersebut, semua perubahan pada working directory akan disimpan. My Image
Menambahkan File Baru pada repository
Untuk membuat file dapat menggunakan text editor, lalu menyimpan filenya pada direktori aktif (repository)

disini kita akan coba buat satu file bernama README.md menggunakan echo "#Latihan VCS" >> README.md

File README.md berhasil dibuat

My Image

Commit ( Menyimpan perubahan ke database)
unuk menyimpanan perubahan yang ada kedalam data repository local,gunakan perintah git commit -m " Komentar commit

My Image

Membuat Reposity Server
Server reopsitory yang akan kita gunakan adalah " https://github.com "
Anda harus membuat akun terlebih dahulu
Pada website github, kilik tomboh start project, atau Dari menu (icon + ) klik New repository My Image
Isi nama repository, misal :labpy1
Lalu klik tombol Create repository My Image
Membahkan Remote Repository
Remote Repository merupakan repository server yang akan digunakan untuk menyimpan setiap perubahan pada local repository, sehingga dapat diakses oleh banyak user.
Untuk menambahkan remote repository server, gunakan perintah git remote add origin [url] My Image
Push (Mengirim Perubahan ke server)
Untuk mengirim perubahan pada local repository ke server gunakan perintah git push. git push -u origin master
Perintah ini akan meminta memasukkan username dan password pada akun github.com
Buka laman github.com arahkan pada repositori
Maka perbaruan akan terlihata pada laman tersebut.vsc vsc My Image