# Music-Genre-Classification

Pengklasifikasian genre musik menggunakan Machine Learning

# Dataset
Dataset yang digunakan adalah GTZAN Dataset. Data ini didapatkan dari situs Kaggle. Dataset GTZAN yang terdiri dari 10 genre dengan total 1000 audio.
1. blues
2. classical
3. country
4. disco
5. hiphop
6. jazz
7.metal
8. pop
9. reggae
10.rock

![image](https://github.com/fadhilhemmings/Music-Genre-Classification/assets/87648911/307831ee-b325-4d99-94be-b9ef1282da31)

# Preprocessing
Pada proses ini menggunakan librosa untuk explore data audio, yang mana librosa merupakan sumber induk dari file audio. Selain menggunakan librosa juga menggunakan fourier transform untuk mendapatkan sinyal dalam domain sebagai input, menampilkan dekomposisi menjadi frekuensi, serta mengubah frekuensi menjadi skala log dan amplitudo menjadi desibel, yang mana divisualisasikan dalam bentuk spectrogram.
![image](https://github.com/fadhilhemmings/Music-Genre-Classification/assets/87648911/a0e2f7fa-398d-4df1-a537-2c16e69d4f2e)


# Modelling
Agar menghasilkan klasifikasi yang akurat maka diperlukan algoritma dengan hasil akurasi yang bagus. Berikut adalah beberapa perbandingan antar algoritmanya.

![image](https://github.com/fadhilhemmings/Music-Genre-Classification/assets/87648911/a6bae35f-d43b-4507-b1ec-d2fc9b467345)

Berdasarkan hasil diatas maka digunakanlah algoritma XGBoost karen memiliki tingkat akurasi yang paling tinggi. eXtreme Gradient Boosting (XGBoost) merupakan pengembangan algoritma Gradient Boosting Machine (GBM) dengan beberapa fitur tambahan yang berguna dalam mempercepat proses komputasi dan mencegah terjadinya overfitting. Kunci kecepatan komputasi XGBoost terletak pada optimasi penggunaan memori dan cache di komputer sehingga dapat bekerja secara efisien, meskipun berhadapan dengan data yang berukuran relatif besar.

#  Deployment
Pada tahap ini merupakan penggabungan antara pemrograman web dan python yang dihubungkan menggunakan framerowk flask dengan memanfaatkan platform anaconda sebagai server local. 

