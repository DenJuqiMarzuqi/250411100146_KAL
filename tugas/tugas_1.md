# **Tugas Eliminasi Menggunakan Metode Gauss (Gaussian Elimination)**

## **Tujuan Tugas**

Pada tugas ini mahasiswa diminta menyelesaikan Sistem Persamaan Linear (SPL) menggunakan metode Eliminasi Gauss. Setiap soal harus diselesaikan dengan:

1. Menuliskan sistem persamaan linear.
2. Mengubah ke bentuk matriks augmented.
3. Melakukan operasi baris elementer hingga bentuk eselon baris.
4. Melakukan substitusi balik (back substitution).
5. Menentukan solusi akhir.

---

# **Soal 1: SPL Dua Variabel**

## **Diketahui**

$$
\begin{cases}
x+y=5\
2x-y=1
\end{cases}
$$

---

## **Langkah 1: Bentuk Matriks Augmented**

$$
\left[
\begin{array}{cc|c}
1 & 1 & 5\
2 & -1 & 1
\end{array}
\right]
$$

---

## **Langkah 2: Eliminasi**

Lakukan operasi:

$$
R_2 \leftarrow R_2 - 2R_1
$$

$$
\left[
\begin{array}{cc|c}
1 & 1 & 5\
0 & -3 & -9
\end{array}
\right]
$$

---

## **Langkah 3: Substitusi Balik**

Baris kedua:

$$
-3y=-9
$$

$$
y=3
$$

Substitusi ke persamaan pertama:

$$
x+y=5
$$

$$
x+3=5
$$

$$
x=2
$$

---

## **Jawaban**

$$
\boxed{
x=2,\quad y=3
}
$$

---

# **Soal 2: SPL Tiga Variabel**

## **Diketahui**

$$
\begin{cases}
x+y+z=6\
2x-y+z=3\
x+2y-z=3
\end{cases}
$$

---

## **Langkah 1: Matriks Augmented**

$$
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 6\
2 & -1 & 1 & 3\
1 & 2 & -1 & 3
\end{array}
\right]
$$

---

## **Langkah 2: Eliminasi Kolom Pertama**

$$
R_2 \leftarrow R_2 - 2R_1
$$

$$
R_3 \leftarrow R_3 - R_1
$$

Hasil:

$$
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 6\
0 & -3 & -1 & -9\
0 & 1 & -2 & -3
\end{array}
\right]
$$

---

## **Langkah 3: Eliminasi Kolom Kedua**

$$
R_3 \leftarrow R_3 + \frac{1}{3}R_2
$$

Hasil:

$$
\left[
\begin{array}{ccc|c}
1 & 1 & 1 & 6\
0 & -3 & -1 & -9\
0 & 0 & -\frac{7}{3} & -6
\end{array}
\right]
$$

---

## **Langkah 4: Substitusi Balik**

Baris ketiga:

$$
-\frac{7}{3}z=-6
$$

$$
z=\frac{18}{7}
$$

Baris kedua:

$$
-3y-z=-9
$$

$$
y=\frac{15}{7}
$$

Baris pertama:

$$
x+y+z=6
$$

$$
x=\frac{9}{7}
$$

---

## **Jawaban**

$$
\boxed{
x=\frac97,\quad
y=\frac{15}{7},\quad
z=\frac{18}{7}
}
$$

---

# **Soal 3: SPL Empat Variabel**

## **Diketahui**

$$
\begin{cases}
x+y+z+w=10\
2x-y+z+w=5\
3x+y-z+w=12\
x+2y+3z-w=7
\end{cases}
$$

---

## **Langkah 1: Matriks Augmented**

$$
\left[
\begin{array}{cccc|c}
1 & 1 & 1 & 1 & 10\
2 & -1 & 1 & 1 & 5\
3 & 1 & -1 & 1 & 12\
1 & 2 & 3 & -1 & 7
\end{array}
\right]
$$

---

## **Langkah 2: Eliminasi Kolom Pertama**

$$
R_2 \leftarrow R_2 - 2R_1
$$

$$
R_3 \leftarrow R_3 - 3R_1
$$

$$
R_4 \leftarrow R_4 - R_1
$$

Hasil:

$$
\left[
\begin{array}{cccc|c}
1 & 1 & 1 & 1 & 10\
0 & -3 & -1 & -1 & -15\
0 & -2 & -4 & -2 & -18\
0 & 1 & 2 & -2 & -3
\end{array}
\right]
$$

---

## **Langkah 3: Eliminasi Kolom Kedua**

$$
R_3 \leftarrow R_3 - \frac{2}{3}R_2
$$

$$
R_4 \leftarrow R_4 + \frac{1}{3}R_2
$$

Hasil:

$$
\left[
\begin{array}{cccc|c}
1 & 1 & 1 & 1 & 10\
0 & -3 & -1 & -1 & -15\
0 & 0 & -\frac{10}{3} & -\frac{4}{3} & -8\
0 & 0 & \frac{5}{3} & -\frac{7}{3} & -8
\end{array}
\right]
$$

---

## **Langkah 4: Eliminasi Kolom Ketiga**

$$
R_4 \leftarrow R_4 + \frac{1}{2}R_3
$$

Hasil:

$$
\left[
\begin{array}{cccc|c}
1 & 1 & 1 & 1 & 10\
0 & -3 & -1 & -1 & -15\
0 & 0 & -\frac{10}{3} & -\frac{4}{3} & -8\
0 & 0 & 0 & -3 & -12
\end{array}
\right]
$$

---

## **Langkah 5: Substitusi Balik**

Baris keempat:

$$
-3w=-12
$$

$$
w=4
$$

Baris ketiga:

$$
-\frac{10}{3}z-\frac{4}{3}(4)=-8
$$

$$
z=\frac45
$$

Baris kedua:

$$
-3y-z-w=-15
$$

$$
y=\frac{17}{5}
$$

Baris pertama:

$$
x+y+z+w=10
$$

$$
x=\frac95
$$

---

## **Jawaban**

$$
\boxed{
x=\frac95,\quad
y=\frac{17}{5},\quad
z=\frac45,\quad
w=4
}
$$

---

# **Kesimpulan**

Metode Eliminasi Gauss dilakukan melalui tahapan:

1. Membentuk matriks augmented.
2. Melakukan operasi baris elementer.
3. Mengubah matriks menjadi bentuk eselon baris.
4. Melakukan substitusi balik.
5. Menentukan solusi SPL.

Metode ini dapat digunakan untuk menyelesaikan SPL dengan:

* 2 variabel
* 3 variabel
* 4 variabel
* n variabel

secara sistematis dan efisien.
