# **Singular Value Decomposition (SVD)**

## **Pengertian Singular Value Decomposition (SVD)**

Singular Value Decomposition (SVD) adalah salah satu metode dekomposisi matriks yang paling penting dalam Aljabar Linear.

SVD digunakan untuk memecah sebuah matriks menjadi tiga matriks yang lebih sederhana sehingga lebih mudah dianalisis dan diolah.

Secara umum, jika diberikan matriks:

$$
A \in \mathbb{R}^{m \times n}
$$

maka matriks tersebut dapat didekomposisi menjadi:

$$
A = U\Sigma V^T
$$

dengan:

* (U) = matriks ortogonal kiri (left singular vectors)
* (\Sigma) = matriks diagonal yang berisi singular values
* (V^T) = transpose dari matriks ortogonal kanan

---

# **Definisi Singular Value Decomposition**

SVD merupakan proses faktorisasi matriks yang berlaku untuk semua matriks, baik:

* Matriks persegi
* Matriks persegi panjang
* Matriks singular
* Matriks non-singular

Berbeda dengan invers matriks atau dekomposisi LU yang memiliki syarat tertentu, SVD dapat diterapkan pada hampir semua matriks.

Bentuk umum:

$$
A = U\Sigma V^T
$$

dimana:

$$
U^TU=I
$$

dan

$$
V^TV=I
$$

yang menunjukkan bahwa (U) dan (V) merupakan matriks ortogonal.

---

# **Tujuan Singular Value Decomposition**

Tujuan utama SVD adalah:

1. Menyederhanakan representasi matriks.
2. Mengurangi dimensi data.
3. Mengekstraksi informasi penting dari data.
4. Menemukan struktur tersembunyi pada data.
5. Mempermudah komputasi numerik.

---

# **Fungsi Singular Value Decomposition**

## **1. Reduksi Dimensi (Dimensionality Reduction)**

SVD digunakan untuk mengurangi jumlah fitur pada data tanpa kehilangan terlalu banyak informasi.

Contoh:

* Machine Learning
* Data Mining
* Artificial Intelligence

---

## **2. Kompresi Data**

SVD digunakan untuk menyimpan data dalam ukuran yang lebih kecil.

Contoh:

* Kompresi gambar
* Kompresi video
* Kompresi dokumen

---

## **3. Sistem Rekomendasi**

Platform seperti:

* Netflix
* YouTube
* Spotify

menggunakan konsep yang berkaitan dengan SVD untuk menganalisis preferensi pengguna.

---

## **4. Pengolahan Citra Digital**

Pada citra digital, SVD digunakan untuk:

* Kompresi gambar
* Penghilangan noise
* Pengenalan wajah

---

## **5. Natural Language Processing (NLP)**

Digunakan dalam:

* Analisis dokumen
* Topic modeling
* Semantic analysis

---

# **Komponen-Komponen SVD**

## **1. Matriks U**

Matriks (U) berisi singular vector kiri.

Bentuk:

$$
U=
\begin{bmatrix}
u_1 & u_2 & \cdots & u_m
\end{bmatrix}
$$

Memenuhi:

$$
U^TU=I
$$

---

## **2. Matriks Sigma**

Matriks (\Sigma) adalah matriks diagonal.

Bentuk:

$$
\Sigma=
\begin{bmatrix}
\sigma_1 & 0 & \cdots & 0 \\
0 & \sigma_2 & \cdots & 0 \\
\vdots & \vdots & \ddots & \vdots \\
0 & 0 & \cdots & \sigma_r
\end{bmatrix}
$$

dengan:

$$
\sigma_1 \geq \sigma_2 \geq \cdots \geq \sigma_r \geq 0
$$

Nilai (\sigma_i) disebut singular values.

---

## **3. Matriks V**

Matriks (V) berisi singular vector kanan.

Memenuhi:

$$
V^TV=I
$$

Pada persamaan SVD digunakan:

$$
V^T
$$

karena lebih sesuai untuk perkalian matriks.

---

# **Hubungan SVD dengan Eigenvalue dan Eigenvector**

Inilah hubungan yang paling penting.

SVD dibangun dari eigenvalue dan eigenvector.

Pertama dihitung:

$$
A^TA
$$

Kemudian dicari:

$$
\det(A^TA-\lambda I)=0
$$

untuk memperoleh eigenvalue.

---

## **Hubungan Singular Value dan Eigenvalue**

Jika:

$$
\lambda_i
$$

adalah eigenvalue dari:

$$
A^TA
$$

maka singular value diperoleh dari:

$$
\sigma_i=\sqrt{\lambda_i}
$$

Ini merupakan hubungan utama antara:

* SVD
* Eigenvalue
* Eigenvector

---

# **Hubungan SVD dengan Matriks Transpose**

Pada SVD selalu muncul:

$$
V^T
$$

yang merupakan transpose dari matriks (V).

Selain itu, perhitungan SVD selalu melibatkan:

$$
A^TA
$$

dan

$$
AA^T
$$

yang keduanya menggunakan transpose matriks.

Oleh karena itu, pemahaman transpose sangat penting sebelum mempelajari SVD.

---

# **Hubungan SVD dengan Determinan**

Determinan digunakan untuk:

$$
\det(A-\lambda I)=0
$$

saat mencari eigenvalue.

Karena SVD dibangun dari eigenvalue, maka determinan menjadi salah satu konsep dasar yang mendukung SVD.

---

# **Hubungan SVD dengan Invers Matriks**

SVD dapat digunakan untuk menghitung pseudo-inverse.

Jika:

$$
A=U\Sigma V^T
$$

maka:

$$
A^+ = V\Sigma^+U^T
$$

dimana:

$$
A^+
$$

disebut Moore-Penrose Pseudoinverse.

Metode ini sangat berguna ketika:

* Matriks tidak memiliki invers
* Matriks tidak persegi
* Data berukuran besar

---

# **Hubungan SVD dengan Dekomposisi QR**

SVD dan QR sama-sama merupakan metode dekomposisi matriks.

QR:

$$
A=QR
$$

SVD:

$$
A=U\Sigma V^T
$$

Perbedaannya:

| QR                   | SVD                           |
| -------------------- | ----------------------------- |
| Lebih cepat          | Lebih kuat                    |
| Untuk SPL            | Untuk analisis data           |
| Tidak selalu optimal | Optimal untuk reduksi dimensi |

---

# **Contoh Soal SVD Sederhana**

Diketahui:

$$
A=
\begin{bmatrix}
3 & 0 \\
4 & 5
\end{bmatrix}
$$

Tentukan langkah awal SVD.

---

## **Langkah 1**

Hitung:

$$
A^T=
\begin{bmatrix}
3 & 4 \\
0 & 5
\end{bmatrix}
$$

---

## **Langkah 2**

Hitung:

$$
A^TA =
\begin{bmatrix}
3 & 4 \\
0 & 5
\end{bmatrix}
\begin{bmatrix}
3 & 0 \\
4 & 5
\end{bmatrix}
$$

---

## **Langkah 3**

Hasilnya:

$$
A^TA=
\begin{bmatrix}
25 & 20 \\
20 & 25
\end{bmatrix}
$$

---

## **Langkah 4**

Cari eigenvalue:

$$
\det(A^TA-\lambda I)=0
$$

---

## **Langkah 5**

Setelah diperoleh eigenvalue:

$$
\lambda_1
$$

dan

$$
\lambda_2
$$

maka singular value:

$$
\sigma_1=\sqrt{\lambda_1}
$$

$$
\sigma_2=\sqrt{\lambda_2}
$$

---

# **Implementasi SVD Menggunakan SageMath**

```python
A = matrix(RR,[
[3,0],
[4,5]
])

U,S,V = A.SVD()

print("Matriks U")
print(U)

print("Matriks Sigma")
print(S)

print("Matriks V")
print(V)
```

---

# **Penerapan SVD dalam Dunia Nyata**

## **Machine Learning**

Digunakan untuk:

* Feature Extraction
* Principal Component Analysis (PCA)
* Recommendation System

---

## **Computer Vision**

Digunakan untuk:

* Face Recognition
* Image Compression
* Object Detection

---

## **Natural Language Processing**

Digunakan untuk:

* Latent Semantic Analysis (LSA)
* Information Retrieval
* Text Mining

---

## **Data Science**

Digunakan untuk:

* Data Reduction
* Noise Removal
* Data Compression

---

# **Kesimpulan**

Singular Value Decomposition (SVD) adalah metode dekomposisi matriks yang sangat kuat dengan bentuk:

$$
A=U\Sigma V^T
$$

SVD memiliki hubungan erat dengan:

* Matriks Transpose
* Eigenvalue
* Eigenvector
* Determinan
* Invers Matriks
* Dekomposisi QR

Karena kemampuannya dalam reduksi dimensi, kompresi data, dan analisis data besar, SVD menjadi salah satu teknik paling penting dalam:

* Aljabar Linear
* Machine Learning
* Artificial Intelligence
* Data Science
* Computer Vision
* Natural Language Processing
