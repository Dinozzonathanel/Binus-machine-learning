# Laporan Analisis Supervised Learning, Dataset Tips (Seaborn) : Dinozzo Nathanael Budiman

## Domain Proyek
Analisa mengenai supervised learning dalam bidang classification sebagai intinya, lalu EDA dan Preprocessing masih merupakan bagian dari percobaan karena kedua hal tersebut adalah bagian penting dalam supervised learning, analisis dilaksanakan dengan dataset "tips" dari seaborn

### Latar Belakang
Dilakukan sebagai percobaan extra untuk memperlatih saya untuk membuat model yang dapat melakukan classification dalam supervised learning

## Business Understanding
Analisis sederhana yang dilakukan dengan percobaan membuat model yang dapat melakukan classification dan dengan tambahan EDA dan preprocessing

### Problem Statements
Bagaimana cara untuk melakukan classification dengan dataset baru yang telah saya temukan?, bagaimmana cara untuk melakukan preprocessing dan EDA dalam supervised learning

### Goals
Menyelesaikan percobaan dan mendapatkan hasil yang diharapkan, sebuah model akurat dan sederhana, lalu juga untuk melatih saya dalam melakukan classification

### Solution Statements
Menggunakan website Google Colab untuk membuat model, menggunakan Kaggle untuk mencari dataset ("Tips"), menggunakan github untuk membuat laporan, dan menggunakan website blog.zulma sebagai panduan

# Data Understanding
  | Jenis                   | Keterangan                                                                              |
  | ----------------------- | --------------------------------------------------------------------------------------- |
  | Sumber                  | Seaborn Library |
  | Dataset Owner           | Joe Young |
  | Lisensi                 | M (1995) Practical Data Analysis: Case Studies in Business Statistics |
  | Kategori                | Numerik |
  | Usability               | 100% |
  | Jenis dan Ukuran Berkas | CSV (7.94 kB) |

# EDA, Preprocessing, Classification

**EDA** adalah bagian pertama dan paling mudah dalam percobaan ini, EDA dilakukan untuk melihat diagram tentang data dalam bentuk histoplot, boxplot, dan heatmap
Ini adalah kode yang digunakan : 
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt

df = sns.load_dataset("tips")

-------------------------------

sns.histplot(df["tip"].dropna())
plt.show()

sns.boxplot(x=df["tip"])
plt.show()

sns.heatmap(df.corr(numeric_only=True), annot=True)
plt.show()

-------------------------------

Ini adalah hasil diagram : 

<br>
<image src='https://raw.githubusercontent.com/Dinozzonathanel/Binus-machine-learning/main/Pertemuan2/Images2/one.png' width= 500/>
<br>

<br>
<image src='https://raw.githubusercontent.com/Dinozzonathanel/Binus-machine-learning/main/Pertemuan2/Images2/two.png' width= 500/>
<br>

<br>
<image src='https://raw.githubusercontent.com/Dinozzonathanel/Binus-machine-learning/main/Pertemuan2/Images2/three.png' width= 500/>
<br>
-------------------------------
  
**Preprocessing** merupakan step yang sangat penting dalam supervised learning dan dalam percobaan ini saya telah membuat versi sederhana, satu melakukan cek untuk missing value, satu menghapus fungsi yang tidak digunakan, satu melakukan encoding, satu melakukan train test split , jadi iya menurut ku kali ini cukup sederhana

<br>
<image src='https://raw.githubusercontent.com/Dinozzonathanel/Binus-machine-learning/main/Pertemuan2/Images2/skibidi.png' width= 688/>
<br>
-------------------------------
  
**Classification** merupakan bagian terakhir, dimana saya akhirnya membuat program prediksi untuk data "smoker"

Saya mulai dengan melakukan train test split, lalu membuat logistic regression dan memasukan KNN (K-Nearest Neighbour), dan setelah itu saya melakukan cek akurasi dan melihat nilai-nilai TN, FN, FP, TP, terakhir saya membuat prediction report dan sebuah visualisasi TN, FN, FP, TP

inilah hasil visualisasi tersebut : 

<br>
<image src='https://raw.githubusercontent.com/Dinozzonathanel/Binus-machine-learning/main/Pertemuan2/Images2/classified.png' width= 500/>
<br>
-------------------------------

# Evaluasi
Jadi iya saya telah melatih diri ku sendiri untuk melakukan supervised learning dalam bidang classification, EDA, dan preprocessing, dari itu saya dapat melanjutkan pelajaranku di dalam materi supervised learning dan maju ke step selanjutnya.
