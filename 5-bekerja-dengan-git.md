# Bekerja dengan Git

## NIM - Nama:
### 16921055 - Hafizh Renanto Akhmad

<p>&nbsp;</p>

## Instalasi
1. Kunjungi https://git-scm.com
2. Lihat gambar monitor berwarna hijau di sebelah kanan dan tekan tombol berawalan `Download` untuk mendownload versi terbaru sesuai dengan OS kalian. File format ```.exe``` akan otomatis terunduh.
3. Buka file `.exe` tersebut.
4. Lanjutkan instalasi sesuai dengan keinginan.

<p>&nbsp;</p>

## Git Bash dan Command Prompt
Git Bash adalah terminal khusus untuk Git yang bisa menerima perintah shell/bash. Di sini lah tempat operasi menggunakan Git. Walaupun ada Git Bash, CMD dari Windows juga akan mempunyai kemampuan untuk menerima perindah Git. Saat proses instalasi, kita juga akan diminta memilih darimana saja Git bisa diperintah.

<p>&nbsp;</p>

## 3 Area pada Repo
Setelah Git terinstall, Git mengenal 3 tempat:
- Working tree; folder biasa yang diisi dengan kerjaan.
- Staging area; memberi tahu Git bahwa kita melakukan perubahan
- History; jika melakukan commit, akan masuk dalam _history_.
Setelah folder diinisasi sebagai repo, akan tercipta folder `.git`. Folder ini juga tempat dari 'Staging area' dan 'History' tersimpan.

## Command dalam Git
### `$ git`
Command ini seperti _help_: menampilakn beberapa command yang dapat digunakan. Command ini juga dapat digunakan di CMD untuk memerika apakah Git telah terinstal atau tidak.

### `$ pwd` dan `$ cd`
Ketika Git Bash dibuka, direktori aktif nya ada di user yang sedang digunakan (c/Users/\<user saat ini\>). Command `pwd` dapat digunakan untuk mengecek direktori saat itu. Command `cd` digunakan untuk mengubah direktori aktif dari Git Bash. Contoh:

![](https://cdn.discordapp.com/attachments/941700810335744010/941700817080164382/unknown.png)

_Di sini, saya memindahkan direktori aktif ke C:\Users\hafiz\Downloads dari C:\Users\hafiz_

### `$ ls`
Command ini digunakan untuk melihat isi dari direktori yang sedang aktif.

![](https://cdn.discordapp.com/attachments/941700810335744010/941702889250889768/unknown.png)

### `$ git init`
`git init` adalah command untuk menginisiasi suatu folder menjadi suatu repository. Contoh:

![](https://cdn.discordapp.com/attachments/941700810335744010/941701851408130078/unknown.png)

_Misalnya saya ingin membuat repository di folder 'hello-world'_

### `$ git status` dan `$ git add <file(s)>`
Saat sudah menjadi repository, segala perubahan yang terjadi akan dicatat oleh Git.

Misalkan saya membuat file baru bernama `helloworld.py` di folder 'hello-world'. Ketika kita lakukan command `git status`, maka akan muncul seperti di gambar.

![](https://cdn.discordapp.com/attachments/941700810335744010/941707354393698304/unknown.png)

Ada beberapa informasi:
- lokasi branch
- riwayat commit
- files yang untracked 

Hal ini terjadi karena file `helloworld.py` belum ada di staging area. Cara menyimpan ke staging area adalah dengan:
```
$ git add <nama file>
```
untuk satu file dan
```
# git add .
```
untuk semua file yang belum masuk ke staging area.

Cek dengan `git status` lagi, maka akan didapati hal berikut.

![](https://cdn.discordapp.com/attachments/941700810335744010/941708191127973918/unknown.png)

Sekarang, bisa dilanjutkan proses commit.

### `$ git commit`
Pertama-tama, jika kita menulis command `git commit`, Git Bash akan meminta identitas pengguna seperti di gambar.

![](https://cdn.discordapp.com/attachments/941700810335744010/941712591493922896/unknown.png)

Jika sebelumnya belum pernah menggunakan Git di device yang dipakai, kita diminta untuk memasukkan email dan nama beruturut-turut dengan menggunakan command
```
$ git config --global user.email "<email>"
```
dan
```
$ git config --global user.name "<Nama>"
```
Agar koneksinya gampang, email dan nama disesuaikan dengan informasi di akun GitHub.
Contoh input:

![](https://cdn.discordapp.com/attachments/941700810335744010/941713544473350204/unknown.png)

Sekarang, kita bisa melakukan commit.

```
$ git commit -m "<informasi tentang commit>"
```

![](https://cdn.discordapp.com/attachments/941700810335744010/941772097397604372/unknown.png)