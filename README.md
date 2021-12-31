# [Machine Learning Project HCBP : Supervide Learning (Mendeteksi Promotable employee) dan Unsupervised (segmentasi critical divisi)](https://github.com/andiainunnajib/Machine-learning-project-HCBP/)
* Membuat machine lerning untuk mendeteksi pegawai telkom yang layak promosi atau tidak
* Menggunakan AutoML untuk memilih algoritma yang paling baik pada supervised learning
* Mebuat Machine learnig unsupervised menggunakan K-means untuk melakukan segmentasi critical divisi (yang kekurangan pegawai atau tidak memiliki atasan)

![image](https://user-images.githubusercontent.com/85381045/147800720-f7ce994e-3cc5-4896-bfbb-ff2e15a00da6.png)

## Table of Contents
* **[EDA pada supervised dataset](#eda-pada-supervised-dataset)**

* **[Data PreProcessing](#data-preprocessing)**

* **[AutoML](#automl)**

* **[Supervised Learning](#supervised-learning)**

* **[Unsupervised Learning](#unsupervised-learning)**



### EDA pada supervised dataset

![image](https://user-images.githubusercontent.com/85381045/146637035-b6b2ea28-8711-470f-904b-d4195d5f565e.png)

![image](https://user-images.githubusercontent.com/85381045/146637084-c2d00399-da87-42e4-8c5b-6ad90346df97.png)
Dari hasil korelasi terdapat beberapa kolum yang memiliki korelasi yang tinggi

**Data kosong**
terdapat beberapa data kosong pada kolom tertentu
![image](https://user-images.githubusercontent.com/85381045/146637095-a268b464-168f-4d38-a925-c8cb705be783.png)


### Data Preprocessing

**tidak ada duplicate data dan terdapat outlier pada kolom time BP**
![image](https://user-images.githubusercontent.com/85381045/146637148-2ac5f8cc-e024-4358-b6f6-15014e8eb9cd.png)

data yang memiliki outlier akan dilakukan IQR
![image](https://user-images.githubusercontent.com/85381045/146637194-35b70c99-f194-455b-9d44-8d80eaa210a2.png)

**Hasil normalisasi dan one hots encoding**
![image](https://user-images.githubusercontent.com/85381045/146637236-33cfd612-07ab-4156-9fa2-735bc45fa649.png)

### AutoML
AutoML digunakan biasanya sebelum data dilakukan preprocessing untuk memudahkan dalam pemilihan algoritma pada AutoML sudah memebrikan hasil dari nilai validasi dari beberapa supervised learning

![image](https://user-images.githubusercontent.com/85381045/146637297-01ccd731-d203-46ad-83d4-c0be163c4901.png)

![image](https://user-images.githubusercontent.com/85381045/146637305-2c4ee41d-93ea-4837-9b56-c89fe004ac9a.png)


### Supervised Learning
Menggubakan Gradient bosting machine
![image](https://user-images.githubusercontent.com/85381045/146637394-c59078e6-e509-469d-bb44-24012c3b234a.png)
dan membuat kodingan untuk mendeteksi apakah machine leaning berhasil atau tidak

![image](https://user-images.githubusercontent.com/85381045/146637415-175513ac-072a-4d00-a75a-a91f1ca3d96d.png)

### Unsupervised Learning
pada unsupervised menggunakan algoritma k-means yang melakukan segmentasi divisi yang critical atau tidak dan setelah dilakukan segmentasi ternyata terdapat 4 segment dan dilaukan pembagian segmentasi menjadi potensial 1-4, semakin rendah nilai potensial semakin critical divisi tersebut
![image](https://user-images.githubusercontent.com/85381045/146637435-79699824-2145-4f89-ae2b-19b42e1eb266.png)




