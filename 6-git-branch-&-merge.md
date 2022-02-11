# GitL Branch dan Merge

## NIM - Nama:
### 16921055 - Hafizh Renanto Akhmad

<p>&nbsp;</p>

Proses branching dan merging di Git tidak semudah di GitHub, karena kita mempelajari hal yang dibelakang GitHub itu sendiri.

## Command
### `$ git branch`
Command ini digunakan untuk membuat branch baru dengan memasukkan:
```
$ git branch <nama branch>
```
Dengan memasukkan `$ git branch` saja, semua branch dari repo akan ditampilkan.

![](https://cdn.discordapp.com/attachments/941700810335744010/941772836618522665/unknown.png)

### `$ alias`
Pada video, juga digunakan command `alias`. Untuk menampilkan visualisasi graph, digunakan command
```
$ git log --all --decorate --oneline --graph
```
Command tersebut cukup merepotkan jika harus kita masukkan tiap ingin melihat visualisasi. Sehingga `alias` digunakan untuk mempermudah pemanggilan command dengan menyingkatnya.

![](https://cdn.discordapp.com/attachments/941700810335744010/941773212625285191/unknown.png)

### `$ git checkout`
Command ini digunakan untuk berpindah ke branch lain, dengan syntax
```
$ git checkout <nama_branch_tujuan>
```
![](https://cdn.discordapp.com/attachments/941700810335744010/941774263130677278/unknown.png)
`HEAD` menandakan branch yang saat ini aktif.

Lanjutan:

![](https://cdn.discordapp.com/attachments/941700810335744010/941775262914330714/unknown.png
)
_*menghapus helloworld.py_

![](https://cdn.discordapp.com/attachments/941700810335744010/941776481233801277/unknown.png)
_*menambahkan kembali dan modifikasi helloworld.py_

![](https://cdn.discordapp.com/attachments/941700810335744010/941777086832590898/unknown.png)
_*berpindah ke branch py dan melakukan modifikasi_

![](https://cdn.discordapp.com/attachments/941700810335744010/941778200588079185/unknown.png)
_*melakukan modifikasi namun ingin pindah ke branch master sebelum di commit. Ter_


### `$ git merge`
Command ini digunakan untuk melakukan merge (seperti pada GitHub) dengan memasukkan syntax
```
$ git merge <nama_branch>
```

Ada dua jenis merge:
1. Fast forward: terjadi ketika dua branch yang akan dimerge terhubung secara lansgung.

Contoh:
![](https://cdn.discordapp.com/attachments/941700810335744010/941779052908404806/unknown.png)

2. Three-way merge: terjadi ketika dua branch yang akan dimerge tidak terhubung langsung

Contoh:

![](https://cdn.discordapp.com/attachments/941700810335744010/941781342440521798/unknown.png)

## Menghapus Branch
Command:
```
$ git branch -d <nama_branch>
```

Setelah menggunakan command di atas, kita akan diberi warning jika branch yang ingin dihapus belum dimerge.
Jika sudah sangat yakin akan penghapusan, gunakan command

![](https://cdn.discordapp.com/attachments/941700810335744010/941779503292776488/unknown.png)
_*Lanjutan gambar dari Fast Forward_

```
$ git branch -D <nama_branch>
```