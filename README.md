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

![image](https://github.com/titispajarningsih/prediksi-waktu-yang-dibutuhkan-untuk-antar-makanan-ke-lokasi-tujuan/assets/145205021/e55f0a82-c6dc-487e-a77b-50370db0a2a0)
![image](https://github.com/titispajarningsih/prediksi-waktu-yang-dibutuhkan-untuk-antar-makanan-ke-lokasi-tujuan/assets/145205021/bc8e0e96-c059-428b-9e2f-abdb1021457a)
###### Gambar 1a. Analisis Univariat (Data Kategori)
![image](https://github.com/titispajarningsih/prediksi-waktu-yang-dibutuhkan-untuk-antar-makanan-ke-lokasi-tujuan/assets/145205021/eeda9de4-f334-4644-b238-bbf6ad50f730)


##### Gambar 1b. Analisis Univariat (Data Numerik)
Berdasarkan Gambar 1a , dapat dilihat bahwa distribusi data kategori untuk 'Type_of_vehicle' memiliki perbandingan jumlah yang tidak sama, untuk nilai data 'motorcycle' dengan persentase 57.4% sedangkan nilai data 'bicycle' memiliki persentasi 0.1%. Lebih jauh, pada Gambar 1b, untuk data numerik memiliki karakteristik, yaitu:
* Data Delivery_person_Age paling banyak memesan memiliki usia 27.5 tahun. Akan tetapi, hampir semua variabel memiliki jumlah data yang sama kecuali pada usia 27.5 tahun
* Data Delivery_person_Ratings memiliki rentang 4.6 - 5.0.
* koordinat restaurant latitude restorant mayoritas berada pada 10 - 25  derajat dan koordinat longitude restaurant mayoritas berada 0-82 derajat.
* koordinat location latitude lokasi pengiriman  mayoritas berada pada 10 - 30  derajat dan koordinat longitude lokasi pengiriman mayoritas berada 0-82 derajat.
* distribusi Time_taken(min) value miring ke kanan (right-skewed). Hal ini akan berimplikasi pada model.

![image](https://github.com/titispajarningsih/prediksi-waktu-yang-dibutuhkan-untuk-antar-makanan-ke-lokasi-tujuan/assets/145205021/d63dbf70-f2a5-4842-9e66-b75f0f557aef)
![image](https://github.com/titispajarningsih/prediksi-waktu-yang-dibutuhkan-untuk-antar-makanan-ke-lokasi-tujuan/assets/145205021/8fc7f7f7-a673-4a45-a1f2-12f93724b03f)
![image](https://github.com/titispajarningsih/prediksi-waktu-yang-dibutuhkan-untuk-antar-makanan-ke-lokasi-tujuan/assets/145205021/ebffb84d-681b-4d01-8a3b-3807c359583b)
![image](https://github.com/titispajarningsih/prediksi-waktu-yang-dibutuhkan-untuk-antar-makanan-ke-lokasi-tujuan/assets/145205021/207da6ed-66ca-45e8-9c52-dcb6aec2e3f7)

##### Gambar 2a. Analisis Multivariat (Data Kategori)
![image](https://github.com/titispajarningsih/prediksi-waktu-yang-dibutuhkan-untuk-antar-makanan-ke-lokasi-tujuan/assets/145205021/f6daf11f-324d-47fc-8690-8e7728768a46)

##### Gambar 2b. Analisis Multivariat (Data Numerik)
![image](https://github.com/titispajarningsih/prediksi-waktu-yang-dibutuhkan-untuk-antar-makanan-ke-lokasi-tujuan/assets/145205021/cf615677-43ce-42b0-bbc4-d513927c3f2f)

##### Gambar 2c. Analisis Multivariat (Correlation Matrix)

Pada Gambar 2a tampak persebaran data 'ocean proximity' terhadap 'median house value'. Dengan mengamati rata-rata 'median_house_value' relatif terhadap fitur kategori di atas, diperoleh insight sebagai berikut:

Pada fitur 'data kategorik', rata-rata 'Time_taken(min)' cenderung bervariasi.
Nilai 'Time_taken(min)' terhadap ID dan Delivery_person_ID memiliki rentang variasi 10 - 50. 
Nilai 'Time_taken(min)' terhadap Type_of_vehicle berada pada nilai 20-30 sedangkan Nilai 'Time_taken(min)' terhadap Type_of_order berada pada nilai 25. 
Kesimpulan akhir, fitur kategori 'Type_of_vehicle' memiliki pengaruh terhadap fitur numerik 'Time_taken(min)'.
Pada Gambar 2b, dengan menggunakan fungsi pairplot dari library seaborn, tampak terlihat relasi pasangan dalam dataset. Dari gambar, terlihat plot relasi masing-masing fitur numerik pada dataset. Pada pola sebaran data grafik pairplot, terlihat bahwa 'Delivery_person_Age' memiliki korelasi yang rendah dengan fitur 'Time_taken(min)'. Sedangkan kedua fitur lainnya terlihat memiliki korelasi yang lebih rendah karena sebarannya tidak membentuk pola.

Terakhir, Gambar 2c merupakan Correlation Matrix menunjukkan hubungan antar fitur dalam nilai korelasi. Jika diamati, fitur 'Delivery_person_Age' memiliki skor korelasi yang sebesar (0.28) dengan fitur target 'Time_taken(min)'. Artinya, fitur 'Time_taken(min)' berkorelasi cukup rendah dengan keempat fitur tersebut. Sementara itu, fitur lainnya memiliki korelasi negatif sehingga fitur tersebut dapat dieliminasi.
# Data Preparation
Pada proses *Data Preparation* dilakukan kegiatan seperti *Data Gathering*, *Data Assessing*, dan *Data Cleaning*.
Pada proses *Data Gathering*, data diimpor sedemikian rupa agar bisa dibaca dengan baik menggunakan *datafram*e Pandas.
Untuk proses *Data Assessing*, berikut adalah beberapa pengecekan yang dilakukan:
- Duplicate data (data yang serupa dengan data lainnya)
- Missing value (data atau informasi yang "hilang" atau tidak tersedia)
- Outlier (data yang menyimpang dari rata-rata sekumpulan data yang ada)
 
Pada proses *Data Cleaning*, secara garis besar, terdapat tiga metode yang dapat digunakan antara lain seperti berikut:
- Dropping (metode yang dilakukan dengan cara menghapus sejumlah baris data)
- Imputation (metode yang dilakukan dengan cara mengganti nilai yang "hilang" atau tidak tersedia dengan nilai tertentu yang bisa berupa median atau mean dari data)
- Interpolation (metode menghasilkan titik-titik data baru dalam suatu jangkauan dari suatu data)

Pada kasus proyek ini tidak ditemukan data duplikat. Pada proyek ini tidak ditemukan *Missing Value*. Untuk *outlier* sendiri dilakukan metode *dropping* menggunakan metode IQR. IQR sendiri didapatkan dengan cara mengurangi Q3 dengan Q1 sebagaimana rumusan berikut. 

$$ IQR = Q<sub>3</sub> - Q<sub>1</sub> $$

dimana
Q<sub>1</sub> adalah kuartil pertama dan Q<sub>3</sub> adalah kuartil ketiga.

Dengan menggunakan metode IQR, dapat ditentukan *outlier* melalui suatu nilai batas yang ditentukan. Setelah menggunakan metode IQR dimana *dataset* yang sebelumnya berjumlah 45593 menjadi 33951.
 
Semua proses ini diperlukan dalam rangka membuat model yang baik. 

Untuk mereduksi jumlah fitur dilakukan proses PCA. Teknik reduksi ini adalah prosedur yang mengurangi jumlah fitur dengan tetap mempertahankan informasi pada data. PCA ini adalah teknik untuk mereduksi dimensi, mengekstraksi fitur, dan mentransformasi data dari “n-dimensional space” ke dalam sistem berkoordinat baru dengan dimensi m, di mana m lebih kecil dari n. Pada proyek ini, fitur 'Delivery_person_Age', 'Restaurant_latitude', 'Delivery_location_latitude' divisualisasikan untuk melihat hubungan di antara fitur-fitur tersebut. seperti yang terlihat pada Gambar 3 berikut.
![image](https://github.com/titispajarningsih/prediksi-waktu-yang-dibutuhkan-untuk-antar-makanan-ke-lokasi-tujuan/assets/145205021/f0788c20-c3e0-401a-888e-3392c85e60e0)
##### Gambar 3 Visualisasi Hubungan antar Fitur sebelum Reduksi PCA
Berdasarkan Gambar 3 dapat diketahui yang memiliki hubungan antar fitur hanya dua yaitu 'Restaurant_latitude', 'Delivery_location_latitude'. Selanjutnya, 2 fitur ini dapat direduksi dengan PCA. Sebelum itu, cek proporsi informasi dari kedua komponen PCs tadi.

```
pca.explained_variance_ratio_.round(2)
```
Potongan kode tersebut memberikan keluaran berupa array([1,0]). Berdasarkan hasil ini, yang dipertahankan adalah PC (komponen) pertama saja karena dari output yang dideroleh diketahui bahwa 100% informasi pada kedua fitur 'Restaurant_latitude', 'Delivery_location_latitude' terdapat pada PC pertama. Sedangkan sisanya, sebesar 0% terdapat pada PC kedua dan. PC pertama ini akan menjadi fitur 'delivery_time2' menggantikan ketiga fitur lainnya ('Restaurant_latitude', 'Delivery_location_latitude').


