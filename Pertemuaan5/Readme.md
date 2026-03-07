# Laporan Analisis Supervised Learning, Classification

## Domain Proyek
Membuat sebuah analisis tentang hasil percobaan mengenai Classification, Regresi, dan preprocessing dan mefokuskan bagian Classification sebagai inti pertemuan

### Latar Belakang
Dibuat sebagai percobaan untuk melakukan supervised learning pada machine learning dengan inti classification (pertemuan kali ini)

## Business Understanding
Sebuah analisis sederhana mengenai Classification dalam machine learning (supervised learning) dengan tambahan preprocessing dan regresi dua bagian supervised learning yang sangat importan untuk pelaksanaan supervised learning

### Problem Statements
Apa itu "Classification" dan bagaimanakah cara pengunaan dan apa gunanya?, lalu apa itu KNN (K-Nearest Neighbours) dan apa yang harus dilakukan untuk melakukan percobaan tersebut?

### Goals
Menyelesaikan percobaan sebagai sebuah bagian inti pembelajaran machine learning dan belajar lebih lagi mengenai material tersebut

### Solution Statements 
Dengan menggunakan google colab seperti biasa untuk menggunakan model Python 3.0 dan melaksanakan percobaan dengan seffektif mungkin, lalu menggunakan bantuan website blog.zulma sebagai panduan

# Data Understanding

  | Jenis                   | Keterangan                                                                              |
  | ----------------------- | --------------------------------------------------------------------------------------- |
  | Sumber                  | Seaborn Library |
  | Dataset Owner           | Khashayar Baghizadeh |
  | Lisensi                 | Open Knowledge |
  | Kategori                | Numerik |
  | Usability               | 75% |
  | Jenis dan Ukuran Berkas | CSV (83.88 KB) |

# Preprocessing, Regression, Classification

**Preprocessing** pada percobaan ini cukup sederhana, pertama kita melakukan cek untuk melihat missing value dan memasukan data set yang digunakan yaitu titanic ini lah kode yang digunakan :

import pandas as pd
import seaborn as sns

df = sns.load_dataset("titanic")

df.isnull().sum()

--------------------------------

Setelah itu saya melakukan drop pada semua data yang tidak akan digunakan / memilih fitur yang digunakan ini kodenya :

df = df[['survived','pclass','sex','age','fare']]
df = df.dropna()

--------------------------------

Lalu saya melakukan encoding pada data-data "sex" (secara jujur saya hanya pilih data tersebut karena data-data lain sudah dalam bentuk seharusnya) ini kodenya :

from sklearn.preprocessing import LabelEncoder

le = LabelEncoder()
df["sex"] = le.fit_transform(df["sex"])

--------------------------------

Terakhir saya melakukan train test split, ini kodenya :

from sklearn.model_selection import train_test_split

X = df.drop("survived", axis=1)
y = df["survived"]

X_train, X_test, y_train, y_test = train_test_split(
    X,
    y,
    test_size=0.2,
    random_state=42
)

--------------------------------

**Regresi** mulai susah tetapi ada lumayan banyak step yang mirip dengan yang ada di preprocessing, jadi saya mulai dengan mengimpor semua hal yang diperlukan lalu saya melakukan encoding lagi, memuat training model, dan melakukan train test split, setelah semua process persiapan sudah selesai saya memasukan model Linear Regression dan melakukan tes prediksi, setelah itu saya melihat jumlah MSE, RMSE, dan R2 Score 

Ini adalah nilai-nilainya :
MSE : 0.1372654178608207
RMSE : 0.3704934788371054
R2 Score : 0.4339612286127984

<br>
<image src='https://raw.githubusercontent.com/Dinozzonathanel/Binus-machine-learning/main/Pertemuan2/Images2/download(1).png' width= 500/>
<br>

Dan terakhir saya melihat coefficent dari pclass, sex, age, dan fare : 

Feature  Coefficient
0  pclass    -0.166684
1     sex    -0.505328
2     age    -0.003665
3    fare     0.000157

--------------------------------

**Classification** bagian inti dan terakhir dari percobaan ini, saya mulai dengan melakukan encoding, train test split, dan mempersiapkan model, setelah semua itu selesai saya mengimporkan dan menggunakan KNN (K-Nearest Neighbours), setelah itu saya melakukan cek untuk akurasi yang ternyata sebanyak 0.7988826815642458 atau 79% (sepertinya), lalu saya melihat TN, FN, FP, TP (True Negatives, False Negatives, False Positives, True Positives) inilah nilai-nilainya :

[[90 15]
 [21 53]]

--------------------------------

Setelah itu saya membuat sebuah classification report inilah hasilnya :

precision    recall  f1-score   support

           0       0.81      0.86      0.83       105
           1       0.78      0.72      0.75        74

    accuracy                           0.80       179
   macro avg       0.80      0.79      0.79       179
weighted avg       0.80      0.80      0.80       179

kelihatannya cukup aneh jadi saya tidak bisa membuat tabel rapih karena ke tidak rapihan tabel tersebut

--------------------------------

Terakhir adalah visualisasi/diagram yang telah dibuat mengenai TN, FN, FP, TP dari proses sebelumnya, ini adalah gambarnya :

<br>
<image src='https://raw.githubusercontent.com/Dinozzonathanel/Binus-machine-learning/main/Pertemuan2/Images2/download(2).png' width= 500/>
<br>

# Evaluasi

Jadi saya telah belajar lebih lagi tentang supervised learning dan kali ini intinya adalah classification, setelah melakukan percobaan tersebut saya telah membuat sebuah model yang cukup bagus dan sederhana, selain itu saya juga dapat melatih melakukan preprocessing dan regresi, walaupun susah saya telah menyelesaikan percobaan dengan cukup baik dan sederhana.
