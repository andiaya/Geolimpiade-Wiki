---
title: Perpetaan dan Interpretasi Data Spasial
permalink: /docs/Peta/
layout: single
toc: true
toc_sticky: true
sidebar:
  nav: "docs"
---
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
    8. _Insert_ / Inset: muka peta kecil untuk menunjukkan informasi berupa konteks wilayah yang lebih luas atau detail wilayah lebih sempit.
  ![1209-441](https://github.com/user-attachments/assets/f87ab37b-94a5-48d7-95b5-b59b34bfaf62)\
  Ilustrasi Unsur Peta

# 2. Proyeksi Peta
- Proyeksi adalah proses perubahan yang harus dilakukan saat mengubah geometri benda dari bidang 3 dimensi ke bidang 2 dimensi.
- Bola Bumi memiliki permukaan yang tidak rata. Bola Bumi dapat dimodelkan berdasarkan ketinggian permukaannya (elevation model / topografik), kekuatan gravitasi di permukaannya (geoid model), maupun dalam bentuk bola dengan permukaan rata (ellipsoid model).
- Proyeksi peta diawali dengan membuat model elipsoid Bumi, lalu dilakukan proyeksi matematis ke bidang datar.
- Perubahan dari bentuk 3 dimensi ke 2 dimensi pasti menghasilkan distorsi, biasanya nampak dalam bentuk kenampakan objek yang terlihat seperti tertarik dari sisinya.

  ## 2.1. Bidang Proyeksi
  - Tipe bidang proyeksi menentukan lokasi di bola Bumi yang bertampalan dengan bidang proyeksi.
  - Lokasi yang bertampalan dengan bidang proyeksi memiliki distorsi paling rendah.
  - Tipe bidang proyeksi yaitu:
    1. Silinder (_Cylindrical_): bertampalan dengan bola Bumi pada keliling terpanjang Bumi.
    2. Kerucut (_Conical_): bertampalan dengan bola Bumi pada keliling Bumi yang bukan merupakan keliling terpanjang.
    3. Planar (_Azimuthal_): bertampalan dengan bola Bumi pada 1 titik. Peta hanya bisa menggambarkan satu belahan Bumi.
       - Tipe proyeksi azimuthal dapat diklasifikasikan menjadi 3 jenis berdasarkan penempatan titik hilang perspektifnya (_vanishing point_). Klasifikasi tersebut yaitu:
         1. Gnomonik: memiliki titik hilang di pusat Bumi. Seluruh garis lurus jika digambarkan pada globe juga terlihat lurus pada peta gnomonik.
         2. Stereografik: memiliki titik hilang di sisi Bumi berlawanan. Proyeksi Stereografik mempertahankan bentuk kenampakan di permukaan Bumi dengan mempertahankan sudut.
         3. Orthografik: memiliki titik hilang di jarak tak hingga. Peta nampak seperti kenampakan globe dari sisi samping.
    
    <img width="316" height="159" alt="tipe bidang proyeksi" src="https://github.com/user-attachments/assets/38a4640b-b15f-400a-8ae2-f2188c3341e9" />\
    Urut dari kiri ke kanan bidang proyeksi silinder, kerucut, dan planar
    
    <img width="286" height="176" alt="tipe proyeksi azimuthal" src="https://github.com/user-attachments/assets/99739b72-165c-45c1-a394-9ebd28b54ea6" />\
    Urut dari kiri ke kanan tipe proyeksi azimuthal gnomonik, stereografik, dan orthografik

  - Orientasi bidang proyeksi terhadap bola Bumi juga mempengaruhi area Bumi yang bertampalan. Orientasi bidang proyeksi tersebut yaitu:
    1. Normal: bidang proyeksi memiliki orientasi tegak terhadap bola Bumi. Bidang silinder akan bertampalan di ekuator, bidang kerucut bertampalan di lintang sedang, dan bidang planar bertampalan di satu titik di ekuator.
    2. Transverse: bidang proyeksi berorientasi rebah terhadap bola Bumi. Bidang silinder bertampalan di garis meridian dan antimeridian dan seterusnya.
    3. Oblique: bidang proyeksi berorientasi miring terhadap bola Bumi. Bidang silinder bertampalan memotong 2 garis lintang sedang dan seterusnya.\
    <img width="384" height="131" alt="image" src="https://github.com/user-attachments/assets/247d3f42-bcac-4dc1-ae7f-fbdc172a38a3" />\
    Urut dari kiri ke kanan bidang proyeksi normal, transverse, dan oblique
  
  ## 2.2. Karakteristik Proyeksi Peta
  - Proyeksi menyebabkan distorsi atau perubahan dari bentuk asli permukaan Bumi dengan yang ditunjukkan pada peta.
  - Proyeksi dipilih berdasarkan karakteristik yang akan dipertahankan, yaitu:
    1. Konform: mempertahankan bentuk (arah). Digunakan untuk mengetahui arah kompas antara 2 titik di Bumi. Contoh proyeksi: merkator, lambert kerucut, stereografis.
    2. Ekuidistan: mempertahankan jarak pada satu garis tertentu pada peta, misalnya jarak tiap titik pada peta terhadap titik tengahnya. Contoh proyeksi: azimuthal ekuidistan (akuran antara titik tengah peta dengan titik manapun), kerucut ekuidistan (akurat antara 2 garis lintang tertentu), silinder ekuidistan (jarak akurat di sepanjang ekuator).
    3. Ekuivalen: menunjukkan luas area yang proporsional satu sama lain. Contoh proyeksi: mollweide, albers, gall-peters.

# 3. Sistem Koordinat

## 3.1. Sistem Koordinat Geografis
Sistem ini menggunakan garis lintang dan bujur untuk menentukan lokasi absolut di permukaan bumi yang berbentuk bola (spheroid).

- Lintang (Latitude): Garis horizontal yang sejajar dengan ekuator. Nilainya 0° di Ekuator hingga 90° di Kutub Utara (LU) atau 90° di Kutub Selatan (LS).
- Bujur (Longitude): Garis vertikal yang menghubungkan Kutub Utara dan Selatan. Nilainya 0° di Prime Meridian (Greenwich) hingga 180° ke arah Timur (BT) atau Barat (BB).
- Satuan: Derajat (°), Menit ('), Detik (") atau Derajat Desimal (Decimal Degrees).
- Contoh: Monumen Nasional (Monas) terletak di 6°10'30" LS, 106°49'40" BT.

## 3.2. Sistem Koordinat UTM (Universal Transverse Mercator)
Sistem proyeksi peta yang membagi bumi menjadi 60 zona (masing-masing selebar 6° bujur). Sistem ini menggunakan bidang datar (proyeksi silinder) sehingga menghasilkan satuan meter, bukan derajat.

- Zona: Indonesia terletak di Zona 46, 47, 48, 49, 50, 51, 52, 53, 54.
- Koordinat:
    - Eastings (Timur): Jarak ke timur dari meridian sentral zona (dalam meter).
    - Northings (Utara): Jarak dari ekuator (untuk belahan utara) atau jarak dari ekuator + nilai koreksi (untuk belahan selatan).
- Kelebihan: Lebih mudah untuk mengukur jarak, luas, dan volume secara langsung di peta karena satuannya linier (meter).

# 4. Membaca dan Menginterpretasi Peta

## 4.1. Arah
- Azimuth: Sudut horizontal yang diukur searah jarum jam dari titik Utara Sejati (True North) atau Utara Magnetik. Nilainya 0° hingga 360°.
    - Contoh: Arah Timur = Azimuth 90°.
- Bearing: Sudut horizontal yang diukur dari acuan Utara atau Selatan menuju Barat atau Timur. Nilainya 0° hingga 90° dan selalu disertai huruf arah.
    - Format: [U/S] [Nilai Sudut] [B/T].
    - Contoh: Azimuth 135° = Bearing S 45° T (Dibaca: Selatan 45 derajat ke Timur).

## 4.2. Jarak dan Kemiringan
- Jarak Datar (Horizontal Distance - HD): Panjang garis lurus antara dua titik yang diproyeksikan pada bidang datar (peta). Diukur menggunakan skala peta atau rumus Pythagoras dari koordinat (X,Y).
- Kemiringan (Slope/Gradient): Perbandingan antara beda tinggi vertikal dengan jarak datar. Bisa dinyatakan dalam pecahan desimal, persen (%), atau derajat (°). Untuk mengubah desimal ke persen maka nilai desimal dikali 100%, sedangkan untuk mengubah desimal ke derajat maka dicari arctan dari nilai desimal tersebut (tan^(-1) (Nilai Desimal)).
    - Rumus:
      
      $Kemiringan = \frac{Beda Tinggi}{Jarak Datar}$
      
- Jarak Miring (Slope Distance - SD): Jarak sebenarnya yang harus ditempuh di permukaan tanah yang tidak rata.
    - Rumus Pythagoras:
      
      $SD = \sqrt{(Jarak Datar)^2 + (Beda Tinggi)^2}$

## 4.3. Volume
Perhitungan volume biasanya digunakan dalam pekerjaan Cut and Fill (Galian dan Timbunan) atau perhitungan cadangan tambang.
- Metode Penampang Rata-Rata (Average End Area):
  
  $Volume = \frac{(Luas_1 + Luas_2)}{2} \times JarakAntarPenampang$
  
- Metode Grid/Prismoidal: Menghitung volume berdasarkan grid ketinggian digital (DEM/Digital Elevation Model) menggunakan rumus prisma terpancung.

# 5. Menginterpretasi Citra

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

- Kartogram
    - Peta yang mendistorsi ukuran wilayah (luas area) secara proporsional terhadap nilai data, bukan luas geografis sebenarnya.
    - Fungsi: Untuk menekankan perbedaan jumlah data secara visual.
    - Contoh: Pada kartogram jumlah penduduk dunia, Pulau Jawa akan digambarkan sangat besar (karena penduduknya padat), sementara Papua atau Kalimantan digambarkan lebih kecil dari ukuran sebenarnya karena populasinya sedikit.
