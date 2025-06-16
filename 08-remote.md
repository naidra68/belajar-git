# Git Remote :dizzy_face:

> penjelasan : Semua perintah sebelumnya akan digunakan. Git Remote memiliki arti bahwa kita akan melakukan sesuatu secara langsung pada repo kita yang berada di github. Ketika sudah paham mengenai perintah git di repo local maka akan kita terapkan ke repo github supaya repo local kita sama seperti repo github.

<br>

1. **duplikasi repositori**
```bash
git clone https://github.com/naidra68/belajar-git
```

<br>

2. **inisialisasi repositori**
```bash
git init
```

<br>

3. **menambahkan remote**
```bash
git remote add origin https://github.com/naidra68/belajar-git
```

<br>

4. **melihat remote**
```bash
git remote get-url origin
```

<br>

5. **melihat remote dengan jelas**
```bash
git remote -v
```

<br>

6. **mengubah paksa ke branch main**
```bash
git branch -M main
```

<br>

7. **Perubahan langsung ke repo github (untuk pertama kali)**
```bash
git push -u origin main
```

<br>

8. **Perubahan langsung ke repo github**
```bash
git push
```

<br>

8. **menghapus remote**
```bash
git rm origin
```

<br>

**Terima kasih sudah melihat :heart:**