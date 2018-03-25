Source code ini berfungsi untuk menampilkan List Nilai Tugas, Nilai UTS, Nilai UAS, dan Nilai Akhir pada sebuah kolom penilaian untuk di suatu kelas perkuliahan. Agar memudahkan seorang dosen dalam merekap nilai-nilai para mahasiswanya.
Saya menggunakan Python 3.4.2
Berikut sedikit penjelasannya :
import texttable as tt adalah perintah bahwa code ini akan tampil dalam bentuk tabel seperti pada file Texttable (kalau belum ada, install terlebih dahulu)
nama, nim, nilai_tugas, nila_uts, nilai_uas, nilai_akhir, merupakan poin-poin yang akan dieksekusi
nama.append(input ("Masukkan Nama : "), dan seterusnya, merupakan code yang digunakan agar output menampilkan seperti sebuah formulir yang harus diisi
x.append([idx+1,nama[idx],nim[idx],nilai_tugas[idx],nilai_uts[idx],nilai_uas[idx],nilai_akhir[idx]]) merupakan hasil eksekusi progam yang nantinya akan dimunculkan dalam kolom-kolom tabel
tab.header(['No','Nama','Nim','Nilai Tugas', 'Nilai UTS', 'Nilai UAS','Nilai Akhir']) merupakan format untuk judul pada tabel yang dibuat, posisinya ada di atas atau berbentuk kolom
print (tab.draw()) adalah perintah untuk mengksekusi semua source code
SELAMAT MENCOBA :)
Khalis Sofi_STT Pelita Bangsa_Kelas TI 17 B3_Tugas Bang Sas
