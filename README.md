<div align="center">

# ✍️ gultik

### papan catatan tak terbatas — sepi, bersih, seperti kertas kosong 📜

*klik di mana saja, ketik, coret, tempel gambar, geser ke segala arah.*
*tanpa akun, tanpa server, tanpa library. cuma satu file.*

![HTML](https://img.shields.io/badge/HTML-single%20file-e34f26?style=for-the-badge&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS-vanilla-1572b6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JS-no%20framework-f7df1e?style=for-the-badge&logo=javascript&logoColor=black)
![Dependencies](https://img.shields.io/badge/dependencies-0-success?style=for-the-badge)

![Offline](https://img.shields.io/badge/offline-ready-8a7a5c?style=flat-square)
![Autosave](https://img.shields.io/badge/autosave-✓-8a7a5c?style=flat-square)
![Dark mode](https://img.shields.io/badge/dark%20mode-ikut%20sistem-26231f?style=flat-square)
![Input](https://img.shields.io/badge/mouse%20·%20touchpad%20·%20sentuh%20·%20stylus-✓-8a7a5c?style=flat-square)

</div>

---

## 🌟 Kenapa gultik?

Kebanyakan aplikasi catatan memaksa kamu berpikir dalam baris dan halaman. **gultik** tidak.
Ia cuma sebidang kertas krem yang tidak ada ujungnya. Taruh ide di kiri, gambar panah ke kanan,
tempel screenshot di bawah, lalu geser papan sejauh yang kamu mau. Tidak ada menu, tidak ada popup,
tidak ada notifikasi "tersimpan!". Semuanya diam-diam tersimpan sendiri. 🤫

```
        ┌──────────────────────────────────────────────┐
        │ write  draw  erase  undo                     │
        │                                              │
        │   ide besar hari ini        ╭──────────╮     │
        │   ~~~~~~~~~~~~~~~~~  ───▶   │ 🖼️ gambar │     │
        │                             ╰──────────╯     │
        │        ✏️  coret-coret bebas  〰️〰️〰️          │
        │                                              │
        └──────────────── ∞ ke segala arah ∞ ──────────┘
```

---

## ✨ Fitur

| | Fitur | Keterangan |
|---|---|---|
| ♾️ | **Papan tak terbatas** | Teks, coretan, dan gambar hidup di satu "dunia" yang bergeser bersama. |
| ⌨️ | **Klik & ketik** | Klik di area kosong → blok teks baru muncul tepat di situ. Blok kosong hilang sendiri. |
| 🖊️ | **Coretan bebas** | Garis halus dengan ujung membulat. Satu ketukan = satu titik kecil. |
| 🧽 | **Penghapus** | Seret di atas coretan, teks, atau gambar untuk menghapusnya. |
| 🖼️ | **Gambar** | Tempel dengan Ctrl/Cmd+V atau drag & drop file. Bisa dipindah dengan diseret. |
| ↩️ | **Undo** | Batalkan coretan, penghapusan, atau gambar yang baru ditempel. |
| 🧭 | **Pulang ke isi** | Tekan <kbd>Home</kbd> untuk kembali ke tempat catatanmu berada. |
| 💾 | **Simpan otomatis** | Semua tersimpan di browser dan muncul lagi saat halaman dibuka ulang. |
| 🌗 | **Tema terang & gelap** | Mengikuti pengaturan sistem, termasuk warna coretan. |
| 📱 | **Semua jenis input** | Mouse, touchpad, layar sentuh (dua jari untuk geser), dan stylus (ujung penghapus didukung). |

---

## 🚀 Mulai dalam 5 detik

Tidak perlu install apa pun.

```bash
# cukup buka filenya di browser
start index.html        # Windows
open index.html         # macOS
xdg-open index.html     # Linux
```

Atau kalau mau lewat server lokal:

```bash
python -m http.server 8000
# lalu buka http://localhost:8000
```

> 💡 **Tip:** pasang sebagai tab yang dipin di browser, jadilah ia buku catatan coret-coret harianmu.

---

## 🎮 Cara pakai

### Tiga mode

| Mode | Klik / ketuk | Seret |
|---|---|---|
| ✍️ **write** *(default)* | buat blok teks baru | geser papan · pindahkan gambar |
| 🖊️ **draw** | titik kecil | coretan bebas |
| 🧽 **erase** | hapus yang tersentuh | hapus semua yang dilewati |

Tombol yang aktif di toolbar kiri atas berwarna lebih gelap. Tombol **undo** hanya muncul kalau ada yang bisa dibatalkan.

### 🧭 Menggeser papan

- 🖱️ seret area kosong di mode **write**
- 🖱️ tahan **klik tengah** mouse dari mana saja
- 🔄 **scroll** mouse atau touchpad (tahan <kbd>Shift</kbd> untuk geser horizontal)
- ✌️ **dua jari** di layar sentuh

### 🖼️ Bekerja dengan gambar

1. **Tempel**: salin gambar atau screenshot, lalu <kbd>Ctrl</kbd>+<kbd>V</kbd> / <kbd>Cmd</kbd>+<kbd>V</kbd>.
   Gambar muncul di **posisi klik terakhir**, atau di **tengah layar** kalau belum pernah klik.
2. **Drag & drop**: seret file gambar dari folder ke papan, dan gambar jatuh tepat di situ.
3. **Pindahkan**: seret gambar di mode write.
4. **Hapus**: mode erase atau <kbd>Ctrl</kbd>+klik. Bisa dikembalikan dengan undo.

> 📝 Sedang mengetik di blok teks? Menempel teks tetap jadi teks biasa. Hanya clipboard berisi gambar yang berubah jadi blok gambar.

---

## ⌨️ Pintasan keyboard

| Tombol | Aksi |
|---|---|
| <kbd>Alt</kbd> | pindah antara **write** ⇄ **draw** |
| <kbd>Ctrl</kbd> + klik/seret | hapus sekali gerakan, lalu kembali ke mode sebelumnya |
| <kbd>Ctrl</kbd> + <kbd>Z</kbd> | undo (saat tidak sedang mengetik) |
| <kbd>Ctrl</kbd> + <kbd>S</kbd> | simpan sekarang |
| <kbd>Ctrl</kbd> + <kbd>V</kbd> | tempel gambar |
| <kbd>Esc</kbd> | keluar dari blok teks / kembali ke mode write |
| <kbd>Home</kbd> | kembali ke lokasi isi catatan |

> 🙌 <kbd>Ctrl</kbd> sendirian tidak melakukan apa-apa, jadi <kbd>Ctrl</kbd>+<kbd>C</kbd>/<kbd>V</kbd>/<kbd>X</kbd>/<kbd>A</kbd>/<kbd>Z</kbd> tetap normal saat mengetik.

---

## 🎨 Desain

<table>
<tr>
<th>☀️ Terang</th>
<th>🌙 Gelap</th>
</tr>
<tr>
<td>

| Peran | Warna |
|---|---|
| kertas | `#fbfaf7` |
| tinta | `#26231f` |
| samar | `#a9a294` |

</td>
<td>

| Peran | Warna |
|---|---|
| kertas | `#171614` |
| tinta | `#e6e2d8` |
| samar | `#5f594e` |

</td>
</tr>
</table>

- 🔤 **Catatan**: font serif (Charter / Georgia), sedikit lebih besar dari normal, lebar maks ±30rem
- 🔡 **Toolbar & petunjuk**: sans-serif sistem, kecil, huruf sedikit renggang, semua huruf kecil
- 🖌️ **Coretan**: canvas tajam di layar resolusi tinggi, dan hanya bagian yang terlihat yang digambar

---

## 💾 Penyimpanan

Semua data disimpan di `localStorage` browser kamu dan **tidak pernah dikirim ke mana pun**. 🔒

| Kunci | Isi |
|---|---|
| `gultik.board.v1` | posisi papan, teks, coretan, posisi & ukuran gambar |
| `gultik.img.<id>` | data tiap gambar (sudah diperkecil ke lebar maks 1200px) |

- 📦 Gambar disimpan terpisah supaya teks & coretan **tetap tersimpan** walau penyimpanan penuh.
- 🤐 Kalau penyimpanan browser penuh, aplikasi tidak error, cuma diam-diam gagal menyimpan gambar baru.
- 🧹 Data gambar yang sudah tidak dipakai dibersihkan otomatis saat halaman dibuka.
- 🔄 Catatan lama dari versi sebelumnya dipindahkan otomatis ke papan baru saat pertama kali dibuka.

> ⚠️ Karena tersimpan di browser, menghapus data situs / riwayat browser juga akan menghapus catatanmu. Catatan juga tidak ikut pindah antar browser atau perangkat.

---

## 🗂️ Struktur proyek

```
gultik/
├── 📄 index.html   ← seluruh aplikasi: HTML + CSS + JS dalam satu file
├── 📝 prompt.md    ← spesifikasi fitur
└── 📖 README.md    ← kamu sedang membacanya
```

Di dalam `index.html`, kodenya dibagi per bagian dengan komentar:

```
1. konstanta & state          6. penghapus
2. penyimpanan + migrasi      7. menggeser papan + Home
3. blok teks                  8. pointer (write/draw/erase/pan)
3b. gambar                    8b. tempel & drag-drop gambar
4. canvas coretan             9. toolbar & keyboard
5. undo                       10. start
```

---

## 🧪 Daftar uji cepat

- [ ] klik di area kosong → ketik → klik di luar: teks tetap ada
- [ ] klik lalu langsung klik di luar: blok kosong hilang
- [ ] tekan <kbd>Alt</kbd> → coret → <kbd>Ctrl</kbd>+<kbd>Z</kbd>: coretan hilang
- [ ] <kbd>Ctrl</kbd>+seret di atas coretan → undo: coretan kembali
- [ ] screenshot → <kbd>Ctrl</kbd>+<kbd>V</kbd>: gambar muncul, bisa diseret
- [ ] scroll jauh → <kbd>Home</kbd>: kembali ke catatan
- [ ] reload halaman: semua isi masih ada ✅

---

<div align="center">

**gultik** · dibuat dengan ☕ dan kertas kosong

*click anywhere and type · drag to move around*

</div>
