# Tugas 1: Pengenalan Matriks & Vektor

Pada tugas pertama ini, kita mempraktikkan cara membuat dan mengoperasikan matriks serta vektor di Python.

## Latihan Soal

Diberikan dua matriks:

$$
A = \begin{pmatrix}
2 & 5 \\
1 & 3
\end{pmatrix}, \quad
B = \begin{pmatrix}
4 & -1 \\
0 & 2
\end{pmatrix}
$$

Hitunglah $A + B$ dan $A \times B$.

### Jawaban (Python)

```python
import numpy as np

A = np.array([[2, 5], [1, 3]])
B = np.array([[4, -1], [0, 2]])

# 1. Penjumlahan
print("A + B = \n", A + B)

# 2. Perkalian
print("A x B = \n", np.dot(A, B))
```
