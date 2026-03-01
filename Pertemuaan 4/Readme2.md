# Laporan Analisis Supervised Learning, Regresi dengan data "Top 50 Cryptocurrency" - Dinozzo Nathanael Budiman

## Domain Proyek 
Melakukan sebuah analisis tentang regresi pada data set "Top 50 Cryptocurrency" untuk memahami lebih lagi tentang regresi di dalam machine learning

### Latar Belakang 
Sebagai percobaan melakukan Supervised learning (regression), Preprocessing, dan EDA meggunakan data yang ditemukan dari kaggle melainkan data yang diberikan di Blog.Zulma

## Business Understanding
Analisis sederhana yang dilakukan untuk memahami lebih lagi tentang Supervised learning (regression), melakukan preprocessing untuk regresi, dan EDA untuk melihat data sebelum penggunaan

### Problem Statements
Bagimana saya dapat melakukan Supervised Learning, Preprocessing, dan EDA dengan lengkap dan benar

### Goals
Belajar lebih lagi mengenai materi Machine learning dan yang difokuskan sekarang merupakan Supervised Learning (Regresi) dengan cara menggunakan data "Top 50 Cryptocurrency" yang disediakan (Preprocessing dan EDA juga termasukan)

### Solution Statements
Menggunakan Kaggle untuk mencari data, menggunakan google collab untuk menjalani kode dan untuk mengimpor data, dan menggunakan github untuk mengupload hasil dan laporan

# Data Understanding

 | Jenis                   | Keterangan                                                                              |
  | ----------------------- | --------------------------------------------------------------------------------------- |
  | Sumber                  | Kaggle |
  | Dataset Owner           | Kaushal Nandaniya |
  | Lisensi                 | CC BY-SA 4.0 |
  | Kategori                | Numerik |
  | Usability               | 100% |
  | Jenis dan Ukuran Berkas | CSV (13.83 MB) |

# Aftermath Understanding

### Imports
Jadi sebelum memulai semua hal lain, saya harus memasukan importan yang diperlukan untuk melaksanakan percobaan dengan efesien, inilah importan yang digunakan :

import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
import seaborn as sns

from sklearn.model_selection import train_test_split
from sklearn.linear_model import LinearRegression
from sklearn.metrics import mean_squared_error, r2_score
from sklearn.preprocessing import StandardScaler, LabelEncoder
import matplotlib.pyplot as plt

Lalu ada beberapa kode tambahan yang digunakan untuk mengimpor data dan memastikan kode-kode berupa float

column_names = ['Crypto_Symbol', 'Date', 'Open', 'High', 'Low', 'Close', 'Adj Close', 'Volume']
data = pd.read_csv('crypto50_combined.csv', names=column_names, header=None)

for col in ['Open', 'High', 'Low', 'Close']:
    data[col] = pd.to_numeric(data[col], errors='coerce')

data.columns = data.columns.str.strip()

data = data.dropna(subset=['Open', 'High', 'Low', 'Close'])

X = data[['Open', 'High', 'Low']]
y = data['Close']

print(f"Shape of data after cleaning: {data.shape}")

Bagian terakhir ^^^ digunakan untuk mengcek 

### 


  
