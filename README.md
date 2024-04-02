# PREDIKSI WAKTU YANG DIBUTUHKAN UNTUK MENGHANTAR MAKANAN SAMPAI KE TUJUAN
## DOMAIN PROYEK

Pengiriman makanan merupakan salah satu bentuk paling umum dari layanan pengiriman. Ini melibatkan pengiriman makanan dari restoran atau toko makanan ke rumah atau lokasi lain sesuai permintaan pelanggan. Perubahan gaya hidup mode­rn, seperti meningkatnya ke­sibukan dan urbanisasi, telah meningkatkan permintaan akan solusi praktis untuk makanan. Layanan pe­ngiriman makanan membantu pelanggan yang tidak memiliki waktu atau ke­mampuan untuk memasak sendiri atau pergi ke­ restoran. Pelanggan semakin me­nuntut pengalaman pengiriman yang lebih baik, te­rmasuk waktu pengiriman yang cepat dan konsisten se­rta kualitas makanan yang terjaga. 

Dalam hal ini juga Perusahaan pengiriman makanan harus te­rus menyempurnakan operasi me­reka untuk memenuhi harapan pe­langgan. Perusahaan harus memenuhi permintaan pelanggan tanpa kelebihan atau kekurangan persediaan. Di situlah manajemen rantai pasokan masuk. Ini adalah sesuatu yang perlu diperhatikan perusahaan dengan cermat saat mengelola barang. Sebagian besar bisnis masih fokus pada kegiatan internal. maka untuk mempertimbangkan faktor tersebut tersedia pada _dataset_. sehingga dapat di prediksi waktu yang dibutuhkan untuk mengantar makanan ke lokasi tujuan.

dalam hal ini untuk mengontrol perubahan faktor waktu tersebut model yang akan digunakan merupakan model regresi. Model regresi adalah salah satu alat statistik yang digunakan untuk memahami hubungan antara satu atau lebih variabel independen (prediktor) dan variabel dependen (variabel yang ingin diprediksi). Dalam model regresi, variabel independen digunakan untuk memprediksi atau menjelaskan nilai variabel dependen.


## BUSINESS UNDERSTANDING

Peningkatan model prediksi waktu yang diperlukan untuk mengantar makanan memiliki potensi dampak atau manfaat berupa menjadi salah satu alat bantu dalam pengambilan keputusan oleh calon penerima makanan. Contoh potensi manfaat dari hasil prediksi waktu yang dibutuhkan untuk mengantar makanan yang akurat adalah membantu pembeli dan penjual untuk memudahkan pembelian makanan tanpa harus ke restoran.

## PROBLEM STATEMENTS
* Berdasarkan hasil riset _dataset_, komponen apa yang mempengaruhi prediksi waktu yang dibutuhkan unyuk mengantar makanan?
* Bagaimana memproses _dataset_ agar dapat dibuat model prediksi waktu yang dibutuhkan?
* Bagaimana cara menentukan nilai dari _dataset_ dalam bentuk model prediksi waktu yang diinginkan?
  
## GOALS
*  Meriset semua hasil _dataset_ untuk melihat keterkaitan waktu dan juga faktor apa saja yang dapat mempengaruhi prediksi waktu yang dibutuhkan untuk mengantar makanan.
*  Melakukan proses data preparation dan pengolahan data untuk digunakan sebagai model data dan analisis data lebih lanjut.
*  Menjalankan be­ragam variasi model untuk mendapatkan prediksi waktu yang di perlukan dengan Sejumlah model dibuat, dipelajari, dan die­valuasi.
  
## SOLUTION STATEMENTS
* Untuk meriset semua data, Dalam konteks analisis fitur, lakukan Analisis Univariat digunakan untuk memeriksa karakteristik individual dari setiap fitur, dan Analisis Multivariat digunakan untuk melihat hubungan antara fitur-fitur tersebut.
* Untuk mendapatkan prediksi yang baik dilakukan data preparation dan juga pengolahan data.
* Untuk mendapatkan model yang diinginkan menggunakan performa data numerik.
  
## DATA UNDERSTANDING
Dataset berupa CSV
Dataset terdiri dari 45.593 records dengan 11 buah fitur yang diukur.
Dataset terdiri dari 4 data kategori dan 7 data numerik.
Dataset memiliki missing value sejumlah 3639 records
## VARIABEL-VARIABEL PADA DATASET SEBAGAI BERIKUT
ID                         : Merupakan serangkaian huruf yang merupakan tanda pengenal seseorang.
Delivery_person_ID         : Merupakan identifikasi unik pengirim produk dalam sebuah sistem.
Delivery_person_age        : Merupakan identfikasi usia pengirim produk.
Delivery_person_Ratings    : Merupakan peringkat pengirim produk.
Restaurant_latitude        : Koordinat geografis Restaurant yang digunakan untuk menunjukkan posisi suatu titik dari arah timur ke barat yang digunakan menentukan posisi suatu titik pada permukaan bumi (diukur dalam satuan derajat)
Restaurant_longitude        : Koordinat geografis Restaurant yang digunakan untuk menunjukkan posisi suatu titik dari arah utara ke selatan yang digunakan menentukan posisi suatu titik pada permukaan bumi (diukur dalam satuan derajat)
Delivery_location_Latitude  : Koordinat geografis lokasi pengiriman yang digunakan untuk menunjukkan posisi suatu titik dari arah timur ke barat yang digunakan menentukan posisi suatu titik pada permukaan bumi (diukur dalam satuan derajat)
Delivery_location_Latitude  : Koordinat geografis lokasi pengirimanyang digunakan untuk menunjukkan posisi suatu titik dari arah utara ke selatan yang digunakan menentukan posisi suatu titik pada permukaan bumi (diukur dalam satuan derajat)
Type_of_order               : Tipe produk yang dikirim
Type_of_vehicle             : Tipe kendaraan roda dua yang digunakan
Time_Taken(min)             : Lamanya waktu pengiriman            

Analisis Univariat merupakan bentuk analisis data yang hanya merepresentasikan informasi yang terdapat pada satu variabel. Jenis visualisasi ini umumnya digunakan untuk memberikan gambaran terkait distribusi sebuah variabel dalam suatu dataset. Sedangkan, Analisis Multivariat tmerupakan jenis analisis data yang terdapat dalam lebih dari dua variabel. Jenis visualisasi ini digunakan untuk merepresentasikan hubungan dan pola yang terdapat dalam multidimensional data.
Selain melalui analisis, dilakukan juga Visualisasi Data. Memvisualisasikan data memberikan wawasan mendalam tentang perilaku berbagai fitur-fitur yang tersedia dalam dataset. Teknik visualisasi yang digunakan pada pembuatan model proyek ini adalah dengan menggunakan catplot yang digunakan untuk memplot distribusi data pada data kategori, pairplot yang digunakan untuk melakukan hubungan antar fitur dalam dataset, dan heatmap yang menampilkan korelasi antar fitur yang ada dalam dataset dalam bentuk matriks.

Berikut adalah hasil Exploratory Data Analysis (EDA), dimana Gambar 1 merupakan EDA Analisis Univariat dan Gambar 2 merupakan EDA Analisis Multivariat.

###### Gambar 1a. Analisis Univariat (Data Kategori)


##### Gambar 1b. Analisis Univariat (Data Numerik)


