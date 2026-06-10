# **Vektor**

## **Pengertian Vektor**

Vektor adalah suatu besaran yang memiliki **besar (magnitudo)** dan **arah**.

Berbeda dengan skalar yang hanya memiliki nilai, vektor memiliki nilai sekaligus arah tertentu.

Contoh besaran vektor:

* Kecepatan
* Percepatan
* Gaya
* Perpindahan
* Momentum

Sedangkan contoh besaran skalar:

* Massa
* Waktu
* Suhu
* Energi

---

# **Definisi Vektor**

Secara matematis, vektor dapat direpresentasikan sebagai kumpulan komponen yang tersusun dalam bentuk baris atau kolom.

Vektor dua dimensi dapat ditulis sebagai:

$$
\vec{v} =
\begin{bmatrix}
x \\
y
\end{bmatrix}
$$

atau

$$
\vec{v} = (x,y)
$$

Sedangkan vektor tiga dimensi dapat ditulis sebagai:

$$
\vec{v} =
\begin{bmatrix}
x \\
y \\
z
\end{bmatrix}
$$

atau

$$
\vec{v} = (x,y,z)
$$

---

# **Tujuan Mempelajari Vektor**

Vektor dipelajari untuk:

1. Merepresentasikan arah dan besar suatu objek.
2. Memodelkan pergerakan benda.
3. Menyelesaikan masalah geometri.
4. Digunakan dalam grafika komputer.
5. Digunakan dalam machine learning dan data science.

---

# **Fungsi Vektor**

Vektor digunakan dalam berbagai bidang, seperti:

* Fisika
* Teknik
* Robotika
* Machine Learning
* Computer Vision
* Grafika Komputer
* Sistem Navigasi

---

# **Representasi Vektor**

## **Vektor Dua Dimensi (2D)**

Contoh:

$$
\vec{a} =
\begin{bmatrix}
3 \\
4
\end{bmatrix}
$$

atau

$$
\vec{a} = (3,4)
$$

---

## **Vektor Tiga Dimensi (3D)**

Contoh:

$$
\vec{b} =
\begin{bmatrix}
2 \\
1 \\
5
\end{bmatrix}
$$

atau

$$
\vec{b} = (2,1,5)
$$

---

# **Panjang atau Magnitudo Vektor**

## **Definisi Magnitudo**

Magnitudo adalah panjang suatu vektor.

Notasi:

$$
||\vec{v}||
$$

---

## **Rumus Magnitudo Vektor 2D**

Jika:

$$
\vec{v} =
\begin{bmatrix}
x \\
y
\end{bmatrix}
$$

maka:

$$
||\vec{v}|| =
\sqrt{x^2+y^2}
$$

---

## **Contoh Soal Magnitudo 2D**

Diketahui:

$$
\vec{v} =
\begin{bmatrix}
3 \\
4
\end{bmatrix}
$$

Hitung panjang vektornya.

### **Penyelesaian**

$$
||\vec{v}|| =
\sqrt{3^2+4^2}
$$

$$
\sqrt{9+16}
$$

$$
\sqrt{25}
$$

$$
=5
$$

Jadi:

$$
\boxed{||\vec{v}||=5}
$$

---

## **Rumus Magnitudo Vektor 3D**

Jika:

$$
\vec{v} =
\begin{bmatrix}
x \\
y \\
z
\end{bmatrix}
$$

maka:

$$
||\vec{v}|| =
\sqrt{x^2+y^2+z^2}
$$

---

# **Penjumlahan Vektor**

## **Definisi**

Penjumlahan vektor dilakukan dengan menjumlahkan komponen-komponen yang bersesuaian.

Jika:

$$
\vec{a} =
\begin{bmatrix}
a_1 \\
a_2
\end{bmatrix}
$$

dan

$$
\vec{b} =
\begin{bmatrix}
b_1 \\
b_2
\end{bmatrix}
$$

maka:

$$
\vec{a}+\vec{b} =
\begin{bmatrix}
a_1+b_1 \\
a_2+b_2
\end{bmatrix}
$$

---

## **Contoh Soal Penjumlahan Vektor**

Diketahui:

$$
\vec{a} =
\begin{bmatrix}
2 \\
3
\end{bmatrix}
$$

dan

$$
\vec{b} =
\begin{bmatrix}
4 \\
1
\end{bmatrix}
$$

Maka:

$$
\vec{a}+\vec{b} =
\begin{bmatrix}
6 \\
4
\end{bmatrix}
$$

---

# **Pengurangan Vektor**

## **Definisi**

Pengurangan vektor dilakukan dengan mengurangi komponen yang bersesuaian.

$$
\vec{a}-\vec{b} =
\begin{bmatrix}
a_1-b_1 \\
a_2-b_2
\end{bmatrix}
$$

---

## **Contoh Soal Pengurangan Vektor**

$$
\vec{a} =
\begin{bmatrix}
5 \\
7
\end{bmatrix}
$$

$$
\vec{b} =
\begin{bmatrix}
2 \\
4
\end{bmatrix}
$$

Maka:

$$
\vec{a}-\vec{b} =
\begin{bmatrix}
3 \\
3
\end{bmatrix}
$$

---

# **Perkalian Skalar dengan Vektor**

## **Definisi**

Jika suatu vektor dikalikan dengan bilangan skalar (k), maka setiap komponennya dikalikan dengan (k).

$$
k\vec{v} =
\begin{bmatrix}
kx \\
ky
\end{bmatrix}
$$

---

## **Contoh Soal**

Diketahui:

$$
\vec{v} =
\begin{bmatrix}
2 \\
5
\end{bmatrix}
$$

dan

$$
k=3
$$

Maka:

$$
3\vec{v} =
\begin{bmatrix}
6 \\
15
\end{bmatrix}
$$

---

# **Vektor Satuan (Unit Vector)**

## **Pengertian**

Vektor satuan adalah vektor yang memiliki panjang sama dengan satu.

Notasi:

$$
\hat{u}
$$

---

## **Rumus Vektor Satuan**

Jika:

$$
\vec{v} =
\begin{bmatrix}
x \\
y
\end{bmatrix}
$$

maka:

$$
\hat{u} =
\frac{\vec{v}}{||\vec{v}||}
$$

---

## **Contoh Soal**

Diketahui:

$$
\vec{v} =
\begin{bmatrix}
3 \\
4
\end{bmatrix}
$$

dan:

$$
||\vec{v}||=5
$$

Maka:

$$
\hat{u} =
\frac{1}{5}
\begin{bmatrix}
3 \\
4
\end{bmatrix}
$$

$$
\begin{bmatrix}
\frac35 \\
\frac45
\end{bmatrix}
$$

---

# **Perkalian Titik (Dot Product)**

## **Pengertian**

Dot Product adalah operasi yang menghasilkan bilangan skalar.

---

## **Rumus Dot Product**

Jika:

$$
\vec{a} =
\begin{bmatrix}
a_1 \\
a_2
\end{bmatrix}
$$

dan

$$
\vec{b} =
\begin{bmatrix}
b_1 \\
b_2
\end{bmatrix}
$$

maka:

$$
\vec{a}\cdot\vec{b} =
a_1b_1+a_2b_2
$$

---

## **Contoh Soal Dot Product**

$$
\vec{a} =
\begin{bmatrix}
2 \\
3
\end{bmatrix}
$$

$$
\vec{b} =
\begin{bmatrix}
4 \\
5
\end{bmatrix}
$$

Maka:

$$
\vec{a}\cdot\vec{b} =
(2)(4)+(3)(5)
$$

$$
8+15
$$

$$
=23
$$

---

# **Sudut Antar Vektor**

## **Rumus Sudut Antar Vektor**

$$
\cos\theta =
\frac{\vec{a}\cdot\vec{b}}
{||\vec{a}||||\vec{b}||}
$$

---

## **Kondisi Khusus**

### **Vektor Tegak Lurus**

Jika:

$$
\vec{a}\cdot\vec{b}=0
$$

maka kedua vektor saling tegak lurus.

---

### **Vektor Sejajar**

Jika:

$$
\vec{a}=k\vec{b}
$$

maka kedua vektor sejajar.

---

# **Hubungan Vektor dengan Matriks**

Vektor sebenarnya merupakan bentuk khusus dari matriks.

Vektor kolom:

$$
\begin{bmatrix}
x \\
y \\
z
\end{bmatrix}
$$

merupakan matriks berukuran:

$$
3\times1
$$

Sedangkan vektor baris:

$$
\begin{bmatrix}
x & y & z
\end{bmatrix}
$$

merupakan matriks berukuran:

$$
1\times3
$$

---

# **Penerapan Vektor**

## **Fisika**

* Gaya
* Kecepatan
* Percepatan
* Momentum

---

## **Grafika Komputer**

* Pergerakan objek
* Rotasi
* Transformasi

---

## **Machine Learning**

* Representasi fitur
* Embedding
* PCA
* SVD

---

## **Robotika**

* Navigasi robot
* Posisi dan orientasi

---

# **Kesimpulan**

Vektor adalah besaran yang memiliki:

* Besar (magnitudo)
* Arah

Vektor dapat direpresentasikan dalam bentuk:

$$
\vec{v} =
\begin{bmatrix}
x \\
y
\end{bmatrix}
$$

atau

$$
\vec{v} =
\begin{bmatrix}
x \\
y \\
z
\end{bmatrix}
$$

Operasi dasar pada vektor meliputi:

1. Penjumlahan vektor
2. Pengurangan vektor
3. Perkalian skalar
4. Dot Product
5. Perhitungan sudut antar vektor

Konsep vektor merupakan dasar penting untuk mempelajari:

* Matriks
* Transformasi Linear
* Eigenvalue dan Eigenvector
* SVD
* Machine Learning
* Computer Vision
* Data Science
