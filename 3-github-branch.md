# GitHub: Branch

## NIM - Nama:
### 16921055 - Hafizh Renanto Akhmad

<p>&nbsp;</p>

## Branching
- merupakan proses membuat Git Branch.
- membuat snapshot tanpa mengganggu master branch 'jalur utama' (dapat dijalankan dengan commitnya sendiri)
- biasanya digunakan ketika ingin mengimplementasikan fitur eksperimental atau lebih dari satu orang yang mengerjakan repo yang sama.

<p>&nbsp;</p>

## Merging
adalah proses menggabungkan commit dari branch kembali ke master branch.

<p>&nbsp;</p>

## Membuat branch dengan GitHub
Ada dua cara dalam membuat file baru.
Cara pertama adalah ketika ingin melakukan commit saat mengubah/membuat file. Di bawah kolom deskripsi, kita dapat memilih apakah kita akan melakukan commit terhadap master branch, atau branch baru. Pilih opsi membuat branch baru dan branch baru akan secara otomatis terbuat.

Cara kedua adalah menambahkan langsung pada laman menu Code.
1. Klik tombol di sebelah kiri tombol `Go to File`,
2. Isi kolom dengan nama branch yang diinginkan, dan
3. Klik `Create branch`.

Sekarang, kita sudah memiliki branch baru. Kita dapat melakukan commit terhadap branch baru tersebut dan tidak akan memengaruhi branch master.

<p>&nbsp;</p>

## Melakukan merging dengan GitHub
Jika suatu kita melakukan commit pada suatu branch, pada menu Code, akan terdapat tombol `Compare & pull request`. Untuk melakukan merge,
1. Klik tombol `Compare & pull request` tersebut
2. Terdapat opsi branch `base` dan `compare`. Branch yang dipilih sebagai `base` akan menjadi "base", sedangkan branch yang dipilih sebagai `compare` adalah branch yang akan 'dimasukkan' ke dalam "base". Tentukan branch base dan branch compare.
3. Isi kolom deskripsi dari pull request serta tambahkan keterangan jika diperlukan.
4. Klik tombol `Create pull request`.
5. Pada laman menu `Pull request`, akan muncul pull request baru. Jika tidak ada konflik dengan branch base, kita bisa langsung menekan tombol `Merge pull request`.
6. Isi deskripsi dan komentar terhadap pelaku pull request (walau pada kasus ini, terhadap diri sendiri).
7. Klik `Confirm merge` jika sudah yakin.

Konflik ketika pull request dapat terjadi, salah satunya, karena ada baris yang sama pada file tertentu yang berbeda. 

Jika terdapat konflik antara branch compare dengan branch base, pemilik branch base harus menekan tombol `Resolve conflicts` pada laman menu `Pull request` dan akan diarahkan ke code editor dan menyelesaikannya dengan cara manual.

<p>&nbsp;</p>

## Istilah Umum
- Branch: jalur 'development' bebas dari sebuah commit.
- Checkout: berpindah ke branch/commit yang lain.
- Pull Request: meminta pemilik repo untuk 'mengambil' perubahan yang telah dilakukan.
- Merge: menggabungkan 2 buah branch.
- Merge Conflict: baris yang sama diubah oleh branch yang berbeda.