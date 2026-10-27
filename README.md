# Tadicoba

Dashboard aktivitas harian dan pendamping belajar bahasa Jepang N5–N4 dalam satu website. Tadicoba menggabungkan agenda, latihan soal, kartu kanji, kotoba, flashcard, dan rekap kehadiran belajar.

**[Alamat GitHub Pages](https://tadipuhan.github.io/Dailyactivity/)**

## Fitur

| Menu / fitur | Fungsi |
| --- | --- |
| Ringkasan | Melihat progres tugas dan hasil latihan yang tersimpan. |
| Aktivitas harian | Menambah, mengubah, menghapus, dan menandai agenda selesai. |
| Jepang · 45 hari | Membaca materi dan mengerjakan latihan. Materi dan soal **Day 1–45** tersedia lengkap. |
| Latihan pilihan ganda | Masing-masing hari berisi **40 soal dengan 4 pilihan**, nilai otomatis, dan pembahasan setelah pengiriman. |
| Absensi belajar | Mencatat kehadiran berdasarkan tanggal perangkat saat seluruh 40 jawaban dikirim. |
| Akumulasi bulanan | Menampilkan hari hadir, jumlah latihan, waktu aktif, rata-rata nilai, dan kalender absensi aktual. |
| Kanji N5 | **103 kartu** berisi kanji, arti, jumlah goresan, onyomi, kunyomi, romaji, dan contoh penggunaan. |
| Kanji N4 | **166 kartu** dengan pencarian, filter kelompok, dan penanda belajar. |
| Kotoba N5–N4 | **424 kosakata pilihan** beserta bacaan dan arti bahasa Indonesia. |
| Flashcard | **670 kartu unik** kanji dan kotoba, dengan 4 pilihan jawaban, penilaian otomatis, dan filter latihan. |
| Print / PDF | Cetak materi, soal, atau gabungannya per Day maupun seluruh 45 Day; cetak kanji penuh atau per kelompok. |
| Identitas Tadicoba | Logo pada dashboard, popup nama, tab browser, dan lembar cetak. |
| Personalisasi | Popup nama panggilan, sapaan sesuai waktu, serta tombol untuk mengubah nama. |
| Jam & target | Jam berjalan per detik dan hitung mundur menuju **5 Desember 2026 pukul 00.00**, mengikuti waktu perangkat. |

Tampilan menyesuaikan ukuran HP, tablet, dan laptop. Daftar kanji menggunakan kartu dengan pilihan jumlah kartu per halaman. Lembar cetak kanji memakai **3 kolom pada kertas A4**.

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

## Print dan Simpan PDF

### Materi dan soal Jepang

Buka **Jepang · 45 hari → Print / PDF**, kemudian pilih salah satu mode:

| Mode | Isi |
| --- | --- |
| Print materi saja per Day | Materi dari satu Day yang dipilih. |
| Print soal saja per Day | 40 soal dan bacaan dari satu Day, tanpa kunci atau jawaban pengguna. |
| Print materi dan soal per Day | Materi, bacaan, dan 40 soal dari satu Day. |
| Print full materi 45 Day | Seluruh materi Day 1–45. |
| Print full soal 45 Day | Seluruh 1.800 soal beserta bacaan. |
| Print full materi dan soal 45 Day | Seluruh materi dan soal Day 1–45. |

Untuk mode per Day, pilih hari melalui kolom **Hari belajar**. Setiap Day dimulai pada halaman baru; pada mode gabungan, bagian soal juga dimulai pada halaman baru.

### Kanji N5 dan N4

Buka menu **Kanji N5** atau **Kanji N4**, lalu klik **Print / PDF**.

| Mode | Hasil |
| --- | --- |
| Full N5 / N4 | Seluruh kartu level yang dipilih dalam urutan nomor asli. |
| Full N5 / N4 — pisah per pengelompokan | Seluruh kartu, dengan setiap kelompok dimulai pada halaman baru. |

Kedua mode menggunakan **3 kolom per halaman A4**, berisi kanji, arti, bacaan pilihan, romaji, jumlah goresan, contoh kata, serta contoh kalimat. Filter pencarian, status belajar, dan pagination pada layar tidak membatasi jumlah kartu yang dicetak.

### Mencetak atau menyimpan

1. Tentukan isi, lalu klik **Buka pratinjau cetak**.
2. Klik **Cetak / Simpan PDF** setelah dokumen siap.
3. Pilih printer untuk mencetak fisik, atau **Save as PDF / Simpan sebagai PDF** untuk menyimpan file.
4. Gunakan kertas **A4**, skala **100%**, serta nonaktifkan **header/footer browser** agar bingkai sesuai desain.
5. Periksa jumlah halaman dan rentang halaman sebelum mencetak seluruh paket.

Lembar menggunakan bingkai dark Tadicoba yang berulang pada setiap halaman. Jika browser memblokir jendela baru, pratinjau akan ditampilkan di dalam dashboard. Pilihan printer dan penyimpanan PDF mengikuti fasilitas browser/perangkat.

Mencetak atau menyimpan PDF tidak mencatat absensi; kehadiran tetap diperoleh dari pengiriman 40 jawaban di website.

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

Untuk memulihkan hasil, klik **Pulihkan hasil**, pilih JSON cadangan dari fitur yang sama, lalu periksa riwayat. Riwayat latihan digabung berdasarkan ID percobaan agar tidak berganda, dan tanggal absensi asli dipertahankan. Mengimpor cadangan tidak otomatis membuat kehadiran baru pada hari impor. Draf yang ikut diekspor tidak dimuat ulang oleh fitur pemulihan riwayat saat ini.

Kedua cadangan tersebut terpisah. Keduanya belum mencakup seluruh data, seperti agenda dan nama panggilan. Simpan cadangan sebelum mengganti perangkat atau alamat website.

## Menjalankan secara lokal

1. Unduh atau clone repository ini. Jika file unduhan bernama `Tadicoba.html`, ubah menjadi `index.html` saat menyiapkan repository.
2. Buka file **`index.html`** menggunakan browser modern.
3. Tidak diperlukan instalasi Python, database, atau proses build.

Tampilan, logika, materi, font Jepang, logo, serta bingkai cetak Tadicoba disertakan dalam HTML; tidak perlu mengunggah logo atau bingkai sebagai file terpisah. Beberapa ikon dan utilitas tampilan menggunakan CDN, sehingga pemuatannya membutuhkan internet.

## Struktur repository

| File | Keterangan |
| --- | --- |
| `index.html` | File utama dashboard: HTML, CSS, JavaScript, serta data pembelajaran. |
| `README.md` | Dokumentasi proyek ini. |

## Publikasi melalui GitHub Pages

Nama website yang tampil adalah **Tadicoba**. Nama repository dapat tetap `Dailyactivity`; mengganti nama tampilan tidak mengharuskan penggantian alamat website.

Untuk repository ini, gunakan **Settings → Pages** dengan sumber publikasi berikut:

| Pengaturan | Nilai |
| --- | --- |
| Source | Deploy from a branch |
| Branch | main |
| Folder | / (root) |

Pastikan **`index.html` berada di folder utama**. Setelah deployment selesai, buka alamat GitHub Pages, bukan halaman daftar file repository.

## Memperbarui website

Cadangkan hasil dan progres belajar terlebih dahulu. Unduh HTML Tadicoba terbaru, ubah namanya menjadi `index.html`, lalu ganti file lama pada folder utama repository. Commit perubahan dan push ke GitHub. Periksa deployment pada tab **Actions** sampai selesai.

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

## Materi Day 1–45

| Day | Fokus |
| --- | --- |
| 1 | N5 ke N4 |
| 2 | Kata Kerja |
| 3 | Permintaan dan Aturan |
| 4 | Lampau dan Pengalaman |
| 5 | Kata sifat dan perbandingan |
| 6 | Keberadaan, posisi, dan jumlah |
| 7 | Keinginan, niat, dan rencana |
| 8 | Kemampuan dan hobi |
| 9 | Alasan dan urutan kegiatan |
| 10 | Review terpadu Day 1–9 |
| 11 | Bentuk biasa, pendapat, dan kutipan |
| 12 | Kewajiban, larangan, dan tidak perlu |
| 13 | Memberi, menerima, dan bantuan |
| 14 | Saran, penjelasan, dan dugaan |
| 15 | Sedang berlangsung, keadaan, dan perubahan |
| 16 | Mencoba, persiapan, dan penyelesaian |
| 17 | Syarat と・たら・ば dan konsesi ても |
| 18 | Tampaknya, kabar, dan rencana yang diharapkan |
| 19 | Klausa penjelas, nominalisasi, dan kegiatan bersamaan |
| 20 | Review terpadu Day 11–19 |
| 21 | Niat, keputusan, dan ketetapan |
| 22 | Tujuan, manfaat, dan pemakaian alat |
| 23 | Kebiasaan dan perubahan kemampuan |
| 24 | Bentuk pasif dan sudut pandang |
| 25 | Menyuruh, membiarkan, dan meminta izin |
| 26 | Mulai, selesai, berlebihan, dan kemudahan |
| 27 | Waktu とき・間 dan tahap kegiatan |
| 28 | Pertanyaan di dalam kalimat |
| 29 | Permintaan sopan dan bahasa layanan |
| 30 | Review terpadu Day 21–29 |
| 31 | Keadaan hasil dan persiapan |
| 32 | Pergerakan dan perubahan ていく・てくる |
| 33 | Alasan majemuk dan hasil yang berlawanan |
| 34 | Memilih syarat と・ば・たら・なら |
| 35 | Batas, jumlah, dan perbandingan |
| 36 | Permintaan, harapan, dan bantuan |
| 37 | Dugaan dan bukti dalam konteks |
| 38 | Membaca pengumuman dan jadwal |
| 39 | Instruksi kerja, urutan, dan keselamatan |
| 40 | Review makna dan hubungan antarkalimat |
| 41 | Review potensial, pasif, dan kausatif |
| 42 | Penguatan bacaan kanji dan kosakata |
| 43 | Susunan kalimat dan klausa penjelas |
| 44 | Bacaan pesan, rujukan, dan kesimpulan |
| 45 | Review akhir 45 hari |

Setiap Day dilengkapi materi, kosakata pendukung, bacaan pendek, 40 soal dengan empat pilihan, serta pembahasan setelah pengiriman. Total tersedia **1.800 soal**.

## Cakupan materi

- Materi dan soal tersedia untuk **seluruh Day 1–45**, masing-masing 40 soal dengan empat pilihan jawaban.
- Daftar kanji dan kotoba merupakan bahan belajar pilihan, **bukan daftar resmi lengkap JLPT**.
- Sebagian kanji N4 juga terdapat pada daftar N5. Kartu gabungan flashcard menghindari penggandaan karakter yang sama.
- Paket latihan tertulis ini belum mencakup ujian listening.
- Agenda bawaan merupakan contoh yang bisa disesuaikan. Rekap absensi dan latihan bulanan menggunakan hasil yang benar-benar tersimpan.
- Waktu, tanggal absensi, dan hitung mundur mengikuti perangkat pengguna, bukan verifikasi waktu server.

## Sumber dan atribusi

- [Japan Foundation — Irodori](https://www.irodori.jpf.go.jp/) dan [TUFS — modul tata bahasa Jepang](https://www.coelang.tufs.ac.jp/mt/ja/gmod/), sebagai rujukan pendalaman pola. Susunan materi dan soal dashboard dibuat tersendiri.

- [KANJIDIC2 / EDRDG](https://www.edrdg.org/kanjidic/kanjidic2_ov_legacy.html), melalui [kanji-data](https://github.com/sepTN/kanji-data), untuk jumlah goresan kanji.
- [KanaMastery — N4 Kanji](https://kanamastery.com/jlpt/n4/kanji), sebagai rujukan pengelompokan 166 kanji N4.
- **Noto Sans JP**, disertakan untuk mendukung tampilan huruf Jepang; informasi lisensi font tercantum di dalam HTML.
- [Situs resmi JLPT](https://www.jlpt.jp/e/faq/), untuk informasi resmi mengenai ujian dan cakupan pembelajaran.

Arti ringkas, contoh kalimat, dan terjemahan digunakan sebagai pendamping belajar. Hasil latihan dashboard bukan skor resmi atau jaminan kelulusan JLPT.

---

Dikelola oleh **Tata Dico Puji Handoko** · [Tadipuhan](https://github.com/Tadipuhan)
