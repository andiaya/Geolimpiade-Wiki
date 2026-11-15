---
title: Perpetaan dan Interpretasi Data Spasial
permalink: /docs/Peta1/
layout: single
toc: true
toc_sticky: true
sidebar:
  nav: "docs"
---

<!--
=====================================================================
CATATAN REVISI (hapus blok ini dan semua penanda sebelum publikasi)
Diperiksa: 14 Nov 2026, terhadap versi terbit
https://andiaya.github.io/Geolimpiade-Wiki/docs/Peta/

PENANDA (cari dengan Ctrl+F "[FLAG" / "[GAMBAR-BARU" / "[BAGIAN-BARU"):
  [FLAG-ISI]      kesalahan konsep/fakta, sudah dikoreksi di teks
  [FLAG-CEK]      perlu dicek ulang penulis
  [FLAG-GAMBAR]   masalah pada gambar yang sudah ada
  [GAMBAR-BARU]   gambar baru dari Wikimedia Commons (sudah dilihat langsung)
  [TAMBAH-GAMBAR] usulan gambar yang belum terisi
  [BAGIAN-BARU]   materi baru untuk melengkapi silabus OSN/IGeo
  [KAJIAN-KINI]   narasi baku OSN yang sudah dikritik/diperbarui kajian ilmiah
                  terkini; narasi lama tetap dijelaskan, lalu diberi konteks
  [GAMBAR-BUATAN] ilustrasi skematis buatan revisi ini (berkas SVG terlampir)

HASIL CEK GAMBAR LAMA:
  - 4 gambar, semuanya termuat normal dan tidak terdistorsi.
  - Gambar orientasi bidang proyeksi (4) memakai alt "image"; alt sudah
    diganti. Gambar unsur peta memakai alt "1209-441" (ukuran berkas, bukan
    deskripsi); alt sudah diganti.
  - Gambar unsur peta adalah lembar peta skala 1:25.000 bergaya RBI (BIG)
    yang diberi label; sumber lembar peta perlu dicantumkan.
  - Gambar proyeksi azimutal (3) dan orientasi bidang (4) belum mencantumkan
    sumber.
  - Halaman ini belum membahas penginderaan jauh dan SIG secara umum, padahal
    keduanya termasuk silabus IGeo/OSN; bab baru ditambahkan.
=====================================================================
-->
# 1. Peta
- Peta adalah gambaran permukaan Bumi menggunakan simbol pada bidang datar dan digambar berdasarkan skala.
  - Menggunakan simbol artinya menggunakan bentuk-bentuk geometris untuk mewakili kenampakan di Bumi sebenarnya.
  - Pada bidang datar maksudnya digambar pada media 2 dimensi. Perubahan geometris dari bidang 3 dimensi ke 2 dimensi memerlukan adanya proyeksi matematis.
  - Penggambaran berdasarkan skala artinya peta mempertahankan proporsi dunia nyata, hanya panjang dan luasnya dibuat sepersekian dari nilai sebenarnya.
- Jenis Peta:
  1. Peta Dasar: disebut juga peta topografi. Peta dasar di Indonesia meliputi Peta Rupabumi Indonesia (RBI), Peta Lingkungan Pantai Indonesia (LPI), dan Peta Lingkungan Laut Nasional (LLN). Peta dasar mencakup informasi umum bentukan alami dan buatan manusia di permukaan Bumi.
  2. Peta Tematik: berisi informasi bertema khusus, seperti di antaranya peta batas wilayah, peta negara dunia, peta geologi, peta kepadatan penduduk, peta kemiringan lereng, dan peta penggunaan lahan.
- Unsur Peta: peta mencakup informasi berupa
  - Muka Peta: informasi utama gambaran permukaan Bumi.
  - Informasi Tepi: informasi penyerta peta.
    1. _Title_ / Judul: menunjukkan informasi utama peta.
    2. _Author_ / Pembuat: mencakup nama dan lembaga pembuat serta sumber data.
    3. _Legend_ / Legenda: deskripsi simbol peta.
    4. _Date_ / Waktu Pembuatan: tahun pembuatan peta.
    5. _Orientation_ / Orientasi: simbol arah utara.
    6. _Grid_ / Sistem Koordinat: menunjukkan lokasi absolut objek yang digambarkan peta.
    7. _Scale_ / Skala: perbandingan jarak pada peta dengan jarak horizontal di dunia nyata. Skala dapat ditunjukkan secara numerik, grafis, dan verbal.
    8. _Inset_: muka peta kecil untuk menunjukkan informasi berupa konteks wilayah yang lebih luas atau detail wilayah lebih sempit.
  ![Unsur-unsur peta](https://github.com/user-attachments/assets/f87ab37b-94a5-48d7-95b5-b59b34bfaf62)\
  Ilustrasi unsur peta pada lembar peta skala 1:25.000: muka peta di kiri atas, judul, inset, pembuat, dan legenda di kolom kanan, serta skala numerik dan grafis, orientasi (diagram arah utara sejati, utara grid, dan utara magnetik), dan grid di bagian bawah. **Logikanya:** informasi tepi diletakkan di luar muka peta agar tidak menutupi kenampakan, tetapi tetap dalam satu lembar sehingga peta dapat dibaca tanpa sumber lain.

  > ⚠️ **[FLAG-GAMBAR]** Sumber lembar peta (tampaknya Peta RBI Badan Informasi Geospasial) belum dicantumkan.

- **Perhitungan skala**:
  - Jarak sebenarnya = jarak di peta × penyebut skala. Contoh: 4 cm pada peta 1:25.000 = 100.000 cm = 1 km.
  - Skala peta yang belum diketahui dapat dicari dengan membandingkan jarak dua titik di peta dengan jarak sebenarnya, atau dengan peta lain yang skalanya diketahui: S₁/S₂ = d₂/d₁.
  - Pembesaran atau pengecilan peta mengubah skala numerik (1:25.000 diperbesar 2× menjadi 1:12.500), tetapi **skala grafis tetap benar** karena ikut membesar. Inilah alasan skala grafis lebih disarankan pada peta yang akan difotokopi atau ditampilkan di layar.
  - **Skala besar** (misalnya 1:5.000) menggambarkan wilayah sempit secara detail, sedangkan **skala kecil** (misalnya 1:1.000.000) menggambarkan wilayah luas secara umum. **Logikanya:** pecahan 1/5.000 lebih besar daripada 1/1.000.000.
  - **Interval kontur** (CI) pada peta topografi umumnya = 1/2.000 × penyebut skala. Contoh: peta 1:25.000 memiliki CI 12,5 m.

> 🆕 **[BAGIAN-BARU]** Perhitungan skala dan interval kontur adalah soal hitungan yang hampir selalu muncul di OSN, tetapi belum dijelaskan.


> 🔬 **[KAJIAN-KINI] Peta tidak pernah netral**
>
> **Narasi umum:** Peta adalah gambaran objektif permukaan Bumi.
>
> **Kajian terkini:** Kartografi kritis (Harley, 1989; Monmonier, _How to Lie with Maps_, 1991) menunjukkan bahwa setiap peta adalah hasil **pilihan**: wilayah mana yang ditampilkan di tengah, proyeksi apa yang dipakai, objek apa yang dihilangkan, bagaimana kelas data dibagi, dan nama apa yang dipakai. Pilihan-pilihan ini dapat menyampaikan kepentingan tertentu. Contohnya, Indonesia menamai perairan di utara Kepulauan Natuna sebagai **Laut Natuna Utara** (2017) untuk menegaskan klaim zona ekonomi eksklusifnya, dan peta koroplet yang sama dapat memberi kesan sangat berbeda jika pembagian kelasnya diubah.
>
> **Untuk soal:** Saat menginterpretasikan peta tematik, periksa sumber data, tahun, pembagian kelas, dan proyeksinya sebelum menarik kesimpulan.

# 2. Proyeksi Peta
- Proyeksi adalah proses perubahan yang harus dilakukan saat mengubah geometri benda dari bidang 3 dimensi ke bidang 2 dimensi.
- Bola Bumi memiliki permukaan yang tidak rata. Bentuk Bumi dapat dimodelkan sebagai:
  - **Permukaan topografi**: permukaan fisik Bumi yang sebenarnya, dengan gunung dan lembah.
  - **Geoid**: bidang ekuipotensial gravitasi yang paling mendekati muka laut rata-rata, dan diperpanjang di bawah daratan. Geoid tidak beraturan karena sebaran massa di dalam Bumi tidak merata, dan menjadi acuan **tinggi** (ketinggian di atas permukaan laut).
  - **Elipsoid**: bentuk matematis halus berupa bola yang sedikit pepat di kutub (jari-jari ekuator ±6.378 km, jari-jari kutub ±6.357 km). Elipsoid menjadi acuan **koordinat** (lintang, bujur). Elipsoid yang dipakai beserta posisinya disebut **datum**, misalnya WGS 84 untuk GPS. Indonesia memakai Sistem Referensi Geospasial Indonesia 2013 (SRGI 2013).

  > ✏️ **[FLAG-ISI]** Versi lama mendefinisikan geoid sebagai "kekuatan gravitasi di permukaan" dan elipsoid sebagai "bola dengan permukaan rata". Geoid adalah **bidang ekuipotensial** yang mendekati muka laut rata-rata, sedangkan elipsoid adalah bola **pepat** dengan permukaan halus. Konsep datum ditambahkan.

- Proyeksi peta diawali dengan membuat model elipsoid Bumi, lalu dilakukan proyeksi matematis ke bidang datar.
- Perubahan dari bentuk 3 dimensi ke 2 dimensi pasti menghasilkan distorsi, biasanya nampak dalam bentuk kenampakan objek yang terlihat seperti tertarik dari sisinya.

  ## 2.1. Bidang Proyeksi
  - Tipe bidang proyeksi menentukan lokasi di bola Bumi yang bertampalan dengan bidang proyeksi.
  - Lokasi yang bertampalan dengan bidang proyeksi memiliki distorsi paling rendah.
  - Tipe bidang proyeksi yaitu:
    1. Silinder (_Cylindrical_): bertampalan dengan bola Bumi pada keliling terpanjang Bumi.
    2. Kerucut (_Conical_): bertampalan dengan bola Bumi pada keliling Bumi yang bukan merupakan keliling terpanjang.
    3. Planar (_Azimuthal_): bertampalan dengan bola Bumi pada 1 titik. Sebagian besar proyeksi azimutal hanya dapat menggambarkan satu belahan Bumi atau kurang (gnomonik bahkan kurang dari satu belahan), kecuali azimutal ekuidistan yang dapat menggambarkan seluruh dunia.
       - Tipe proyeksi azimuthal dapat diklasifikasikan menjadi 3 jenis berdasarkan penempatan titik hilang perspektifnya (_vanishing point_). Klasifikasi tersebut yaitu:
         1. Gnomonik: memiliki titik hilang di pusat Bumi. Seluruh garis lurus jika digambarkan pada globe juga terlihat lurus pada peta gnomonik.
         2. Stereografik: memiliki titik hilang di sisi Bumi berlawanan. Proyeksi Stereografik mempertahankan bentuk kenampakan di permukaan Bumi dengan mempertahankan sudut.
         3. Orthografik: memiliki titik hilang di jarak tak hingga. Peta nampak seperti kenampakan globe dari sisi samping.

    - Bidang proyeksi juga dapat **menyinggung** (_tangent_, satu garis atau titik singgung) atau **memotong** (_secant_, dua garis potong) bola Bumi. Proyeksi secant memiliki dua garis tanpa distorsi, sehingga distorsi tersebar lebih merata di seluruh peta. Contohnya UTM, yang memakai silinder secant dengan faktor skala 0,9996 di meridian tengah.

    
    <img width="316" height="159" alt="tipe bidang proyeksi" src="https://github.com/user-attachments/assets/38a4640b-b15f-400a-8ae2-f2188c3341e9" />\
    Urut dari kiri ke kanan bidang proyeksi silinder, kerucut, dan planar. **Logikanya:** perhatikan jarak grid bidang proyeksi terhadap globe. Silinder paling dekat di ekuator, sehingga cocok untuk wilayah tropis seperti Indonesia; kerucut paling dekat di lintang tengah, sehingga cocok untuk negara lintang tengah yang membentang timur-barat; dan planar paling dekat di kutub.
    
    <img width="286" height="176" alt="tipe proyeksi azimuthal" src="https://github.com/user-attachments/assets/99739b72-165c-45c1-a394-9ebd28b54ea6" />\
    Urut dari kiri ke kanan tipe proyeksi azimuthal gnomonik, stereografik, dan orthografik. **Cara membaca:** garis putus-putus adalah "sinar" dari titik proyeksi melalui globe ke bidang datar. Pada gnomonik, sinar berasal dari pusat globe, sehingga lingkaran lintang di tepi makin berjauhan; pada stereografik dari kutub seberang, sehingga jarak lintang membesar perlahan; dan pada orthografik sinarnya sejajar, sehingga lingkaran lintang di tepi makin rapat.

  - Orientasi bidang proyeksi terhadap bola Bumi juga mempengaruhi area Bumi yang bertampalan. Orientasi bidang proyeksi tersebut yaitu:
    1. Normal: bidang proyeksi memiliki orientasi tegak terhadap bola Bumi. Bidang silinder akan bertampalan di ekuator, bidang kerucut bertampalan di lintang sedang, dan bidang planar bertampalan di **kutub** (aspek polar).
    2. Transverse: bidang proyeksi berorientasi rebah terhadap bola Bumi. Bidang silinder bertampalan di garis meridian dan antimeridian, dan bidang planar bertampalan di satu titik di ekuator (aspek ekuatorial).
    3. Oblique: bidang proyeksi berorientasi miring terhadap bola Bumi. Bidang silinder bertampalan memotong 2 garis lintang sedang dan seterusnya.\
    <img width="384" height="131" alt="Orientasi bidang proyeksi" src="https://github.com/user-attachments/assets/247d3f42-bcac-4dc1-ae7f-fbdc172a38a3" />\
    Urut dari kiri ke kanan bidang proyeksi normal, transverse, dan oblique. Garis tebal pada globe menunjukkan garis singgung silinder: ekuator (normal), sebuah meridian (transverse), dan lingkaran besar yang miring (oblique). **Logikanya:** distorsi paling kecil di sekitar garis singgung, sehingga orientasi dipilih agar garis singgung melewati wilayah yang dipetakan. Wilayah yang memanjang utara-selatan (misalnya Chili) paling cocok dengan aspek transverse.

    > ✏️ **[FLAG-ISI]** Pada aspek normal, bidang planar menyinggung bola Bumi di **kutub**, bukan di ekuator; titik singgung di ekuator adalah aspek transverse (ekuatorial).
  
  ## 2.2. Karakteristik Proyeksi Peta
  - Proyeksi menyebabkan distorsi atau perubahan dari bentuk asli permukaan Bumi dengan yang ditunjukkan pada peta.
  - Proyeksi dipilih berdasarkan karakteristik yang akan dipertahankan, yaitu:
    1. Konform: mempertahankan **sudut** di setiap titik, sehingga bentuk wilayah kecil tetap benar (bentuk wilayah luas tetap berubah). Pada proyeksi Mercator, garis arah kompas tetap (loksodrom/_rhumb line_) tampak sebagai garis lurus, sehingga proyeksi ini dipakai untuk navigasi laut. Contoh proyeksi: Mercator, Lambert kerucut konform, stereografis.
    2. Ekuidistan: mempertahankan jarak pada satu garis tertentu pada peta, misalnya jarak tiap titik pada peta terhadap titik tengahnya. Contoh proyeksi: azimuthal ekuidistan (akurat antara titik tengah peta dengan titik manapun), kerucut ekuidistan (akurat antara 2 garis lintang tertentu), silinder ekuidistan (jarak akurat di sepanjang ekuator).
    3. Ekuivalen: menunjukkan luas area yang proporsional satu sama lain. Contoh proyeksi: Mollweide, Albers, Gall-Peters.
    4. Kompromi: tidak mempertahankan satu sifat pun secara sempurna, tetapi menyeimbangkan distorsi bentuk dan luas sehingga tampilan dunia terlihat "wajar". Contoh proyeksi: Robinson dan Winkel Tripel (dipakai National Geographic sejak 1998).
  - Tidak ada proyeksi yang sekaligus konform dan ekuivalen. Garis lurus pada proyeksi gnomonik adalah **lingkaran besar** (rute terpendek), sehingga gnomonik dipakai untuk merencanakan rute penerbangan dan pelayaran jarak jauh.

  <img width="260" alt="Indikatriks Tissot pada proyeksi Mercator" src="https://commons.wikimedia.org/wiki/Special:FilePath/Tissot_indicatrix_world_map_Mercator_proj.svg?width=600" /> <img width="340" alt="Indikatriks Tissot pada proyeksi Mollweide" src="https://commons.wikimedia.org/wiki/Special:FilePath/Tissot_indicatrix_world_map_Mollweide_proj.svg?width=680" />\
  Indikatriks Tissot pada proyeksi Mercator (kiri) dan Mollweide (kanan). Setiap lingkaran merah mewakili lingkaran berukuran sama di permukaan Bumi. **Cara membandingkan:** pada Mercator, semua indikatriks tetap berupa **lingkaran** (bentuk terjaga, konform), tetapi makin besar ke arah kutub (luas sangat terdistorsi; Greenland tampak sebesar Afrika padahal luasnya hanya ±1/14 luas Afrika). Pada Mollweide, semua indikatriks memiliki **luas yang sama** (ekuivalen), tetapi makin pipih dan miring ke arah tepi peta (bentuk terdistorsi). **Logikanya:** indikatriks menunjukkan bahwa setiap proyeksi harus mengorbankan salah satu sifat. _Sumber: [Eric Gaba](https://commons.wikimedia.org/wiki/File:Tissot_indicatrix_world_map_Mercator_proj.svg), CC BY-SA 4.0; [Eric Gaba](https://commons.wikimedia.org/wiki/File:Tissot_indicatrix_world_map_Mollweide_proj.svg), CC BY-SA 4.0 (Wikimedia Commons)._

  > 🖼️ **[GAMBAR-BARU]** Ditautkan dari Wikimedia Commons. Isi gambar sudah dicek langsung dan lisensinya diambil dari metadata berkas.

  > ✏️ **[FLAG-ISI]** Definisi konform diperjelas (mempertahankan **sudut**, bukan bentuk secara keseluruhan), dan kategori proyeksi kompromi ditambahkan.


> 🔬 **[KAJIAN-KINI] Mercator, Gall-Peters, dan peta dunia yang "benar"**
>
> **Narasi umum:** Proyeksi Mercator salah karena memperbesar negara-negara Eropa, dan proyeksi Gall-Peters adalah peta dunia yang benar dan adil.
>
> **Kajian terkini:** Mercator (1569) dirancang untuk **navigasi**: garis arah kompas tetap tampak lurus, dan sifat itu memang tidak dapat dicapai tanpa memperbesar wilayah lintang tinggi. Masalahnya terletak pada penggunaan Mercator untuk peta dunia umum atau peta tematik. Arno Peters (1973) mempromosikan proyeksi "baru" yang ternyata sama dengan proyeksi James Gall (1855). Proyeksi ini memang ekuivalen (luasnya benar), tetapi bentuk benua sangat terdistorsi: Afrika dan Amerika Selatan tampak memanjang ke bawah. Pada 1989, tujuh organisasi geografi dan kartografi Amerika Utara mengeluarkan resolusi agar **semua** peta dunia berbentuk persegi panjang, termasuk Mercator dan Gall-Peters, tidak dipakai untuk peta dunia umum. Kartografer kini menganjurkan proyeksi ekuivalen dengan distorsi bentuk lebih kecil, seperti Equal Earth (2018), atau proyeksi kompromi seperti Winkel Tripel. Web Mercator tetap dipakai Google Maps karena bersifat konform, sehingga bentuk jalan dan bangunan pada skala besar tidak terdistorsi.
>
> **Untuk soal:** Pilih proyeksi sesuai tujuan: konform untuk navigasi dan peta skala besar, ekuivalen untuk peta tematik sebaran (misalnya kepadatan penduduk), dan kompromi untuk peta dunia umum.

<img width="200" alt="Peta dunia proyeksi Mercator" src="https://commons.wikimedia.org/wiki/Special:FilePath/Mercator_projection_SW.jpg?width=600" /> <img width="230" alt="Peta dunia proyeksi Gall-Peters" src="https://commons.wikimedia.org/wiki/Special:FilePath/Gall%E2%80%93Peters_projection_SW.jpg?width=600" /> <img width="250" alt="Peta dunia proyeksi Equal Earth" src="https://commons.wikimedia.org/wiki/Special:FilePath/Equal_Earth_projection_SW.jpg?width=600" />\
Dunia dalam proyeksi Mercator (kiri), Gall-Peters (tengah), dan Equal Earth (kanan). **Cara membandingkan:** pada Mercator, Greenland tampak hampir sebesar Afrika dan Antarktika membentang sangat lebar; pada Gall-Peters, luasnya benar tetapi Afrika dan Amerika Selatan tampak memanjang dan Eropa memipih; pada Equal Earth, luasnya juga benar tetapi bentuk benua lebih mendekati globe karena meridiannya melengkung. **Logikanya:** tidak ada proyeksi yang sempurna; yang ada hanya proyeksi yang cocok atau tidak cocok untuk tujuan tertentu. _Sumber: [Strebe](https://commons.wikimedia.org/wiki/File:Mercator_projection_SW.jpg), CC BY-SA 3.0; [Strebe](https://commons.wikimedia.org/wiki/File:Gall%E2%80%93Peters_projection_SW.jpg), CC BY-SA 3.0; [Strebe](https://commons.wikimedia.org/wiki/File:Equal_Earth_projection_SW.jpg), CC BY-SA 4.0 (Wikimedia Commons)._

> 🖼️ **[GAMBAR-BARU]** Ditautkan dari Wikimedia Commons. Isi gambar sudah dicek langsung dan lisensinya diambil dari metadata berkas.

# 3. Sistem Koordinat

## 3.1. Sistem Koordinat Geografis
Sistem ini menggunakan garis lintang dan bujur untuk menentukan lokasi absolut di permukaan bumi yang berbentuk bola (spheroid).

- Lintang (Latitude): Garis horizontal yang sejajar dengan ekuator. Nilainya 0° di Ekuator hingga 90° di Kutub Utara (LU) atau 90° di Kutub Selatan (LS).
- Bujur (Longitude): Garis vertikal yang menghubungkan Kutub Utara dan Selatan. Nilainya 0° di Prime Meridian (Greenwich) hingga 180° ke arah Timur (BT) atau Barat (BB).
- Satuan: Derajat (°), Menit ('), Detik (") atau Derajat Desimal (Decimal Degrees).
- Contoh: Monumen Nasional (Monas) terletak di 6°10'30" LS, 106°49'40" BT.

## 3.2. Sistem Koordinat UTM (Universal Transverse Mercator)
Sistem proyeksi peta yang membagi bumi menjadi 60 zona (masing-masing selebar 6° bujur), dari 80° LS hingga 84° LU. Sistem ini menggunakan proyeksi Mercator **transverse** (silinder rebah, secant) untuk setiap zona, sehingga menghasilkan satuan meter, bukan derajat.

- Nomor zona = ⌊(bujur + 180°) / 6°⌋ + 1. Contoh: Jakarta (106,8° BT) berada di zona ⌊286,8/6⌋ + 1 = 48.

- Zona: Indonesia terletak di Zona 46, 47, 48, 49, 50, 51, 52, 53, 54.
- Koordinat:
    - Eastings (Timur): Jarak ke timur dari meridian sentral zona (dalam meter), ditambah **easting semu** 500.000 m agar tidak ada nilai negatif. Titik di barat meridian sentral memiliki easting <500.000 m.
    - Northings (Utara): Jarak dari ekuator (untuk belahan utara). Untuk belahan selatan, nilainya adalah 10.000.000 m dikurangi jarak dari ekuator (**northing semu**), sehingga makin ke selatan nilainya makin kecil. Karena wilayah Indonesia melintasi ekuator, setiap zona dibagi menjadi zona utara (N) dan selatan (S), misalnya 48S untuk Jakarta.
- Kelebihan: Lebih mudah untuk mengukur jarak, luas, dan volume secara langsung di peta karena satuannya linier (meter).

- Kekurangan: Koordinat UTM hanya berlaku di dalam satu zona; wilayah yang melintasi batas zona harus diolah dengan hati-hati.

> ✏️ **[FLAG-ISI]** Sistem UTM memakai proyeksi silinder **transverse** dan secant, bukan sekadar "bidang datar". Nilai easting semu 500.000 m dan northing semu 10.000.000 m serta rumus nomor zona ditambahkan.


# 4. Membaca dan Menginterpretasi Peta

## 4.1. Arah
- Azimuth: Sudut horizontal yang diukur searah jarum jam dari titik Utara Sejati (True North) atau Utara Magnetik. Nilainya 0° hingga 360°.
    - Contoh: Arah Timur = Azimuth 90°.
- Bearing: Sudut horizontal yang diukur dari acuan Utara atau Selatan menuju Barat atau Timur. Nilainya 0° hingga 90° dan selalu disertai huruf arah.
    - Format: [U/S] [Nilai Sudut] [B/T].
    - Contoh: Azimuth 135° = Bearing S 45° T (Dibaca: Selatan 45 derajat ke Timur).

- **Azimut balik** (_back azimuth_): azimut dari titik tujuan kembali ke titik awal = azimut ± 180°. Contoh: azimut 60° memiliki azimut balik 240°.
- Ada tiga arah utara: **utara sejati** (ke kutub geografis), **utara grid** (arah garis grid peta), dan **utara magnetik** (arah jarum kompas). Selisih utara sejati dan utara magnetik disebut **deklinasi magnetik**, yang berubah menurut tempat dan waktu sehingga harus dikoreksi saat memakai kompas di lapangan.


## 4.2. Jarak dan Kemiringan
- Jarak Datar (Horizontal Distance - HD): Panjang garis lurus antara dua titik yang diproyeksikan pada bidang datar (peta). Diukur menggunakan skala peta atau rumus Pythagoras dari koordinat (X,Y).
- Kemiringan (Slope/Gradient): Perbandingan antara beda tinggi vertikal dengan jarak datar. Bisa dinyatakan dalam pecahan desimal, persen (%), atau derajat (°). Untuk mengubah desimal ke persen maka nilai desimal dikali 100%, sedangkan untuk mengubah desimal ke derajat maka dicari arctan dari nilai desimal tersebut (tan^(-1) (Nilai Desimal)).
    - Rumus:
      
      $Kemiringan = \frac{Beda Tinggi}{Jarak Datar}$
      
- Jarak Miring (Slope Distance - SD): Jarak sebenarnya yang harus ditempuh di permukaan tanah yang tidak rata.
    - Rumus Pythagoras:
      
      $SD = \sqrt{(Jarak Datar)^2 + (Beda Tinggi)^2}$

- Membaca garis kontur:
  - Garis kontur menghubungkan titik-titik dengan ketinggian yang sama dan tidak pernah berpotongan (kecuali pada tebing menggantung).
  - Kontur rapat berarti lereng curam; kontur renggang berarti lereng landai.
  - Kontur berbentuk huruf V yang **ujungnya menunjuk ke arah hulu** (ke tempat lebih tinggi) menunjukkan lembah atau alur sungai; kontur berbentuk V atau U yang ujungnya menunjuk ke arah tempat lebih rendah menunjukkan punggungan.
  - Lingkaran kontur tertutup menunjukkan puncak bukit; jika diberi garis-garis kecil ke arah dalam (_hachure_), menunjukkan cekungan.
  - Contoh hitungan: dua titik pada ketinggian 250 m dan 300 m terpisah 2 cm pada peta 1:25.000. Jarak datar = 500 m, sehingga kemiringan = 50/500 = 0,1 = 10% ≈ 5,7°.

> 🆕 **[BAGIAN-BARU]** Aturan membaca garis kontur ditambahkan karena menjadi dasar soal kemiringan lereng dan profil topografi.


## 4.3. Volume
Perhitungan volume biasanya digunakan dalam pekerjaan Cut and Fill (Galian dan Timbunan) atau perhitungan cadangan tambang.
- Metode Penampang Rata-Rata (Average End Area):
  
  $Volume = \frac{(Luas_1 + Luas_2)}{2} \times JarakAntarPenampang$
  
- Metode Grid/Prismoidal: Menghitung volume berdasarkan grid ketinggian digital (DEM/Digital Elevation Model) menggunakan rumus prisma terpancung.

# 5. Menginterpretasi Citra

## 5.1. Dasar Penginderaan Jauh
> 🆕 **[BAGIAN-BARU]** Dasar-dasar penginderaan jauh belum ada di wiki, padahal kunci interpretasi di bawah memerlukan pemahaman tentang cara citra direkam.

- **Penginderaan jauh** adalah perolehan informasi tentang objek tanpa kontak langsung, dengan merekam gelombang elektromagnetik yang dipantulkan atau dipancarkan objek.
- Sistem **pasif** merekam pantulan sinar Matahari atau pancaran panas objek (misalnya Landsat, Sentinel-2), sedangkan sistem **aktif** memancarkan gelombangnya sendiri lalu merekam pantulannya (radar/SAR seperti Sentinel-1, dan LiDAR), sehingga dapat bekerja pada malam hari dan menembus awan.
- **Resolusi citra**:
  - Spasial: ukuran objek terkecil yang dapat dibedakan (ukuran piksel), misalnya 30 m (Landsat) atau 10 m (Sentinel-2).
  - Spektral: jumlah dan lebar kanal (_band_) gelombang yang direkam.
  - Temporal: selang waktu perekaman ulang di tempat yang sama, misalnya 16 hari (satu satelit Landsat) atau 5 hari (dua satelit Sentinel-2).
  - Radiometrik: jumlah tingkat kecerahan yang dapat dibedakan (misalnya 8 bit = 256 tingkat).
- **Pantulan spektral**: setiap objek memantulkan gelombang secara berbeda. Vegetasi sehat memantulkan sedikit cahaya merah (diserap klorofil) tetapi sangat banyak inframerah dekat (dipantulkan struktur daun); air menyerap hampir seluruh inframerah dekat sehingga tampak gelap; tanah kering memantulkan cukup tinggi dan merata. Perbedaan inilah yang dimanfaatkan **NDVI** = (NIR − Merah) / (NIR + Merah), dengan nilai −1 sampai +1. Nilai tinggi (>0,5) menunjukkan vegetasi rapat, nilai sekitar 0 menunjukkan tanah atau lahan terbangun, dan nilai negatif menunjukkan air.

## 5.2. Kunci Interpretasi Citra
Interpretasi citra (Foto Udara atau Satelit) memerlukan pengenalan objek berdasarkan 9 Kunci Interpretasi Citra:
1.  Rona/Warna (Tone/Color): Tingkat kegelapan atau kecerahan. Contoh: Air jernih berona gelap/hitam, pasir berona putih.
2.  Bentuk (Shape): Konfigurasi umum objek. Contoh: Gedung sekolah biasanya berbentuk L, I, atau U; Gunung api berbentuk kerucut.
3.  Ukuran (Size): Panjang, lebar, tinggi, atau luas relatif. Contoh: Ukuran lapangan sepak bola vs. lapangan voli.
4.  Tekstur (Texture): Frekuensi perubahan rona (halus atau kasar). Contoh: Hutan alami bertekstur kasar, sawah bertekstur halus.
5.  Pola (Pattern): Susunan spasial objek. Contoh: Pola permukiman transmigrasi berpola grid (kotak-kotak) teratur.
6.  Bayangan (Shadow): Membantu mengenali ketinggian dan bentuk samping. Contoh: Bayangan cerobong asap atau menara.
7.  Situs (Site): Letak objek terhadap lingkungan sekitarnya. Contoh: Stasiun kereta api selalu terletak di sepanjang jalur rel.
8.  Asosiasi (Association): Hubungan/keterkaitan dengan objek lain. Contoh: Lapangan parkir luas yang penuh mobil berasosiasi dengan pusat perbelanjaan (mal).
9.  Konvergensi Bukti: Penggunaan kombinasi beberapa kunci di atas untuk menghasilkan kesimpulan yang akurat.

# 6. Grafik Spasial (Kartografi Tematik)

- Choropleth
    - Peta yang menunjukkan nilai statistik diskontinu menggunakan gradasi warna atau arsiran pada unit administratif (batas administrasi).
    - Fungsi: Menunjukkan kepadatan penduduk per Kecamatan, tingkat kemiskinan per Kabupaten, atau hasil pemilu per Provinsi.
    - Karakteristik: Warna lebih gelap = Nilai lebih tinggi.
    - Data yang dipetakan harus berupa **nilai relatif** (kepadatan, persentase, nilai per kapita), bukan jumlah mutlak. **Logikanya:** wilayah yang luas akan tampak "penting" hanya karena luasnya; jumlah penduduk total lebih tepat ditampilkan dengan simbol proporsional atau titik.
    - Pembagian kelas (interval sama, kuantil, _natural breaks_, atau logaritmik) sangat memengaruhi kesan yang ditampilkan peta.

    <img width="480" alt="Peta koroplet kepadatan penduduk provinsi di Indonesia 2020" src="https://commons.wikimedia.org/wiki/Special:FilePath/Indonesia_provinces_population_density_2020.svg?width=960" />\
    Peta koroplet kepadatan penduduk provinsi di Indonesia tahun 2020 (jiwa/km²). **Cara membaca:** DKI Jakarta berwarna paling gelap (≥10.001), provinsi-provinsi di Jawa berwarna hijau zaitun (1.001–10.000), sebagian besar Sumatra, Sulawesi, Bali, dan Nusa Tenggara berwarna kuning (101–1.000), sedangkan Kalimantan, Maluku, dan Papua berwarna paling pucat. **Logikanya:** kelasnya disusun secara **logaritmik** (setiap kelas 10× kelas sebelumnya), karena kepadatan Jakarta lebih dari 1.000 kali kepadatan Papua; dengan interval sama, hampir semua provinsi akan jatuh di kelas yang sama. Kelemahan koroplet juga terlihat: seluruh Provinsi Papua diberi satu warna, padahal kepadatan di Jayapura jauh lebih tinggi daripada di pedalaman. _Sumber: [Afrogindahood](https://commons.wikimedia.org/wiki/File:Indonesia_provinces_population_density_2020.svg), CC BY-SA 4.0 (Wikimedia Commons)._

    > 🖼️ **[GAMBAR-BARU]** Ditautkan dari Wikimedia Commons. Isi gambar sudah dicek langsung dan lisensinya diambil dari metadata berkas.

- Kartogram
    - Peta yang mendistorsi ukuran wilayah (luas area) secara proporsional terhadap nilai data, bukan luas geografis sebenarnya.
    - Fungsi: Untuk menekankan perbedaan jumlah data secara visual.
    - Contoh: Pada kartogram jumlah penduduk dunia, Pulau Jawa akan digambarkan sangat besar (karena penduduknya padat), sementara Papua atau Kalimantan digambarkan lebih kecil dari ukuran sebenarnya karena populasinya sedikit.

- Peta Titik (_Dot Density_)
    - Setiap titik mewakili sejumlah objek tertentu (misalnya 1 titik = 1.000 jiwa), sehingga menunjukkan **persebaran** dan konsentrasi secara langsung, tanpa dibatasi batas administrasi.

    <img width="380" alt="Peta kolera John Snow 1854" src="https://commons.wikimedia.org/wiki/Special:FilePath/Snow-cholera-map-1.jpg?width=760" />\
    Peta asli John Snow (1854) tentang wabah kolera di Soho, London. Setiap batang hitam kecil adalah satu kematian, ditumpuk di depan rumah korban. **Cara membaca:** kematian mengelompok di sekitar pompa air di Broad Street, di bagian tengah peta. **Logikanya:** pola titik ini menunjukkan bahwa kolera menular melalui air yang tercemar, bukan melalui "udara busuk" seperti yang dipercaya saat itu. Peta ini sering dianggap sebagai cikal bakal analisis spasial dan epidemiologi. _Sumber: [John Snow](https://commons.wikimedia.org/wiki/File:Snow-cholera-map-1.jpg), domain publik (Wikimedia Commons)._

    > 🖼️ **[GAMBAR-BARU]** Ditautkan dari Wikimedia Commons. Isi gambar sudah dicek langsung dan lisensinya diambil dari metadata berkas.

- Simbol Proporsional: ukuran simbol (lingkaran, kotak) sebanding dengan nilai data di suatu titik atau wilayah, cocok untuk data jumlah mutlak seperti jumlah penduduk kota.
- Isoplet/Isoline: garis yang menghubungkan titik-titik dengan nilai yang sama untuk data yang berubah secara **kontinu**, misalnya kontur (ketinggian), isoterm (suhu), isobar (tekanan), dan isohiet (curah hujan).
- Peta Aliran (_Flow Map_): garis atau panah yang tebalnya sebanding dengan besarnya arus, misalnya arus migrasi, perdagangan, atau lalu lintas.

> 🆕 **[BAGIAN-BARU]** Jenis-jenis peta tematik lain (titik, simbol proporsional, isoplet, aliran) dan aturan data relatif untuk koroplet ditambahkan.

# 7. Sistem Informasi Geografis (SIG)
> 🆕 **[BAGIAN-BARU]** Konsep dasar SIG belum ada di wiki, padahal sering diujikan dalam bentuk analisis tumpang susun (_overlay_) dan penyangga (_buffer_).

- **SIG** adalah sistem untuk mengumpulkan, menyimpan, menganalisis, dan menampilkan data yang memiliki referensi lokasi.
- **Model data**:
  - **Vektor**: objek digambarkan sebagai titik (sumur, kota), garis (jalan, sungai), atau poligon (batas desa, danau), dengan tabel atribut. Cocok untuk objek yang batasnya tegas.
  - **Raster**: wilayah dibagi menjadi sel atau piksel yang masing-masing memiliki satu nilai, misalnya citra satelit dan model elevasi digital (DEM). Cocok untuk data yang berubah secara kontinu.
- **Analisis dasar**:
  - **Tumpang susun** (_overlay_): menggabungkan beberapa lapisan peta untuk mencari wilayah yang memenuhi beberapa syarat sekaligus, misalnya kesesuaian lahan (lereng landai **dan** tanah subur **dan** bukan kawasan lindung) atau peta risiko bencana (bahaya × kerentanan).
  - **Penyangga** (_buffer_): membuat zona pada jarak tertentu dari suatu objek, misalnya sempadan sungai 50 m atau radius 400–800 m dari stasiun.
  - **Analisis jaringan**: mencari rute terpendek atau wilayah jangkauan layanan berdasarkan jaringan jalan.
  - **Interpolasi**: memperkirakan nilai di tempat tanpa data dari titik-titik pengukuran di sekitarnya, misalnya peta curah hujan dari data stasiun.
- Di Indonesia, **Kebijakan Satu Peta** (Perpres No. 9 Tahun 2016, diperbarui dengan Perpres No. 23 Tahun 2021) bertujuan agar semua kementerian dan lembaga memakai satu peta dasar dan satu standar, sehingga tumpang tindih perizinan lahan dapat dikurangi.

