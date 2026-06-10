# **Matriks Transpose**

## **Pengertian Matriks Transpose**
Transpose matriks adalah suatu operasi pada matriks yang dilakukan dengan menukar posisi baris menjadi kolom dan kolom menjadi baris.

Dengan kata lain, setiap elemen pada baris ke-$i$ dan kolom ke-$j$ akan berpindah menjadi elemen pada baris ke-$j$ dan kolom ke-$i$.

Transpose matriks merupakan salah satu operasi dasar dalam aljabar linear yang banyak digunakan dalam berbagai bidang matematika, statistika, machine learning, dan komputasi numerik.

---

## **Definisi Matriks Transpose**
Jika diberikan matriks:

$$
A = [a_{ij}]
$$

maka transpose dari matriks $A$ ditulis sebagai:

$$
A^T
$$

dengan definisi:

$$
(A^T)_{ij} = A_{ji}
$$

Artinya, indeks baris dan kolom saling ditukar.

---

## **Notasi Matriks Transpose**
Transpose matriks biasanya dinotasikan sebagai:

$$
A^T
$$

atau

$$
\text{Transpose}(A)
$$

Contoh:

Jika:

$$
A =
\begin{bmatrix}
1 & 2 & 3 \\
4 & 5 & 6
\end{bmatrix}
$$

maka:

$$
A^T =
\begin{bmatrix}
1 & 4 \\
2 & 5 \\
3 & 6
\end{bmatrix}
$$

---

## **Tujuan Mempelajari Matriks Transpose**
Tujuan mempelajari transpose matriks antara lain:
1. Memahami transformasi bentuk matriks.
2. Digunakan dalam operasi perkalian matriks.
3. Digunakan pada dekomposisi matriks.
4. Digunakan dalam machine learning dan data science.
5. Digunakan dalam perhitungan sistem persamaan linear.

---

## **Fungsi Matriks Transpose**

### **1. Membentuk Matriks Simetris**
Suatu matriks dikatakan simetris jika:

$$
A = A^T
$$

Contoh:

$$
A =
\begin{bmatrix}
1 & 2 & 3 \\
2 & 4 & 5 \\
3 & 5 & 6
\end{bmatrix}
$$

Karena:

$$
A = A^T
$$

maka matriks tersebut adalah matriks simetris.

---

### **2. Digunakan dalam Dekomposisi QR**
Pada dekomposisi QR berlaku:

$$
Q^TQ = I
$$

dengan:
* $Q^T$ adalah transpose matriks $Q$
* $I$ adalah matriks identitas

---

### **3. Digunakan dalam Machine Learning**
Pada regresi linear digunakan persamaan:

$$
X^TX
$$

yang melibatkan transpose matriks data.

---

### **4. Digunakan dalam Perhitungan Vektor**
Perkalian titik (dot product) dapat ditulis sebagai:

$$
x^Ty
$$

---

## **Cara Menentukan Matriks Transpose**

### **Langkah-Langkah**
1. Ambil setiap baris matriks.
2. Ubah menjadi kolom.
3. Ambil setiap kolom matriks.
4. Ubah menjadi baris.

---

## **Contoh Transpose Matriks $2 \times 2$**
Diketahui:

$$
A =
\begin{bmatrix}
1 & 2 \\
3 & 4
\end{bmatrix}
$$

Transpose matriksnya adalah:

$$
A^T =
\begin{bmatrix}
1 & 3 \\
2 & 4
\end{bmatrix}
$$

---

## **Contoh Transpose Matriks $2 \times 3$**
Diketahui:

$$
A =
\begin{bmatrix}
1 & 2 & 3 \\
4 & 5 & 6
\end{bmatrix}
$$

Transpose matriksnya:

$$
A^T =
\begin{bmatrix}
1 & 4 \\
2 & 5 \\
3 & 6
\end{bmatrix}
$$

Perhatikan bahwa:

$$
A_{2\times3} \rightarrow A^T_{3\times2}
$$

---

## **Contoh Transpose Matriks $3 \times 3$**
Diketahui:

$$
A =
\begin{bmatrix}
1 & 2 & 3 \\
4 & 5 & 6 \\
7 & 8 & 9
\end{bmatrix}
$$

Maka:

$$
A^T =
\begin{bmatrix}
1 & 4 & 7 \\
2 & 5 & 8 \\
3 & 6 & 9
\end{bmatrix}
$$

---

## **Sifat-Sifat Matriks Transpose**

### **1. Transpose dari Transpose**
Jika suatu matriks ditranspose dua kali:

$$
(A^T)^T = A
$$

---

### **2. Transpose Penjumlahan Matriks**
$$
(A+B)^T = A^T + B^T
$$

---

### **3. Transpose Pengurangan Matriks**
$$
(A-B)^T = A^T - B^T
$$

---

### **4. Transpose Perkalian Skalar**
Jika $k$ adalah skalar:

$$
(kA)^T = kA^T
$$

---

### **5. Transpose Perkalian Matriks**
Jika $A_{m\times n}$ dan $B_{n\times p}$ maka:

$$
(AB)^T = B^TA^T
$$

Perhatikan bahwa urutan matriks dibalik.

---

## **Contoh Soal Sifat Transpose**
Diketahui:

$$
A =
\begin{bmatrix}
1 & 2 \\
3 & 4
\end{bmatrix}
$$

dan

$$
B =
\begin{bmatrix}
5 & 6 \\
7 & 8
\end{bmatrix}
$$

Tentukan:

$$
(A+B)^T
$$

### **Penyelesaian**
Hitung terlebih dahulu:

$$
A+B =
\begin{bmatrix}
6 & 8 \\
10 & 12
\end{bmatrix}
$$

Kemudian:

$$
(A+B)^T =
\begin{bmatrix}
6 & 10 \\
8 & 12
\end{bmatrix}
$$

---

## **Hubungan Matriks Transpose dan Matriks Simetris**

### **Definisi Matriks Simetris**
Suatu matriks disebut simetris jika:

$$
A = A^T
$$

Contoh:

$$
A =
\begin{bmatrix}
2 & 3 & 1 \\
3 & 5 & 4 \\
1 & 4 & 6
\end{bmatrix}
$$

Karena:

$$
A = A^T
$$

maka matriks tersebut simetris.

---

## **Hubungan Matriks Transpose dan Matriks Antisimetris**

### **Definisi Matriks Antisimetris**
Suatu matriks disebut antisimetris jika:

$$
A^T = -A
$$

Contoh:

$$
A =
\begin{bmatrix}
0 & 2 & -1 \\
-2 & 0 & 3 \\
1 & -3 & 0
\end{bmatrix}
$$

Karena:

$$
A^T = -A
$$

maka matriks tersebut merupakan matriks antisimetris.

---

## **Penerapan Matriks Transpose**
Transpose matriks digunakan dalam:
1. Sistem Persamaan Linear.
2. Machine Learning.
3. Deep Learning.
4. Analisis Data.
5. Pengolahan Citra Digital.
6. Grafika Komputer.
7. Dekomposisi QR.
8. Eigenvalue dan Eigenvector.

---

## **Contoh Soal Lengkap**
Diketahui:

$$
A =
\begin{bmatrix}
2 & 4 & 6 \\
1 & 3 & 5
\end{bmatrix}
$$

Tentukan transpose dari matriks tersebut.

### **Penyelesaian**
Tukar setiap baris menjadi kolom:

Baris pertama: $[2 \quad 4 \quad 6]$ menjadi kolom pertama.

Baris kedua: $[1 \quad 3 \quad 5]$ menjadi kolom kedua.

Sehingga:

$$
A^T =
\begin{bmatrix}
2 & 1 \\
4 & 3 \\
6 & 5
\end{bmatrix}
$$

---

## **Kesimpulan**
Transpose matriks adalah operasi menukar baris menjadi kolom dan kolom menjadi baris.

Jika:

$$
A = [a_{ij}]
$$

maka:

$$
(A^T)_{ij} = A_{ji}
$$

Transpose memiliki banyak kegunaan dalam Aljabar Linear, Sistem Persamaan Linear, Machine Learning, Data Science, Dekomposisi Matriks, dan Analisis Numerik, dan menjadi salah satu operasi dasar yang harus dipahami sebelum mempelajari invers matriks, dekomposisi QR, eigenvalue, dan transformasi linear.
