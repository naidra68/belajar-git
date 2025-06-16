# Git Branch :neutral_face:

> penjelasan : Digunakan ketika ingin membuat cabang dari branch utama yaitu `main`. Dengan branch inilah kolaborasi dapat dilihat dengan jelas karena kita bisa membuat branch spesifik dan orang lain akan bekerja di branch tersebut tanpa menganggu branch utama atau branch `main`. Contohnya, saya ingin teman saya **Amin** membuat fitur login dan saya membuat fitur register, maka teman saya **Amin** akan membuat branch `login` dan saya akan membuat branch `register`, kita berdua bisa bekerja dengan branch masing-masing tanpa menganggu kodingan kita satu sama lain.

<br>

## 1. **Melihat daftar branch**

```bash
git branch
```
> penjelasan : melihat semua daftar branch. Ketika anda baru menggunakan git maka langkah pertama adalah melihat branch anda terlebih dahulu.
<br>

## 2. **Membuat branch**

```bash
git branch login
```
> penjelasan : membuat branch dengan nama `login`.
<br>

## 3. **Beralih ke branch lain**

```bash
git checkout login
```
```bash
git switch login
```
> Penjelsan : Ada dua cara untuk beralih, kita bisa menggunakan checkout ataupun switch tidak masalah sesuai selera kita aja. Terkadang saya meggunakan checkout, terkadang juga saya menggunakan switch.
<br>

## 4. **Membuat dan Beralih ke branch lain**

```bash
git checkout -b login
```

> Penjelasan : Jika dirasa tidak menyukai cara bertele-tele seperti membuat branch dulu lalu beralih ke branch yg dibuat maka bisa menggunakan perintah diatas. Perintah tersebut akan membuat sekaligus beralih ke branch yang telah dibuat. Lebih simple karena dua kondisi terpenuhi.
<br>

## 5. **Menghapus branch**

```bash
git branch -d login
```

> Penjelasan : Ketika sudah selesai dengan menambah fitur baru, menggabungkan fitur baru ke branch `main` dan melakukan perubahan ke repo github maka anda bisa menghapus branch tersebut jika sudah tidak terpakai lagi.
<br>

**Terima kasih sudah melihat :heart:**