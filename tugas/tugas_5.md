# **Tugas 5 : Invers Matriks Menggunakan Metode Adjoin**

## **Rumus yang Digunakan**

Matriks adjoin diperoleh dari:

$$
(\operatorname{adj}A)_{ij} =
(-1)^{i+j}M_{ji}
$$

dan invers matriks diperoleh dari:

$$
A^{-1} =
\frac{1}{\det(A)}
\operatorname{adj}(A)
$$

---

# **Soal 4**

## **Diketahui**

$$
A=
\begin{bmatrix}
-7 & -5 \\
1 & 4
\end{bmatrix}
$$

---

## **Langkah 1: Menghitung Determinan**

$$
\det(A) =
(-7)(4)-(-5)(1)
$$

$$
= -28+5
$$

$$
= -23
$$

---

## **Langkah 2: Membentuk Matriks Kofaktor**

Untuk matriks:

$$
A=
\begin{bmatrix}
a & b \\
c & d
\end{bmatrix}
$$

adjoinnya adalah:

$$
\operatorname{adj}(A) =
\begin{bmatrix}
d & -b \\
-c & a
\end{bmatrix}
$$

Sehingga:

$$
\operatorname{adj}(A) =
\begin{bmatrix}
4 & 5 \\
-1 & -7
\end{bmatrix}
$$

---

## **Langkah 3: Menghitung Invers**

$$
A^{-1} =
\frac{1}{-23}
\begin{bmatrix}
4 & 5 \\
-1 & -7
\end{bmatrix}
$$

$$
=
\begin{bmatrix}
-\frac{4}{23} & -\frac{5}{23} \\
\frac{1}{23} & \frac{7}{23}
\end{bmatrix}
$$

---

## **Jawaban**

$$
\boxed{
A^{-1} =
\begin{bmatrix}
-\frac{4}{23} & -\frac{5}{23} \\
\frac{1}{23} & \frac{7}{23}
\end{bmatrix}
}
$$

---

# **Soal 5**

## **Diketahui**

$$
A=
\begin{bmatrix}
0 & 2 & -3 \\
1 & -2 & -1 \\
0 & 0 & 1
\end{bmatrix}
$$

---

## **Langkah 1: Menghitung Determinan**

Dari soal sebelumnya telah diperoleh:

$$
\det(A)=-2
$$

Karena:

$$
\det(A)\neq0
$$

maka matriks memiliki invers.

---

## **Langkah 2: Menentukan Matriks Kofaktor**

Hitung setiap minor dan kofaktor.

### Kofaktor Baris 1

$$
C_{11} =
\begin{vmatrix}
-2 & -1 \\
0 & 1
\end{vmatrix}
= -2
$$

$$
C_{12} =
-\begin{vmatrix}
1 & -1 \\
0 & 1
\end{vmatrix}
= -1
$$

$$
C_{13} =
\begin{vmatrix}
1 & -2 \\
0 & 0
\end{vmatrix}
= 0
$$

---

### Kofaktor Baris 2

$$
C_{21} =
-\begin{vmatrix}
2 & -3 \\
0 & 1
\end{vmatrix}
= -2
$$

$$
C_{22} =
\begin{vmatrix}
0 & -3 \\
0 & 1
\end{vmatrix}
= 0
$$

$$
C_{23} =
-\begin{vmatrix}
0 & 2 \\
0 & 0
\end{vmatrix}
= 0
$$

---

### Kofaktor Baris 3

$$
C_{31} =
\begin{vmatrix}
2 & -3 \\
-2 & -1
\end{vmatrix}
= -8
$$

$$
C_{32} =
-\begin{vmatrix}
0 & -3 \\
1 & -1
\end{vmatrix}
= -3
$$

$$
C_{33} =
\begin{vmatrix}
0 & 2 \\
1 & -2
\end{vmatrix}
= -2
$$

---

## **Langkah 3: Matriks Kofaktor**

$$
C=
\begin{bmatrix}
-2 & -1 & 0 \\
-2 & 0 & 0 \\
-8 & -3 & -2
\end{bmatrix}
$$

---

## **Langkah 4: Matriks Adjoin**

Transpose matriks kofaktor:

$$
\operatorname{adj}(A) = C^T =
\begin{bmatrix}
-2 & -2 & -8 \\
-1 & 0 & -3 \\
0 & 0 & -2
\end{bmatrix}
$$

---

## **Langkah 5: Menghitung Invers**

$$
A^{-1} =
\frac{1}{-2}
\begin{bmatrix}
-2 & -2 & -8 \\
-1 & 0 & -3 \\
0 & 0 & -2
\end{bmatrix}
$$

$$
=
\begin{bmatrix}
1 & 1 & 4 \\
\frac{1}{2} & 0 & \frac{3}{2} \\
0 & 0 & 1
\end{bmatrix}
$$

---

## **Jawaban**

$$
\boxed{
A^{-1} =
\begin{bmatrix}
1 & 1 & 4 \\
\frac{1}{2} & 0 & \frac{3}{2} \\
0 & 0 & 1
\end{bmatrix}
}
$$

---

# **Soal 6**

## **Diketahui**

$$
A=
\begin{bmatrix}
1 & -3 & 1 & 1 \\
-3 & 1 & 1 & 1 \\
1 & 1 & -3 & 1 \\
1 & 1 & 1 & -3
\end{bmatrix}
$$

---

## **Langkah 1: Menghitung Determinan**

Dari soal sebelumnya telah diperoleh:

$$
\det(A)=0
$$

---

## **Langkah 2: Menentukan Keberadaan Invers**

Syarat matriks memiliki invers adalah:

$$
\det(A)\neq0
$$

Namun:

$$
\det(A)=0
$$

Sehingga matriks merupakan matriks singular.

---

## **Kesimpulan**

Karena:

$$
\det(A)=0
$$

maka:

$$
A^{-1} \text{ tidak ada}
$$

atau

$$
\boxed{
A^{-1}\text{ tidak terdefinisi}
}
$$

---

# **Ringkasan Jawaban**

### Soal 4

$$
\boxed{
A^{-1} =
\begin{bmatrix}
-\frac{4}{23} & -\frac{5}{23} \\
\frac{1}{23} & \frac{7}{23}
\end{bmatrix}
}
$$

### Soal 5

$$
\boxed{
A^{-1} =
\begin{bmatrix}
1 & 1 & 4 \\
\frac{1}{2} & 0 & \frac{3}{2} \\
0 & 0 & 1
\end{bmatrix}
}
$$

### Soal 6

$$
\boxed{
A^{-1} \text{ tidak ada}
}
$$
