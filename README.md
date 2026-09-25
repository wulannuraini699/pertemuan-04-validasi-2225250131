# Pertemuan 04 Seleksi Multi-Kondisi dan Validasi Input

**Nama:** Wulan Nur'aini  
**NIM:** 2225250131  
**Kelas:** 3E  

---

## Tujuan
Membangun program validasi dan klasifikasi nilai menggunakan rantai `if-elif-else` serta penanganan kesalahan berbasis `try-except` dalam bahasa Python.

---
## Hasil Pengujian
Latihan 1
| Kategori | Syarat Logika | Contoh Input | Output Diharapkan |
|--------- | ------------- | ------------ | ----------------- |
| A | nilai >= 85 | 85 dan 100 | Predikat A |
| B | nilai >= 70 | 70 dan 84.9 | Predikat B |
| C | nilai >= 60 | 60 dan 69.9 | Predikat C |
| D | nilai >= 50 | 50 dan 59.9 | Predikat D |
| E | nilai < 50 (selain di atas) | 0 dan 49.9 | Predikat E |

Tabel Hasil Pengujian Latihan 1 
| Masukan | Keluaran Diharapkan | Keluaran Aktual | Status |
| :---: | :--- | :--- | :---: |
| `92` | Nilai 92.00 memperoleh predikat A. | Nilai 92.00 memperoleh predikat A. | Sesuai |
| `85` | Nilai 85.00 memperoleh predikat A. | Nilai 85.00 memperoleh predikat A. | Sesuai |
| `84.9` | Nilai 84.90 memperoleh predikat B. | Nilai 84.90 memperoleh predikat B. | Sesuai |
| `70` | Nilai 70.00 memperoleh predikat B. | Nilai 70.00 memperoleh predikat B. | Sesuai |
| `60` | Nilai 60.00 memperoleh predikat C. | Nilai 60.00 memperoleh predikat C. | Sesuai |
| `50` | Nilai 50.00 memperoleh predikat D. | Nilai 50.00 memperoleh predikat D. | Sesuai |
| `49.9` | Nilai 49.90 memperoleh predikat E. | Nilai 49.90 memperoleh predikat E. | Sesuai |

Tabel Hasil Pengujian Latihan 2 
| Masukan | Keluaran Diharapkan | Keluaran Aktual | Status |
| :---: | :--- | :--- | :---: |
| `-7` | Bilangan negatif | Bilangan negatif | Sesuai |
| `0` | Nol | Nol | Sesuai |
| `8` | Bilangan positif genap | Bilangan positif genap | Sesuai |
| `13` | Bilangan positif ganjil | Bilangan positif ganjil | Sesuai |


## Cara Menjalankan Program
python3 praktik/validasi_klasifikasi_nilai.py

### Menjalankan Program Latihan:
```bash
python3 latihan/01_predikat_nilai.py
python3 latihan/02_kategori_bilangan.py
python3 latihan/03_validasi_rentang.py
python3 latihan/04_validasi_tipe.py
python3 latihan/05_klasifikasi_segitiga_sudut.py
