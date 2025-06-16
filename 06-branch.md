# Git Branch :neutral_face:

> penjelasan : Digunakan ketika ingin membuat cabang dari branch utama yaitu main. Dengan branch inilah kolaborasi dapat dilihat dengan jelas karena kita bisa membuat branch spesifik dan orang lain akan bekerja di branch tersebut tanpa menganggu branch utama atau branch main. Contohnya, saya ingin teman saya Amin membuat fitur login dan saya membuat fitur register, maka teman saya Amin akan membuat branch login dan saya akan membuat branch register akan kita berdua bisa bekerja dengan branch masing-masing tanpa menganggu kodingan kita satu sama lain.

<br>

**Melihat daftar branch**

```bash
git branch
```

<br>

**Membuat branch**

```bash
git branch login
```

<br>

**Beralih ke branch lain**

```bash
git checkout login
```
```bash
git switch login
```
> ada dua cara untuk beralih, kita bisa menggunakan checkout ataupun switch tidak masalah sesuai selera kita aja. Terkadang saya meggunakan checkout, terkadang juga saya menggunakan switch.
<br>

**Membuat dan Beralih ke branch lain**

```bash
git checkout -b login
```

> Jika dirasa tidak menyukai cara bertele-tele seperti membuat branch dulu lalu beralih ke branch yg dibuat maka bisa menggunakan perintah diatas. Perintah tersebut akan membuat sekaligus beralih ke branch yang telah dibuat. Lebih simple karena dua kondisi terpenuhi.
<br>

**Terima kasih sudah melihat :heart:**