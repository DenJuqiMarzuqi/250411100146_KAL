# **Tugas 2 : Transformasi Matriks**

## **Tujuan Tugas**

Pada tugas ini mahasiswa diminta memahami konsep transformasi matriks dan pengaruhnya terhadap titik atau objek pada bidang koordinat.

Mahasiswa diharapkan mampu:

1. Memahami konsep transformasi linear.
2. Menentukan matriks transformasi.
3. Melakukan transformasi terhadap titik atau vektor.
4. Menganalisis hasil transformasi.
5. Mengimplementasikan transformasi menggunakan perkalian matriks.

---

# **Pengertian Transformasi Matriks**

Transformasi matriks adalah proses mengubah posisi, ukuran, bentuk, atau orientasi suatu objek menggunakan operasi perkalian matriks.

Secara umum:

$$
T(\mathbf{x})=A\mathbf{x}
$$

dimana:

* (T) = transformasi
* (A) = matriks transformasi
* (\mathbf{x}) = vektor awal

---

# **Bentuk Umum Transformasi**

Jika:

$$
A=
\begin{bmatrix}
a & b\
c & d
\end{bmatrix}
$$

dan

$$
\mathbf{x}
==========

\begin{bmatrix}
x\
y
\end{bmatrix}
$$

maka:

$$
A\mathbf{x}
===========

\begin{bmatrix}
a & b\
c & d
\end{bmatrix}
\begin{bmatrix}
x\
y
\end{bmatrix}
=============

\begin{bmatrix}
ax+by\
cx+dy
\end{bmatrix}
$$

---

# **Soal 1: Transformasi Dilatasi (Scaling)**

## **Diketahui**

Titik:

$$
P=
\begin{bmatrix}
2\
3
\end{bmatrix}
$$

Matriks dilatasi:

$$
A=
\begin{bmatrix}
2 & 0\
0 & 2
\end{bmatrix}
$$

Tentukan hasil transformasi titik (P).

---

## **Penyelesaian**

Gunakan:

$$
P'=AP
$$

$$
P'
==

\begin{bmatrix}
2 & 0\
0 & 2
\end{bmatrix}
\begin{bmatrix}
2\
3
\end{bmatrix}
$$

# $$

\begin{bmatrix}
4\
6
\end{bmatrix}
$$

---

## **Jawaban**

$$
\boxed{
P'
==

\begin{bmatrix}
4\
6
\end{bmatrix}
}
$$

---

# **Soal 2: Transformasi Refleksi terhadap Sumbu-X**

## **Diketahui**

Titik:

$$
P=
\begin{bmatrix}
4\
2
\end{bmatrix}
$$

Matriks refleksi terhadap sumbu-X:

$$
R_x=
\begin{bmatrix}
1 & 0\
0 & -1
\end{bmatrix}
$$

Tentukan hasil transformasi.

---

## **Penyelesaian**

$$
P'
==

R_xP
$$

# $$

\begin{bmatrix}
1 & 0\
0 & -1
\end{bmatrix}
\begin{bmatrix}
4\
2
\end{bmatrix}
$$

# $$

\begin{bmatrix}
4\
-2
\end{bmatrix}
$$

---

## **Jawaban**

$$
\boxed{
P'
==

\begin{bmatrix}
4\
-2
\end{bmatrix}
}
$$

---

# **Soal 3: Transformasi Rotasi 90° Berlawanan Arah Jarum Jam**

## **Diketahui**

Titik:

$$
P=
\begin{bmatrix}
1\
2
\end{bmatrix}
$$

Matriks rotasi:

$$
R=
\begin{bmatrix}
0 & -1\
1 & 0
\end{bmatrix}
$$

Tentukan hasil transformasi.

---

## **Penyelesaian**

$$
P'
==

RP
$$

# $$

\begin{bmatrix}
0 & -1\
1 & 0
\end{bmatrix}
\begin{bmatrix}
1\
2
\end{bmatrix}
$$

# $$

\begin{bmatrix}
-2\
1
\end{bmatrix}
$$

---

## **Jawaban**

$$
\boxed{
P'
==

\begin{bmatrix}
-2\
1
\end{bmatrix}
}
$$

---

# **Soal 4: Transformasi Shear Horizontal**

## **Diketahui**

Titik:

$$
P=
\begin{bmatrix}
2\
1
\end{bmatrix}
$$

Matriks shear:

$$
S=
\begin{bmatrix}
1 & 2\
0 & 1
\end{bmatrix}
$$

Tentukan hasil transformasi.

---

## **Penyelesaian**

$$
P'
==

SP
$$

# $$

\begin{bmatrix}
1 & 2\
0 & 1
\end{bmatrix}
\begin{bmatrix}
2\
1
\end{bmatrix}
$$

# $$

\begin{bmatrix}
4\
1
\end{bmatrix}
$$

---

## **Jawaban**

$$
\boxed{
P'
==

\begin{bmatrix}
4\
1
\end{bmatrix}
}
$$

---

# **Tabel Matriks Transformasi Dasar**

## **1. Dilatasi**

$$
\begin{bmatrix}
k & 0\
0 & k
\end{bmatrix}
$$

---

## **2. Refleksi terhadap Sumbu-X**

$$
\begin{bmatrix}
1 & 0\
0 & -1
\end{bmatrix}
$$

---

## **3. Refleksi terhadap Sumbu-Y**

$$
\begin{bmatrix}
-1 & 0\
0 & 1
\end{bmatrix}
$$

---

## **4. Rotasi Sudut (\theta)**

$$
\begin{bmatrix}
\cos\theta & -\sin\theta\
\sin\theta & \cos\theta
\end{bmatrix}
$$

---

## **5. Shear Horizontal**

$$
\begin{bmatrix}
1 & k\
0 & 1
\end{bmatrix}
$$

---

## **6. Shear Vertikal**

$$
\begin{bmatrix}
1 & 0\
k & 1
\end{bmatrix}
$$

---

# **Implementasi Menggunakan SageMath**

## **Dilatasi**

```python
A = matrix([[2,0],
            [0,2]])

P = vector([2,3])

A*P
```

---

## **Refleksi Sumbu-X**

```python
A = matrix([[1,0],
            [0,-1]])

P = vector([4,2])

A*P
```

---

## **Rotasi 90 Derajat**

```python
A = matrix([[0,-1],
            [1,0]])

P = vector([1,2])

A*P
```

---

# **Kesimpulan**

Transformasi matriks digunakan untuk mengubah posisi, ukuran, bentuk, maupun orientasi suatu objek.

Transformasi dasar yang sering digunakan adalah:

1. Dilatasi (Scaling)
2. Refleksi (Reflection)
3. Rotasi (Rotation)
4. Shear

Semua transformasi tersebut dapat direpresentasikan menggunakan perkalian matriks:

$$
T(\mathbf{x})=A\mathbf{x}
$$

Konsep transformasi matriks menjadi dasar dalam:

* Grafika Komputer
* Computer Vision
* Robotika
* Machine Learning
* Pengolahan Citra Digital
* Geometri Transformasi
