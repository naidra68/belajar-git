# Git Remote Branch :smile:

> penjelasan : Merupakan langkah-langkah selanjutnya, ketika kita sudah fork repo orang lain, memasukkannya ke local, selalu up to date dengan repo asli, dan kita sudah membuat fitur baru pada repo fork kita serta kita akan menambahkan fitur kita ke repo asli maka langkah ini yang harus diterapkan.

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

5. **meneruskan perubahan**
```bash
git push origin features
```
> penjelasan : Digunakan untuk meneruskan perubahan ke github.
<br>

6. **Pull Request**

> penjelasan : Untuk melakukan Pull Request, saya ataupun anda bisa langsung ke github dan ajukan PR kepada pemilik repo asli. Jika disetujui maka perubahan anda akan diterapkan ke repo asli si pemilik.
<br>

7. **git fetch**
```bash
git fetch naidra68
```
> penjelasan : Digunakan ketika kita ingin melihat perubahan up to date dari repo asli.
<br>

8. **kembali ke branch main**
```bash
git checkout main
```
> penjelasan : Kembali ke branch main untuk melakukan merge jika terdapat perubahan dari repo asli agar repo local kita dapat up to date.
<br>

9. **git merge dari naidra68 ke ardian**
```bash
git merge naidra68/main
```
> penjelasan : Merge agar repo local kita sama seperti repo asli alias up to date.
<br>

10. **meneruskan perubahan ke repo github**
```bash
git push -u origin main
```
> penjelasan : Meneruskan perubahan ke repo github agar repo github kita sudah up to date dengan repo local dan repo asli.
<br>

10. **menghapus branch**
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