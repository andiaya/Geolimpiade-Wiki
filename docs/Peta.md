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

# 3. Sistem Koordinat

# 4. Membaca dan Menginterpretasi Peta
- Arah
- Jarak
- Kemiringan
- Volume

# 5. Menginterpretasi Citra
- 9 Kunci Interpretasi

# 6. Grafik Spasial
- Choropleth
- Kartogram
