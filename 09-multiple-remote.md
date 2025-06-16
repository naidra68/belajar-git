# Git Remote (Multiple Remote)

> penjelasan : Ini merupakan langkah-langkah jika saya ingin fork repo project orang lain ke repo saya dan nanti-nya saya akan bekerja pada project tersebut.

<br>

1. **forking repositori orang lain**

> penjelasan : Kita forking terlebih dahulu repositori orang lain, jika di asumsikan bahwa saya adalah orang lain maka saya akan forking repo saya sendiri dengan akun sebagai orang lain tersebut.

<br>

2. **duplikasi repositori**
```bash
git clone https://github.com/ardian/belajar-git
```
> penjelasan : Duplikasi repositori yang telah di fork tadi, lihat url nya saya memakai akun github bernama "ardian" karena saya sudah fork belajar-git dari akun "naidra68".
<br>

3. **melihat daftar remote**
```bash
git remote
```
> penjelasan : Untuk melihat daftar remote kita. Ketika pertama kali dicoba maka akan tampil tulisan "origin", itu merupakan default dari git yang memiliki arti bahwa ketika saya akan melakukan perubahan pada repo local (di komputer saya) maka yang tersimpan akan masuk ke dalam repo github "ardian" dan bukan ke "naidra68".
<br>

4. **git remote view**
```bash
git remote -v
```
> penjelasan : Untuk mengetahui bahwa origin kita itu masuk ke dalam repo mana, apakah di "ardian" atau di "naidra68".
<br>

5. **git remote add**
```bash
git remote add naidra68 https://github.com/naidra68/belajar-git
```
> penjelasan : Untuk menambahkan remote, berfungsi jika kita ingin up to date dengan repo asli maka kita perlu menambahkan repo asli ke dalam remote kita. Jika dibandingkan, lihatlah url dari no 2 dan no 5 ini pasti ada perbedaan dibagian username-nya.
<br>

5. **git fetch**
```bash
git fetch naidra68
```
> penjelasan : Digunakan untuk melihat posisi commit dari repo asli ada dimana. Ini dilakukan agar repo local dan repo github hasil fork kita sudah up to date dengan repo asli-nya. Untuk mengetahui hal ini saya bisa mengetikkan `git log --all --decorate --oneline --graph`. Saran untuk saya dan mungkin kita semua. Sering-sering gunakan fetch ini untuk mengetahui pembaruan dari repo asli-nya supaya kita tau gitu kalau di repo asli ada perubahan atau tidak.
<br>

6. **git merge**
```bash
git merge naidra68/main
```
> penjelasan : Ketika saya melakukan fetch dan mendapati bahwa repo asli telah ada pembaruan maka agar repo local kita sama seperti repo asli-nya adalah dengan cara merge. Perintah diatas bisa dilihat bahwa sebelumnya saya sudah membuat remote dengan nama naidra68 maka saya tinggal ketik saja naidra68/nama-branch.
<br>

7. **git push**
```bash
git push -u origin main
```
> penjelasan : Setelah repo local kita sudah up to date dengan repo asli-nya maka langkah selanjutnya adalah kita push perubahan yang ada di local ke repo fork kita. Karena kalau tidak dilakukan, maka repo fork punya kita sendiri masih ketinggalan dari repo local dan repo asli.
<br>

**Terima kasih sudah melihat :heart:**