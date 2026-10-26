# Daily Compass

Dashboard aktivitas harian dan pendamping belajar bahasa Jepang N5–N4 dalam satu website. Daily Compass menggabungkan agenda, latihan soal, kartu kanji, kotoba, flashcard, dan rekap kehadiran belajar.

**[Buka dashboard](https://tadipuhan.github.io/Dailyactivity/)**

## Fitur

| Menu / fitur | Fungsi |
| --- | --- |
| Ringkasan | Melihat progres tugas dan hasil latihan yang tersimpan. |
| Aktivitas harian | Menambah, mengubah, menghapus, dan menandai agenda selesai. |
| Jepang · 45 hari | Membaca materi dan mengerjakan latihan. Paket yang tersedia saat ini adalah **Day 1–4**. |
| Latihan pilihan ganda | Masing-masing hari berisi **40 soal dengan 4 pilihan**, nilai otomatis, dan pembahasan setelah pengiriman. |
| Absensi belajar | Mencatat kehadiran berdasarkan tanggal perangkat saat seluruh 40 jawaban dikirim. |
| Akumulasi bulanan | Menampilkan hari hadir, jumlah latihan, waktu aktif, rata-rata nilai, dan kalender absensi aktual. |
| Kanji N5 | **103 kartu** berisi kanji, arti, jumlah goresan, onyomi, kunyomi, romaji, dan contoh penggunaan. |
| Kanji N4 | **166 kartu** dengan pencarian, filter kelompok, dan penanda belajar. |
| Kotoba N5–N4 | **424 kosakata pilihan** beserta bacaan dan arti bahasa Indonesia. |
| Flashcard | **670 kartu unik** kanji dan kotoba, dengan 4 pilihan jawaban, penilaian otomatis, dan filter latihan. |
| Personalisasi | Popup nama panggilan, sapaan sesuai waktu, serta tombol untuk mengubah nama. |
| Jam & target | Jam berjalan per detik dan hitung mundur menuju **5 Desember 2026 pukul 00.00**, mengikuti waktu perangkat. |

Tampilan menyesuaikan ukuran HP, tablet, dan laptop. Daftar kanji menggunakan kartu dengan pilihan jumlah kartu per halaman.

## Cara menggunakan

1. Buka alamat dashboard atau file `index.html` di browser.
2. Isi nama panggilan pada kunjungan pertama.
3. Tambahkan agenda pribadi melalui menu **Aktivitas harian**.
4. Buka **Jepang · 45 hari**, pilih Day, lalu baca materi sebelum memulai latihan.
5. Jawab seluruh 40 soal dan kirim jawaban untuk melihat nilai serta mencatat kehadiran.
6. Gunakan **Kanji N5**, **Kanji N4**, **Kotoba**, dan **Flashcard** untuk pengulangan.
7. Pantau riwayat melalui **Akumulasi bulanan**.

### Aturan absensi dan nilai

- Kehadiran tercatat setelah **40 jawaban dikirim**, termasuk jika nilainya belum mencapai target.
- Satu tanggal dihitung sebagai **satu hari hadir** meskipun pengguna mengirim beberapa latihan.
- Pengiriman pertama untuk suatu Day dicatat sebagai soal baru; percobaan berikutnya sebagai pengulangan.
- Nilai **≥80%** menandai Day tuntas sebagai target belajar pribadi, bukan standar kelulusan JLPT.
- Latihan flashcard dan penanda kartu kanji **tidak menggantikan absensi 40 soal**.
- Jawaban flashcard yang salah dijadwalkan ulang besok, sedangkan jawaban benar empat hari kemudian.

## Penyimpanan data

Data disimpan menggunakan **localStorage pada browser**, meliputi nama panggilan, agenda, draf jawaban, hasil latihan, absensi, penanda kanji/kotoba, serta progres flashcard.

**Website ini belum memiliki akun dan sinkronisasi antarperangkat.** Mengubah nama panggilan hanya mengubah tampilan, bukan membuat profil data baru. Pada browser dan alamat website yang sama, data tetap menggunakan penyimpanan yang sama.

- Data laptop dan HP belum otomatis tersinkron.
- Menghapus data situs/browser dapat menghapus progres.
- File lokal, alamat GitHub Pages, dan custom domain dapat memiliki penyimpanan yang berbeda.
- Upload versi baru ke alamat website yang sama umumnya mempertahankan data browser selama data situs dan nama kunci penyimpanan tidak dihapus atau diubah.

### Cadangkan dan pulihkan

| Data | Lokasi fitur |
| --- | --- |
| Jawaban dan riwayat latihan/absensi | Menu Jepang → **Cadangkan hasil (JSON)** / **Pulihkan hasil** |
| Penanda kanji, kotoba, dan progres flashcard | Menu Flashcard → **Cadangkan progres belajar** / **Pulihkan progres** |

Kedua cadangan tersebut terpisah. Keduanya belum mencakup seluruh data, seperti agenda dan nama panggilan. Simpan cadangan sebelum mengganti perangkat atau alamat website.

## Menjalankan secara lokal

1. Unduh atau clone repository ini.
2. Buka file **`index.html`** menggunakan browser modern.
3. Tidak diperlukan instalasi Python, database, atau proses build.

Tampilan, logika, materi, dan font Jepang disertakan dalam HTML. Beberapa ikon dan utilitas tampilan menggunakan CDN, sehingga pemuatannya membutuhkan internet.

## Struktur repository

| File | Keterangan |
| --- | --- |
| `index.html` | File utama dashboard: HTML, CSS, JavaScript, serta data pembelajaran. |
| `README.md` | Dokumentasi proyek ini. |

## Publikasi melalui GitHub Pages

Untuk repository ini, gunakan **Settings → Pages** dengan sumber publikasi berikut:

| Pengaturan | Nilai |
| --- | --- |
| Source | Deploy from a branch |
| Branch | main |
| Folder | / (root) |

Pastikan **`index.html` berada di folder utama**. Setelah deployment selesai, buka alamat GitHub Pages, bukan halaman daftar file repository.

## Memperbarui website

Ganti `index.html` dengan versi terbaru, commit perubahan, lalu push ke GitHub. Periksa deployment pada tab **Actions** sampai selesai.

Jika bekerja melalui Git lokal:

1. Pastikan perubahan lokal sudah di-commit.
2. Ambil perubahan dari GitHub:

   ```bash
   git pull --rebase origin main
   ```

3. Jika proses selesai tanpa konflik, kirim perubahan:

   ```bash
   git push origin main
   ```

Jika muncul `CONFLICT`, selesaikan konflik sebelum melanjutkan push. Hindari force push untuk mengatasi penolakan `fetch first` karena dapat menimpa riwayat perubahan.

## Cakupan materi

- Roadmap menampilkan target **45 hari**, tetapi materi dan soal yang tersedia saat ini baru **Day 1–4**.
- Daftar kanji dan kotoba merupakan bahan belajar pilihan, **bukan daftar resmi lengkap JLPT**.
- Sebagian kanji N4 juga terdapat pada daftar N5. Kartu gabungan flashcard menghindari penggandaan karakter yang sama.
- Paket latihan tertulis ini belum mencakup ujian listening.
- Agenda bawaan merupakan contoh yang bisa disesuaikan. Rekap absensi dan latihan bulanan menggunakan hasil yang benar-benar tersimpan.
- Waktu, tanggal absensi, dan hitung mundur mengikuti perangkat pengguna, bukan verifikasi waktu server.

## Sumber dan atribusi

- [KANJIDIC2 / EDRDG](https://www.edrdg.org/kanjidic/kanjidic2_ov_legacy.html), melalui [kanji-data](https://github.com/sepTN/kanji-data), untuk jumlah goresan kanji.
- [KanaMastery — N4 Kanji](https://kanamastery.com/jlpt/n4/kanji), sebagai rujukan pengelompokan 166 kanji N4.
- **Noto Sans JP**, disertakan untuk mendukung tampilan huruf Jepang; informasi lisensi font tercantum di dalam HTML.
- [Situs resmi JLPT](https://www.jlpt.jp/e/faq/), untuk informasi resmi mengenai ujian dan cakupan pembelajaran.

Arti ringkas, contoh kalimat, dan terjemahan digunakan sebagai pendamping belajar. Hasil latihan dashboard bukan skor resmi atau jaminan kelulusan JLPT.

---

Dikelola oleh **Tata Dico Puji Handoko** · [Tadipuhan](https://github.com/Tadipuhan)
