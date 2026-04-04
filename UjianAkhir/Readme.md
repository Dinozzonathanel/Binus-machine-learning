# Laporan Analisis Model Supervised Learning (Praktikum Lengkap) - Dinozzo Nathanael Budiman

## Domain Proyek
Membuat sebuah model supervised learning dengan semua bagian lengkap dari pembelajaran-pembelajaran sebelumnya mengenai supervised learning, proyek memiliki inti pembuatan model, evaluasi model (lengkap), dan validasi silang, untuk membuat model prediksi saya menggunakan metode yang telah diajari oleh kak Azhar Rizki Zulma yaitu yaitu decision tree.

### Latar Belakang 
Proyek ini dibuat sebagai penutup dan ujian terakhir dari kursus machine learning binus center Bintaro, saya di biarkan untuk membuat sebuah model dalam google colab dan membuat sebuah laporan sebelum memasukan hasil dari pembuatan ku kedalam github untuk diserahkan melalui Gmail dan Whatsapp

## Business Understanding
Pembuatan sebuah model dalam kursus machine learning binus sebagai ujian akhir dari kursus tersebut, saya diberikan instruksi untuk membuat sebuah model lengkap dengan evaluasi serta dengan validasi silang untuk di analisis dan di evaluasikan lagi di dalam laporan.

### Problem Statements 
Bagaimanakah cara saya dapat membuat model prediksi yang lengkap menggunakan evaluasi lengkap, decision tree, validasi silang, dan lain-lain.

### Goals
Menyelesaikan dan menghasilkan model yang cukup bagus untuk dianalisis dengan evaluasi lengkap dan menggunakan validasi silang untuk menghindari over fitting dan under fitting dalam model tersebut, selain itu saya juga ingin untuk mendapatkan nilai yang tinggi dan menyelasaikan kursus machine learning dengan lengkap dan dengan pengetahuan yang diperlukan untuk melanjutkan pembelajaranku dalam programming sebagai seorang murid.

### Solution Statements
Menggunakan website google colab untuk menjalankan program yang digunakan untuk pembuatan model serta dengan evaluasinya dan lain-lain, lalu dengan menggunakan github saya mengupload hasil dari percobaan dan membuat sebuah laporan sebelum mengirim hasil melalui Whatsapp dan Email

# Data Understanding

  | Jenis                   | Keterangan                                                                              |
  | ----------------------- | --------------------------------------------------------------------------------------- |
  | Sumber                  | Kaggle, Seaborn |
  | Dataset Owner           | Pascal |
  | Lisensi                 | N/A |
  | Kategori                | Numerik |
  | Usability               | 50% |
  | Jenis dan Ukuran Berkas | CSV (3.86 KB) |

# Percobaan

## Pembuatan model

### Preprocessing
Seperti semua percobaan yang saya pernah lakukan sebelumnya, saya awali pembuatan model dengan melakukan impor dataset serta dengan fungsi-fungsi yang akan digunakan dalam pembuatan model, setelah semua itu diimpor secara sukes saya mulai dengan melakukan encoding pada semua bagian dari dataset untuk menghindari adanya desimal pada dataset sebelum dimasukan kedalam program untuk membuat model prediksi dengan seharusnya, selanjutnya saya mulai melanjutkan dengan melakukan train test split.

### Pembuatan Model
Dengan itu saya memulai pembuatan model, pertama saya menyetelkan fungsi decision tree untuk membuat prediksi :

from sklearn.tree import DecisionTreeClassifier

tree = DecisionTreeClassifier(
    max_depth=4,
    random_state=42
)

tree.fit(X_train, y_train)

y_pred = tree.predict(X_test)

Lalu saya melakukan logistic regression, sebelum masuk ke dalam evaluasi

### Evaluasi Model
Saya mulai mengevaluasikan model saya dengan membuat confusion matrix dan melihat True Positive, False Positive, True Negative, dan False Negative, setelah mendapatkan hasilnya yaitu:

[[41  0]
 [ 0 14]]

Setelah melakukan itu saya melihat Accuracy, Percision, Recall Score, F1 Score yang semua hasilnya 1.0, setelah itu semua selesai saya akhirnya membuat tabel classification report :

### Training
              precision    recall  f1-score   support

           0       1.00      1.00      1.00       131
           1       1.00      1.00      1.00        86

    accuracy                           1.00       217
   macro avg       1.00      1.00      1.00       217
weighted avg       1.00      1.00      1.00       217

### Test
              precision    recall  f1-score   support

           0       1.00      1.00      1.00        41
           1       1.00      1.00      1.00        14

    accuracy                           1.00        55
   macro avg       1.00      1.00      1.00        55
weighted avg       1.00      1.00      1.00        55

<br>
<image src='https://raw.githubusercontent.com/Dinozzonathanel/Binus-machine-learning/main/Pertemuan2/Images2/evaluation.jpg' width= 500/>
<br>

<br>
<image src='https://raw.githubusercontent.com/Dinozzonathanel/Binus-machine-learning/main/Pertemuan2/Images2/visual.png' width= 500/>
<br>

### Validasi Silang (Cross Fitting)
Terakhir saya melakukan cross fitting, saya menggunakan program tersebut untuk menbulatkan hasil dari "score" semua nilai-nilai seperti akurasi, persisi, dll, dan dari itu hasilnya adalah :

Scores: [1. 1. 1. 1. 1.]
Mean Accuracy: 1.0

dan terakhir saya melakukan program:

from sklearn.model_selection import StratifiedKFold

skf = StratifiedKFold(n_splits=5)

### Pembandingan
Jadi setelah melihat kedua model yaitu model Training dan Test, mereka berdoa rata-rata sama dan akurat dan sepertinya hanya support yang berbeda tetapi saya tidak tau jika itu memengaruhi apapun, secara logika jika lebih besar supportnya juga lebih bagus berarti model Training lebih bagus, tetapi masih saja keduanya rata-rata cukup bagus.

Tetapi karena itu saya merasa ada terjadinya overfitting pada kedua model karena banyak atau kurangnya data pada dataset.


# Evaluasi (Laporan)
Saya merasa cukup baik dengan hasilku, tetapi menurut saya sepertinya karena banyak data (Atau kurangnya) model mengalami overfitting, model terlihat akurat dan memiliki persisi tinggi dan saya telah membuat laporan lengkap yang dari pandangan ku bagus, saya senang dapat belajar dan membuat percobaan ini mengetahui bahwa ini mungkin merupakan tugas terakhir dari kursus ini, tetapi dengan itu saya akan mencoba untuk belajar lebih lagi sebagai seorang murid, Terimakasih sudah membaca.
