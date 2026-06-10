# **Eliminasi Gaussian**

Eliminasi Gaussian adalah algoritma dalam aljabar linear untuk menyelesaikan sistem persamaan linear, menentukan pangkat matriks, atau mencari invers suatu matriks. Metode ini dinamai dari matematikawan Jerman, Carl Friedrich Gauss.

---

## **Langkah-Langkah Eliminasi Gaussian**

1. **Matriks Augmentasi**: Tuliskan sistem persamaan linear (SPL) dalam bentuk matriks augmented.
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

[Keterangan/Rumus Bentuk Umum SPL]

dengan:

[Keterangan Variabel/Koefisien]

#### **2.2 Operasi Baris Elementer (OBE)**
Dalam Eliminasi Gaussian diperbolehkan:
* Menukar dua baris.
* Mengalikan baris dengan konstanta bukan nol.
* Menambahkan kelipatan suatu baris ke baris lain.

---

### **BAB III: Pembahasan**

#### **3.1 SPL Tiga Variabel**
Diketahui:

[Persamaan SPL 3 Variabel]

**Langkah 1: Matriks Augmented**

[Matriks Augmented SPL 3 Variabel]

**Langkah 2: Eliminasi Kolom Pertama**

[Proses OBE Eliminasi Kolom Pertama]

Hasil:

[Hasil Eliminasi Kolom Pertama]

**Langkah 3: Eliminasi Kolom Kedua**

[Proses OBE Eliminasi Kolom Kedua]

[Hasil Eselon Baris Segitiga Atas]

*Sudah berbentuk eselon baris (segitiga atas).*

**Substitusi Balik**
* **Baris 3**: [Substitusi Baris 3]
* **Baris 2**: [Substitusi Baris 2]
* **Baris 1**: [Substitusi Baris 1]

**Solusi SPL 3 Variabel**

[Solusi SPL 3 Variabel]

#### **3.2 SPL Empat Variabel**
Diketahui:

[Persamaan SPL 4 Variabel]

**Langkah 1: Matriks Augmented**

[Matriks Augmented SPL 4 Variabel]

**Langkah 2: Eliminasi Kolom Pertama**

Hasil:

[Hasil Eliminasi Kolom Pertama]

**Langkah 3: Eliminasi Kolom Kedua dan Ketiga**

Setelah dilakukan OBE lanjutan diperoleh bentuk eselon baris:

[Hasil Eselon Baris Akhir]

**Substitusi Balik**
* **Baris 4**: [Substitusi Baris 4]
* **Baris 3**: [Substitusi Baris 3] *(Catatan: berdasarkan hitungan dari file intro: z = 3, y = 2, x = 1)*
* **Baris 2**: [Substitusi Baris 2]
* **Baris 1**: [Substitusi Baris 1]

**Solusi SPL 4 Variabel**

[Solusi SPL 4 Variabel]

---

### **BAB IV: Kesimpulan**
* Eliminasi Gaussian menyelesaikan SPL dengan membentuk matriks eselon baris menggunakan serangkaian OBE.
* Setelah bentuk segitiga atas diperoleh, solusi variabel dicari secara runtut menggunakan metode substitusi balik.
* Kedua contoh sistem persamaan di atas memiliki solusi tunggal.

---

## **Integrasi SageMath Interaktif**

[Integrasi SageMath Interaktif]
