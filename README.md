# Tadicoba — Daily Activity

Tadicoba adalah dashboard aktivitas harian dan ruang belajar bahasa Jepang serta bahasa Inggris. Proyek ini dikemas dalam satu file HTML yang memuat antarmuka, logika, materi, dan sebagian aset. Kamu bisa membukanya di browser atau menerbitkannya sebagai situs statis.

## Yang bisa digunakan

| Area | Fitur |
| --- | --- |
| Dashboard | Agenda harian, pelacakan kebiasaan, rekap bulanan, dan progres belajar |
| Bahasa Jepang | Dasar hiragana dan katakana, Materi Harian 45 hari, latihan pilihan ganda, referensi kanji dan kotoba, flashcard, cerita, Mode Berpetualang Nao, dan simulasi JLPT N5/N4 |
| Bahasa Inggris | Materi dan latihan A1–B1, referensi kata kerja dan tata bahasa, serta cerita bacaan |

## Menjalankan proyek

1. Unduh file HTML terbaru. Jika namanya `index(1).html`, ubah menjadi `index.html`.
2. Buka file tersebut di browser dan pilih Bahasa Jepang atau Bahasa Inggris.
3. Untuk membuka tampilan Frosted Lavender, pilih **Bahasa Jepang → Materi harian → Baca materi**.

Proyek tidak memerlukan proses instalasi atau build. Jika Python sudah terpasang dan kamu ingin menjalankannya lewat server lokal, buka terminal di folder yang berisi `index.html` dan jalankan:

```bash
python -m http.server 8000
```

Buka `http://localhost:8000/` di browser.

## Frosted Lavender di desktop dan mobile

Tombol **Kembali** dan **Materi** berdampingan di kiri atas. Judul menunjukkan hari belajar yang sedang dibuka. Panel **Materi** menyediakan tab **Bagian** untuk berpindah topik dan **Hari** untuk memilih materi harian lain.

| Desktop | Mobile |
| --- | --- |
| Area baca melebar saat panel Materi ditutup. | Panel Materi mengambang di atas bacaan dan menutup setelah bagian atau hari dipilih. |
| Judul dan navigasi bagian berada di header. | Judul harian mendapat baris sendiri. Tombol Sebelumnya dan Berikutnya berada di bawah judul. |
| Tabel memanfaatkan lebar area baca. | Tabel lebar dapat digeser ke samping tanpa ikut menggeser halaman. |

Gunakan **Dengarkan** untuk memutar contoh, **Furigana** untuk menampilkan atau menyembunyikan bacaan kanji, dan **Mulai latihan** untuk membuka soal hari yang sedang dipelajari. Pada soal pemahaman bacaan, teks muncul tepat sebelum rangkaian soal yang merujuknya.

## Publikasi di GitHub Pages

Taruh `index.html` di folder yang dipakai sebagai sumber GitHub Pages, misalnya root repositori. Commit dan push perubahan, lalu cek hasil publikasi di tab **Actions**. Jika sumber Pages memakai folder `docs`, gunakan `docs/index.html`.

## Data dan penggunaan offline

- Progres disimpan di browser. Gunakan fitur ekspor dan impor cadangan untuk memindahkan data ke browser atau perangkat lain. Alamat `localhost`, file lokal, dan GitHub Pages dapat memiliki penyimpanan progres terpisah.
- File utama memuat materi dan aset tersemat. Sebagian fitur atau aset yang mengambil data dari luar tetap membutuhkan koneksi internet.
- Audio menggunakan suara yang tersedia di browser atau perangkat. Ketersediaan suara bahasa Jepang dapat berbeda antarperangkat.
