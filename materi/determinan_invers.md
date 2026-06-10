# **Determinan dan Invers Matriks**

## **Pengertian Determinan Matriks**
Determinan adalah suatu nilai skalar (bilangan tunggal) yang diperoleh dari suatu matriks persegi. Determinan memberikan informasi penting mengenai sifat suatu matriks, seperti apakah matriks tersebut memiliki invers atau tidak.

Determinan biasanya dilambangkan dengan:

$$
\det(A)
$$

atau

$$
|A|
$$

dengan $A$ adalah matriks persegi.

---

## **Definisi Determinan Matriks**
Jika diberikan matriks persegi:

$$
A =
\begin{bmatrix}
a & b \\
c & d
\end{bmatrix}
$$

maka determinannya adalah:

$$
\det(A) = ad - bc
$$

Determinan hanya dapat dihitung pada matriks persegi, yaitu matriks yang jumlah baris dan kolomnya sama.

---

## **Fungsi Determinan Matriks**
Determinan memiliki beberapa fungsi penting, yaitu:
1. Menentukan apakah suatu matriks memiliki invers.
2. Menyelesaikan sistem persamaan linear.
3. Menentukan luas atau volume transformasi linear.
4. Digunakan dalam metode Cramer.
5. Digunakan pada perhitungan eigenvalue dan eigenvector.

---

## **Tujuan Mempelajari Determinan Matriks**
Tujuan mempelajari determinan adalah:
* Mengetahui sifat suatu matriks.
* Menentukan keberadaan invers matriks.
* Menyelesaikan sistem persamaan linear.
* Memahami transformasi geometris.

---

## **Syarat Matriks Memiliki Invers**
Suatu matriks memiliki invers jika:

$$
\det(A) \neq 0
$$

Jika:

$$
\det(A) = 0
$$

maka matriks disebut matriks singular dan tidak memiliki invers.

---

## **Determinan Matriks Ordo $2 \times 2$**

### **Rumus Determinan Matriks $2 \times 2$**
Misalkan:

$$
A =
\begin{bmatrix}
a & b \\
c & d
\end{bmatrix}
$$

maka:

$$
\det(A) = ad - bc
$$

### **Contoh Soal Determinan $2 \times 2$**
Diketahui:

$$
A =
\begin{bmatrix}
3 & 2 \\
1 & 4
\end{bmatrix}
$$

Tentukan determinannya.

#### **Penyelesaian**
Gunakan rumus:

$$
\det(A) = ad - bc
$$

Substitusi nilai:

$$
\det(A) = (3)(4) - (2)(1)
$$

$$
\det(A) = 12 - 2 = 10
$$

Jadi:

$$
\boxed{\det(A) = 10}
$$

---

## **Determinan Matriks Ordo $3 \times 3$**

### **Metode Aturan Sarrus**
Diberikan:

$$
A =
\begin{bmatrix}
a & b & c \\
d & e & f \\
g & h & i
\end{bmatrix}
$$

Maka:

$$
\det(A) = aei + bfg + cdh - ceg - bdi - afh
$$

### **Contoh Soal Determinan $3 \times 3$**
Diketahui:

$$
A =
\begin{bmatrix}
1 & 2 & 3 \\
0 & 4 & 5 \\
1 & 0 & 6
\end{bmatrix}
$$

Hitung determinannya.

#### **Penyelesaian**
Gunakan metode Sarrus:

$$
\det(A) = (1)(4)(6) + (2)(5)(1) + (3)(0)(0) - (3)(4)(1) - (2)(0)(6) - (1)(5)(0)
$$

$$
\det(A) = 24 + 10 + 0 - 12 - 0 - 0
$$

$$
\det(A) = 22
$$

Jadi:

$$
\boxed{\det(A) = 22}
$$

---

## **Pengertian Invers Matriks**
Invers matriks adalah matriks yang jika dikalikan dengan matriks asal menghasilkan matriks identitas.

Jika $A^{-1}$ adalah invers dari matriks $A$, maka:

$$
AA^{-1} = I
$$

atau

$$
A^{-1}A = I
$$

dengan:

$$
I =
\begin{bmatrix}
1 & 0 \\
0 & 1
\end{bmatrix}
$$

### **Definisi Invers Matriks**
Invers matriks merupakan kebalikan dari matriks yang digunakan untuk menyelesaikan berbagai permasalahan aljabar linear. Konsep invers matriks mirip dengan:

$$
a \times \frac{1}{a} = 1
$$

pada bilangan biasa.

### **Fungsi Invers Matriks**
Invers matriks digunakan untuk:
1. Menyelesaikan sistem persamaan linear.
2. Digunakan dalam kriptografi.
3. Digunakan dalam machine learning.
4. Digunakan pada transformasi geometris.
5. Digunakan dalam simulasi numerik.

### **Tujuan Mempelajari Invers Matriks**
Tujuan mempelajari invers matriks adalah:
* Menyelesaikan SPL secara efisien.
* Memahami transformasi linear.
* Mengembangkan metode numerik.

---

## **Rumus Invers Matriks $2 \times 2$**
Misalkan:

$$
A =
\begin{bmatrix}
a & b \\
c & d
\end{bmatrix}
$$

Maka:

$$
A^{-1} = \frac{1}{ad-bc}
\begin{bmatrix}
d & -b \\
-c & a
\end{bmatrix}
$$

dengan syarat:

$$
ad - bc \neq 0
$$

---

## **Contoh Soal Invers Matriks $2 \times 2$**
Diketahui:

$$
A =
\begin{bmatrix}
2 & 1 \\
3 & 4
\end{bmatrix}
$$

Tentukan invers matriks $A$.

### **Langkah 1: Hitung Determinan**
$$
\det(A) = (2)(4) - (1)(3)
$$

$$
\det(A) = 8 - 3 = 5
$$

### **Langkah 2: Gunakan Rumus Invers**
$$
A^{-1} = \frac{1}{5}
\begin{bmatrix}
4 & -1 \\
-3 & 2
\end{bmatrix}
$$

### **Langkah 3: Sederhanakan**
$$
A^{-1} =
\begin{bmatrix}
\frac{4}{5} & -\frac{1}{5} \\
-\frac{3}{5} & \frac{2}{5}
\end{bmatrix}
$$

Jadi:

$$
\boxed{
A^{-1} =
\begin{bmatrix}
\frac{4}{5} & -\frac{1}{5} \\
-\frac{3}{5} & \frac{2}{5}
\end{bmatrix}
}
$$

---

## **Verifikasi Invers Matriks**
Periksa:

$$
AA^{-1} =
\begin{bmatrix}
2 & 1 \\
3 & 4
\end{bmatrix}
\begin{bmatrix}
\frac{4}{5} & -\frac{1}{5} \\
-\frac{3}{5} & \frac{2}{5}
\end{bmatrix}
$$

Hasilnya:

$$
\begin{bmatrix}
1 & 0 \\
0 & 1
\end{bmatrix}
$$

yang merupakan matriks identitas.

---

## **Menyelesaikan SPL Menggunakan Invers Matriks**
Misalkan:

$$
AX = B
$$

Maka:

$$
X = A^{-1}B
$$

### **Contoh Soal SPL Menggunakan Invers**
Diketahui:

$$
\begin{cases}
2x + y = 5 \\
3x + 4y = 11
\end{cases}
$$

Bentuk matriks:

$$
A =
\begin{bmatrix}
2 & 1 \\
3 & 4
\end{bmatrix}
$$

$$
X =
\begin{bmatrix}
x \\
y
\end{bmatrix}
$$

$$
B =
\begin{bmatrix}
5 \\
11
\end{bmatrix}
$$

Gunakan:

$$
X = A^{-1}B
$$

dengan:

$$
A^{-1} =
\begin{bmatrix}
\frac{4}{5} & -\frac{1}{5} \\
-\frac{3}{5} & \frac{2}{5}
\end{bmatrix}
$$

Maka:

$$
X =
\begin{bmatrix}
\frac{4}{5} & -\frac{1}{5} \\
-\frac{3}{5} & \frac{2}{5}
\end{bmatrix}
\begin{bmatrix}
5 \\
11
\end{bmatrix}
$$

$$
X =
\begin{bmatrix}
\frac{20}{5} - \frac{11}{5} \\
-\frac{15}{5} + \frac{22}{5}
\end{bmatrix}
$$

$$
X =
\begin{bmatrix}
\frac{9}{5} \\
\frac{7}{5}
\end{bmatrix}
$$

Sehingga:

$$
\boxed{
x = \frac{9}{5}, \quad
y = \frac{7}{5}
}
$$

---

## **Perbedaan Determinan dan Invers Matriks**

| Determinan | Invers |
| :--- | :--- |
| Menghasilkan satu nilai skalar | Menghasilkan matriks baru |
| Hanya berupa skalar | Berupa matriks |
| Digunakan untuk mengecek keberadaan invers | Digunakan untuk menyelesaikan SPL |
| Dilambangkan dengan $\det(A)$ atau $\|A\|$ | Dilambangkan dengan $A^{-1}$ |

---

## **Kesimpulan**
Determinan adalah nilai skalar yang diperoleh dari suatu matriks persegi dan digunakan untuk mengetahui sifat-sifat matriks.
Invers matriks adalah kebalikan suatu matriks yang memenuhi $AA^{-1} = I$.
Suatu matriks hanya memiliki invers jika $\det(A) \neq 0$.

Determinan dan invers matriks merupakan konsep dasar yang sangat penting dalam Sistem Persamaan Linear, Aljabar Linear, Machine Learning, Analisis Numerik, Grafika Komputer, dan Data Science.
