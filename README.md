# PREDIKSI WAKTU YANG DIBUTUHKAN UNTUK MENGHANTAR MAKANAN SAMPAI KE TUJUAN
## DOMAIN PROYEK

Pengiriman makanan merupakan salah satu bentuk paling umum dari layanan pengiriman. Ini melibatkan pengiriman makanan dari restoran atau toko makanan ke rumah atau lokasi lain sesuai permintaan pelanggan. Perubahan gaya hidup mode­rn, seperti meningkatnya ke­sibukan dan urbanisasi, telah meningkatkan permintaan akan solusi praktis untuk makanan[1]. Layanan pe­ngiriman makanan membantu pelanggan yang tidak memiliki waktu atau ke­mampuan untuk memasak sendiri atau pergi ke­ restoran. Pelanggan semakin me­nuntut pengalaman pengiriman yang lebih baik, te­rmasuk waktu pengiriman yang cepat dan konsisten se­rta kualitas makanan yang terjaga[2]. 

Dalam hal ini juga Perusahaan pengiriman makanan harus te­rus menyempurnakan operasi me­reka untuk memenuhi harapan pe­langgan. Perusahaan harus memenuhi permintaan pelanggan tanpa kelebihan atau kekurangan persediaan. Di situlah manajemen rantai pasokan masuk. Ini adalah sesuatu yang perlu diperhatikan perusahaan dengan cermat saat mengelola barang. Sebagian besar bisnis masih fokus pada kegiatan internal. maka untuk mempertimbangkan faktor tersebut tersedia pada _dataset_. sehingga dapat di prediksi waktu yang dibutuhkan untuk mengantar makanan ke lokasi tujuan[3][4][5].

dalam hal ini untuk mengontrol perubahan faktor waktu tersebut model yang akan digunakan merupakan model regresi. Model regresi adalah salah satu alat statistik yang digunakan untuk memahami hubungan antara satu atau lebih variabel independen (prediktor) dan variabel dependen (variabel yang ingin diprediksi). Dalam model regresi, variabel independen digunakan untuk memprediksi atau menjelaskan nilai variabel dependen.


## BUSINESS UNDERSTANDING

Peningkatan model prediksi waktu yang diperlukan untuk mengantar makanan memiliki potensi dampak atau manfaat berupa menjadi salah satu alat bantu dalam pengambilan keputusan oleh calon penerima makanan[6]. Contoh potensi manfaat dari hasil prediksi waktu yang dibutuhkan untuk mengantar makanan yang akurat adalah membantu pembeli dan penjual untuk memudahkan pembelian makanan tanpa harus ke restoran.

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
* Dataset berupa CSV
* Dataset terdiri dari 45.593 records dengan 11 buah fitur yang diukur.
* Dataset terdiri dari 4 data kategori dan 7 data numerik.
* Dataset memiliki missing value sejumlah 0 records.
  
## VARIABEL-VARIABEL PADA DATASET SEBAGAI BERIKUT
* ID                         : Merupakan serangkaian huruf yang merupakan tanda pengenal seseorang.
* Delivery_person_ID         : Merupakan identifikasi unik pengirim produk dalam sebuah sistem.
* Delivery_person_age        : Merupakan identfikasi usia pengirim produk.
* Delivery_person_Ratings    : Merupakan peringkat pengirim produk.
* Restaurant_latitude        : Koordinat geografis Restaurant yang digunakan untuk menunjukkan posisi suatu titik dari arah timur ke barat yang digunakan menentukan posisi suatu titik pada permukaan bumi (diukur dalam satuan derajat)
Restaurant_longitude        : Koordinat geografis Restaurant yang digunakan untuk menunjukkan posisi suatu titik dari arah utara ke selatan yang digunakan menentukan posisi suatu titik pada permukaan bumi (diukur dalam satuan derajat)
* Delivery_location_Latitude  : Koordinat geografis lokasi pengiriman yang digunakan untuk menunjukkan posisi suatu titik dari arah timur ke barat yang digunakan menentukan posisi suatu titik pada permukaan bumi (diukur dalam satuan derajat)
* Delivery_location_Latitude  : Koordinat geografis lokasi pengirimanyang digunakan untuk menunjukkan posisi suatu titik dari arah utara ke selatan yang digunakan menentukan posisi suatu titik pada permukaan bumi (diukur dalam satuan derajat)
  
* Type_of_order               : Tipe produk yang dikirim
* Type_of_vehicle             : Tipe kendaraan roda dua yang digunakan
* Time_Taken(min)             : Lamanya waktu pengiriman            

Analisis Univariat merupakan bentuk analisis data yang hanya merepresentasikan informasi yang terdapat pada satu variabel. Jenis visualisasi ini umumnya digunakan untuk memberikan gambaran terkait distribusi sebuah variabel dalam suatu dataset. Sedangkan, Analisis Multivariat tmerupakan jenis analisis data yang terdapat dalam lebih dari dua variabel. Jenis visualisasi ini digunakan untuk merepresentasikan hubungan dan pola yang terdapat dalam multidimensional data.

Selain melalui analisis, dilakukan juga Visualisasi Data. Memvisualisasikan data memberikan wawasan mendalam tentang perilaku berbagai fitur-fitur yang tersedia dalam dataset[6][7]. Teknik visualisasi yang digunakan pada pembuatan model proyek ini adalah dengan menggunakan catplot yang digunakan untuk memplot distribusi data pada data kategori, pairplot yang digunakan untuk melakukan hubungan antar fitur dalam dataset, dan heatmap yang menampilkan korelasi antar fitur yang ada dalam dataset dalam bentuk matriks.

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

Pada Gambar 2a tampak persebaran data 'kategorik' terhadap 'Time_taken(min)'. Dengan mengamati rata-rata 'Time_taken(min) relatif terhadap fitur kategori di atas, diperoleh insight sebagai berikut:

Pada fitur 'data kategorik', rata-rata 'Time_taken(min)' cenderung bervariasi.
Nilai 'Time_taken(min)' terhadap ID dan Delivery_person_ID memiliki rentang variasi 10 - 50. 
Nilai 'Time_taken(min)' terhadap Type_of_vehicle berada pada nilai 20-30 sedangkan Nilai 'Time_taken(min)' terhadap Type_of_order berada pada nilai 25. 
Kesimpulan akhir, fitur kategori 'Type_of_vehicle' memiliki pengaruh terhadap fitur numerik 'Time_taken(min)'.
Pada Gambar 2b, dengan menggunakan fungsi pairplot dari library seaborn, serta tampak terlihat relasi pasangan dalam dataset. Dari gambar, terlihat plot relasi masing-masing fitur numerik pada dataset. Pada pola sebaran data grafik pairplot, terlihat bahwa 'Delivery_person_Age' memiliki korelasi yang rendah dengan fitur 'Time_taken(min)'. Sedangkan kedua fitur lainnya terlihat memiliki korelasi yang lebih rendah karena sebarannya tidak membentuk pola.

Terakhir, Gambar 2c merupakan Correlation Matrix menunjukkan hubungan antar fitur dalam nilai korelasi. Jika diamati, fitur 'Delivery_person_Age' memiliki skor korelasi yang sebesar (0.28) dengan fitur target 'Time_taken(min)'. Artinya, fitur 'Time_taken(min)' berkorelasi cukup rendah dengan keempat fitur tersebut. Sementara itu, fitur lainnya memiliki korelasi negatif sehingga fitur tersebut dapat dieliminasi.

## Data Preparation
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
Potongan kode tersebut memberikan keluaran berupa array([1,0]). Berdasarkan hasil ini, yang dipertahankan adalah PC (komponen) pertama saja karena dari output yang dideroleh diketahui bahwa 100% informasi pada kedua fitur 'Restaurant_latitude', 'Delivery_location_latitude' terdapat pada PC pertama. Sedangkan sisanya, sebesar 0% terdapat pada PC kedua dan. PC pertama ini akan menjadi fitur 'delivery_time2' menggantikan kedua fitur lainnya ('Restaurant_latitude', 'Delivery_location_latitude').

Setelah data dibersihkan, *dataset* dibagi menjadi data train dan data test untuk proses *Modeling*, dimana rasio pembagian data yang dipilih adalah 90:10 mengingat data test untuk rasio tersebut sudah terbilang cukup. 
Adapun detail dari *dataset* tersebut adalah:
- Total sampel di dalam *dataset* train:30555
- Total sampel di dalam *dataset* test: 3396

Seperti yang dijelaskan di awal, model yang dipilih adalah model regresi karena merupakan salah satu algoritma yang paling umum digunakan dalam pembuatan model prediksi. Dalam bentuk yang sederhana, regresi terdiri dari intersep dan slope yang dituliskan dalam rumusan berikut

$$ y = a + bX $$

dimana: 
- y adalah variabel kriterium (variabel terikat yang digunakan untuk memprediksi)
- a adalah intersep (variabel konstan yang memiliki arti sebagai titik perpotongan suatu garis dengan sumbu Y),
- b adalah slope (nilai koefisien yang menyatakan ukuran kemiringan suatu garis), dan
- X adalah variabel prediktor (variabel yang digunakan untuk memprediksi atau menjelaskan variabel lain dalam suatu model)

Secara umum, regresi ini itu sendiri digunakan untuk meramalkan pengaruh variabel prediktor terhadap variabel kriterium atau membuktikan ada atau tidaknya hubungan fungsional antara variabel bebas (X) dengan variabel terikat (y).

Namun begitu terdapat kelebihan dan kekurangan dari model regresi, yaitu:

Kelebihan regresi:
- Kemudahan untuk digunakan
- Kekuatan Prediktor dalam mengidentifikasi sekuat apa pengaruh yang diberikan oleh variabel prediktor (variabel independen) terhadap variabel lainnya (variabel dependen).
- Dapat memprediksi nilai/tren di masa yang mendatang

Kelemahan dari model regresi adalah karena hasil ramalan dari analisis regresi merupakan nilai estimasi sehingga kemungkinan untuk tidak sesuai dengan data aktual tetaplah ada.

Pada proyek yang dikerjakan, algoritma regresi yang coba dibandingkan adalah regresi linear, regresi ridge, *random forest regressor*, dan *random forest regressor* dengan hyperparamter tuning. Regresi linear adalah teknik analisis data yang memprediksi nilai data yang tidak diketahui dengan menggunakan nilai data lain yang terkait dan diketahui dimana secara matematis dimodelkan sebagai persamaan linier, regresi ridge merupakan metode estimasi koefisien regresi yang diperoleh melalui penambahan konstanta bias c, dan random forest adalah suatu algoritma yang digunakan pada klasifikasi data dalam jumlah yang besar dimana teknik klasifikasi *random forest* dilakukan melalui penggabungan pohon dengan melakukan training pada sampel data yang dimiliki.

Untuk meningkatkan model, maka dilakukan *hyperparamter tuning*. Adapun paramater yang di-tuning antara lain n_estimators', 'max_depth', 'min_samples_split', dan 'min_samples_leaf. Untuk memudahkan proses *tuning* digunakan GridSearchCV. GridSearchCV itu sendiri merupakan bagian dari modul scikit-learn yang dapat digunakan untuk mendapatkan nilai *hyperparameter* secara otomatis. Grid Search adalah metode yang digunakan untuk mencari parameter yang paling tepat untuk meningkatkan performa model dengan mencoba seluruh kombinasi *hyperparameter* yang diberikan.

Berikut adalah nilai parameter *tuning*
```
params = {'n_estimators' : [50,80,100],
          'max_depth' : [3,5,10],
           'min_samples_split':[2,3,4],
            'min_samples_leaf': [2,3,4]}
```
Berdasarkan hasil pengujian, terpilih grid.best_params_ yaitu 
```
{'max_depth': 10,
 'min_samples_leaf': 4,
 'min_samples_split': 2,
 'n_estimators': 100}
```
Parameter dengan nilai inilah yang kemudian dibuat sebagai model.

## Evaluation
Adapun metrik yang sebagai alat ukur perfoma model yang dibuat antara lain **MSE · MAE · R<sup>2</sup>**. 

Berikut merupakan rumus dari masing-masing metrik yang digunakan:

$$ MAE = (1/n) Σ |y<sub>i</sub> - ŷ<sub>i</sub>| $$

$$ MSE = (1/n) Σ (y<sub>i</sub> - ŷ<sub>i</sub>)<sup>2</sup> $$

$$ R<sup>2</sup> = 1 - (MSE / Var(y)) $$

y<sub>i</sub> mewakili nilai yang diamati,
ŷ<sub>i</sub> mewakili nilai prediksi,
n adalah jumlah titik data,
Var(y) mewakili varians dari nilai yang diamati.

Berikut merupakan penjelasan kegunaan dari masing-masing metrik yang digunakan:
- MAE menghitung rata-rata dari selisih absolut antara nilai prediksi dan nilai aktual. Semakin kecil nilai MAE, semakin baik kualitas model tersebut.
- MSE menghitung rata-rata dari selisih kuadrat antara nilai prediksi dan nilai aktual. Semakin kecil nilai MSE, semakin baik kualitas model tersebut.
- R<sup>2</sup> digunakan untuk menilai seberapa besar pengaruh variabel independen tertentu terhadap variabel dependen

Tabel 1 berikut merupakan perbandingan 4 buah model yang coba dibandingkan.

|     |Model 1|Model 2|Model 3|Model 4|
|---|---|---|---|---|
|R<sup>2</sup>|-74.52030902734705|-74.30663755394067|-0.28436114329343876|-0.17376766906387964|
|MSE|75.46161185307521|75.35478353653197| 9.840967040852833| 9.407739205161636|
|MAE|74.10977269043104|74.00364805451821|8.182609554658141|7.846619330024802|

Tabel 1. Perbandingan Performa MAE, MSE, dan R<sup>2</sup> Model

Berdasarkan Tabel 1, secara umum Model 3 (RF1) dan Model 4 (RF2) menampilkan hasil performa yang lebih baik dimana masing-masing memiliki nilai R^2 yaitu sebesar -0.28436114329343876 dan-0.17376766906387964.

Secara lebih jauh perbandingan Model 1, 2, 3, dan 4 bisa dilihat pada Gambar 4 berikut.

![image](https://github.com/titispajarningsih/prediksi-waktu-yang-dibutuhkan-untuk-antar-makanan-ke-lokasi-tujuan/assets/145205021/d735e334-05b3-4248-9557-a131c5351d35)


##### Gambar 4. Perbandingan Model berdasarkan Nilai Error (dalam 1e6)

Berdasarkan Gambar 4 dapat terlihat bahwa nilai error train dan test dari Model 3 (RF1) dan Model 4 (RF2) jauh lebih baik dibandingkan model lainnya.

Selain itu dilakukan perbandingan nilai y_true terhadap nilai prediksi harga rumah dari 4 buah model yang dibuat. Tabel 2 juga merupakan hasil dari evaluasi model yang telah dibuat.

|     |y_true|prediksi_LR|prediksi_RR|prediksi_RF1|prediksi_RF2|
|---|---|---|---|---|---|
|25003	|22|10.3|10.3|19.7|20.6|

Tabel 2. Perbandingan Model


Berdasarkan hasil evaluasi, maka terlihat bahwa prediksi waktu pengiriman dengan *Random Forest* (RF), baik RF1 (tanpa tuning) ataupun RF2 (dengan tuning) memberikan hasil yang paling mendekati y_true, dimana nilai y_true yaitu 22 dan nilai RF1 dan RF2 masing-masing yaitu 19.7 dan 20.6. Dengan demikian bisa disimpulkan bahwa model yang telah dikembangkan dapat memprediksi prediksi waktu pengiriman dengan cukup baik dengan menggunakan *Random Forest Regressor*.

# REFERENSI
[1] https://www.parcel2go.com/shipping-advice

[2] https://www.parcel2go.com/content-hub/everything-you-need-to-know-about-sending-a-parcel

[3] https://www.parcel2go.com/services/next-day-delivery

[4] https://www.parcel2go.com/content-hub/how-to-send-a-parcel

[5] https://www.parcel2go.com/services/send-a-parcel

[6] https://www.general-index.com/pages/data-delivery

[7] https://www.tickdata.com/data-delivery-overview/

[8] https://www.promptcloud.com/blog/data-delivery-formats-pros-cons/

[9] https://docs.oracle.com/en/cloud/saas/data-cloud/data-cloud-help-center/IntegratingBlueKaiPlatform/data_delivery.html 

[10] https://www.enformion.com/data-delivery-options/


