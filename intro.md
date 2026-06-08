# Selamat Datang di Website Statis KAL

Ini adalah website statis yang dibuat menggunakan **Jupyter Book**. Website ini digunakan untuk mendokumentasikan tugas atau materi kuliah **Komputasi Aljabar Linier (KAL)** di Universitas Trunojoyo Madura.

## Cara Mengembangkan Website Ini

1. **Persiapan Lingkungan**: Pastikan Anda memiliki Python dan pip terinstal di komputer Anda.
2. **Install Jupyter Book**:
   Jalankan perintah ini di Command Prompt / PowerShell:
   ```bash
   pip install jupyter-book
   ```
3. **Build Website**:
   Untuk membuat/membangun website statis (HTML), jalankan perintah berikut di terminal pada folder ini:
   ```bash
   jupyter-book build .
   ```
4. **Buka Hasil Build**:
   Setelah proses build selesai, buka file HTML hasil build di folder berikut menggunakan browser Anda:
   `_build/html/index.html`

---

## Struktur File Proyek

* `_config.yml`: File konfigurasi utama (judul website, penulis, logo, dll.).
* `_toc.yml`: File daftar isi (*Table of Contents*) untuk mengatur menu navigasi di sebelah kiri.
* `intro.md`: Halaman utama / beranda website.
* `biodata/`: Folder yang berisi file biodata Anda (`index.md`).
* `materi/`: Folder yang berisi file materi kuliah (`index.md`, `materi_1.md`, `notebook_contoh.ipynb`).
* `tugas/`: Folder yang berisi file tugas kuliah (`index.md`, `tugas_1.md`).

