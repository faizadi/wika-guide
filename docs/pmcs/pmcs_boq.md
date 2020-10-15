---
id: pmcs_boq
title: Mengisi Excel RAB Lembar 2
custom_edit_url: https://github.com/faizadi/wika-guide/edit/master/docs/pmcs/pmcs_boq.md
---
`Anda berada di dalam panduan: PMCS`

## Lorem

| Kolom | Penjelasan dan Aturan Main | Keterangan |
|----------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------|
| Kode Tahap | Maksimal panjang karakter = 6<br><br>Disarankan menggunakan  angka, apabila tidak cukup dapat menggunakan kombinasi huruf dan  angka<br><br>Tidak diperbolehkan terdapat kode yang sama  untuk baris berbeda<br><br>Contoh isi = 010010 | Wajib diisi |
| Nama Tahap Pekerjaan | Maksimal panjang karakter = 250<br><br>Tidak dapat  menggunakan karakter simbol. Kecuali karakter simbol berikut ini . / , !  & % @ ( ) \ # = + < > - $ | Wajib diisi |
| Level | Diisi angka 1-7<br><br>Level menentukan urutan WBS tahap<br><br>Contoh isi = 4 | Wajib diisi |
| Parent | Maksimal panjang karakter = 6<br><br>Diisi kode tahap yang  ditunjuk sebagai parent item tahap<br><br>Tidak dapat input  kode diluar isi kolom tahap<br><br>Contoh isi = 01 | Wajib diisi |
| Sat (Satuan) | Maksimal panjang karakter = 10<br><br>Tidak dapat  menggunakan karakter simbol. Kecuali karakter simbol berikut ini . / , !  & % @ ( ) \ # = + < > - $<br><br>Contoh isi = m2  (per meter persegi) | Wajib diisi |
| Vol Kontrak | Diisi angka dengan separator desimal menggunakan tanda  titik<br><br>Tidak dapat diisi 0 untuk input RAB  RKP<br><br>Contoh isi = 154.75 | Wajib diisi, khusus item tahap yang level WBSnya terendah |
| Harga Kontrak | Diisi angka harga satuan per item tahap<br><br>Nominal tidak  diinput menggunakan separator rupiah<br><br>Contoh isi =  18000 | Wajib diisi, khusus item tahap yang level WBSnya terendah |
| Total Kontrak | Diisi angka total harga per item tahap<br><br>Nominal tidak  diinput menggunakan separator rupiah<br><br>Contoh isi =  2785500 | Wajib diisi, khusus item tahap yang level WBSnya terendah |
| Vol RAB | Diisi angka dengan separator desimal menggunakan tanda  titik<br><br>Tidak dapat diisi 0 untuk input RAB  RKP<br><br>Contoh isi = 154.75 | Wajib diisi, khusus item tahap yang level WBSnya terendah |
| Kode Member | Khusus Proyek JO<br><br>Tidak dapat diisi diluar kode member yang terdaftar | Tidak wajib |

> Catatan:
> - Semua kolom wajib berformat general/text
> - Penginputan kode tahap tiap baris dari atas kebawah wajib berurutan dari kode terkecil sampai terbesar
> - Mega proyek dapat menggunakan awalan kode 01, 02, 03, dst agar tidak bercampur antara item tahap ke-1 dan 11 apabila diurutkan, karena item pekerjaan banyak
