# Laporan Percobaan Decision Tree dan Random Forest (Titanic) - Dinozzo Nathanael Budiman

## Domain Proyek
Membuat sebuah analisis sederhana mengenai hasil dari percobaan decision tree dan random forest menggunakan dataset titanic yang disediakan sebelumnya

### Latar Belakang
Dilakukan sebagai percobaan setelah perjelasaan yang telah diberikan pada pertemuaan ke 6 dan dari apa yang pernah diklarifikasi pada pertemuaan sebelumnya

## Business Understanding 
Sebuah analisis sederhana mengenai Decision Tree dan Random Forest dalam machine learning (supervised learning) dan sebuah perbandingan keduanya

### Problem Statements
Apa itu decision tree dan random forest? Lalu bagaimana cara kerja keduanya? (Akurasi dan cara penggunaan juga menjadi pertanyaan)

### Goals
Untuk menghasilkan model yang cukup akurat dan belajar untuk mengerti mengenai decision tree dan random forest yang menjadi inti pertemuaan ke enam

### Solution Statements 
Sekali lagi menggunakan aplikasi google colab untuk menjalankan program yang akan membuat decision tree dan random forest serta dengan hasil visualisasinya, lalu penggunaan github sebagai tempat pembuatan laporan dan aplikasi yang digunakan untuk mengupload hasil kerja serta dengan website blog zulma yang digunakan sebagai panduan

# Data Understanding
  | Jenis                   | Keterangan                                                                              |
  | ----------------------- | --------------------------------------------------------------------------------------- |
  | Sumber                  | Seaborn Library |
  | Dataset Owner           | Khashayar Baghizadeh |
  | Lisensi                 | Open Knowledge |
  | Kategori                | Numerik |
  | Usability               | 75% |
  | Jenis dan Ukuran Berkas | CSV (83.88 KB) |

# Pembandingan

## Decision Tree

Decision Tree dibuat menggunakan kode ini : 

<br>
<image src='https://raw.githubusercontent.com/Dinozzonathanel/Binus-machine-learning/main/Pertemuan2/Images2/huh.png' width= 500/>
<br>

Tentu sebelum penggunaan kode tersebut saya perlu melakukan importan data set, encoding, pemilihan fungsi, dan train test split tetapi yang saya tunjukan diatas merupakan kode yang digunakan untuk decision tree, selanjutnya saya melakukan sebuah cek untuk akurasi model dan visualisasi decision tree ini adalah gambar keduanya : 

<br>
<image src='https://raw.githubusercontent.com/Dinozzonathanel/Binus-machine-learning/main/Pertemuan2/Images2/wha.png' width= 500/>
<br>

## Random Forest

Random Forest dibuat menggunakan kode ini : 

<br>
<image src='https://raw.githubusercontent.com/Dinozzonathanel/Binus-machine-learning/main/Pertemuan2/Images2/toilet.png' width= 500/>
<br>

Lalu seperti yang saya lakukan dengan decision tree saya melakukan tes akurasi dengan hasil 77 persen akurasi (yang decision tree hanya 75 persen)

## Importance

<br>
<image src='https://raw.githubusercontent.com/Dinozzonathanel/Binus-machine-learning/main/Pertemuan2/Images2/importan.png' width= 500/>
<br>

Ini adalah pengaruh setiap "variabel"/"Fungsi" dalam dataset titanic yang digunakan untuk membuat prediksi

## Perbandingan

Setelah analisis yang cepat saya sudah melihat beberapa hal yang menunjukan pemenang dari perbandingan ini, pertama setelah melihat hasil persentase akurasi kedua model saya lihat bahwa Random Forest 2 persesn lebih akurat, kenapa? sepertinya hal ini disebabkan oleh 1 hal sederhana yaitu bahwa random forest merupakan banyak decision tree jadi ya sudah pasti lebih bagus dari satu.

## Visualisasi Confusion Matrix

<br>
<image src='https://raw.githubusercontent.com/Dinozzonathanel/Binus-machine-learning/main/Pertemuan2/Images2/download(67).png' width= 500/>
<br>

# Evaluasi
Saya telah melakukan sebuah percobaan sederhana dan belajar cara pengunaan decision tree dan random forest, saya belajar Pro dan Kontra dari decision tree, penggunaan decision tree serta dengan artinya, random tree juga dijelaskan mengenai penggunaan dan arti, dan akhirnya saya juga membandingkan keduanya melalui percobaan ini.
