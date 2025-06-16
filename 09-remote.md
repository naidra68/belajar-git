# Git Remote :dizzy_face:

> penjelasan : Semua perintah sebelumnya akan digunakan. Git Remote memiliki arti bahwa kita akan melakukan sesuatu secara langsung pada repo kita yang berada di github. Ketika sudah paham mengenai perintah git di repo local maka akan kita terapkan ke repo github supaya repo local kita sama seperti repo github.

<br>

## 1. **duplikasi repositori (via https)**
```bash
git clone https://github.com/naidra68/belajar-git
```
> penjelasan : menduplikasi repositori kita ataupun orang lain yang berada di github.
<br>

## 2. **inisialisasi repositori**
```bash
git init
```
> penjelasan : Inisialisasi repo kita agar terkonek dengan git.
<br>

## 3. **menambahkan remote (via https)**
```bash
git remote add origin https://github.com/naidra68/belajar-git
```
> penjelasan : Untuk menambahkan remote repo github kita ke repo local. Ini harus dilakukan karena nanti saat kita melakukan perubahan di local maka kita bisa meneruskan perubahan tersebut ke github.
<br>

## 4. **melihat remote**
```bash
git remote get-url origin
```
> penjelasan : Untuk melihat remote yang terkonek.
<br>

## 5. **melihat remote dengan jelas**
```bash
git remote -v
```
> penjelasan : untuk melihat remote yang terkonek dengan nama remote-nya.
<br>

## 6. **mengubah paksa ke branch main**
```bash
git branch -M main
```
> penjelasan : Ini dilakukan untuk memastikan bahwa branch utama kita di local itu bernama `main`. Jika anda menggunakan git versi terbaru, langkah ini mungkin dapat di skip karena git versi terbaru menggunakan nama branch utama `main`. Sedangkan git versi sebelumya menggunakan nama branch `master`. Perintah inilah yang mengubah paksa dari branch `master` ke `main`.
<br>

## 7. **Meneruskan perubahan ke github (untuk pertama kali)**
```bash
git push -u origin main
```
> penjelasan : Perintah push digunakan untuk meneruskan perubahan repo local kita ke repo github kita. `-u origin main` berarti ini akan diteruskan ke nama remote kita yaitu `origin` sesuai point no 3 dan nama branch kita yaitu `main` sesuai point no 6.
<br>

## 8. **Meneruskan perubahan ke github**
```bash
git push
```
> penjelasan : meneruskan perubahan, anda bisa menggunakan hanya perintah `git push` saja jika sudah melakukan perintah di point no 7.
<br>

## 9. **Perubahan dengan branch baru/ada**
```bash
git push origin main:develop
```
> penjelasan : Jika ingin membuat branch baru dan ingin branch baru memiliki file yang ada di branch `main` maka perintah itu akan dilaksanakan. `main:develop` berarti kita akan meneruskan dari `main` ke branch `develop`. Jika branch `develop` tidak ada di repo github maka secara otomatis akan dibuatkan. Perlu di ingat bahwa branch ini akan ada di repo github saja dan di repo local branch develop tidak akan dibuat.
<br>

## 10. **Perubahan dengan semua branch**
```bash
git push origin -all
```
> penjelasan : Ketika memiliki project dengan banyak branch dan banyak perubahan pada branch tersebut, kita bisa push satu-persatu namun itu terlalu memakan waktu. gunakan `-all` akan meneruskan perubahan semua-nya ke repo github kita sekaligus.
<br>

## 10. **menghapus branch repo github**
```bash
git push -d origin develop
```
> penjelasan : Menghapus branch yang ada di repo github, kita bisa menggunakan perintah diatas. Perintah untuk menghapus branch repo local dan branch repo github akan berbeda. Perlu diingat bahwa jika anda menghapus branch di repo github anda maka di repo local anda masih terdapat branch tersebut karena kita harus menghapus branch secara manual.
<br>

## 12. **menghapus remote**
```bash
git rm origin
```
> penjelasan : Untuk menghapus remote.
<br>

**Terima kasih sudah melihat :heart:**