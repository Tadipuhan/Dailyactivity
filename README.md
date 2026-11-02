# Tadicoba

**Satu ruang, dua perjalanan.** Website belajar mandiri Bahasa Jepang dan Bahasa Inggris dengan materi, latihan, kosakata, cerita, serta pendamping belajar **Nao**.

Antarmuka menggunakan Bahasa Indonesia. Pilihan Jepang atau Inggris menentukan **bahasa yang dipelajari**, bukan bahasa antarmuka.

<<<<<<< HEAD
> Dokumentasi versi dua bahasa, diperbarui 2 November 2026. Aplikasi berjalan sebagai website statis berbasis HTML, CSS, dan JavaScript. Progres tersimpan di browser; belum ada akun atau sinkronisasi cloud.
=======
> Dokumentasi untuk versi **Kotoba Menu N5–N1**, dengan Dasar Jepang, Nao, dan tampilan Desain Terpadu, diperbarui **1 November 2026**. Website dijalankan dari `index.html` tanpa instalasi atau proses build.
>>>>>>> bcf7939f7405ad8857d8cbf214c126766e1529e9

## Ringkasan

<<<<<<< HEAD
| Bagian | Cakupan |
| --- | --- |
| Bahasa Jepang | Rencana belajar 45 hari, dasar kana, materi N5–N4, latihan, referensi kanji dan kotoba pilihan N5–N1. |
| Bahasa Inggris | Tujuh modul dasar A1, 105 kosakata, 105 soal harian, alfabet dan cara membaca, verbs, referensi tenses, serta lima cerita A1. |
| Latihan berbicara | Lima kalimat per bahasa dengan mikrofon, contoh audio, dan penanda kecocokan transkrip. |
| Nao | Maskot 2D: versi ungu untuk Jepang dan versi sage berambut putih untuk Inggris. |
| Penyimpanan | Data lokal pada browser/perangkat yang digunakan, dengan fitur cadangan yang tersedia di aplikasi. |
=======
- [Pembaruan 1 November 2026](#pembaruan-1-november-2026)
- [Pembaruan 29 Oktober 2026](#pembaruan-29-oktober-2026)
- [Fitur utama](#fitur-utama)
- [Desain dan navigasi](#desain-dan-navigasi)
- [Mulai menggunakan](#mulai-menggunakan)
- [Dasar Jepang](#dasar-jepang)
- [Materi, latihan, dan absensi](#materi-latihan-dan-absensi)
- [Kanji, kotoba, dan flashcard](#kanji-kotoba-dan-flashcard)
- [Maskot Nao dan pengaturan suara](#maskot-nao-dan-pengaturan-suara)
- [Cerita dan audio](#cerita-dan-audio)
- [Print dan simpan PDF](#print-dan-simpan-pdf)
- [Penyimpanan dan cadangan](#penyimpanan-dan-cadangan)
- [Menjalankan secara lokal](#menjalankan-secara-lokal)
- [Publikasi melalui GitHub Pages](#publikasi-melalui-github-pages)
- [Memperbarui website](#memperbarui-website)
- [Pemecahan masalah](#pemecahan-masalah)
- [Materi Day 1–45](#materi-day-145)
- [Teknologi dan atribusi](#teknologi-dan-atribusi)

## Pembaruan 1 November 2026

- Mengubah arti **367 kartu kanji N2** dan **1.232 kartu kanji N1** menjadi bahasa Indonesia, dengan padanan ringkas dan pemisah “·” seperti N5–N3. Label bahasa, pencarian, dan cetak ikut disesuaikan.
- Menambahkan cakupan kotoba **N3, N2, dan N1**, masing-masing **100 kata pilihan awal** dengan bacaan kana, arti Indonesia, dan kelompok tema. Daftar ini belum mencakup seluruh kosakata ketiga level.
- Menggabungkan 28 kata yang sudah ada dengan label level tambahan, sehingga tidak membuat baris duplikat. Total kini **696 kata unik**.
- Mengubah sidebar menjadi **Kotoba ⌄**, yang membuka submenu **Kotoba N5, N4, N3, N2, dan N1** seperti menu Kanji. Memilih level langsung membuka halaman dengan filter level tersebut serta mengosongkan filter pencarian dan penanda.
- Memperluas filter dan data flashcard untuk kotoba N5–N1. Kartu kanji pada flashcard tetap mencakup N5–N4.
- Memperluas cetak kotoba menjadi **12 mode**: gabungan N5–N1 atau satu dari lima level, masing-masing dalam mode gabungan kelompok atau dipisah per kelompok.
- Mempertahankan ID kata lama dan kunci penyimpanan progres agar penanda yang sudah tersimpan tetap dapat digunakan pada alamat situs yang sama.

**Pemeriksaan pembaruan ini:** sintaks JavaScript, jumlah dan keunikan data, keluaran tabel 12 mode cetak, serta logika buka-tutup submenu, pemilihan level, dan status aktif telah diperiksa. Tampilan visual dan dialog cetak browser versi ini belum diuji langsung. Pembaruan file tidak berarti website GitHub Pages sudah diperbarui.

## Pembaruan 29 Oktober 2026

- Menambahkan **Nao**, maskot chibi interaktif dengan latar transparan, bubble dialog oval ringkas tanpa label nama, kedipan, gerak mulut, dan arah pandang mengikuti pointer.
- Menyesuaikan posisi mata dan mulut terhadap kemiringan wajah pada setiap pose; memperbaiki area kedip dan posisi mulut pada reaksi salah.
- Mengunci skala gambar dan titik acuan wajah saat berganti reaksi. Perubahan teks bubble tidak mengubah posisi karakter.
- Menghubungkan reaksi Nao dengan navigasi menu, hasil jawaban flashcard, dan penyelesaian latihan harian.
- Menambahkan pengaturan suara, kurangi gerakan, sembunyikan, dan tampilkan kembali Nao; preferensinya disimpan di browser.
- Mengatur gaya suara **anak perempuan ekspresif berbahasa Indonesia**, dengan variasi nada, tempo, dan jeda per reaksi. Suara tetap berasal dari perangkat, belum berupa rekaman pengisi suara khusus.
- Menerapkan ilustrasi **S01 Torii** pada sidebar dan **B05 Kumo** pada latar halaman; keduanya tertanam dalam HTML.
- Memperbaiki gambar latar yang tidak muncul dengan mengganti variabel CSS berisi data gambar besar menjadi deklarasi `background-image` langsung, serta menyesuaikan skala motif Kumo.

**Status pemeriksaan:** sintaks JavaScript dan data kedua gambar telah diperiksa. Tampilan serta interaksi versi terbaru belum terverifikasi melalui browser pengujian. Dokumentasi ini tidak menyatakan pembaruan sudah diunggah ke GitHub Pages.

## Fitur utama

| Menu / fitur | Kegunaan |
| --- | --- |
| Dashboard | Ringkasan agenda, progres latihan, grafik mingguan, status kehadiran, serta tombol lanjut belajar. |
| Aktivitas harian | Menambah, mengedit, menghapus, dan menandai agenda selesai. |
| Dasar Jepang | Hiragana, katakana, aturan membaca, audio perangkat, animasi goresan, serta latihan kana empat pilihan. |
| Materi harian — Studio Fokus | Memilih **Day 1–45**, membaca materi, lalu mengerjakan **40 soal dengan 4 pilihan** per Day. Total **1.800 soal**. |
| Rekap bulanan | Kalender kehadiran, jumlah percobaan latihan, waktu aktif, nilai, dan evaluasi bulanan. |
| Kanji | Submenu dan tab **N5, N4, N3, N2, N1**, dengan kartu, pencarian, filter, penanda belajar, dan cetak. |
| Kotoba | Submenu buka-tutup **N5–N1**, **696 kata unik**, bacaan kana, arti Indonesia, kelompok tema, penanda belajar, dan cetak. |
| Flashcard | Kanji N5–N4 dan kotoba N5–N1, dengan filter level, empat pilihan jawaban, dan umpan balik langsung. |
| Cerita | Tiga cerita orisinal, pilihan versi N5/N4, furigana, terjemahan per paragraf, dan audio sesuai dukungan perangkat. |
| Maskot Nao | Pendamping chibi dengan reaksi kontekstual, bubble dialog, kedipan, gerak mulut, arah pandang pointer, serta pengaturan suara dan gerakan. |
| Latar Jepang | Sidebar S01 Torii dan background B05 Kumo, disematkan langsung dalam HTML. |
| Tema | **Terang, Gelap, atau Sistem**, dengan pilihan tema tersimpan di browser. |
| Personalisasi | Nama panggilan, sapaan sesuai waktu, jam berjalan, dan hitung mundur ke **5 Desember 2026 pukul 00.00** menurut waktu perangkat. |
| Print / PDF | Materi dan soal per Day atau seluruh 45 Day; kanji dan kotoba lengkap atau dipisah per kelompok. |
>>>>>>> bcf7939f7405ad8857d8cbf214c126766e1529e9

Materi merupakan sarana latihan mandiri. Menyelesaikan paket bukan sertifikasi A1, skor resmi JLPT, atau jaminan kelulusan.

## Mulai menggunakan

1. Buka website, lalu pilih **Bahasa Jepang** atau **Bahasa Inggris**.
2. Pengguna Jepang melanjutkan melalui intro Shōji menuju dashboard.
3. Pengguna Inggris masuk ke dashboard **Sage Study**. Tutorial Nao menjelaskan urutan belajar untuk pemula dan dapat dibuka kembali melalui menu.
4. Pelajari materi sebelum mengerjakan latihan.
5. Simpan cadangan progres secara berkala melalui menu yang tersedia.

Pilihan terakhir diingat untuk tombol **Lanjutkan** pada halaman pemilih. Gunakan **Ganti pelajaran** untuk kembali memilih bahasa.

## Bahasa Jepang

- Materi harian **Day 1–45**, berfokus pada penguatan N5 dan persiapan N4.
- **40 soal pilihan ganda per hari**, dengan empat pilihan dan pembahasan; total 1.800 soal.
- Dasar **hiragana dan katakana**, aturan membaca, bantuan audio, serta latihan kana.
- Referensi **kanji N5–N1**, termasuk bacaan, arti, pencarian, filter, serta contoh atau urutan goresan sesuai data yang tersedia.
- **Kotoba pilihan N5–N1**, dengan submenu level yang dapat dibuka dan ditutup.
- Flashcard, penanda belajar, ringkasan aktivitas, dan rekap progres.
- Tiga cerita dengan pilihan versi N5/N4, furigana, terjemahan, serta audio sesuai dukungan perangkat.
- Cetak materi, soal, kanji, atau kotoba melalui fitur yang tersedia; pilih **Simpan sebagai PDF** pada dialog cetak browser bila diperlukan.

Daftar level lanjutan adalah referensi pilihan dan tidak boleh dianggap sebagai seluruh daftar kosakata resmi JLPT. Ketersediaan data berbeda pada setiap entri.

## Bahasa Inggris — Sage Study

Dashboard menggunakan warna sage, ivory, dan hijau gelap. Pada laptop, area aplikasi mengikuti tinggi layar; sidebar memiliki scroll sendiri jika menu melebihi ruang. Materi panjang dapat digulir di area konten. Pada layar kecil, susunan menyesuaikan ruang yang tersedia.

### Urutan belajar untuk pemula

1. **Alfabet & membaca:** kenali 26 huruf, nama huruf, perbedaan nama dan bunyi, serta contoh pengucapan.
2. **Verbs:** pelajari `be`, kata kerja tindakan, dan contoh kalimat sederhana.
3. **Materi & latihan:** mulai dari Day 1, lalu lanjutkan secara bertahap hingga Day 7.
4. **Kosakata:** dengarkan dan ulangi kata dari modul yang dipelajari.
5. **Cerita A1:** baca, dengarkan, periksa terjemahan, lalu jawab pertanyaan pemahaman.
6. **Latihan berbicara:** dengarkan contoh dan ucapkan kalimat melalui mikrofon.

Satu modul boleh dikerjakan dalam beberapa sesi. Tujuh modul bukan janji menguasai seluruh kompetensi A1 dalam tujuh hari.

### Menu

<<<<<<< HEAD
| Menu | Isi |
=======
Tombol **Cek awal · 10 soal** menyediakan pemeriksaan singkat dengan kedua aksara. Latihan mengambil huruf dasar; contoh kata dapat memuat gabungan bunyi dan vokal panjang yang dibahas pada aturan membaca.

Ringkasan **20 sesi terakhir** disimpan pada perangkat. Latihan kana **tidak mencatat absensi** dan tidak menggantikan latihan 40 soal per Day. Riwayat kana belum termasuk ekspor/pemulihan JSON utama.

Audio menggunakan suara Jepang dari perangkat melalui Web Speech API. Jika suara Jepang tidak tersedia, tombol audio dinonaktifkan dan latihan tetap dapat dikerjakan melalui teks. Ketersediaan serta kualitas suara bergantung pada browser dan perangkat.

## Materi, latihan, dan absensi

- Seluruh **Day 1–45** sudah memiliki materi dan latihan.
- Setiap Day berisi **40 soal dengan empat pilihan jawaban**. Nilai dan pembahasan ditampilkan setelah pengiriman.
- Draf pilihan jawaban disimpan pada browser agar dapat dilanjutkan.
- Kehadiran tercatat setelah seluruh **40 jawaban dikirim**, meskipun nilainya belum mencapai target.
- Satu tanggal dihitung sebagai **satu hari hadir**; beberapa latihan pada hari yang sama tetap tersimpan sebagai percobaan terpisah.
- Nilai **≥80%** menandai Day tuntas sebagai target pribadi, bukan standar kelulusan resmi JLPT.
- Tanggal kehadiran mengikuti **tanggal perangkat saat jawaban dikirim**, bukan waktu server.
- Membaca materi, mencetak, menandai kanji, membaca cerita, dan mengerjakan flashcard tidak menggantikan absensi 40 soal.
- Waktu belajar dalam rekap berasal dari waktu aktif latihan yang tersimpan pada pengiriman, bukan seluruh waktu membuka website.

Tombol cadangan dan tautan pengulangan tersedia pada **Materi harian → Alat belajar & cadangan**.

## Kanji, kotoba, dan flashcard

### Cakupan kartu kanji

| Level | Jumlah kartu | Bahasa arti | Contoh penggunaan |
| --- | ---: | --- | --- |
| N5 | 103 | Indonesia | Kalimat Jepang, bacaan kana, terjemahan Indonesia, dan contoh kata. |
| N4 | 166 | Indonesia | Kalimat Jepang, bacaan kana, terjemahan Indonesia, dan contoh kata. |
| N3 | 367 | Indonesia | Kalimat Jepang, bacaan kana, terjemahan Indonesia, dan contoh kata pada seluruh kartu. |
| N2 | 367 | Indonesia | Belum dilengkapi contoh kalimat seperti N5–N3. |
| N1 | 1.232 | Indonesia | Belum dilengkapi contoh kalimat seperti N5–N3. |

Kartu menampilkan karakter, arti, onyomi, kunyomi, romaji, jumlah goresan, dan penanda belajar. Tombol animasi pada **seluruh level N5–N1** membuka urutan goresan dengan kontrol langkah, putar/jeda, ulangi, kecepatan, dan nomor goresan. Data vektor disematkan dalam HTML sehingga animasi tidak memerlukan pengambilan data dari server. Pemutaran dimulai atas tindakan pengguna. Format arti N3–N1 memakai pemisah **“·”**, mengikuti N4/N5. Beberapa bacaan kamus pada level lanjutan menggunakan tanda titik untuk memisahkan bagian kanji dan okurigana.

Gunakan submenu **Kanji** atau tab level untuk berpindah halaman. Pencarian, filter kelompok, status, dan pilihan jumlah kartu per halaman membantu meninjau daftar. N3–N1 dikelompokkan berdasarkan jumlah goresan.

Daftar ini merupakan **referensi belajar pilihan, bukan daftar resmi lengkap JLPT**. Penetapan level dapat berbeda dari sumber atau buku lain, dan sebagian karakter dapat muncul pada beberapa level. Makna kanji serta bacaannya dapat berubah sesuai kata dan konteks.

### Kotoba N5–N1

Klik **Kotoba ⌄** pada sidebar untuk membuka atau menutup submenu, lalu pilih level. Di HP, buka **Menu** terlebih dahulu. Pilihan level, pencarian kata/kana/arti, dan filter penanda juga tersedia pada halaman Kotoba. Gunakan **Hapus filter** untuk kembali ke semua level.

| Level | Jumlah kata yang berlabel level tersebut | Cakupan |
| --- | ---: | --- |
| N5 | 188 | Daftar pilihan yang sudah tersedia. |
| N4 | 250 | Daftar pilihan yang sudah tersedia. |
| N3 | 100 | Paket awal pilihan; belum seluruh kosakata N3. |
| N2 | 100 | Paket awal pilihan; belum seluruh kosakata N2. |
| N1 | 100 | Paket awal pilihan; belum seluruh kosakata N1. |

Total **696 kata unik**. Jumlah per level tidak dapat langsung dijumlahkan sebagai jumlah kata unik, karena satu kata dapat memiliki beberapa label level. Kata yang sama dengan bacaan sama menggunakan satu baris dan satu penanda belajar. Setiap baris berisi kata, bacaan kana, arti Indonesia, kelompok tema, dan penanda **Baru / Ragu atau ulangi / Lancar**.

Pengelompokan merupakan panduan belajar Tadicoba, bukan penetapan level resmi JLPT. Kata dapat dipelajari lebih awal atau lebih akhir pada buku lain. Daftar baru tidak mengubah materi harian 45 hari menjadi kursus N3–N1.

### Flashcard

Flashcard mencakup **kanji N5–N4 dan kotoba N5–N1**. Filter N3–N1 saat ini berisi kotoba; belum ada kartu kanji lanjutan pada kumpulan flashcard. Pilih level, jenis materi, kelompok kartu, arah latihan, dan jumlah kartu per sesi, lalu tekan **Mulai / acak sesi**.

Jawaban salah dijadwalkan ulang besok; jawaban benar empat hari kemudian. Penilaian langsung menunjukkan jawaban yang benar dan progres tersimpan pada browser.

## Maskot Nao dan pengaturan suara

Nao tampil sebagai pendamping di sudut layar. Klik karakter untuk mendapatkan petunjuk umum; klik **×** pada bubble untuk menutup dialog dan menghentikan ucapannya. Label nama di atas bubble dihilangkan.

### Reaksi dan animasi

Enam pose yang tersedia adalah **netral, menyapa, berpikir, senang, bingung, dan merayakan**. Pemakaiannya mengikuti tindakan yang sudah dihubungkan, bukan percakapan AI bebas.

| Pemicu | Respons |
>>>>>>> bcf7939f7405ad8857d8cbf214c126766e1529e9
| --- | --- |
| Dashboard | Modul terakhir, progres tujuh modul, akses tutorial, dan pilihan latihan. |
| Alfabet & membaca | Huruf, bantuan fonetik, contoh audio, pola bunyi, tekanan kata, serta beberapa akhiran umum. |
| Verbs | 30 kata kerja dasar, bentuk V1/V2/V3/-ing, arti, contoh, pola negatif dan pertanyaan, serta latihan mandiri. |
| Referensi tenses | Dua belas bentuk tense/aspect yang umum diajarkan, dengan pola dan contoh; materi lanjutan berfungsi sebagai referensi. |
| Cerita A1 | Lima cerita, terjemahan Indonesia, kosakata bantuan, audio, serta pertanyaan dan pembahasan. |
| Tutorial Nao | Panduan mulai belajar untuk pemula. |
| Materi & latihan | Tujuh modul, masing-masing berisi 15 kosakata dan 15 soal. |
| Kosakata | Tabel kosakata dengan filter Day. |
| Hasil & cadangan | Riwayat latihan dan pengelolaan cadangan progres Inggris. |
| Latihan berbicara | Sesi lima kalimat menggunakan mikrofon. |

Referensi tenses tidak menjadikan semua bentuk continuous cocok untuk semua verb. Perhatikan penjelasan penggunaan dan pengecualian di materi.

### Lima cerita A1

1. **A New Friend** — perkenalan.
2. **Ben’s Morning** — rutinitas.
3. **At the Fruit Shop** — belanja.
4. **A Rainy Afternoon** — kegiatan yang sedang berlangsung.
5. **Our Picnic Plan** — rencana.

## Nao dan animasi

Nao menjadi pendamping belajar 2D dan identitas visual Tadicoba.

- **Jepang:** rambut lavender, mata ungu, hoodie gelap, serta headphone beraksen ungu.
- **Inggris:** rambut putih, mata hijau, hoodie sage, dan headphone hijau.
- Pose Inggris: **Menyapa** saat masuk, **Bersandar** saat standby, dan **Menjelaskan** saat menu disorot atau dipilih.
- Pergantian pose menggunakan crossfade dan easing.
- Mata berkedip, mulut bergerak sesekali, dan rambut diberi gerakan ringan. Mata pada dashboard Inggris mengikuti pointer pada perangkat yang mendukungnya.
- Gerakan menyesuaikan preferensi **reduced motion** perangkat/browser.

Gerakan mulut dekoratif tidak otomatis merupakan lip sync dengan seluruh audio. Model 3D bukan bagian dari website ini.

## Latihan berbicara dan mikrofon

1. Buka **Latihan berbicara** pada bahasa yang dipilih.
2. Dengarkan contoh dengan tombol audio.
3. Tekan tombol mikrofon dan berikan izin akses.
4. Baca satu kalimat dengan suara jelas.
5. Setelah pengenalan selesai, periksa bagian hijau dan merah, lalu ulangi atau lanjutkan.

**Hijau dan merah menunjukkan kecocokan hasil transkripsi dengan kalimat target, bukan penilaian bunyi atau aksen secara fonetis.** Pengenalan suara bisa keliru meskipun pengguna membaca dengan benar. Pada Jepang, pembandingan menggunakan normalisasi kana.

Fitur menggunakan `SpeechRecognition` atau `webkitSpeechRecognition`, bila tersedia. Dukungan browser berbeda. Halaman harus berjalan dalam secure context; gunakan **HTTPS atau localhost** untuk pengujian mikrofon. Layanan pengenalan suara dapat memerlukan internet dan dapat memproses audio melalui layanan browser. Tidak ada jaminan fitur mikrofon bekerja offline.

Nilai sesi berbicara tidak boleh disamakan dengan hasil latihan pilihan ganda; hasil sesi mikrofon belum disimpan sebagai riwayat progres permanen.

## Audio

<<<<<<< HEAD
Pembacaan contoh menggunakan `speechSynthesis` dan suara yang tersedia di browser/sistem operasi. Bahasa, pilihan suara, dan kualitasnya bergantung pada perangkat. Contoh audio dapat dipakai tanpa menyalakan mikrofon bila dukungan pembacaan suara tersedia.
=======
Daftar cerita menampilkan tiga kartu:

1. **Kucing Kecil dan Payung Biru** — kebaikan dan persahabatan.
2. **Kelinci dan Roti Bulan** — berbagi dan kerja sama.
3. **Hari-hari Sebuah Benih Kecil** — kesabaran dan merawat.

Setiap cerita mempunyai versi **N5 dan N4**, masing-masing delapan paragraf. Kata yang berada di luar daftar kanji versi terpilih ditampilkan dalam kana.

- Klik kartu untuk membaca, lalu gunakan **Semua cerita** untuk kembali ke daftar.
- Buka/tutup terjemahan Indonesia di bawah setiap paragraf.
- Gunakan jendela **Pengaturan baca** untuk memilih versi kanji N5/N4 dan mengaktifkan atau mematikan furigana.
- Pada HP, panel pengaturan menyesuaikan layar dan ditempatkan di atas navigasi bawah.
- Dengarkan seluruh cerita atau satu paragraf melalui kontrol audio pada bacaan.

Audio memakai **Web Speech API** dan suara Jepang yang tersedia pada browser/perangkat. Pilihan laki-laki/perempuan hanya dapat digunakan sesuai ketersediaan suara; jika tidak ditemukan, pilih suara Jepang dari daftar perangkat. Pilihan gender bukan pengubahan nada suara untuk meniru gender. Kecepatan baca juga dapat disesuaikan.

Jika suara Jepang belum tersedia, aktifkan atau unduh suara Jepang di pengaturan perangkat, lalu tekan **Muat ulang suara**. Sebagian suara memerlukan internet. Cerita tetap dapat dibaca tanpa audio.

## Print dan simpan PDF

### Materi dan soal

Buka **Materi harian → Print / PDF**. Tersedia enam mode:

| Mode | Isi |
| --- | --- |
| Materi saja per Day | Materi satu hari yang dipilih. |
| Soal saja per Day | 40 soal beserta bacaan satu hari. |
| Materi dan soal per Day | Materi serta 40 soal satu hari. |
| Full materi 45 Day | Seluruh materi Day 1–45. |
| Full soal 45 Day | Seluruh 1.800 soal beserta bacaan. |
| Full materi dan soal 45 Day | Seluruh materi dan soal Day 1–45. |

Soal dicetak tanpa kunci dan tanpa jawaban pengguna. Setiap Day dimulai pada halaman baru; pada paket gabungan, bagian soal juga dimulai pada halaman baru.

### Kanji

Pada level kanji yang dipilih, klik **Print / PDF**, kemudian pilih:

- **Full level** — seluruh kartu dalam urutan nomor asli.
- **Full level — pisah per pengelompokan** — setiap kelompok dimulai pada halaman baru.

Tata letak kanji memakai **tiga kolom pada kertas A4**. Kartu N5/N4/N3 menyertakan contoh kalimat dan contoh kata. Kartu N2/N1 mengikuti data yang tersedia pada level tersebut. Filter dan pagination layar tidak membatasi isi cetakan.

### Kotoba N5–N1

Buka **Kotoba → pilih level → Print / PDF**. Tersedia **12 pilihan**: gabungan seluruh N5–N1, atau N5/N4/N3/N2/N1 saja; masing-masing tersedia dalam urutan penuh atau dipisah per kelompok. Kata berlabel beberapa level hanya dicetak sekali pada mode gabungan. N3–N1 mencetak seluruh kata pilihan yang tersedia saat ini, masing-masing 100 kata, bukan seluruh kosakata level JLPT. Cetakan berbentuk tabel nomor, level, kata, bacaan, dan arti. Pada mode kelompok, setiap kelompok dimulai pada halaman baru. Pilihan cetak mencakup seluruh data sesuai mode, bukan hanya halaman atau hasil filter yang sedang terlihat.

### Mencetak atau menyimpan sebagai PDF

1. Pilih isi, lalu klik **Buka pratinjau cetak**.
2. Tunggu dokumen siap dan klik **Cetak / Simpan PDF**.
3. Pilih printer atau **Save as PDF / Simpan sebagai PDF** pada dialog browser.
4. Gunakan **A4**, skala **100%**, dan matikan header/footer browser agar bingkai sesuai desain.
5. Periksa pratinjau dan jumlah halaman sebelum mencetak paket penuh.

Lembar memakai bingkai dark Tadicoba yang berulang pada tiap halaman. Tema gelap website tidak mengubah kertas menjadi berlatar gelap. Jika popup diblokir, pratinjau ditampilkan di dalam dashboard. Ketersediaan printer dan ekspor PDF mengikuti browser/perangkat.
>>>>>>> bcf7939f7405ad8857d8cbf214c126766e1529e9

## Penyimpanan dan cadangan

- Progres Jepang dan Inggris menggunakan penyimpanan yang terpisah.
- Data disimpan menggunakan `localStorage`; belum ada login, server aplikasi, atau database online.
- Browser, profil, perangkat, dan alamat situs yang berbeda mempunyai ruang penyimpanan berbeda.
- Menghapus data situs atau berpindah alamat dapat membuat progres lama tidak terbaca.
- Buat cadangan melalui fitur aplikasi sebelum mengganti perangkat, browser, atau alamat hosting. Impor cadangan pada bagian bahasa yang sesuai.
- Unduhan file HTML baru tidak memindahkan progres ke perangkat lain secara otomatis.

Kunci penyimpanan Inggris yang digunakan:

<<<<<<< HEAD
| Kunci | Kegunaan |
| --- | --- |
| `tadicoba-english-a1-v1` | Modul terpilih, draf jawaban, dan riwayat percobaan latihan Inggris. |
| `tadicoba-last-course-v1` | Pilihan bahasa terakhir. |
| `tadicoba-en-nao-guide-v1` | Penanda tutorial awal Nao sudah dilihat. |
=======
- Data laptop dan HP **belum tersinkron otomatis**.
- Menghapus data situs/browser dapat menghapus progres.
- File lokal, GitHub Pages, dan custom domain dapat memakai ruang penyimpanan berbeda.
- Memperbarui HTML pada alamat website yang sama umumnya mempertahankan data, selama penyimpanan situs dan kunci datanya tidak dihapus atau diganti.

### Cakupan cadangan JSON

| Fitur | Data yang dicadangkan | Lokasi |
| --- | --- | --- |
| Cadangkan hasil (JSON) | Hasil jawaban, riwayat percobaan, serta tanggal absensi; ekspor juga menyertakan draf. | Materi harian → Alat belajar & cadangan. |
| Cadangkan progres belajar | Penanda N5/N4, kotoba, dan progres flashcard. | Flashcard. |

Untuk memulihkan, pilih **Pulihkan hasil** atau **Pulihkan progres** pada fitur yang sesuai, lalu pilih JSON yang sebelumnya diekspor dari fitur tersebut.

Riwayat latihan digabung berdasarkan ID percobaan agar tidak berganda. Tanggal absensi asli dipertahankan; impor tidak membuat kehadiran baru pada hari impor. Draf yang ikut diekspor belum dimuat kembali oleh pemulihan riwayat saat ini.

**Cadangan progres belajar belum mencakup penanda kanji N3/N2/N1.** Penanda kotoba N5–N1 dan progres flashcard terkait sudah termasuk cadangan progres belajar. Kedua cadangan juga belum mencakup seluruh data seperti agenda, nama, tema, preferensi romaji, riwayat latihan kana, dan pengaturan Nao. Penanda kanji N3–N1 tetap tersimpan pada browser asal, tetapi belum dapat dipindahkan melalui dua fitur cadangan tersebut.
>>>>>>> bcf7939f7405ad8857d8cbf214c126766e1529e9

## Menjalankan secara lokal

Gunakan file HTML versi pilihan sebagai `index.html`. File inti menggabungkan antarmuka, logika, materi, serta aset yang disematkan; tidak memerlukan instalasi npm atau proses build.

Struktur minimal:

<<<<<<< HEAD
```text
Tadicoba/
├── index.html
└── README.md
```
=======
HTML memuat CSS, JavaScript, materi, font Jepang, logo, bingkai cetak, sprite Nao, serta gambar Torii dan Kumo. Gambar dan sprite tidak memerlukan berkas terpisah; rekaman pengisi suara khusus belum disertakan. Aset utama tidak perlu diunggah satu per satu. Beberapa utilitas/ikon lama memakai CDN, sehingga ketersediaan utilitas tersebut dapat memerlukan koneksi internet.
>>>>>>> bcf7939f7405ad8857d8cbf214c126766e1529e9

Membuka HTML langsung dapat dipakai untuk melihat materi, tetapi fitur tertentu berbeda dukungannya pada alamat `file://`. Untuk pengujian lokal yang lebih konsisten:

```bash
cd Tadicoba
python -m http.server 8000 --bind 127.0.0.1
```

Pada Windows, jika perintah `python` tidak tersedia, gunakan `py -m http.server 8000 --bind 127.0.0.1`. Kemudian buka `http://localhost:8000`.

## Hosting

Aplikasi dapat ditempatkan pada hosting statis yang menyajikan HTML melalui HTTPS. Untuk GitHub Pages, gunakan berkas `index.html` pada folder sumber publikasi repository dan aktifkan Pages sesuai pengaturan repository tersebut.

Jika yang tampil justru teks kode, pastikan yang dibuka adalah alamat website hasil publikasi, bukan halaman raw atau pratinjau kode di repository. Pastikan pula nama file benar-benar berakhiran `.html`, bukan `.html.txt`.

Simpan progres sebelum memindahkan situs ke domain/alamat lain. README ini tidak menyatakan bahwa file terbaru sudah dipublikasikan ke hosting.

## Mengubah isi aplikasi

1. Buat salinan HTML sebelum mengedit.
2. Cari bagian data atau fungsi yang ingin diubah; hindari mengganti semua teks dengan pola yang terlalu umum.
3. Materi Inggris disimpan dalam struktur `lessons`; kosakata verb, cerita, dan panduan tenses berada pada struktur terpisah.
4. Pertahankan kunci penyimpanan agar progres pengguna tetap terbaca. Perubahan struktur data memerlukan migrasi.
5. Periksa pemilihan bahasa, pergantian menu, Nao, cetak, serta ekspor/impor cadangan setelah perubahan.
6. Uji ulang fitur mikrofon melalui HTTPS/localhost dan browser target.

<<<<<<< HEAD
HTML juga memuat template cetak dalam JavaScript. Penggantian global `</html>` atau `</body>` bisa merusak template tersebut. Aset base64 membuat file cukup besar; jangan mengubah blok aset jika tidak diperlukan.
=======
## Memperbarui website

1. Cadangkan hasil dan progres yang didukung terlebih dahulu.
2. Unduh HTML Tadicoba terbaru, yaitu `Tadicoba-Kotoba-Menu.html`.
3. Ubah namanya menjadi **`index.html`**.
4. Ganti `index.html` lama di folder utama repository dan unggah README terbaru bila diperlukan.
5. Commit perubahan, lalu periksa deployment pada tab **Actions**.
6. Setelah selesai, muat ulang website. Gunakan hard refresh jika browser masih menampilkan versi lama.

Jika memakai Git lokal, ambil perubahan remote sebelum mengirim pembaruan. Jika terjadi konflik, selesaikan konflik terlebih dahulu; jangan memakai force push sebagai cara rutin mengatasi penolakan push.
>>>>>>> bcf7939f7405ad8857d8cbf214c126766e1529e9

## Pemecahan masalah

| Kendala | Pemeriksaan |
| --- | --- |
| Mikrofon tidak aktif | Periksa secure context, dukungan API, izin situs, perangkat input, dan koneksi layanan pengenalan suara. |
| Ucapan benar tetapi ditandai merah | Periksa transkrip yang dikenali, dengarkan contoh, dan coba kembali. Penilaian berbasis transkrip memiliki keterbatasan. |
| Audio tidak keluar | Periksa volume, dukungan `speechSynthesis`, ketersediaan suara bahasa target, dan interaksi tombol. |
| Progres hilang | Pastikan browser, profil, serta alamat situs sama. Gunakan cadangan yang sudah diekspor. |
| Nao tidak terlihat atau lapisan mata bergeser | Pastikan menggunakan satu file HTML lengkap dari versi yang dipilih; jangan mencampur CSS/rig dari revisi lain. |
| Tampilan terlalu besar | Periksa zoom browser dan ukuran viewport; tampilan pada HP berbeda dari laptop. |
| Unduhan gagal | Unduh ulang dari tautan berkas terbaru dan pastikan penyimpanan perangkat tersedia. |

## Teknologi dan atribusi

- HTML, CSS, JavaScript, SVG, dan Canvas untuk antarmuka serta animasi.
- `localStorage`, `speechSynthesis`, dan pengenalan suara browser untuk fitur lokal yang didukung.
- [Japan Foundation — Irodori](https://www.irodori.jpf.go.jp/) dan [TUFS — modul tata bahasa Jepang](https://www.coelang.tufs.ac.jp/mt/ja/gmod/) sebagai rujukan pendalaman pola. Susunan materi dan soal dashboard dibuat tersendiri.
- [KANJIDIC2 / EDRDG](https://www.edrdg.org/wiki/index.php?title=KANJIDIC_Project), melalui [kanji-data](https://github.com/sepTN/kanji-data), untuk referensi bacaan, arti dasar, goresan, dan level lanjutan. Pertahankan atribusi/lisensi sumber, termasuk [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/), sesuai data yang digunakan.
- [KanaMastery — N4 Kanji](https://kanamastery.com/jlpt/n4/kanji) sebagai rujukan daftar N4 yang digunakan sebelumnya.
- [KanjiVG](https://kanjivg.tagaini.net/), © Ulrich Apel dan kontributor, berlisensi [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/). Data diadaptasi untuk pemutaran SVG; atribusi dan salinan lisensi disertakan dalam HTML.
- [Marugoto — Hiragana](https://a1.marugotoweb.jp/en/hiragana.php) dan [Katakana](https://a1.marugotoweb.jp/en/katakana.php) sebagai rujukan aksara.
- Noto Sans JP untuk font Jepang yang disematkan; informasi lisensi tersedia dalam HTML.
- Pertahankan pemberitahuan hak cipta dan lisensi komponen/data yang disertakan. Lisensi data tertentu tidak otomatis menjadi lisensi seluruh proyek.

Logo Tadicoba dan maskot Nao merupakan identitas visual proyek. Materi dan cerita tidak mewakili soal resmi JLPT atau sertifikasi CEFR.

---

Dikelola oleh **Tata Dico Puji Handoko**.
