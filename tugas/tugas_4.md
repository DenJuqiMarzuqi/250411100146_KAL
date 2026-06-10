# **Tugas 4 : Determinan Matriks Menggunakan Ekspansi Baris (Ekspansi Kofaktor)**

## **Tujuan**

Pada tugas ini, determinan matriks akan dihitung menggunakan metode **ekspansi baris (Laplace Expansion)**.

Rumus umum ekspansi kofaktor adalah:

$$
\det(A) =
\sum_{k=1}^{n}
(-1)^{i+k}
a_{ik}
M_{ik}
$$

dengan:

$$
M_{ij} =
\det(A_{ij})
$$

dimana:

* $a_{ij}$ adalah elemen matriks pada baris ke-$i$ dan kolom ke-$j$
* $M_{ij}$ adalah minor dari elemen $a_{ij}$
* $A_{ij}$ adalah submatriks yang diperoleh dengan menghapus baris ke-$i$ dan kolom ke-$j$

---

# **Soal 1**

## **Diketahui**

$$
A=
\begin{bmatrix}
-7 & -5 \\
1 & 4
\end{bmatrix}
$$

---

## **Penyelesaian**

Untuk matriks ordo $2 \times 2$, determinan dihitung menggunakan rumus:

$$
\det(A) = ad-bc
$$

Substitusi nilai:

$$
\det(A) = (-7)(4)-(-5)(1)
$$

$$
= -28+5
$$

$$
= -23
$$

---

## **Jawaban**

$$
\boxed{
\det(A)=-23
}
$$

---

# **Soal 2**

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

## **Penyelesaian**

Gunakan ekspansi kofaktor pada baris pertama.

$$
\det(A) = 0M_{11} - 2M_{12} + (-3)M_{13}
$$

---

### **Menghitung Minor $M_{11}$**

Hilangkan baris pertama dan kolom pertama:

$$
M_{11} =
\begin{vmatrix}
-2 & -1 \\
0 & 1
\end{vmatrix}
$$

$$
= (-2)(1)-(-1)(0)
$$

$$
= -2
$$

Karena elemen pertama bernilai nol:

$$
0M_{11}=0
$$

---

### **Menghitung Minor $M_{12}$**

Hilangkan baris pertama dan kolom kedua:

$$
M_{12} =
\begin{vmatrix}
1 & -1 \\
0 & 1
\end{vmatrix}
$$

$$
= (1)(1)-(-1)(0)
$$

$$
= 1
$$

Kontribusi kofaktor:

$$
-2M_{12} = -2(1) = -2
$$

---

### **Menghitung Minor $M_{13}$**

Hilangkan baris pertama dan kolom ketiga:

$$
M_{13} =
\begin{vmatrix}
1 & -2 \\
0 & 0
\end{vmatrix}
$$

$$
= (1)(0)-(-2)(0)
$$

$$
= 0
$$

Kontribusi kofaktor:

$$
(-3)M_{13} = 0
$$

---

### **Menghitung Determinan**

$$
\det(A) = 0 - 2 + 0
$$

$$
= -2
$$

---

## **Jawaban**

$$
\boxed{
\det(A)=-2
}
$$

---

# **Soal 3**

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

## **Penyelesaian**

Untuk mempermudah perhitungan determinan, lakukan operasi baris elementer:

$$
R_2 \leftarrow R_2 + 3R_1
$$

$$
R_3 \leftarrow R_3 - R_1
$$

$$
R_4 \leftarrow R_4 - R_1
$$

Diperoleh:

$$
\begin{bmatrix}
1 & -3 & 1 & 1 \\
0 & -8 & 4 & 4 \\
0 & 4 & -4 & 0 \\
0 & 4 & 0 & -4
\end{bmatrix}
$$

Karena kolom pertama sekarang memiliki banyak nol, lakukan ekspansi pada kolom pertama.

$$
\det(A) =
1 \cdot
\begin{vmatrix}
-8 & 4 & 4 \\
4 & -4 & 0 \\
4 & 0 & -4
\end{vmatrix}
$$

---

### **Menghitung Determinan Matriks 3×3**

Gunakan ekspansi pada baris pertama:

$$
-8
\begin{vmatrix}
-4 & 0 \\
0 & -4
\end{vmatrix}
-
4
\begin{vmatrix}
4 & 0 \\
4 & -4
\end{vmatrix}
+
4
\begin{vmatrix}
4 & -4 \\
4 & 0
\end{vmatrix}
$$

---

### **Minor Pertama**

$$
\begin{vmatrix}
-4 & 0 \\
0 & -4
\end{vmatrix} =
16
$$

---

### **Minor Kedua**

$$
\begin{vmatrix}
4 & 0 \\
4 & -4
\end{vmatrix} =
-16
$$

---

### **Minor Ketiga**

$$
\begin{vmatrix}
4 & -4 \\
4 & 0
\end{vmatrix} =
16
$$

---

### **Substitusi**

$$
\det(A) = (-8)(16) - 4(-16) + 4(16)
$$

$$
= -128 + 64 + 64
$$

$$
= 0
$$

---

## **Jawaban**

$$
\boxed{
\det(A)=0
}
$$

---

# **Kesimpulan**

Dari hasil perhitungan diperoleh:

### **Soal 1**

$$
\boxed{
\det(A)=-23
}
$$

### **Soal 2**

$$
\boxed{
\det(A)=-2
}
$$

### **Soal 3**

$$
\boxed{
\det(A)=0
}
$$

Metode ekspansi kofaktor sangat efektif digunakan untuk matriks berukuran kecil hingga menengah. Untuk matriks yang lebih besar, biasanya digunakan metode eliminasi Gauss atau dekomposisi matriks agar perhitungan lebih efisien.
