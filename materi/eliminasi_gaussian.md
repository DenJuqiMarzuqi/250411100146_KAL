# **Eliminasi Gaussian**

## **Pendahuluan**

### **Latar Belakang**
Sistem Persamaan Linear (SPL) adalah kumpulan beberapa persamaan linear yang memiliki variabel yang sama dan diselesaikan secara bersamaan. Salah satu metode yang sistematis untuk menyelesaikan SPL adalah **Eliminasi Gaussian**, yaitu metode yang menggunakan Operasi Baris Elementer (OBE) untuk mengubah matriks menjadi bentuk segitiga atas (bentuk eselon baris), kemudian dilakukan substitusi balik.

### **Tujuan**
1. Memahami konsep SPL.
2. Memahami langkah-langkah Eliminasi Gaussian.
3. Menyelesaikan SPL dengan 3 dan 4 variabel secara sistematis.

---

## **Landasan Teori**

### **Bentuk Umum SPL**
Bentuk umum SPL dalam bentuk representasi matriks dapat dituliskan sebagai:

$$
Ax = b
$$

dengan ketentuan:
$$
A \in \mathbb{R}^{m \times n}, \quad x \in \mathbb{R}^{n}, \quad b \in \mathbb{R}^{m}
$$

### **Operasi Baris Elementer (OBE)**
Dalam metode Eliminasi Gaussian, operasi yang diperbolehkan pada matriks augmented adalah:
1. Menukar posisi dua baris.
2. Mengalikan elemen-elemen suatu baris dengan konstanta bukan nol ($k \neq 0$).
3. Menambahkan kelipatan dari suatu baris ke baris yang lain.

---

## **Langkah-Langkah Eliminasi Gaussian**

1. **Matriks Augmentasi**: Tuliskan sistem persamaan linear (SPL) dalam bentuk matriks augmented $[A|b]$.
2. **Eliminasi Maju (Forward Elimination)**: Mengubah matriks augmented menjadi bentuk eselon baris (segitiga atas) menggunakan serangkaian Operasi Baris Elementer (OBE).
3. **Substitusi Balik (Back Substitution)**: Menyelesaikan nilai-nilai variabel dari baris paling bawah secara bertahap menuju ke atas.

---

## **Visualisasi Interaktif (GeoGebra)**

[Ini Geogebra isi sendiri]

---

## **Kesimpulan**
Eliminasi Gaussian adalah algoritma fundamental dalam aljabar linear untuk menyelesaikan sistem persamaan linear, menentukan pangkat matriks, atau mencari invers suatu matriks. Metode ini dinamai dari matematikawan Jerman, Carl Friedrich Gauss, dan sangat praktis untuk menyelesaikan persamaan linear multi-variabel.
