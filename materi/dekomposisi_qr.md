# **Dekomposisi Matriks QR**

## **Pengertian Dekomposisi QR**

Dekomposisi QR adalah suatu teknik dalam aljabar linear yang digunakan untuk memfaktorkan sebuah matriks \(A\) menjadi hasil perkalian dua matriks, yaitu matriks ortogonal \(Q\) dan matriks segitiga atas \(R\).

Secara matematis:

$$
A = QR
$$

dengan:

- \(Q\) adalah matriks ortogonal.
- \(R\) adalah matriks segitiga atas (upper triangular matrix).

---

## **Definisi Dekomposisi QR**

Jika diberikan matriks:

$$
A \in \mathbb{R}^{m \times n}
$$

maka dekomposisi QR menghasilkan:

$$
A = QR
$$

dengan syarat:

$$
Q^TQ = I
$$

dimana:

- \(Q^T\) adalah transpose matriks \(Q\)
- \(I\) adalah matriks identitas

dan

$$
R=
\begin{bmatrix}
r_{11} & r_{12} & \cdots & r_{1n}\\
0 & r_{22} & \cdots & r_{2n}\\
0 & 0 & \ddots & \vdots\\
0 & 0 & \cdots & r_{nn}
\end{bmatrix}
$$

---

## **Tujuan Dekomposisi QR**

Dekomposisi QR digunakan untuk:

1. Menyelesaikan Sistem Persamaan Linear (SPL)
2. Menghitung Least Squares Problem
3. Menentukan Eigenvalue
4. Digunakan pada Machine Learning
5. Digunakan dalam Analisis Numerik

---

## **Fungsi Dekomposisi QR**

### **1. Menyelesaikan SPL**

Jika:

$$
Ax=b
$$

dan

$$
A=QR
$$

maka:

$$
QRx=b
$$

Karena \(Q\) ortogonal:

$$
Rx=Q^Tb
$$

Sehingga penyelesaian menjadi lebih mudah.

---

### **2. Mengurangi Kompleksitas Perhitungan**

Dekomposisi QR membuat operasi matriks menjadi lebih stabil dibanding eliminasi Gauss biasa.

---

### **3. Digunakan dalam Machine Learning**

Pada regresi linear:

$$
Ax \approx b
$$

QR digunakan untuk mencari solusi terbaik dengan metode Least Squares.

---

## **Metode Gram-Schmidt**

Metode Gram-Schmidt adalah metode yang paling umum digunakan untuk memperoleh matriks \(Q\).

Misalkan kolom-kolom matriks \(A\) adalah:

$$
A=
\begin{bmatrix}
a_1 & a_2 & \cdots & a_n
\end{bmatrix}
$$

Langkah pertama:

$$
u_1=a_1
$$

$$
q_1=\frac{u_1}{||u_1||}
$$

Langkah kedua:

$$
u_2=a_2-\operatorname{proj}_{u_1}(a_2)
$$

dengan

$$
\operatorname{proj}_{u_1}(a_2)
=
\frac{a_2^Tu_1}{u_1^Tu_1}u_1
$$

Kemudian:

$$
q_2=\frac{u_2}{||u_2||}
$$

Proses dilanjutkan hingga seluruh vektor menjadi ortogonal.

---

# **Contoh Soal Dekomposisi QR Matriks 4×4**

## **Diketahui Matriks**

$$
A=
\begin{bmatrix}
1 & 1 & 0 & 0\\
1 & 0 & 1 & 0\\
0 & 1 & 1 & 1\\
0 & 0 & 1 & 1
\end{bmatrix}
$$

Tentukan dekomposisi QR dari matriks tersebut.

---

## **Langkah 1: Bentuk Matriks Q**

Dengan proses Gram-Schmidt diperoleh:

$$
Q=
\begin{bmatrix}
0.7071 & 0.4082 & -0.2887 & -0.5000\\
0.7071 & -0.4082 & 0.2887 & 0.5000\\
0 & 0.8165 & 0.2887 & -0.5000\\
0 & 0 & 0.8660 & 0.5000
\end{bmatrix}
$$

---

## **Langkah 2: Bentuk Matriks R**

Matriks \(R\) diperoleh dari:

$$
R=Q^TA
$$

hasilnya:

$$
R=
\begin{bmatrix}
1.4142 & 0.7071 & 0.7071 & 0\\
0 & 1.2247 & 0.4082 & 0.8165\\
0 & 0 & 1.1547 & 1.1547\\
0 & 0 & 0 & 0.5000
\end{bmatrix}
$$

---

## **Verifikasi**

Periksa:

$$
A=QR
$$

$$
QR=
\begin{bmatrix}
1 & 1 & 0 & 0\\
1 & 0 & 1 & 0\\
0 & 1 & 1 & 1\\
0 & 0 & 1 & 1
\end{bmatrix}
=A
$$

Sehingga dekomposisi QR benar.

## **Implementasi Menggunakan SageMath**

### **Membuat Matriks 4×4**

```python
A = matrix([
    [1,1,0,0],
    [1,0,1,0],
    [0,1,1,1],
    [0,0,1,1]
])

A
```

### **Melakukan Dekomposisi QR**

```python
A = matrix(RR,[
    [1,1,0,0],
    [1,0,1,0],
    [0,1,1,1],
    [0,0,1,1]
])

Q,R = A.QR()

print("Matriks Q:")
print(Q)

print("\nMatriks R:")
print(R)
```

### **Verifikasi Hasil**

```python
Q*R
```

Output yang diperoleh akan sama dengan matriks awal $A$.

---

## **Kelebihan Dekomposisi QR**
1. Stabil secara numerik.
2. Cocok untuk matriks berukuran besar.
3. Banyak digunakan dalam Machine Learning.
4. Digunakan pada algoritma pencarian eigenvalue.
5. Lebih akurat dibanding eliminasi Gauss pada beberapa kasus.

---

## **Kesimpulan**
Dekomposisi QR adalah metode pemfaktoran matriks:

$$
A = QR
$$

dimana:

$$
Q^TQ = I
$$

dan $R$ merupakan matriks segitiga atas.

Metode ini banyak digunakan dalam Sistem Persamaan Linear, Least Squares, Machine Learning, Analisis Numerik, dan Perhitungan Eigenvalue, sehingga menjadi salah satu teknik paling penting dalam aljabar linear modern.