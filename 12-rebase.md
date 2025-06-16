# Git Rebase :smiley:

> penjelasan : Ini merupakan workflow dimana jika kita memiliki banyak team dan banyak project maka worflow rebase ini cocok digunakan karena agar waktu merge yang dijalankan adalah fast-forward.

<br>

1. **membuat branch baru**
```bash
git branch features
```

> penjelasan : Kita harus membuat branch kita sendiri, ingat bahwa branch main di repo local ataupun repo hasil fork kita harus di samakan seperti branch main pada repo asli. Jangan pernah merubah file di branch main. Buatlah branch baru.

<br>

2. **beralih branch**
```bash
git checkout features
```
> penjelasan : Digunakan untuk beralih branch.

<br>

3. **melakukan commit**
```bash
git commit -m "tulis pesan anda disini"
```
> penjelasan : Digunakan untuk commit.

<br>

4. **melihat staging area**
```bash
git status
```
> penjelasan : Digunakan untuk melihat staging area.

<br>

5. **melihat log dalam bentuk graph**
```bash
git log --all --decorate --oneline --graph
```
> penjelasan : Digunakan untuk melihat visualiasi commit.
<br>

5. **cek repo asli**
```bash
git pull
```
> penjelasan : Digunakan untuk mengecek repo asli yang berada di github apakah ada perubahan atau tidak. pindah ke branch Main jika anda masih dibranch lain sebelum mengetikkan git pull.
<br>

6. **rebase branch features**
```bash
git rebase main
```
> penjelasan : Digunakan untuk rebase atau membuat si branch features sejajar dengan branch main. ingat bahwa ini baru sejajar aja belum sepenuhnya selesai, dengan rebase inilah nanti agar ketika kita akan merge tidak akan menggunakan three way merge namun menggunakan fast forward merge. Pastikan anda berada di branch features sebelum mengetikkan git rebase main.
<br>

7. **rebase branch main ke branch features**
```bash
git rebase features
```
> penjelasan : Kenapa terbaik dari no 6? Karena kita sudah rebase branch features ke branch main maka branch main tertinggal dari branch feature. Guanakan rebase lagi untuk memindahkan main ke features. Anda harus berada di branch main terlebih dahulu.
<br>

8. **meneruskan perubahan ke repo github**
```bash
git push -u origin main
```
> penjelasan : Meneruskan perubahan ke repo github agar repo github kita sudah up to date dengan repo local dan repo asli.
<br>

9. **menghapus branch**
```bash
git branch -d features
```
> penjelasan : Digunakan untuk menghapus branch yang sudah tidak digunakan lagi.
<br>

10. **menghapus branch repo github**
```bash
git push origin -d features
```
> penjelasan : Digunakan untuk menghapus branch yang sudah tidak digunakan lagi pada repo github kita.
<br>

**Terima kasih sudah melihat :heart:**