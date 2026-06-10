# **Dekomposisi QR**

## **Pengertian Dekomposisi QR**

Dekomposisi QR adalah pemfaktoran suatu matriks persegi atau persegi panjang $A$ menjadi hasil kali dua buah matriks, yaitu matriks ortogonal $Q$ dan matriks segitiga atas $R$:

$$
A = QR
$$

di mana:
- **Matriks $Q$** adalah matriks ortogonal (atau ortonormal) yang kolom-kolomnya saling tegak lurus dan memiliki panjang satu, sehingga memenuhi sifat $Q^TQ = I$.
- **Matriks $R$** adalah matriks segitiga atas, di mana semua elemen di bawah diagonal utamanya bernilai nol.

---

## **Ortogonalisasi Gram-Schmidt**

Proses ortogonalisasi Gram-Schmidt adalah metode standar yang digunakan untuk mengonversi kumpulan vektor kolom dari matriks $A$ menjadi kumpulan vektor ortonormal yang membentuk kolom-kolom matriks $Q$. 

Proses ini memproyeksikan setiap vektor kolom terhadap vektor-vektor yang telah diortonormalkan sebelumnya untuk menghilangkan komponen yang tidak tegak lurus.

---

## **Visualisasi Interaktif (GeoGebra)**

[Ini Geogebra isi sendiri]

---

## **Kesimpulan**
Dekomposisi QR memiliki peranan penting dalam analisis numerik dan aljabar linear komputer. Metode ini digunakan secara luas untuk menyelesaikan masalah kuadrat terkecil (least squares), menghitung nilai eigen, dan memecahkan sistem persamaan linear dengan stabilitas numerik yang sangat tinggi dibandingkan dengan eliminasi biasa.
