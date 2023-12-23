# Tutorial Git
#
## 1. Pendahuluan
Git adalah Free and Open Source Version Control System(sistem kontrol versi gratis dan terbuka) terdistribusi yang mendeteksi perubahan dalam kumpulan file komputer mana pun, umumnya digunakan untuk mengelola projek pemprograman. Git mendukung banyak bahasa pemprograman seperti Java, Python, HTML, dsb juga mendukung fotmat gambar (.JPG, .PNG, .JPEG, .SVG).  

Latar belakang Git dari projek Open Source Linux Kernel, Tahun 1991-2001 Linux Kernel hanya di develop hanya dengan menfaatkan patch dan archived files untuk mengelola projek. Lalu Tahun 2002 Linux Kernel memulai dengan DVCs bernama bitkeeper. Namum 2005 hubungan dengan perusahaan bitkeeper kurang baik, sehingga pembuat linux(Linus Torvalds) membuat DVCs sendiri yaitu Git.  

Git di perkenalkan pertama kali pada tahun 2005. Git sendiri menggunakan algoritma hashing SHA-1 dan lebih mengedepankan perubahan yang terjadi di file tersebut. Untuk website dari Git [Website Git](https://git-scm.com/). Git dapat diunduh di OS

- Windows
- Android (Terminal Package Manager Apt/Pkg)
- MacOS
- Linux

## 2. Tipe Sistem Kontrol
1. Local Version Control  
	(Version control yang berjalan pada local komputer)  

2. Centralized Version Control (subversion)  
	(Version control yang berjalan pada local dan di server(database), di local hanya versi yang terbaru dan di server full versinya )  

3. Distributed Version Control (Git dll)  
	(alternatif dari CVCs, dalam DVCs tidak hanya versi terakhirnya saja namun semua riwayat di copy, sehingga jika server down maka masih biasa berkerja) 

## 3. Terminologi
Beberapa istilah-istilah yang umum terkait Git.

- Repo = repository, sebutan projek di Git, folder kosong yang akan kita jadikan git repo
- Branch = cabang bebas dari commit seperti master, main dll
- Hash = penanda unik pada commit berupa Angka dan huruf, Git menggunakan Algoritma SHA-1, hash harus di jaga agar data tetap valid jika hash yang di belakang rusak maka data yang di depan tidak valid/rusak)
- Commit = rekaman / snapshot pada repo
- Snapshot = berisikan semua perubahan yang terjadi pada semua file yang kita commit, dan setiap snapshot akan menghasilkan hash
- Remote = sumber / sever yang memiliki repo github, gitlab
- Checkout = berpindah ke sebuah commit
- Clone = menggambil repo dari remote
- Push = mengirim commit ke repo server
- Pull = mengambil commit dari repo server
- Merge = menggabungka branch
- HEAD = pointer menuju hash paling akhir/versi terbaru
- .git = adalah isi dari repository kita.

## 4. Area pada Git
Pada saat menggunakan git terdapat area-area atau mudahnya level saat file itu berada pada git.


- Working directory [READ] = Tempat file yang belum di track / new file.
- Staging index/staging area [GREEN] = Tempat file yang sudah di track dan siap untuk commit.
- Commit [BLACK] = File sudah di commit, dan aman di repo.

## 5. Instalasi
Cara install Git di OS Windows, MacOS, Linux.

#### Instal di Windows

#### Instal di MacOS

#### Instal di Linux

## 5. Penggunaan Dasar Git
Untuk penggunaan git bisa melalui terminal (Command Line) atau antarmuka (GUI).

#### Terminal/Command Line
Untuk menggunakan terminal jika di Linux langsung bisa dijalankan, jika di windows perlu set up environtment variables. Di windows bisa dengan CMD,PowerShell,Git Terminal. Disini akan menggunakan Git Terminal & untuk repo onlinenya menggunakan Github. Sebelum menggunakan Git perlu konfigurasi.  

Konfigurasi nama.
```Bash
$ git config --global user.name "nama anda"
# Contoh
$ git config --global user.name "ifandika"
```
Lalu konfigurasi email.
```Bash
$ git config --global user.email "email anda"
# Contoh
$ git config --global user.email "ifandika014@gmail.com"
```
Untuk melihat semua konfigurasi.
```Bash
$ git config --list --show-origin
# Atau
$ git config --list
diff.astextplain.textconv=astextplain
filter.lfs.clean=git-lfs clean -- %f
filter.lfs.smudge=git-lfs smudge -- %f
filter.lfs.process=git-lfs filter-process
filter.lfs.required=true
http.sslbackend=openssl
http.sslcainfo=C:/Program Files/Git/mingw64/etc/ssl/certs/ca-bundle.crt
core.autocrlf=true
core.fscache=true
core.symlinks=false
pull.rebase=false
credential.helper=manager
credential.https://dev.azure.com.usehttppath=true
init.defaultbranch=master
user.email=ifandika014@gmail.com
user.name=ifandika
```
