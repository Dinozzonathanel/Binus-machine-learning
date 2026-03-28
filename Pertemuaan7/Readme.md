# Laporan Hasil Evaluasi Model Prediksi Python (Titanic) - Dinozzo Nathanael Budiman

## Domain Proyek
Membuat sebuah analisis sederhana mengenai hasil dari evaluasi model decision tree yang telah saya buat menggunakan data set seaborn "Titanic" yang sudah dipersiapkan dan disediakan.

### Latar Belakang
Dilakukan sebagai latihan dan penyelesaian untuk materi Machine Learning untuk mengevaluasi hasil buatan model yang telah dibuat (dalam percobaan, model yang dievaluasi adalah decision tree dengan logistic regression). Banyak materi yang sudah pernah dipelajari digabungkan jadi satu untuk menyelesaikan evaluasi lengkap.

## Business Understanding 
Sebuah analisis sederhana mengenai evaluasi sebuah decision tree dalam materi machine learning (Supervised learning) sebagai bagian terakhir dari materi machine learning.

### Problem Statements
Walaupun saya telah belajar kebanyakan kode ini, bagaimanakah cara saya dapat melakukan sebuah evaluasi yang benar-benar lengkap dengan visualisasi, cross-validation, confusion matrix, accuracy, precision, dll.?

### Goals
Untuk menyelesaikan dan menghasilkan model sebaik mungkin dengan mengevaluasi dan membetulkan model yang sudah dibuat, lalu melihat dan memvisualisasikan hasil tes dan pelatihan model juga.

### Solution Statements
Seperti biasa, menggunakan aplikasi Google Colab untuk menjalankan program yang akan bukan hanya membuat decision tree, tetapi juga mengevaluasi model tersebut agar akurasi model bisa dilihat dan dibetulkan.

# Data Understanding 
  | Jenis                   | Keterangan                                                                              |
  | ----------------------- | --------------------------------------------------------------------------------------- |
  | Sumber                  | Seaborn Library |
  | Dataset Owner           | Khashayar Baghizadeh |
  | Lisensi                 | Open Knowledge |
  | Kategori                | Numerik |
  | Usability               | 75% |
  | Jenis dan Ukuran Berkas | CSV (83.88 KB) |

# Hasil Evaluasi

## Confusion Matrix
setelah melakukan impor dataset dan dibuatnya sebuah decision tree dan logistic regression saya mulai evaluasi dengan melakukan cek confusion matrix yang akan meliha true positif, false positif, true negative, dan false negative

Ini lah hasilnya dan visualisasinya :

[[68 19]
 [16 40]]

<br>
<image src='https://raw.githubusercontent.com/Dinozzonathanel/Binus-machine-learning/main/Pertemuan2/Images2/download89.png' width= 500/>
<br>

## Accuracy, Precision, Recall, F1 score
Setelah menyelesaikan confusion matrix saya langsung masuk kedalam bagian akurasi, presisi, recall, dan F1 score untuk melanjutkan evaluasi secara lengkap, bagian ini penting untuk melihat jika model saya cukup bagus atau tidak dan ini juga merupakan bagian sebelum classification report yang akan membantu mencari overfitting atau underfitting

Inilah hasilnya : 
Accuracy: 0.7552447552447552 (75%)
Precision: 0.6779661016949152 (67% wkwk)
Recall: 0.7142857142857143 (71%)
F1 Score: 0.6956521739130435 (69%)

## Classification Report 
Classification report adalah kumpulan keseluruhan hasil dari akurasi, presisi, dll, lalu karena itu classification report dapat membantu saya dalam melihat jika model saya memiliki overfitting ataupun underfitting

Inilah hasilnya : 

<br>
<image src='https://raw.githubusercontent.com/Dinozzonathanel/Binus-machine-learning/main/Pertemuan2/Images2/report.png' width= 500/>
<br>

## Cross Validation
Saya tidak punya komentar tentang ini, tetapi cross validation dilakukan untuk mempastikan dan membantu melawan masalah overfitting atau underfitting

Ini hasilnya :

<br>
<image src='https://raw.githubusercontent.com/Dinozzonathanel/Binus-machine-learning/main/Pertemuan2/Images2/rabbi.png' width= 500/>
<br>

# Evaluasi (tentang evaluasi)
Jadi setelah menyelesaikan ini saya belajar cara menggunakan banyak metode evaluasi baru dan akhirnya semua metode dan code yang digunakan untuk evaluasi pun dimasukan ke dalam program untuk melakukan evaluasi lengkap mengenai decision tree yang sudah dibuat, saya mendapatkan hasil bagus dengan akurasi training 0.82 (82%) dan akurasi test 0.76 (76%) yang menunjukan tidak ada overfitting ataupun underfitting.
