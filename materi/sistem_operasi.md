# **Operasi Matriks**

## **Pengertian Matriks**

Matriks adalah susunan bilangan yang disusun dalam bentuk baris dan kolom serta dibatasi oleh tanda kurung atau kurung siku.

Secara umum, matriks berordo $m \times n$ ditulis sebagai:

$$
A =
\begin{bmatrix}
a_{11} & a_{12} & \cdots & a_{1n} \\
a_{21} & a_{22} & \cdots & a_{2n} \\
\vdots & \vdots & \ddots & \vdots \\
a_{m1} & a_{m2} & \cdots & a_{mn}
\end{bmatrix}
$$

dengan:
* $m$ = jumlah baris
* $n$ = jumlah kolom

---

## **Operasi Penjumlahan Matriks**

### **Pengertian Penjumlahan Matriks**
Penjumlahan matriks adalah operasi menjumlahkan elemen-elemen yang bersesuaian dari dua matriks yang memiliki ordo yang sama.

### **Definisi Penjumlahan Matriks**
Jika:

$$
A = [a_{ij}]
$$

dan

$$
B = [b_{ij}]
$$

maka:

$$
A + B = [a_{ij} + b_{ij}]
$$

### **Syarat Penjumlahan Matriks**
Dua matriks dapat dijumlahkan apabila memiliki ordo yang sama.

Misalnya:

$$
A_{2\times2} + B_{2\times2}
$$

diperbolehkan.

Sedangkan:

$$
A_{2\times2} + B_{3\times2}
$$

tidak dapat dilakukan.

### **Tujuan Penjumlahan Matriks**
Penjumlahan matriks digunakan untuk:
* Menggabungkan data numerik.
* Menjumlahkan transformasi linear.
* Digunakan dalam analisis statistik dan komputasi.

### **Contoh Penjumlahan Matriks**
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

Maka:

$$
A + B =
\begin{bmatrix}
1+5 & 2+6 \\
3+7 & 4+8
\end{bmatrix}
$$

$$
A + B =
\begin{bmatrix}
6 & 8 \\
10 & 12
\end{bmatrix}
$$

---

## **Operasi Pengurangan Matriks**

### **Pengertian Pengurangan Matriks**
Pengurangan matriks adalah operasi mengurangi elemen-elemen yang bersesuaian pada dua matriks yang memiliki ordo sama.

### **Definisi Pengurangan Matriks**
Jika:

$$
A = [a_{ij}]
$$

dan

$$
B = [b_{ij}]
$$

maka:

$$
A - B = [a_{ij} - b_{ij}]
$$

### **Tujuan Pengurangan Matriks**
Pengurangan matriks digunakan untuk:
* Menentukan selisih data.
* Mengukur perubahan suatu sistem.
* Digunakan dalam analisis numerik.

### **Contoh Pengurangan Matriks**
Diketahui:

$$
A =
\begin{bmatrix}
8 & 7 \\
6 & 5
\end{bmatrix}
$$

dan

$$
B =
\begin{bmatrix}
2 & 3 \\
1 & 4
\end{bmatrix}
$$

Maka:

$$
A - B =
\begin{bmatrix}
8-2 & 7-3 \\
6-1 & 5-4
\end{bmatrix}
$$

$$
A - B =
\begin{bmatrix}
6 & 4 \\
5 & 1
\end{bmatrix}
$$

---

## **Operasi Perkalian Matriks**

### **Pengertian Perkalian Matriks**
Perkalian matriks adalah operasi yang dilakukan dengan mengalikan baris pada matriks pertama dengan kolom pada matriks kedua.

### **Definisi Perkalian Matriks**
Jika:

$$
A_{m\times n}
$$

dan

$$
B_{n\times p}
$$

maka:

$$
AB = C_{m\times p}
$$

dengan:

$$
c_{ij} = \sum_{k=1}^{n} a_{ik}b_{kj}
$$

### **Syarat Perkalian Matriks**
Perkalian matriks dapat dilakukan jika:

$$
\text{Jumlah kolom } A = \text{Jumlah baris } B
$$

### **Tujuan Perkalian Matriks**
Perkalian matriks digunakan untuk:
* Transformasi geometri.
* Grafika komputer.
* Machine Learning.
* Sistem persamaan linear.
* Pemrosesan sinyal.

### **Contoh Perkalian Matriks**
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

Maka:

$$
AB =
\begin{bmatrix}
(1)(5)+(2)(7) & (1)(6)+(2)(8) \\
(3)(5)+(4)(7) & (3)(6)+(4)(8)
\end{bmatrix}
$$

$$
AB =
\begin{bmatrix}
19 & 22 \\
43 & 50
\end{bmatrix}
$$

---

## **Operasi Pembagian Matriks**

### **Pengertian Pembagian Matriks**
Dalam aljabar linear, pembagian matriks secara langsung tidak didefinisikan seperti pada bilangan biasa. Sebagai gantinya digunakan konsep invers matriks.

### **Definisi Pembagian Matriks**
Jika:

$$
A \div B
$$

maka dituliskan sebagai:

$$
AB^{-1}
$$

dengan syarat:

$$
\det(B) \neq 0
$$

### **Tujuan Pembagian Matriks**
Pembagian matriks digunakan untuk:
* Menyelesaikan sistem persamaan linear.
* Analisis transformasi linear.
* Komputasi numerik.

### **Contoh Pembagian Matriks**
Diketahui:

$$
A =
\begin{bmatrix}
4 & 2 \\
6 & 8
\end{bmatrix}
$$

dan

$$
B =
\begin{bmatrix}
1 & 0 \\
0 & 2
\end{bmatrix}
$$

Invers matriks $B$:

$$
B^{-1} =
\begin{bmatrix}
1 & 0 \\
0 & \frac{1}{2}
\end{bmatrix}
$$

Maka:

$$
A \div B = AB^{-1}
$$

$$
\begin{bmatrix}
4 & 2 \\
6 & 8
\end{bmatrix}
\begin{bmatrix}
1 & 0 \\
0 & \frac{1}{2}
\end{bmatrix}
$$

$$
\begin{bmatrix}
4 & 1 \\
6 & 4
\end{bmatrix}
$$

---

## **Perbedaan Operasi Matriks**

| Operasi | Syarat |
| :--- | :--- |
| **Penjumlahan** | Ordo harus sama |
| **Pengurangan** | Ordo harus sama |
| **Perkalian** | Kolom A = Baris B |
| **Pembagian** | Matriks pembagi harus memiliki invers |

---

## **Kesimpulan**
Operasi dasar matriks terdiri dari:
1. Penjumlahan matriks.
2. Pengurangan matriks.
3. Perkalian matriks.
4. Pembagian matriks melalui invers.

Operasi-operasi tersebut merupakan dasar dari berbagai bidang ilmu seperti Aljabar Linear, Data Science, Machine Learning, Grafika Komputer, Sistem Persamaan Linear, dan Analisis Numerik. Pemahaman operasi matriks menjadi langkah awal sebelum mempelajari determinan, invers matriks, eliminasi Gauss, dekomposisi LU, dan dekomposisi QR.
