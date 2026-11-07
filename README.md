# gultik

**Nama:** Tristan Birendra

## Tentang repository

Repository ini berisi **gultik**, aplikasi papan catatan tak terbatas dalam satu file HTML yang dibuat dengan bantuan AI, beserta prompt yang dipakai untuk membuatnya.

Tujuannya untuk mempraktikkan materi workshop *Building with AI, Managing Change with GitHub*: menulis prompt yang jelas untuk AI, lalu mencatat setiap perubahan proyek dengan Git dan menyimpannya di GitHub. Riwayat commit di repository ini menunjukkan alurnya, mulai dari prompt pertama, aplikasi awal, sampai penambahan fitur gambar.

## Dokumentasi workshop

**Kegiatan:** Workshop Day 1, *Building with AI, Managing Change with GitHub*
**Pemateri:** Nugi Farhan, Senior Product Designer

### Rangkuman materi

Workshop dibagi menjadi dua bagian besar: membuat dan mengembangkan proyek dengan AI, lalu mengelola perubahan dan kolaborasi dengan Git dan GitHub.

**Prompt engineering.** Prompt adalah instruksi yang kita berikan ke model AI untuk mendapatkan hasil tertentu. Prompt yang singkat seperti "Create student task planner" memberi hasil yang asal-asalan, sedangkan prompt dengan konteks yang jelas memberi hasil yang jauh lebih sesuai. Struktur prompt yang baik terdiri dari empat bagian: Role (peran AI), Task (tujuan), Context (requirements dan batasan), dan Format (bentuk hasil yang diminta). Beberapa taktik tambahan: pakai kata kerja yang jelas, tentukan panjang dan format output, sebutkan target pembaca, sertakan data atau dokumen yang relevan, dan jelaskan istilah penting. Manfaatnya antara lain performa AI lebih baik, hasil lebih bisa diprediksi, dan respons yang bias atau menyinggung berkurang.

**Git.** Git adalah version control system yang mencatat siapa, kapan, dan apa saja yang berubah dalam file. Git dibuat oleh Linus Torvalds pada tahun 2005. Alur kerjanya melewati tiga tempat: working directory (file yang sedang dikerjakan), staging area (daftar perubahan yang akan masuk ke commit berikutnya), dan direktori `.git` (tempat seluruh riwayat proyek disimpan).

**Git vs GitHub.** Git adalah alat untuk melacak perubahan secara lokal di komputer, sedangkan GitHub adalah platform web untuk menyimpan repository Git secara online dan berkolaborasi dengan orang lain.

**Perintah dasar.**

```
git init                     memulai repository baru
git add .                    memindahkan perubahan ke staging area
git commit -m "pesan"        menyimpan perubahan ke repository
git remote add origin <url>  menghubungkan repository lokal ke GitHub
git push origin main         mengirim commit ke GitHub
git pull origin main         mengambil perubahan dari GitHub
git clone <url>              menyalin repository dari GitHub
```

**Setup.** Install Git, cek dengan `git --version`, atur identitas dengan `git config --global user.name` dan `user.email`, install VS Code, lalu buat SSH key (`ssh-keygen -t ed25519`), tambahkan ke GitHub, dan cek koneksinya dengan `ssh -T git@github.com`.

**Praktik.** Membuat aplikasi sederhana dengan AI lewat prompt, memasukkannya ke Git, commit dan push ke GitHub, lalu membuat perubahan dan commit serta push lagi.

### Poin penting yang saya pelajari

- Hasil AI sangat bergantung pada seberapa jelas prompt-nya. Menuliskan requirements dan batasan secara detail membuat hasilnya jauh lebih sesuai.
- Prompt bisa disimpan sebagai file (`prompt.md`) dan ikut dicatat di Git, jadi perubahan fitur bisa dilacak dari prompt sampai kodenya.
- Bedanya Git dan GitHub: Git bekerja di komputer sendiri, GitHub tempat menyimpannya secara online.
- Perubahan tidak langsung masuk ke riwayat; harus lewat staging area dulu (`git add`) sebelum di-commit.
- Pesan commit sebaiknya singkat dan menjelaskan apa yang berubah, dan satu commit sebaiknya berisi satu perubahan.
- SSH key dipakai supaya bisa push ke GitHub tanpa memasukkan password setiap kali.

### Pendapat pribadi tentang Day 1

Kurang seru, kadang bikin ngantuk.

---

## Tentang aplikasi

gultik adalah papan catatan tak terbatas dalam satu file HTML. Klik di mana saja untuk mengetik, coret-coret, tempel gambar, dan geser papan ke segala arah. Tanpa akun, tanpa server, tanpa library.

### Cara menjalankan

Buka `index.html` di browser. Tidak perlu install apa pun.

### Cara pakai

Ada tiga mode di toolbar kiri atas:

- **write**: klik area kosong untuk membuat blok teks. Seret area kosong untuk menggeser papan.
- **draw**: seret untuk mencoret.
- **erase**: seret di atas coretan, teks, atau gambar untuk menghapusnya.

Papan juga bisa digeser dengan klik tengah mouse, scroll, atau dua jari di layar sentuh.

Gambar bisa ditambahkan dengan Ctrl+V atau drag & drop file ke papan, lalu dipindah dengan cara diseret di mode write.

### Pintasan keyboard

| Tombol | Aksi |
| --- | --- |
| Alt | pindah antara write dan draw |
| Ctrl + klik/seret | hapus sekali gerakan |
| Ctrl + Z | undo (saat tidak mengetik) |
| Ctrl + S | simpan |
| Ctrl + V | tempel gambar |
| Esc | keluar dari blok teks / kembali ke write |
| Home | kembali ke lokasi catatan |

### Penyimpanan

Semua isi tersimpan otomatis di `localStorage` browser dan tidak dikirim ke mana pun. Artinya catatan hilang kalau data browser dihapus, dan tidak ikut pindah ke browser atau perangkat lain.

Gambar diperkecil ke lebar maksimal 1200px sebelum disimpan. Kalau penyimpanan penuh, gambar baru tidak tersimpan, tapi teks dan coretan tetap aman.

### Struktur

```
index.html   seluruh aplikasi (HTML, CSS, JS)
prompt.md    prompt yang dipakai untuk membuat aplikasi
README.md    dokumen ini
```
