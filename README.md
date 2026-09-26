# Pertemuan 04 Seleksi Multi-Kondisi dan Validasi Input

**Nama:** Wulan Nur'aini  
**NIM:** 2225250131  
**Kelas:** 3E  

---

## Tujuan
Membangun program validasi dan klasifikasi nilai menggunakan rantai `if-elif-else` serta penanganan kesalahan berbasis `try-except` dalam bahasa Python.

---
## Hasil Pengujian

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

Tabel Hasil Pengujian Latihan 3 
| Masukan | Keluaran Diharapkan | Keluaran Aktual | Status |
| :---: | :--- | :--- | :---: |
| `45` | Sudut lancip | Sudut lancip | Sesuai |
| `90` | Sudut siku-siku | Sudut siku-siku | Sesuai |
| `135` | Sudut tumpul | Sudut tumpul | Sesuai |
| `0` | Masukan ditolak: sudut harus lebih dari 0 dan kurang dari 180. | Masukan ditolak: sudut harus lebih dari 0 dan kurang dari 180. | Sesuai |
| `180` | Masukan ditolak: sudut harus lebih dari 0 dan kurang dari 180. | Masukan ditolak: sudut harus lebih dari 0 dan kurang dari 180. | Sesuai |
| `-30` | Masukan ditolak: sudut harus lebih dari 0 dan kurang dari 180. | Masukan ditolak: sudut harus lebih dari 0 dan kurang dari 180. | Sesuai |

Tabel Hasil Pengujian Latihan 4 
| Masukan | Keluaran Diharapkan | Keluaran Aktual | Status |
| :---: | :--- | :--- | :---: |
| `15` | Persentase = 75.00 persen<br>Tuntas | Persentase = 75.00 persen<br>Tuntas | Sesuai |
| `14` | Persentase = 70.00 persen<br>Belum tuntas | Persentase = 70.00 persen<br>Belum tuntas | Sesuai |
| `20` | Persentase = 100.00 persen<br>Tuntas | Persentase = 100.00 persen<br>Tuntas | Sesuai |
| `0` | Persentase = 0.00 persen<br>Belum tuntas | Persentase = 0.00 persen<br>Belum tuntas | Sesuai |
| `21` | Masukan ditolak: jumlah harus berada pada rentang 0 sampai 20. | Masukan ditolak: jumlah harus berada pada rentang 0 sampai 20. | Sesuai |
| `dua belas` | Masukan ditolak: jumlah harus berupa bilangan bulat. | Masukan ditolak: jumlah harus berupa bilangan bulat. | Sesuai |

Tabel Hasil Pengujian Latihan 5 
| Masukan (A, B, C) | Keluaran Diharapkan | Keluaran Aktual | Status |
| :---: | :--- | :--- | :---: |
| `60, 60, 60` | Segitiga lancip | Segitiga lancip | Sesuai |
| `90, 45, 45` | Segitiga siku-siku | Segitiga siku-siku | Sesuai |
| `120, 30, 30` | Segitiga tumpul | Segitiga tumpul | Sesuai |
| `100, 50, 40` | Masukan ditolak: jumlah ketiga sudut harus 180 derajat. | Masukan ditolak: jumlah ketiga sudut harus 180 derajat. | Sesuai |
| `0, 90, 90` | Masukan ditolak: setiap sudut harus lebih dari 0 derajat. | Masukan ditolak: setiap sudut harus lebih dari 0 derajat. | Sesuai |

Tabel Hasil Pengujian Utama
| Ujian | Tugas | Kehadiran | Nilai Akhir | Keluaran Diharapkan | Keluaran Aktual | Status |
| :---: | :---: | :---: | :---: | :--- | :--- | :---: |
| `90` | `80` | `95` | 86.00 | Predikat A, Lulus | Nilai akhir : 86.00<br>Predikat: A<br>Status: Lulus | Sesuai |
| `75` | `70` | `85` | 73.00 | Predikat B, Lulus | Nilai akhir : 73.00<br>Predikat: B<br>Status: Lulus | Sesuai |
| `60` | `60` | `80` | 60.00 | Predikat C, Lulus | Nilai akhir : 60.00<br>Predikat: C<br>Status: Lulus | Sesuai |
| `55` | `50` | `90` | 53.00 | Predikat D, Belum lulus | Nilai akhir : 53.00<br>Predikat: D<br>Status: Belum lulus | Sesuai |
| `40` | `30` | `100` | 36.00 | Predikat E, Belum lulus | Nilai akhir : 36.00<br>Predikat: E<br>Status: Belum lulus | Sesuai |
| `90` | `90` | `75` | 90.00 | Nilai akhir tetap tampil, status Tidak memenuhi syarat kehadiran | Nilai akhir : 90.00<br>Status: Tidak memenuhi syarat kehadiran. | Sesuai |
| `105` | `80` | `90` | - | Pesan penolakan rentang nilai ujian | Masukan ditolak: nilai ujian di luar rentang 0 sampai 100. | Sesuai |
| `80` | `-5` | `90` | - | Pesan penolakan rentang nilai tugas | Masukan ditolak: nilai tugas di luar rentang 0 sampai 100. | Sesuai |
| `80` | `80` | `abc` | - | Pesan penolakan tipe | Masukan ditolak: seluruh data harus berupa angka. | Sesuai |

## Cara Menjalankan Program
python3 praktik/validasi_klasifikasi_nilai.py

### Menjalankan Program Latihan:
```bash
python3 latihan/01_predikat_nilai.py
python3 latihan/02_kategori_bilangan.py
python3 latihan/03_validasi_rentang.py
python3 latihan/04_validasi_tipe.py
python3 latihan/05_klasifikasi_segitiga_sudut.py
