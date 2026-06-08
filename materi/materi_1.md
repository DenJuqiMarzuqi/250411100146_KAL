# Materi 1: Pengenalan Komputasi Aljabar Linier

Aljabar Linier Komputasi adalah cabang matematika yang sangat penting dalam bidang Ilmu Komputer, Sains Data, dan Kecerdasan Buatan (AI). Di sini, kita akan mendokumentasikan konsep-konsep dasar seperti matriks, vektor, dan operasinya.

## Apa itu Matriks?

Matriks adalah susunan bilangan, simbol, atau ekspresi, yang disusun dalam baris dan kolom. 

$$
A = \begin{pmatrix}
1 & 2 \\
3 & 4
\end{pmatrix}
$$

### Operasi Matriks Dasar:
1. **Penjumlahan Matriks**: Menjumlahkan elemen yang bersesuaian pada dua matriks berukuran sama.
2. **Perkalian Skalar**: Mengalikan seluruh elemen matriks dengan konstanta skalar.
3. **Perkalian Matriks**: Mengalikan baris matriks pertama dengan kolom matriks kedua.

## Contoh Kode Python untuk Membuat Matriks
Kita bisa merepresentasikan matriks di Python menggunakan library `numpy`:

```python
import numpy as np

# Membuat matriks 2x2
A = np.array([[1, 2], [3, 4]])
print(A)
```
