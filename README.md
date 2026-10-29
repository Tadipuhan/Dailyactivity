# Tadicoba

**Ruang untuk progresmu.** Dashboard aktivitas harian dan pendamping belajar bahasa Jepang dalam satu website statis, dengan materi N5–N4 selama 45 hari, dasar hiragana/katakana, referensi kanji N5–N1, flashcard, cerita, dan rekap absensi belajar.

[Buka website](https://tadipuhan.github.io/Dailyactivity/) · [Repository](https://github.com/Tadipuhan/Dailyactivity)

> Dokumentasi untuk versi **Dasar Jepang + Nao**, dengan tampilan Desain Terpadu, diperbarui **29 Oktober 2026**. Website dijalankan dari `index.html` tanpa instalasi atau proses build.

## Daftar isi

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
| Kotoba N5–N4 | **424 kosakata pilihan** beserta bacaan, arti, dan pilihan cetak. |
| Flashcard | **670 kartu unik N5–N4**, mencakup kanji dan kotoba dengan empat pilihan jawaban serta umpan balik langsung. |
| Cerita | Tiga cerita orisinal, pilihan versi N5/N4, furigana, terjemahan per paragraf, dan audio sesuai dukungan perangkat. |
| Maskot Nao | Pendamping chibi dengan reaksi kontekstual, bubble dialog, kedipan, gerak mulut, arah pandang pointer, serta pengaturan suara dan gerakan. |
| Latar Jepang | Sidebar S01 Torii dan background B05 Kumo, disematkan langsung dalam HTML. |
| Tema | **Terang, Gelap, atau Sistem**, dengan pilihan tema tersimpan di browser. |
| Personalisasi | Nama panggilan, sapaan sesuai waktu, jam berjalan, dan hitung mundur ke **5 Desember 2026 pukul 00.00** menurut waktu perangkat. |
| Print / PDF | Materi dan soal per Day atau seluruh 45 Day; kanji dan kotoba lengkap atau dipisah per kelompok. |

## Desain dan navigasi

| Bagian | Arah desain |
| --- | --- |
| Dashboard | Dashboard klasik dengan ringkasan progres dan tindakan belajar utama. |
| Materi harian | Studio Fokus: daftar Day 1–45, area materi, serta tombol latihan dan cetak. |
| Kanji | Kartu yang menonjolkan karakter, arti, bacaan, dan contoh jika tersedia. |
| Daftar cerita | Portal cerita berbentuk kartu; klik kartu untuk masuk ke bacaan. |
| HP dan tablet | Tata letak adaptif, menu navigasi buka-tutup, dan navigasi bawah pada layar lebih kecil. |
| Tema gelap | Warna latar, teks, tombol, formulir, dan kartu disesuaikan untuk tampilan gelap; motif Kumo diberi lapisan warna gelap. |
| Sidebar | S01 Torii: gerbang torii, cahaya bulan, kabut ungu, dan lampion, dengan lapisan gelap untuk keterbacaan menu. |
| Background | B05 Kumo: awan Jepang bernuansa lavender dengan skala motif yang tetap saat halaman memanjang. |
| Nao | Karakter transparan di sudut layar, dengan dialog ringkas dan ukuran lebih kecil pada HP. |

Logo T ungu, tipografi, tombol, dan bentuk kartu digunakan secara konsisten. Ilustrasi cerita menjadi pelengkap, sementara materi dan tombol belajar tetap menjadi fokus. Versi sebelum penambahan Nao dan latar Jepang telah diperiksa pada lebar **320–1920 piksel**. Perubahan terbaru masih memerlukan pemeriksaan visual di desktop dan HP.

## Mulai menggunakan

1. Buka website atau file `index.html`.
2. Isi nama panggilan saat pertama masuk. Nama dapat diubah melalui **Ubah nama**; di HP, buka **Menu** terlebih dahulu.
3. Sesuaikan agenda melalui **Aktivitas harian**.
4. Jika baru belajar, buka **Dasar Jepang** terlebih dahulu. Menu ini opsional; materi Day 1 tetap dapat langsung dibuka.
5. Buka **Materi harian**, pilih Day, dan baca materinya.
6. Tekan **Kerjakan 40 soal**, jawab semuanya, lalu kirim untuk melihat penilaian dan mencatat kehadiran.
7. Ulangi materi melalui **Kanji**, **Kotoba**, **Flashcard**, atau **Cerita**.
8. Lihat perkembangan pada **Dashboard** dan **Rekap bulanan**.
9. Cadangkan hasil belajar secara berkala melalui ekspor JSON.

Pilihan tema ada pada bagian atas website. Mode **Sistem** mengikuti preferensi terang/gelap perangkat.

## Dasar Jepang

Menu **Dasar Jepang** berada sebelum Materi harian pada sidebar. Di HP, buka menu navigasi untuk menemukannya. Tautan pengantar juga tersedia pada Day 1. Tidak ada syarat kelulusan kana untuk membuka materi harian.

### Hiragana dan katakana

- **46 huruf dasar per aksara**, disusun dalam tabel bunyi.
- **25 bentuk dakuten/handakuten per aksara** dan **33 gabungan yōon per aksara**.
- Pilihan untuk menampilkan atau menyembunyikan romaji pada tabel; preferensi disimpan di browser.
- Klik huruf untuk membuka bacaan, catatan, contoh kata jika tersedia, audio, dan urutan goresan.
- Pada gabungan seperti きゃ, animasi ditampilkan per komponen huruf, termasuk kana kecil.

Animasi memakai jalur goresan vektor yang disematkan dalam HTML. Gunakan kontrol langkah, putar/jeda, ulangi, kecepatan, dan nomor goresan untuk mengamati penulisannya. Animasi membantu mengenali urutan; tetap berlatih menulis sendiri.

### Aturan membaca

Materi ringkas mencakup penggunaan kedua aksara, bunyi dasar, shi/chi/tsu/fu, dakuten dan handakuten, kana kecil ゃ・ゅ・ょ, っ kecil, vokal panjang, bacaan partikel は・へ・を, serta huruf yang bentuknya mirip.

### Latihan kana

1. Pilih hiragana, katakana, atau keduanya.
2. Pilih jenis latihan: huruf ke bacaan, bacaan ke huruf, atau kata ke bacaan.
3. Pilih **10 atau 20 soal**, lalu mulai.
4. Jawab dari **empat pilihan** untuk mendapatkan umpan balik langsung.
5. Tinjau nilai dan huruf yang perlu diulang pada akhir sesi.

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
| N2 | 367 | Inggris | Belum dilengkapi contoh kalimat seperti N5–N3. |
| N1 | 1.232 | Inggris | Belum dilengkapi contoh kalimat seperti N5–N3. |

Kartu menampilkan karakter, arti, onyomi, kunyomi, romaji, jumlah goresan, dan penanda belajar. Tombol animasi pada **seluruh level N5–N1** membuka urutan goresan dengan kontrol langkah, putar/jeda, ulangi, kecepatan, dan nomor goresan. Data vektor disematkan dalam HTML sehingga animasi tidak memerlukan pengambilan data dari server. Pemutaran dimulai atas tindakan pengguna. Format arti N3 memakai pemisah **“·”**, mengikuti N4/N5. Beberapa bacaan kamus pada level lanjutan menggunakan tanda titik untuk memisahkan bagian kanji dan okurigana.

Gunakan submenu **Kanji** atau tab level untuk berpindah halaman. Pencarian, filter kelompok, status, dan pilihan jumlah kartu per halaman membantu meninjau daftar. N3–N1 dikelompokkan berdasarkan jumlah goresan.

Daftar ini merupakan **referensi belajar pilihan, bukan daftar resmi lengkap JLPT**. Penetapan level dapat berbeda dari sumber atau buku lain, dan sebagian karakter dapat muncul pada beberapa level. Makna kanji serta bacaannya dapat berubah sesuai kata dan konteks.

### Flashcard

Flashcard saat ini mencakup **N5–N4**, bukan N3–N1. Pilih level, jenis materi, kelompok kartu, arah latihan, dan jumlah kartu per sesi, lalu tekan **Mulai / acak sesi**.

Jawaban salah dijadwalkan ulang besok; jawaban benar empat hari kemudian. Penilaian langsung menunjukkan jawaban yang benar dan progres tersimpan pada browser.

## Maskot Nao dan pengaturan suara

Nao tampil sebagai pendamping di sudut layar. Klik karakter untuk mendapatkan petunjuk umum; klik **×** pada bubble untuk menutup dialog dan menghentikan ucapannya. Label nama di atas bubble dihilangkan.

### Reaksi dan animasi

Enam pose yang tersedia adalah **netral, menyapa, berpikir, senang, bingung, dan merayakan**. Pemakaiannya mengikuti tindakan yang sudah dihubungkan, bukan percakapan AI bebas.

| Pemicu | Respons |
| --- | --- |
| Memilih menu navigasi yang terhubung | Dialog singkat sesuai konteks halaman, misalnya materi, kanji, atau cerita. |
| Menjawab flashcard dengan benar | Ekspresi senang dan informasi kata, bacaan, serta artinya. |
| Menjawab flashcard dengan salah | Ekspresi bingung dan jawaban yang benar beserta bacaan serta artinya. |
| Menyelesaikan pengiriman latihan harian | Reaksi merayakan dan ajakan meninjau pembahasan. |
| Mengklik Nao | Pose berpikir dan petunjuk belajar umum. |

Integrasi ini belum mencakup respons khusus pada setiap tombol atau setiap soal kana. Jawaban Nao disiapkan dalam kode berdasarkan pemicu dan data latihan; tidak memerlukan API percakapan.

- Gambar karakter memiliki latar transparan.
- Posisi kedip dan mulut mengikuti koordinat serta kemiringan wajah tiap pose.
- Skala gambar dan titik acuan wajah dibuat tetap saat pergantian reaksi.
- Pupil mengikuti pointer pada area halaman, kemudian kembali ke posisi netral saat pointer keluar.
- Gerak mulut mengikuti waktu pemutaran suara, atau durasi teks saat suara dimatikan. Animasi ini belum merupakan sinkronisasi bibir per fonem.

### Pengaturan Nao

Buka **Pengaturan** di bawah karakter:

| Kontrol | Fungsi |
| --- | --- |
| Suara Nao · anak perempuan | Mengaktifkan ucapan bahasa Indonesia dengan gaya suara anak perempuan yang ekspresif. |
| Kurangi gerakan | Mengurangi animasi wajah dan arah pandang; juga mengikuti preferensi kurangi gerakan dari perangkat. |
| Sembunyikan Nao | Menyembunyikan karakter dan dialog serta menghentikan ucapannya. |
| Tampilkan Nao | Memunculkan kembali karakter setelah disembunyikan. |

Suara tidak otomatis aktif pada pemakaian pertama. Gaya anak perempuan menjadi setelan bawaan saat suara diaktifkan; pilihan aktif/nonaktif pengguna tetap disimpan.

### Cara kerja suara

**Bahasa ucapan Nao tetap Indonesia, sesuai isi bubble.** Nuansa anime/chibi diterapkan melalui prioritas pemilihan suara serta variasi nada, tempo, dan jeda: lebih ceria saat benar, lebih lembut saat salah, serta penasaran saat memberi petunjuk.

HTML mengutamakan suara anak perempuan Indonesia jika tersedia, kemudian suara perempuan Indonesia, dan memakai suara Indonesia lain sebagai pilihan terakhir. Pemilihan berdasarkan bahasa serta nama suara dari browser; informasi usia dan gender tidak selalu tersedia atau dapat dipastikan.

**Belum ada rekaman MP3/WAV atau pengisi suara khusus yang tertanam.** Suara masih menggunakan `speechSynthesis` / Web Speech API, sehingga hasil antarperangkat dapat berbeda dan tidak dijamin menyerupai pengisi suara anime. Jika suara Indonesia belum tersedia, aktifkan suara Indonesia di pengaturan perangkat. Beberapa mesin suara memerlukan internet.

Audio Nao terpisah dari audio Jepang pada kana dan cerita. Pengaturan gaya suara Nao tidak mengubah suara pembacaan cerita atau huruf Jepang.

Preferensi Nao disimpan pada kunci localStorage `tadicoba-nao-settings-v1`. Preferensi ini belum termasuk cadangan JSON utama. Nao disembunyikan saat mencetak.

## Cerita dan audio

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

### Kotoba N5–N4

Buka **Kotoba → Print / PDF**. Pilih seluruh N5–N4, N5 saja, atau N4 saja; masing-masing tersedia dalam urutan penuh atau dipisah per kelompok. Cetakan berbentuk tabel nomor, level, kata, bacaan, dan arti. Pada mode kelompok, setiap kelompok dimulai pada halaman baru. Pilihan cetak mencakup seluruh data sesuai mode, bukan hanya halaman atau hasil filter yang sedang terlihat.

### Mencetak atau menyimpan sebagai PDF

1. Pilih isi, lalu klik **Buka pratinjau cetak**.
2. Tunggu dokumen siap dan klik **Cetak / Simpan PDF**.
3. Pilih printer atau **Save as PDF / Simpan sebagai PDF** pada dialog browser.
4. Gunakan **A4**, skala **100%**, dan matikan header/footer browser agar bingkai sesuai desain.
5. Periksa pratinjau dan jumlah halaman sebelum mencetak paket penuh.

Lembar memakai bingkai dark Tadicoba yang berulang pada tiap halaman. Tema gelap website tidak mengubah kertas menjadi berlatar gelap. Jika popup diblokir, pratinjau ditampilkan di dalam dashboard. Ketersediaan printer dan ekspor PDF mengikuti browser/perangkat.

## Penyimpanan dan cadangan

Tadicoba memakai **localStorage browser**, tanpa database server. Nama panggilan, tema, agenda, draf, hasil latihan, absensi, penanda kanji/kotoba, dan progres flashcard, preferensi romaji, dan ringkasan latihan kana, serta preferensi Nao disimpan pada perangkat yang digunakan.

**Nama panggilan bukan akun login.** Mengganti nama tidak membuat profil data baru. Pada browser dan alamat website yang sama, penyimpanan tetap sama.

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

**Cadangan progres belajar belum mencakup penanda N3/N2/N1.** Kedua cadangan juga belum mencakup seluruh data seperti agenda, nama, tema, preferensi romaji, riwayat latihan kana, dan pengaturan Nao. Penanda N3–N1 tetap tersimpan pada browser asal, tetapi belum dapat dipindahkan melalui dua fitur cadangan tersebut.

## Menjalankan secara lokal

1. Unduh atau clone repository.
2. Pastikan file dashboard bernama **`index.html`**.
3. Buka file itu dengan browser modern.

Tidak diperlukan Python, Node.js, database, API key, atau proses build untuk menjalankan dashboard. Fitur inti tersedia di HTML; suara Jepang untuk materi dan suara Indonesia untuk Nao tetap bergantung pada perangkat.

HTML memuat CSS, JavaScript, materi, font Jepang, logo, bingkai cetak, sprite Nao, serta gambar Torii dan Kumo. Gambar dan sprite tidak memerlukan berkas terpisah; rekaman pengisi suara khusus belum disertakan. Aset utama tidak perlu diunggah satu per satu. Beberapa utilitas/ikon lama memakai CDN, tetapi pemeriksaan fitur inti dilakukan juga dengan permintaan eksternal diblokir.

### Struktur repository

| File | Keterangan |
| --- | --- |
| `index.html` | Dashboard, tampilan, logika, data belajar, dan aset utama. |
| `README.md` | Dokumentasi proyek. |

Banyak menu ditampilkan melalui perpindahan bagian dalam **satu HTML**; tidak diperlukan file HTML terpisah untuk setiap menu.

## Publikasi melalui GitHub Pages

Untuk repository `Tadipuhan/Dailyactivity`:

1. Unggah **`index.html`** dan **`README.md`** ke folder utama repository.
2. Buka **Settings → Pages**.
3. Pada bagian publikasi, pilih **Deploy from a branch**.
4. Pilih branch **main**, folder **/ (root)**, lalu simpan.
5. Tunggu deployment selesai, kemudian buka alamat GitHub Pages.

Alamat website: **https://tadipuhan.github.io/Dailyactivity/**

Nama tampilan **Tadicoba** tidak mengharuskan nama repository berubah. Pastikan nama file halaman utama tepat `index.html`, bukan `index.html.txt` atau nama HTML unduhan yang belum diganti.

Rujukan: [pengaturan sumber publikasi GitHub Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site) dan [file halaman awal GitHub Pages](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site).

## Memperbarui website

1. Cadangkan hasil dan progres yang didukung terlebih dahulu.
2. Unduh HTML Tadicoba terbaru, yaitu `Tadicoba-Dasar-Jepang-Nao.html`.
3. Ubah namanya menjadi **`index.html`**.
4. Ganti `index.html` lama di folder utama repository dan unggah README terbaru bila diperlukan.
5. Commit perubahan, lalu periksa deployment pada tab **Actions**.
6. Setelah selesai, muat ulang website. Gunakan hard refresh jika browser masih menampilkan versi lama.

Jika memakai Git lokal, ambil perubahan remote sebelum mengirim pembaruan. Jika terjadi konflik, selesaikan konflik terlebih dahulu; jangan memakai force push sebagai cara rutin mengatasi penolakan push.

## Pemecahan masalah

| Masalah | Yang diperiksa |
| --- | --- |
| Yang terbuka halaman repository, bukan dashboard | Buka alamat `github.io` pada bagian publikasi, bukan halaman daftar file GitHub. |
| Website menampilkan README atau tidak menemukan halaman | Periksa keberadaan `index.html` pada branch dan folder sumber Pages. |
| Update belum terlihat | Pastikan deployment berhasil dan muat ulang tanpa cache. |
| Progres hilang setelah pindah HP/browser/domain | Penyimpanan terpisah; pulihkan cadangan yang didukung pada perangkat tujuan. |
| Nama berubah tetapi hasil latihan tetap sama | Nama hanya personalisasi tampilan, bukan pemisahan akun. |
| N2/N1 masih berbahasa Inggris | Terjemahan Indonesia dan contoh lengkap baru tersedia untuk N5/N4/N3. |
| Audio tidak tersedia | Periksa dukungan browser, suara Jepang perangkat, dan daftar suara pada halaman cerita. |
| Nao tidak terlihat | Klik **Tampilkan Nao** jika sebelumnya disembunyikan; pastikan HTML terbaru sudah digunakan. |
| Nao tidak bersuara | Aktifkan **Pengaturan → Suara Nao · anak perempuan**, periksa volume, dan ketersediaan suara Indonesia perangkat. |
| Suara Nao berbeda di HP dan komputer | Versi ini memakai mesin suara perangkat, belum rekaman pengisi suara khusus yang seragam. |
| Sidebar atau background masih polos | Pastikan memakai HTML terbaru dengan gambar latar langsung, bukan versi lama yang menyimpan data gambar besar dalam variabel CSS. Jika sudah dipublikasikan, periksa deployment dan muat ulang tanpa cache. |
| Print tidak membuka popup | Gunakan pratinjau di dalam dashboard atau izinkan popup untuk situs ini. |

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

## Teknologi dan atribusi

- **HTML, CSS, dan JavaScript** untuk antarmuka serta logika; **SVG** untuk grafik dan ikon.
- **localStorage** untuk penyimpanan lokal; **Web Speech API** untuk audio kana, pembacaan cerita, dan suara Indonesia Nao; **Canvas 2D** untuk animasi sprite Nao; dialog cetak browser untuk printer/PDF.
- [Japan Foundation — Irodori](https://www.irodori.jpf.go.jp/) dan [TUFS — modul tata bahasa Jepang](https://www.coelang.tufs.ac.jp/mt/ja/gmod/) sebagai rujukan pendalaman pola. Susunan materi dan soal dashboard dibuat tersendiri.
- [KANJIDIC2 / EDRDG](https://www.edrdg.org/wiki/index.php/KANJIDIC_Project), melalui [kanji-data](https://github.com/sepTN/kanji-data), untuk referensi bacaan, arti dasar, jumlah goresan, dan pengelompokan level lanjutan. Data mengikuti atribusi/lisensi sumber, termasuk [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/).
- [KanaMastery — N4 Kanji](https://kanamastery.com/jlpt/n4/kanji) sebagai rujukan daftar N4 yang digunakan sebelumnya.
- [KanjiVG](https://kanjivg.tagaini.net/) — data jalur dan urutan goresan kana/kanji, © Ulrich Apel dan kontributor, berlisensi [CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/). Data diadaptasi untuk pemutaran SVG; atribusi dan salinan lisensi disertakan dalam HTML. Lisensi ini berlaku pada data terkait, bukan otomatis seluruh proyek.
- [Marugoto — Hiragana](https://a1.marugotoweb.jp/en/hiragana.php), [Katakana](https://a1.marugotoweb.jp/en/katakana.php), dan [Irodori — sumber belajar](https://www.irodori.jpf.go.jp/en/resources.html) untuk rujukan dasar aksara dan membaca.
- **Noto Sans JP** untuk font Jepang yang disematkan; informasi lisensi font tersedia di HTML.
- Logo dan bingkai cetak memakai identitas **Tadicoba**. Ilustrasi Nao, sidebar Torii, dan latar Kumo dibuat dengan bantuan generasi gambar untuk Tadicoba. Cerita, contoh latihan, serta padanan Indonesia disusun untuk pembelajaran Tadicoba.

Materi tertulis dan cerita bukan soal resmi JLPT. Paket 45 hari belum mencakup ujian listening; audio cerita merupakan bantuan membaca. Nilai dashboard bukan skor resmi atau jaminan kelulusan JLPT.

---

Dikelola oleh **Tata Dico Puji Handoko** · [Tadipuhan](https://github.com/Tadipuhan)
