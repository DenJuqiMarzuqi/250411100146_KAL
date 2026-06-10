# **Tugas: Singular Value Decomposition (SVD)**

## **Aplikasi SVD pada Kompresi Gambar Berwarna**

Di bawah ini adalah kode untuk mengompresi gambar menggunakan metode SVD. Perhatikan penggunaan path berkas gambar yang tepat dan pemisahan channel warna (R, G, B).

```python
import cv2
import numpy as np
import matplotlib.pyplot as plt

# ✅ Menggunakan foto wajah abdul_hadi_marzuqi.jpeg
image = cv2.imread('abdul_hadi_marzuqi.jpeg', cv2.IMREAD_GRAYSCALE)

# Kalau cv2 tidak ada, pakai ini sebagai gantinya:
# from PIL import Image
# image = np.array(Image.open('abdul_hadi_marzuqi.jpeg').convert('L'))

plt.imshow(image, cmap='gray')
plt.title('Foto Wajah Asli')
plt.axis('off')
plt.show()
```

```python
U, S, Vt = np.linalg.svd(image, full_matrices=False)

print(f"Shape U : {U.shape}")
print(f"Shape S : {S.shape}")
print(f"Shape Vt: {Vt.shape}")

print(f"\n10 singular value terbesar : {S[:10].astype(int)}")
print(f"10 singular value terkecil : {S[-10:].round(2)}")
```

### **Output:**
```text
Shape U : (1240, 768)
Shape S : (768,)
Shape Vt: (768, 768)

10 singular value terbesar : [154393  27632  14055  12537   9949   9102   8669   7959   6007   5703]
10 singular value terkecil : [0.58 0.54 0.48 0.44 0.4  0.38 0.32 0.2  0.18 0.16]
```

```python
fig, axes = plt.subplots(1, 6, figsize=(18, 4))
fig.suptitle('Pengenalan Wajah via SVD — Pengaruh Jumlah Singular Values',
             fontweight='bold', fontsize=13)

n_values = [1, 5, 10, 20, 50, len(S)]
labels   = [
    'n=1\n(blur total)',
    'n=5\n(siluet)',
    'n=10\n(mulai jelas)',
    'n=20\n(fitur wajah)',
    'n=50\n(detail halus)',
    'Original'
]

for ax, n, label in zip(axes, n_values, labels):
    recon = np.array(U[:, :n]) @ np.diag(S[:n]) @ np.array(Vt[:n, :])
    ax.imshow(recon, cmap='gray')
    ax.set_title(label, fontsize=9)
    ax.axis('off')

plt.tight_layout()
plt.show()
```

```python
print("=" * 45)
print(" Analisis Kompresi Wajah")
print("=" * 45)
print(f"{'n':>6} | {'Rasio Kompresi':>14} | {'Info Tersimpan':>14}")
print("-" * 45)

total_energy = np.sum(S**2)
m, k = image.shape

for n in [1, 5, 10, 20, 50, 100, 200]:
    if n > len(S):
        break
    rasio  = (m * k) / (n * (m + k + 1))
    energy = np.sum(S[:n]**2) / total_energy * 100
    print(f"{n:>6} | {rasio:>13.1f}x | {energy:>13.2f}%")

print("-" * 45)
print(f"{'Original':>6} | {'1.0x':>14} | {'100.00%':>14}")
```

### **Output:**
```text
=============================================
 Analisis Kompresi Wajah
=============================================
     n | Rasio Kompresi | Info Tersimpan
---------------------------------------------
     1 |         474.0x |         93.20%
     5 |          94.8x |         97.96%
    10 |          47.4x |         99.09%
    20 |          23.7x |         99.57%
    50 |           9.5x |         99.87%
   100 |           4.7x |         99.97%
   200 |           2.4x |         99.99%
---------------------------------------------
Original |           1.0x |        100.00%
```
