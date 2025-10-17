# Data GeoJSON Desa Karyawangi Kecamatan Parongpong Kabupaten Bandung Barat - Proyek SIG

Dokumentasi ini berisi data geospasial dalam format GeoJSON untuk wilayah Desa Karyawangi, Kecamatan Parongpong, Kabupaten Bandung Barat.

Informasi Pengembang:

- Nama: Indra Agustin
- NPM: 714230051
- Mata Kuliah: Sistem Informasi Geografis
- Kelas: 3B

## 1. Deskripsi Wilayah

Desa Karyawangi merupakan salah satu desa yang terletak di Kecamatan Parongpong, Kabupaten Bandung Barat, Provinsi Jawa Barat. Wilayah ini berada di dataran tinggi yang sejuk dan subur, menjadikannya kawasan agrowisata yang populer. Desa Karyawangi dikenal dengan potensi wisata alamnya, seperti air terjun (curug) dan area perkemahan, serta menjadi salah satu sentra pertanian bunga potong dan sayuran di kawasan Bandung Utara. Letaknya yang strategis di dekat kawasan wisata Lembang membuat desa ini terus berkembang.

## 2. Letak dan Batas Wilayah

### Letak Geografis

Desa Karyawangi berada di lereng Gunung Tangkuban Parahu dan Burangrang, yang secara geografis memberikan keuntungan berupa tanah vulkanik yang subur dan pemandangan alam yang indah.

### Batas Administrasi

Berdasarkan data dari portal resmi desa dan referensi akademis, batas-batas wilayah administrasi Desa Karyawangi adalah sebagai berikut:

- Sebelah Utara: Berbatasan dengan Kabupaten Subang.

- Sebelah Timur: Berbatasan dengan Desa Cihideung (Kecamatan Parongpong).

- Sebelah Selatan: Berbatasan dengan Desa Sariwangi (Kecamatan Parongpong).

- Sebelah Barat: Berbatasan dengan Desa Cihanjuang Rahayu (Kecamatan Parongpong).

## 3. Struktur Data GeoJSON

Contoh struktur GeoJSON (FeatureCollection) yang umum digunakan untuk menyimpan fitur geospasial. Contoh di bawah menunjukkan sebuah fitur bertipe LineString yang merepresentasikan jalan:

```json
{
  "type": "FeatureCollection",
  "features": [
    {
      "type": "Feature",
      "properties": {
        "@id": "way/318100665",
        "foot": "designated",
        "highway": "primary",
        "lanes": 2,
        "name": "Karyawangi",
        "oneway": "no",
        "ref": 247,
        "source": "GPS",
        "surface": "asphalt"
      },
      "geometry": {
        "type": "LineString",
        "coordinates": [
          [107.5827991, -6.8029249],
          [107.5828894, -6.8029336],
          [107.5830713, -6.8030084]
        ]
      }
    }
  ]
}
```

Penjelasan singkat field penting:

- "type": "FeatureCollection" — objek GeoJSON paling atas yang berisi kumpulan fitur.
- "properties": menyimpan atribut atau metadata feature, seperti nama jalan, jumlah lajur, sumber data, dan atribut lain yang relevan.
- "geometry": menjelaskan bentuk geometris feature; pada contoh ini bertipe "LineString" yang dibentuk dari serangkaian koordinat [longitude, latitude].

## 4. Sumber Data Proyek

Sumber Data Geospasial (GeoJSON)

Data untuk pemetaan Wilayah Desa Karyawangi menggunakan format GeoJSON. Objek jalan direpresentasikan sebagai geometri LineString, dan informasi detailnya (seperti nama jalan) disimpan sebagai atribut di dalam bagian "properties".

Sumber Data Batas Wilayah
Informasi batas wilayah administrasi yang tercantum pada Bab 2 diverifikasi dari beberapa sumber berikut:

- Portal Resmi Desa Karyawangi: https://karyawangi.digitaldesa.id
- Portal Resmi Desa Tetangga: https://sariwangi.digitaldesa.id (untuk konfirmasi batas selatan)
- Repository Akademis: https://repository.upi.edu (penelitian yang menyebutkan perbatasan antar desa)

## 5. Cara Menggunakan File

Untuk melihat visualisasi data dari file .geojson ini, Anda dapat menggunakan beberapa cara:

- geojson.io: Buka situs https://geojson.io dan seret (drag and drop) file GeoJSON Anda ke dalam halaman tersebut.
- QGIS: Buka software QGIS, lalu tambahkan layer baru dengan memilih opsi "Vector Layer" dan pilih file GeoJSON Anda.
