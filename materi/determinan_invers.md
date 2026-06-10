# **Determinan dan Invers Matriks**

## **Menghitung Determinan**

Misalkan terdapat matriks persegi $A$:
$$
A = [a_{ij}]_{n \times n}
$$

### **Matriks $1 \times 1$**
Jika ukuran matriks persegi hanya $1 \times 1$, nilai determinannya adalah elemen tunggal dari matriks tersebut:
$$
\det(A) = a_{11}
$$

### **Matriks $n \times n$ ($n \geq 2$)**
Untuk matriks berukuran $2 \times 2$ atau lebih besar, kita dapat menggunakan metode ekspansi kofaktor (misalnya pada baris pertama):
$$
\det(A) = \sum_{j=1}^{n} (-1)^{1+j} \, a_{1j} \, \det(A_{1j})
$$

*Keterangan: $A_{1j}$ adalah submatriks sisa setelah baris ke-1 dan kolom ke-$j$ dihapus dari matriks utama $A$.*

---

## **Menyelesaikan SPL $4 \times 4$ dengan Matriks Invers**

Diberikan sebuah Sistem Persamaan Linear (SPL) dalam bentuk representasi matriks:
$$
\begin{bmatrix} 
1 & 1 & 1 & 1 \\ 
2 & -1 & 1 & -1 \\ 
1 & 2 & -1 & 1 \\ 
3 & -1 & 2 & 1 
\end{bmatrix} 
\begin{bmatrix} 
x_1 \\ 
x_2 \\ 
x_3 \\ 
x_4 
\end{bmatrix} = \begin{bmatrix} 
10 \\ 
-1 \\ 
6 \\ 
11 
\end{bmatrix}
$$

Penyelesaian SPL ini dapat dicari dengan menggunakan hubungan rumus invers:
$$
AX = B \Rightarrow X = A^{-1}B
$$

Kita dapat menghitung matriks invers $A^{-1}$ menggunakan metode adjoin atau operasi baris dasar untuk menghasilkan solusi nilai variabel $X$.

---

## **Visualisasi Interaktif (GeoGebra)**

[Ini Geogebra isi sendiri]

---

## **Kesimpulan**
Determinan dan invers matriks adalah alat krusial untuk menganalisis sifat-sifat matriks persegi dan mencari penyelesaian dari sistem persamaan linear secara langsung. Jika determinan suatu matriks bernilai nol ($\det(A) = 0$), maka matriks tersebut tidak memiliki invers (matriks singular).
