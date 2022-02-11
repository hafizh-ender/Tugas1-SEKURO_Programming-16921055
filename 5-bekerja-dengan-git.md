# Bekerja dengan Git

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

## 3 area pada repo
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

Ada beberapa informasi:
- lokasi branch
- riwayat commit
- files yang untracked 

Misalkan saya membuat di folder 'hello-world'.
### `$ git commit`
### `$ git config`
### `$ git branch`