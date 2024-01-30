# Latihan-SKLearn-K-means

**Tahapan Latihan**

Tahapan pada latihan kali ini adalah sebagai berikut:

- Konversi data menjadi Dataframe.

- Lakukan preprocessing data.

- Hilangkan kolom 'CustomerID' dan 'gender'.

- Latih model K-Means.

- Buat plot untuk Elbow dan Cluster

# Codelab

Dataset yang akan Anda gunakan adalah data pengunjung sebuah mall fiktif. Dataset bisa Anda dapatkan pada tautan https://www.kaggle.com/vjchoudhary7/customer-segmentation-tutorial-in-python berikut.

Setelah Anda berhasil mengunduh datanya, buka Notebook pada Google Colab dan unggah dataset Mall Customer Segmentation Data pada session storage Google Colab.

Pada cell pertama, kita ubah file csv kita ke dalam dataframe pandas dan menampilkan 3 baris pertama dari dataframe.

![1](https://github.com/brnabidin/Latihan-SKLearn-K-means/assets/67081096/637f04f6-86c7-493e-ad25-69e761430926)

Tampilan dari 3 baris pertama dataframe di atas seperti berikut.

![20200430224650330de4b6a3da9b3dc6e31e9a6de6301b](https://github.com/brnabidin/Latihan-SKLearn-K-means/assets/67081096/9ef84d6b-d932-4fa7-b664-ab60fb934fd2)

Kemudian kita akan melakukan sedikit preprocessing yaitu mengubah nama kolom agar lebih seragam. Lalu kolom gender adalah kolom kategorik, maka kita akan mengubah data tersebut menjadi data numerik.

![2](https://github.com/brnabidin/Latihan-SKLearn-K-means/assets/67081096/074effb2-ac22-465e-beb6-f8fcbf9318df)

Setelah dilakukan preprocessing dengan mengubah nama kolom supaya lebih seragam, maka hasilnya seperti di bawah ini.

![202004302250389bbd2c50306e7116d35e903eb41ab339](https://github.com/brnabidin/Latihan-SKLearn-K-means/assets/67081096/28edc528-c79d-42f4-9a1f-5467ddbee83b)

Di tahap selanjutnya kita akan mengimpor K-Means. Di tahap ini juga kita akan menghilangkan kolom Customer ID dan gender karena kurang relevan untuk proses clustering. Selanjutnya kita akan menentukan nilai K yang optimal dengan metode Elbow. Library K-means dari SKLearn menyediakan fungsi untuk menghitung inersia dari K-Means dengan jumlah K tertentu. Di sini kita akan membuat list yang berisi inersia dari nilai K antara 1 sampai 11.

![3](https://github.com/brnabidin/Latihan-SKLearn-K-means/assets/67081096/26f1fd3e-d3c1-4f86-b229-b4d7d885fa47)

Jalankan kode di bawah untuk membuat plot inersia dari setiap nilai K. Sesuai plot di bawah, kita bisa melihat bahwa elbow berada di nilai K sama dengan 5, di mana penurunan inersia tidak lagi signifikan setelah nilai K sama dengan 5. Jangan lupa mengimpor library yang dibutuhkan untuk membuat plot ya.

![4](https://github.com/brnabidin/Latihan-SKLearn-K-means/assets/67081096/e712e73e-3f78-4fd8-9a1f-580f2a1531d3)

Hasil dari kode di atas menampilkan plot inersia sebagai berikut.

![202004302253449b67112da588a52a3656846e0c4d767e](https://github.com/brnabidin/Latihan-SKLearn-K-means/assets/67081096/98bb504d-d834-4166-a743-b2e0713e4f66)

Terakhir kita bisa melatih kembali K-Means dengan jumlah K yang didapat dari metode Elbow. Lalu kita bisa membuat plot hasil pengklasteran K-Means dengan menjalankan kode di bawah.

![5](https://github.com/brnabidin/Latihan-SKLearn-K-means/assets/67081096/5752d242-4d15-4ad4-802a-64108c01ed83)

Sehingga jika kode di atas dijalankan, maka tampilan KMeans dengan 5 klaster seperti di bawah ini.

![dos_2b9aa27c74c179f48d4f4d8f3358f60a20220510155404](https://github.com/brnabidin/Latihan-SKLearn-K-means/assets/67081096/a9dcd02e-af21-46a0-9147-e46a3f2130bb)
