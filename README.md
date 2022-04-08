# Kasus Covid 19 di DKI Jakarta
Dataset ini berisi Data Riwayat Covid-19 Provinsi DKI Jakarta Bulan April 2020

# Machine Learning
Machine learning membantu memprediksi asal pasien Covid-19 di Provinsi DKI Jakarta Bulan April 2020

# Variabel pada dataset ini:
- id_kel : ID Kelurahan
- nama_provinsi : Nama Provinsi
- nama_kota : Nama Kota
- nama_kecamatan : Nama Kecamatan
- nama_kelurahan : Nama Kelurahan
- odp : Orang Dalam Pengawasan
- proses_pemantauan : Proses Pemantauan
- selesai_pemantauan : Selesai Pemantauan
- pdp : Pasien Dalam Pengawasan
- masih_dirawat : Masih Dirawat
- pulang_dan_sehat : Pulang dan Sehat
- positif : Positif
- dirawat : Dirawat
- sembuh : Sembuh
- meninggal : Meninggal
- self_isolation : Self Isolation
- keterangan : Keteranga

# Persiapan Data
Code yang dipakai :
- Python 3.7.13
- Packages : Pandas, Numpy, Sklearn, Matplotlib, Seaborn
- 
# Dataset :
- Link Dataset : https://data.jakarta.go.id/dataset/data-rekap-harian-kasus-covid19-per-kelurahan-di-provinsi-dki-jakarta-bulan-april-2020

# Data Cleaning
- Pengecekan Missing Values dan pembersihannya
- Check apabila ada kolom dan baris yang duplikat
- Outlier

# Exploratory Data Analysis
Berikut adalah data asal pasien Covid-19 di Provinsi DKI Jakarta Bulan April 2020
![Screenshot (20)](https://user-images.githubusercontent.com/101379389/162385549-b2eee732-70ef-4afa-8582-cf40e84949d5.png)

Korelasi hubungan antara variabel yang ada
![Corr](https://user-images.githubusercontent.com/101379389/162386041-45debdc2-253e-4dc7-8fbe-b1052685bf32.png)

# Modelling
- Split data menjadi menjadi train data dan set dengan besar 0.25 atau 25%
- Menggunakan Random Forest dan Decision Tree

## Menentukan Target

![Screenshot (21)](https://user-images.githubusercontent.com/101379389/162388367-f916a6ca-e2cb-4172-9817-5125d3f89f66.png)

## Menggunakan Over Sampling 
Saya ingin menggunakan balanced data dan merasa data kurang banyak sehingga diputuskan menggunakan Over Sampling

![Screenshot (22)](https://user-images.githubusercontent.com/101379389/162389462-aee4eac7-322a-41d9-aa31-f48ac281b374.png)

# Random Forest - Metric Evaluation
![Screenshot (23)](https://user-images.githubusercontent.com/101379389/162389738-a5883bc8-e1d4-42ea-9870-bf1b2e76617a.png)

# Decision Tree - Metric Evaluation
![Screenshot (25)](https://user-images.githubusercontent.com/101379389/162390396-ea1579c7-2082-4338-b07c-f7cc71a3c295.png)

# Hyperparameter Tuning - Random Forest

![HT Random Forest](https://user-images.githubusercontent.com/101379389/162390528-b622280e-42cd-4ac7-adf7-dc2e013d2bba.png)

![Screenshot (26)](https://user-images.githubusercontent.com/101379389/162390650-e7ba9f73-f353-4f85-b1ba-3867558e7072.png)

- Dengan menggunakan metode Random Forest, hasil recall menunjukkan 0.98, artinya dari 100% data, KNN mampu menjelaskan 98% orang yang masuk rumah sakit berasal dari Jawa Barat
