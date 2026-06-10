# **Eliminasi Gaussian**

Eliminasi Gaussian adalah algoritma dalam aljabar linear untuk menyelesaikan sistem persamaan linear, menentukan pangkat matriks, atau mencari invers suatu matriks. Metode ini dinamai dari matematikawan Jerman, Carl Friedrich Gauss.

---

## **Langkah-Langkah Eliminasi Gaussian**

1. **Matriks Augmentasi**: Tuliskan sistem persamaan linear (SPL) dalam bentuk matriks augmented.

$$
[A \mid b]
$$

2. **Eliminasi Maju (Forward Elimination)**: Mengubah matriks augmented menjadi bentuk eselon baris (segitiga atas) menggunakan Operasi Baris Elementer (OBE).
3. **Substitusi Balik (Back Substitution)**: Menyelesaikan nilai-nilai variabel dari baris paling bawah ke atas.

---

## **Laporan Praktikum: Penyelesaian SPL dengan Eliminasi Gaussian**

### **BAB I: Pendahuluan**

#### **1.1 Latar Belakang**
Sistem Persamaan Linear (SPL) adalah kumpulan beberapa persamaan linear yang memiliki variabel yang sama dan diselesaikan secara bersamaan. Salah satu metode yang sistematis untuk menyelesaikan SPL adalah Eliminasi Gaussian, yaitu metode yang menggunakan Operasi Baris Elementer (OBE) untuk mengubah matriks menjadi bentuk segitiga atas, kemudian dilakukan substitusi balik.

#### **1.2 Tujuan**
* Memahami konsep SPL.
* Memahami langkah-langkah Eliminasi Gaussian.
* Menyelesaikan SPL 3 dan 4 variabel secara sistematis.

---

### **BAB II: Landasan Teori**

#### **2.1 Bentuk Umum SPL**
Bentuk umum SPL dalam bentuk matriks:

$$
Ax = b
$$

dengan:

$$
A \in \mathbb{R}^{m \times n}, \quad x \in \mathbb{R}^{n}, \quad b \in \mathbb{R}^{m}
$$

#### **2.2 Operasi Baris Elementer (OBE)**
Dalam Eliminasi Gaussian diperbolehkan:
* Menukar dua baris.
* Mengalikan baris dengan konstanta bukan nol.
* Menambahkan kelipatan suatu baris ke baris lain.

---

### **BAB III: Pembahasan**

#### **3.1 SPL Tiga Variabel**
Diketahui:

$$
\begin{cases}
2x + y - z = 8 \\
-3x - y + 2z = -11 \\
-2x + y + 2z = -3
\end{cases}
$$

**Langkah 1: Matriks Augmented**

$$
\left[
\begin{array}{ccc|c}
2 & 1 & -1 & 8 \\
-3 & -1 & 2 & -11 \\
-2 & 1 & 2 & -3
\end{array}
\right]
$$

**Langkah 2: Eliminasi Kolom Pertama**

$$
R_2 = R_2 + \frac{3}{2}R_1
$$

$$
R_3 = R_3 + R_1
$$

Hasil:

$$
\left[
\begin{array}{ccc|c}
2 & 1 & -1 & 8 \\
0 & \frac{1}{2} & \frac{1}{2} & 1 \\
0 & 2 & 1 & 5
\end{array}
\right]
$$

**Langkah 3: Eliminasi Kolom Kedua**

$$
R_3 = R_3 - 4R_2
$$

$$
\left[
\begin{array}{ccc|c}
2 & 1 & -1 & 8 \\
0 & \frac{1}{2} & \frac{1}{2} & 1 \\
0 & 0 & -1 & 1
\end{array}
\right]
$$

*Sudah berbentuk eselon baris (segitiga atas).*

**Substitusi Balik**
* **Baris 3**: 

$$
-z = 1 \Rightarrow z = -1
$$

* **Baris 2**: 

$$
0.5y + 0.5(-1) = 1
$$

$$
0.5y = 1.5 \Rightarrow y = 3
$$

* **Baris 1**:

$$
2x + y - z = 8
\Rightarrow
2x + 3 - (-1) = 8
$$

$$
2x + 4 = 8
\Rightarrow
2x = 4
\Rightarrow
x = 2
$$

**Solusi SPL 3 Variabel**

$$
x = 2,\qquad y = 3,\qquad z = -1
$$

#### **3.2 SPL Empat Variabel**
Diketahui:

```{math}
\begin{cases}
x + y + z + w = 10 \\
2x - y + z + w = 5 \\
3x + y - z + w = 12 \\
x + 2y + 3z - w = 7
\end{cases}
```

**Langkah 1: Matriks Augmented**

$$
\left[
\begin{array}{cccc|c}
1 & 1 & 1 & 1 & 10 \\
2 & -1 & 1 & 1 & 5 \\
3 & 1 & -1 & 1 & 12 \\
1 & 2 & 3 & -1 & 7
\end{array}
\right]
$$

**Langkah 2: Eliminasi Kolom Pertama**

$$
R_2 = R_2 - 2R_1
$$

$$
R_3 = R_3 - 3R_1
$$

$$
R_4 = R_4 - R_1
$$

Hasil:

$$
\left[
\begin{array}{cccc|c}
1 & 1 & 1 & 1 & 10 \\
0 & -3 & -1 & -1 & -15 \\
0 & -2 & -4 & -2 & -18 \\
0 & 1 & 2 & -2 & -3
\end{array}
\right]
$$

**Langkah 3: Eliminasi Kolom Kedua dan Ketiga**

Setelah dilakukan OBE lanjutan diperoleh bentuk eselon baris:

$$
\left[
\begin{array}{cccc|c}
1 & 1 & 1 & 1 & 10 \\
0 & -3 & -1 & -1 & -15 \\
0 & 0 & -\frac{10}{3} & -\frac{4}{3} & -8 \\
0 & 0 & 0 & -3 & -12
\end{array}
\right]
$$

**Substitusi Balik**
**Baris 4:**

$$
-3w = -12
\Rightarrow
w = 4
$$

**Baris 3:**

$$
-\frac{10}{3}z - \frac{4}{3}(4) = -8
$$

$$
-\frac{10}{3}z - \frac{16}{3} = -8
$$

$$
-\frac{10}{3}z = -8 + \frac{16}{3}
$$

$$
-\frac{10}{3}z = -\frac{24}{3} + \frac{16}{3}
$$

$$
-\frac{10}{3}z = -\frac{8}{3}
$$

$$
z = \frac{-8/3}{-10/3}
= \frac{8}{10}
= \frac{4}{5}
= 0.8
$$

**Baris 2:**

$$
-3y - z - w = -15
$$

Substitusikan nilai \(z = 0.8\) dan \(w = 4\):

$$
-3y - 0.8 - 4 = -15
$$

$$
-3y = -10.2
$$

$$
y = 3.4
$$

**Baris 1:**

$$
x + y + z + w = 10
$$

Substitusikan nilai \(y = 3.4\), \(z = 0.8\), dan \(w = 4\):

$$
x + 3.4 + 0.8 + 4 = 10
$$

$$
x + 8.2 = 10
$$

$$
x = 1.8
$$

### Hasil Akhir

$$
\boxed{
x = 1.8,\quad
y = 3.4,\quad
z = 0.8,\quad
w = 4
}
$$

**Solusi SPL 4 Variabel**

$$
x = 1,\qquad y = 2,\qquad z = 3,\qquad w = 4
$$

---

### **BAB IV: Kesimpulan**
* Eliminasi Gaussian menyelesaikan SPL dengan membentuk matriks eselon baris menggunakan serangkaian OBE.
* Setelah bentuk segitiga atas diperoleh, solusi variabel dicari secara runtut menggunakan metode substitusi balik.
* Kedua contoh sistem persamaan di atas memiliki solusi tunggal.

---

## Integrasi SageMath Interaktif

Diketahui SPL:

$$
\begin{cases}
x+y+z=6\\
2x-y+z=3\\
x+2y-z=3
\end{cases}
$$

Matriks augmented:

$$
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 6\\
2 & -1 & 1 & 3\\
1 & 2 & -1 & 3
\end{array}
\right]
$$

Lakukan operasi baris elementer:

$$
R_2 \leftarrow R_2 - 2R_1
$$

$$
R_3 \leftarrow R_3 - R_1
$$

Sehingga diperoleh:

$$
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 6\\
0 & -3 & -1 & -9\\
0 & 1 & -2 & -3
\end{array}
\right]
$$

### Implementasi SageMath

```python
A = matrix([[1, 1, 1, 6],
            [2, -1, 1, 3],
            [1, 2, -1, 3]])

# R2 <- R2 - 2R1
A.add_multiple_of_row(1, 0, -2)

# R3 <- R3 - R1
A.add_multiple_of_row(2, 0, -1)

print(A)
```

Output:

$$
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 6\\
0 & -3 & -1 & -9\\
0 & 1 & -2 & -3
\end{array}
\right]
$$

Lanjutkan eliminasi:

$$
R_3 \leftarrow R_3 + \frac{1}{3}R_2
$$

Sehingga:

$$
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 6\\
0 & -3 & -1 & -9\\
0 & 0 & -\frac{7}{3} & -6
\end{array}
\right]
$$

### SageMath Lengkap

```python
A = matrix([[1, 1, 1, 6],
            [2, -1, 1, 3],
            [1, 2, -1, 3]])

# Eliminasi kolom pertama
A.add_multiple_of_row(1, 0, -2)
A.add_multiple_of_row(2, 0, -1)

# Eliminasi kolom kedua
A.add_multiple_of_row(2, 1, 1/3)

print(A)
```

Dari baris ketiga:

$$
-\frac{7}{3}z=-6
$$

$$
z=\frac{18}{7}
$$

Substitusi ke baris kedua:

$$
-3y-z=-9
$$

$$
y=\frac{15}{7}
$$

Substitusi ke baris pertama:

$$
x+y+z=6
$$

$$
x=\frac{9}{7}
$$

### Solusi SPL

$$
\boxed{
x=\frac{9}{7},\quad
y=\frac{15}{7},\quad
z=\frac{18}{7}
}
$$
