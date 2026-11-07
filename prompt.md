Kamu membantu saya membuat aplikasi catatan papan tak terbatas (infinite canvas) yang minimalis dalam bentuk satu halaman web.

## Goal

Buat aplikasi catatan di mana pengguna bisa klik di mana saja untuk mengetik, menggambar coretan bebas, menghapus, dan menggeser papan ke segala arah, dengan tampilan sepi dan bersih seperti kertas kosong.

## Requirements

- Papan tidak punya batas: semua teks dan coretan berada di satu "dunia" yang ikut bergeser bersama saat papan digeser.
- Mode **write** (default): klik di area kosong membuat blok teks baru tepat di posisi klik dan langsung bisa diketik. Kalau klik lalu diseret, papan bergeser dan tidak membuat blok teks.
- Blok teks yang dibiarkan kosong otomatis terhapus saat kehilangan fokus.
- Mode **draw**: menggambar garis bebas dengan ujung membulat dan lengkungan halus. Satu ketukan meninggalkan titik kecil.
- Mode **erase**: menyeret di atas coretan atau blok teks akan menghapusnya.
- Toolbar kecil di pojok kiri atas berisi tombol teks huruf kecil: write, draw, erase, dan undo. Tombol yang aktif berwarna lebih gelap. Tombol undo hanya muncul kalau ada yang bisa dibatalkan.
- Undo bisa membatalkan coretan terakhir maupun penghapusan (coretan dan teks yang terhapus kembali lagi).
- Cara menggeser papan: seret area kosong di mode write, klik tengah mouse dari mana saja, scroll mouse/touchpad, atau dua jari di layar sentuh.
- Pintasan keyboard:
  - Tekan Alt untuk berpindah antara write dan draw.
  - Tahan Ctrl sambil klik/seret untuk menghapus sekali gerakan, lalu kembali ke mode sebelumnya. Ctrl sendirian tidak melakukan apa-apa supaya Ctrl+C, V, X, A, Z tetap normal saat mengetik.
  - Ctrl+Z untuk undo saat tidak di mode write.
  - Ctrl+S untuk menyimpan.
  - Esc untuk keluar dari blok teks atau kembali ke mode write.
  - Home untuk kembali ke lokasi isi catatan.
- Ada satu baris petunjuk samar di tengah layar ("click anywhere and type · drag to move around") yang hilang begitu ada isi di papan.
- Semua isi (posisi papan, teks, coretan) tersimpan otomatis di browser tanpa notifikasi, dan muncul lagi saat halaman dibuka ulang.
- Jika ada data catatan lama dari versi sebelumnya, pindahkan otomatis ke papan baru saat pertama kali dibuka.

## Constraints

- Gunakan HTML, CSS, dan JavaScript murni (vanilla) dalam satu file, tanpa library atau framework eksternal.
- Bahasa antarmuka adalah Bahasa Inggris dengan huruf kecil semua.
- Tampilan terang memakai latar krem kertas (#fbfaf7), tinta cokelat tua (#26231f), dan teks samar (#a9a294). Tampilan gelap mengikuti pengaturan sistem dengan latar #171614, tinta #e6e2d8, dan teks samar #5f594e. Warna coretan ikut berganti sesuai tema.
- Teks catatan memakai font serif (Charter atau Georgia), ukuran sedikit lebih besar dari normal, dengan lebar blok maksimal sekitar 30rem.
- Toolbar dan petunjuk memakai font sistem sans-serif berukuran kecil dengan jarak huruf sedikit renggang.
- Coretan digambar di canvas yang tajam di layar resolusi tinggi dan hanya menggambar bagian yang terlihat di layar agar tetap ringan.
- Halaman tidak boleh ikut scroll; hanya papan yang bergeser.
- Bisa dipakai dengan mouse, touchpad, layar sentuh, dan stylus.
- Jaga kode tetap rapi dan beri komentar singkat untuk tiap bagian utama.

## Output

Berikan kode lengkap dalam satu file `index.html`, jelaskan secara singkat fungsi tiap bagian kode, cara membukanya di browser, dan cara menguji interaksi utamanya (mengetik, menggambar, menghapus, undo, menggeser papan, pintasan keyboard, dan penyimpanan setelah halaman dimuat ulang).

Jangan mengklaim aplikasi sudah berfungsi sebelum kamu memeriksa perilakunya.
