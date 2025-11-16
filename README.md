# Manipulasi Citra Digital – Metode Masking & Penampakan Penggaris pada Gambar

Repository ini berisi source code program manipulasi citra digital yang dilakukan untuk memenuhi tugas mata kuliah Pengolahan Citra Digital. Program ini menerapkan **metode masking** serta menampilkan **overlay penggaris (ruler)** pada gambar agar dapat diukur berdasarkan skala pixel.

---

## 📌 Fitur Program
Program ini memiliki beberapa kemampuan utama:

### ✔ 1. Membaca dan menampilkan gambar  
Program memuat satu gambar yang dipilih dari file ZIP sesuai instruksi dosen.

### ✔ 2. Melakukan *Masking*  
Masking digunakan untuk mengolah piksel tertentu pada gambar sambil mempertahankan struktur visual aslinya.

### ✔ 3. Menampilkan Penggaris (Ruler Overlay)  
Program menambahkan ruler berupa garis horizontal/vertikal dengan tanda setiap beberapa pixel (misal tiap 50 px).  
Ruler ini digunakan untuk membantu pengukuran objek pada gambar.

### ✔ 4. Menyimpan gambar hasil manipulasi  
Gambar hasil proses akan disimpan sebagai file baru.

---

## 📁 Struktur Folder
📦 Nama-Repository-Kamu
┣ 📜 Masking.py
┣ 📜 gambar_input.jpg
┣ 📜 hasil_output.jpg
┗ 📜 README.md

---

## 🛠️ Instalasi & Persiapan

### 1. Pastikan Python 3 sudah terinstal
Cek dengan:
```bash
python --version
Install dependency (OpenCV & Numpy)
pip install opencv-python numpy

▶ Cara Menjalankan Program

Masukkan file gambar yang kamu pilih dari ZIP ke dalam folder proyek.

Jalankan program Python berikut:

python Masking.py


Hasil gambar akan muncul di window OpenCV dan disimpan sebagai:

hasil_output.jpg

📷 Contoh Output

Gambar asli

Gambar hasil masking

Gambar dengan overlay penggaris (misal skala 0–300 px)

Output akan berbeda tergantung gambar yang kamu pilih dan parameter ruler.

✨ Penjelasan Singkat Metode
🔹 Masking

Masking adalah proses memanipulasi bagian tertentu dari gambar menggunakan operasi logika atau filter tertentu. Contohnya:

Menyembunyikan area tertentu

Menyorot area tertentu

Melakukan operasi logika AND, OR, XOR pada channel piksel

🔹 Penggaris (Ruler Overlay)

Ruler dibuat dengan cara:

Membuat garis lurus menggunakan OpenCV (cv2.line)

Memberikan tanda setiap beberapa piksel (tick marks)

Memberi label angka menggunakan cv2.putText

Ruler tidak mengubah gambar asli, hanya menambah overlay di atasnya.
