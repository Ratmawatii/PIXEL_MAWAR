# Bukti Citra Digital = Piksel + Angka

Tugas: membuktikan bahwa citra digital tersusun dari piksel dan angka, menggunakan Python di Google Colab.

## Isi repository
| File | Keterangan |
|------|------------|
| `bukti_citra_digital.ipynb` | Notebook utama (jalankan di Google Colab) |
| `piksel.csv` | Contoh keluaran: potongan foto sebagai teks angka (opsional) |
| `foto/` | Foto yang dipakai (opsional) |

## Cara menjalankan
1. Buka Google Colab, pilih **File > Upload notebook**, pilih `bukti_citra_digital.ipynb`
   (atau buka langsung dari GitHub: **File > Open notebook > GitHub**).
2. Jalankan semua sel berurutan (**Runtime > Run all**).
3. Pada sel "Upload foto", pilih foto Anda.

## Tahapan pembuktian
1. File foto = deretan byte (magic number)
2. Decode menjadi array NumPy (tinggi x lebar x 3)
   - 2b. Metadata EXIF (kamera, waktu, GPS) dibaca dan dibuktikan terpisah dari piksel
3. Satu piksel = 3 angka (R, G, B)
4. Zoom ekstrem: kotak piksel beserta angkanya
5. Pemisahan kanal R, G, B
6. Grayscale sebagai rumus matematika
7. Histogram
8. Mengubah angka mengubah gambar
9. Gambar dibuat dari angka murni
10. Round-trip PNG (lossless) vs JPEG (lossy)
11. Foto disimpan sebagai CSV lalu dibangun ulang
12. menampilkan meta data 

## Identitas
- Nama  : RATMAWATI
- NIM   : 24260013
- MATKUL : PENGOLAHAN CITRA DIGITAL
