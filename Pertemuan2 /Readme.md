# Laporan analisis data "Titanic" - Dinozzo Nathanael Budiman

## Domain Proyek
Membuat sebuah analisis tentang data korban Titanic yang telah disediakan sebagai latihan untuk pembuatan laporan dalam kursus dan pelajaran Machine Learning

### Latar Belakang
Dibuat untuk melatih pembuatan laporan dan menganalisis data menggunakan Exploratory Data Analysis/EDA dan visualisasi data

## Business Understanding
Analisis yang cukup sederhana yang dibuat untuk melihat data yang tersedia, mencari fitur serta dengan penggunaan EDA, dll

### Problem Statements 
Bagaimana cara menvisualisasikan data dan menggunakan EDA dalam menganalisasi data korban titanic yang telah disediakan sebelumnya

## Goals
Bisa belajar lebih lagi tentang analisasi data (merupakan EDA pada pertemuan ini), dan untuk mempelajari dan menanalisasi data titanic yang telah disediakan

## Solution Statements
Dengan menggunakan kode yang disediakan dalam bahasa programming Python dan menggunakan website google colab, saya dapat melakukan sebuah analisasi penuh

# Data Understanding

  | Jenis                   | Keterangan                                                                              |
  | ----------------------- | --------------------------------------------------------------------------------------- |
  | Sumber                  | Seaborn Library |
  | Dataset Owner           | Khashayar Baghizadeh |
  | Lisensi                 | Open Knowledge |
  | Kategori                | Numerik |
  | Usability               | 75% |
  | Jenis dan Ukuran Berkas | CSV (83.88 KB) |

  ## Detail penjelasan dari dalam dataset :

  **Jumlah Baris dan Kolom**
  Ada sebanyak 891 baris dan 15 kolom

  **Bentuk data**
  Bentuk data dari dataset tersebut bervariasi, ini adalah bentuk data yang digunakan serta dengan banyak kali bentuk tersebut digunakan :
  dtypes: bool(2), category(2), float64(2), int64(4), object(5)

**Histogram**

<br>
<image src='https://raw.githubusercontent.com/Dinozzonathanel/Binus-machine-learning/main/Pertemuan2/Images/Histogram2.png' width= 500/>
<br>

Ini diatas merupakan distribusi umur setiap penumpang pada titanic ^^

**Boxplot**

<br>
<image src='https://raw.githubusercontent.com/Dinozzonathanel/Binus-machine-learning/main/Pertemuan2/Images/Boxplot2.png' width= 500/>
<br>

Ini merupakan outlier yang telah dideteksi pada data umur/usia di dalam data set "titanic" ^^

**Heatmap Korelasi**

<br>
<image src='https://raw.githubusercontent.com/Dinozzonathanel/Binus-machine-learning/main/Pertemuan2/Images/Heatmap2.png' width= 500/>
<br>

Ini merupakan hubungan antar fitur-fitur numerik di dalam data tersebut ^^

**Deskripsi data**

| Keterangan |   survived	  |  pclass	   |  age	      |  sibsp	   |    parch	  |    fare    |
|------------|--------------|------------|------------|------------|------------|------------|       
| count	     |   891.000000 | 891.000000 | 714.000000 |	891.000000 | 891.000000 |	891.000000 |
| mean	     |   0.383838 	| 2.308642	 | 29.699118	|  0.523008	 | 0.381594	  | 32.204208  |
| std	       |   0.486592	  | 0.836071	 | 14.526497	|  1.102743	 | 0.806057	  | 49.693429  |
| min	       |   0.000000	  | 1.000000	 | 0.420000	  |  0.000000	 | 0.000000	  | 0.000000   |
| 25%	       |   0.000000	  | 2.000000	 | 20.125000	|  0.000000	 | 0.000000	  | 7.910400   |
| 50%	       |   0.000000	  | 3.000000	 | 28.000000	|  0.000000	 | 0.000000	  | 14.454200  |
| 75%	       |   1.000000	  | 3.000000	 | 38.000000	|  1.000000	 | 0.000000	  | 31.000000  |
| max	       |   1.000000	  | 3.000000	 | 80.000000	|  8.000000	 | 6.000000	  | 512.329200 |

## Evaluasi

Jadi dari analisis ini saya telah belajar beberapa hal baru dengan penggunaan dan pembuatan laporan seperti cara untuk memasukan gambar, tabel, dll, lalu saya juga dapat menganalisis sebuah data set yang menarik tentang korban dari tragedi titanic, jadi saya telah belajar lebih lagi tentang materi analisis data yang akan digunakan dalam pembelajaran machine learning dan telah belajar lebih lagi tentang kejadiaan titanic
