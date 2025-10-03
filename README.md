# IBM-Summarizing-Data

## Deskripsi
Notebook ini menunjukkan pipeline lengkap untuk mengolah data COVID-19 Indonesia, memvisualisasikan tren kasus dan kematian, serta menggunakan model IBM Granite dari Replicate untuk membuat ringkasan naratif berbasis AI terhadap data kumulatif tersebut.

## Isi Utama Notebook
1. Instalasi dan Import Library
   - langchain_community
   - replicate
   - pandas
   - matplotlib
   - dll

2. Pengambilan dan Persiapan Data
   - Mengunduh dataset COVID-19 dari sumber Kaggle yang berisi data harian global
   - Memfilter data untuk Indonesia
   - Mengubah kolom tanggal menjadi format datetime dan mengelompokkan data per bulan
   - Membuat dataframe lengkap yang berisi kasus baru, kumulatif, kematian baru, dan kumulatif per tanggal
     
3. Visualisasi Data
   - Membuat grafik tren kasus kumulatif dan kematian kumulatif per bulan
   - Penyesuaian tampilan grafik agar mudah dibaca (rotasi label, format angka)

4. Penyusunan Ringkasan Data
   - Menyusun ringkasan bulanan dalam bentuk teks yang mudah dibaca
   - Mendefinisikan prompt AI yang mendeskripsikan data dan mengarahkan model untuk membuat ringkasan tren, lonjakan, penurunan, dan insight penting
     
5. Integrasi dengan IBM Granite (Replicate)
   - Setup API Replicate
   - Mengirim prompt bersama data ringkasan ke model Granite
   - Menerima dan menampilkan output ringkasan AI
