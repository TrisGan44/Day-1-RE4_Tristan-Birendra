# gultik

Papan catatan tak terbatas dalam satu file HTML. Klik di mana saja untuk mengetik, coret-coret, tempel gambar, dan geser papan ke segala arah. Tanpa akun, tanpa server, tanpa library.

## Cara menjalankan

Buka `index.html` di browser. Tidak perlu install apa pun.

## Cara pakai

Ada tiga mode di toolbar kiri atas:

- **write**: klik area kosong untuk membuat blok teks. Seret area kosong untuk menggeser papan.
- **draw**: seret untuk mencoret.
- **erase**: seret di atas coretan, teks, atau gambar untuk menghapusnya.

Papan juga bisa digeser dengan klik tengah mouse, scroll, atau dua jari di layar sentuh.

Gambar bisa ditambahkan dengan Ctrl+V atau drag & drop file ke papan, lalu dipindah dengan cara diseret di mode write.

## Pintasan keyboard

| Tombol | Aksi |
| --- | --- |
| Alt | pindah antara write dan draw |
| Ctrl + klik/seret | hapus sekali gerakan |
| Ctrl + Z | undo (saat tidak mengetik) |
| Ctrl + S | simpan |
| Ctrl + V | tempel gambar |
| Esc | keluar dari blok teks / kembali ke write |
| Home | kembali ke lokasi catatan |

## Penyimpanan

Semua isi tersimpan otomatis di `localStorage` browser dan tidak dikirim ke mana pun. Artinya catatan hilang kalau data browser dihapus, dan tidak ikut pindah ke browser atau perangkat lain.

Gambar diperkecil ke lebar maksimal 1200px sebelum disimpan. Kalau penyimpanan penuh, gambar baru tidak tersimpan, tapi teks dan coretan tetap aman.

## Struktur

```
index.html   seluruh aplikasi (HTML, CSS, JS)
prompt.md    spesifikasi fitur
README.md    dokumen ini
```
