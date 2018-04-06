## Source code ini akan menampilkan List Nilai Tugas, Nilai UTS, Nilai UAS, dan Nilai Akhir pada sebuah kolom penilaian yang akan memudahkan seorang dosen dalam merekap nilai-nilai para mahasiswanya.

## Saya menggunakan Python 3.4.2

## hasil outputnya berupa tabel menggunakan module Texttable yang sudah ada di library
```javascript
import texttable as tt
```
## menggunakan while untuk perulangan
```javascript
x = [[]]

jawab = "y"

tab = tt.Texttable()

while (jawab == 'y'):
```
## menu yang akan dieksekusi
```javascript
nama = []
nim = []
nilai_tugas = []
nilai_uts = []
nilai_uas = []
nilai_akhir = []
jawab = input("Tambah data [y/n]?  ")
```
## inputan untuk mengeksekusi program
```javascript
    nama.append(input("Masukkan Nama: "))
    nim.append(input("Masukkan Nim: "))
    tugas = int(input("Nilai Tugas: "))
    tugas = float(tugas)
    nilai_tugas.append(tugas)
    uts = int(input("Nilai UTS: "))
    uts = float(uts)
    nilai_uts.append(uts)
    uas = int(input("Nilai UAS: "))
    uas = float(uas)
    nilai_uas.append(uas)
    hasil = (tugas+uts+uas)/3
    nilai_akhir.append(hasil)
    jawab = input("Tambah data [y/n]?  ")
```
## perintah yang akan ditampilkan pada tabel
```javascript
idx = nama.index(i)
    x.append([idx+1,nama[idx],nim[idx],nilai_tugas[idx],nilai_uts[idx],nilai_uas[idx],nilai_akhir[idx]])
tab.add_rows(x)
tab.set_cols_align(['l','l','l','r','r','r','r'])
tab.header(['No','Nama','Nim','Nilai Tugas', 'Nilai UTS', 'Nilai UAS','Nilai Akhir'])
print (tab.draw())
```
## demikian sedikit penjelasan dari saya, semoga bermanfaat. Selamat mencoba...
