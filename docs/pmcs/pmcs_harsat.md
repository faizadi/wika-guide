---
id: pmcs_harsat
title: Mengisi Excel RAB Lembar 1
custom_edit_url: https://github.com/faizadi/wika-guide/edit/master/docs/pmcs/pmcs_harsat.md
---
`Anda berada di dalam panduan: PMCS`

Pengisian template excel lembar pertama hanya dilakukan saat awal penggunaan PMCS dan saat terjadi perubahan RAB, sehingga tidak perlu dilakukan setiap bulan. 

Singkatnya, lembar pertama digunakan untuk menginput daftar Harga Satuan per item Sumber Daya dan kodefikasi item.

## Langkah Pengisian

1. Buka menu `1. Restore Harga Satuan Sumber Daya`.

   <img src="../assets/pmcs/drawio_menulem1.svg" alt="gbr-menu-lembar1"/>

2. Silahkan unduh template excel, tekan tombol `Download`.

   <img src="../assets/pmcs/drawio_upllem1.svg" alt="gbr-upload-lembar1"/>

3. Buka dokumen menggunakan [Microsoft Excel](pmcs_spec#kebutuhan-perangkat-lunak). Dokumen menggunakan format `.xls`.  
   Contoh tampilan excel:

   <img src="../assets/pmcs/drawio_lem1.svg" alt="gbr-template-lembar1"/>

   ### Aturan Main

   Merujuk pada gambar diatas, inilah penjelasan dan hal-hal yang harus diperhatikan saat mengisi template excel. Karena umumnya [kendala saat upload](pmcs_harsat#notifikasi-gagal-upload) disebabkan oleh kesalahan pengisian data.

   | Kolom | Penjelasan | Keterangan |
   |-------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------|
   | Kode Sumber Daya | Harus diisi sebanyak 6 karakter<br><br>Tidak diperbolehkan  terdapat kode yang sama untuk baris berbeda<br><br>Lihat  Nomenklatur kode sumber daya<br><br>3 digit awal diisi sama  dengan isi kolom Kode Master<br><br>Contoh isi = AF1010 | Wajib diisi |
   | Nama Sumber Daya | Maksimal panjang karakter = 200<br><br>Tidak dapat  menggunakan karakter simbol. Kecuali karakter simbol berikut ini . / , !  & % @ ( ) \ # = + < > - $<br><br>Contoh isi =  Besi Beton US SNI 16mm Ulir | Wajib diisi |
   | UOM (Satuan) | Maksimal panjang karakter = 10<br><br>Tidak dapat  menggunakan karakter simbol. Kecuali karakter simbol berikut ini . / , !  & % @ ( ) \ # = + < > - $<br><br>Contoh isi = kg (per kilo gram) | Wajib diisi |
   | UOM_2 | Maksimal panjang karakter = 10<br><br>Tidak dapat  menggunakan karakter simbol. Kecuali karakter simbol berikut ini . / , !  & % @ ( ) \ # = + < > - $<br><br>Hanya diisi  apabila terdapat satuan konversi atau jika kolom Konversi diisi | Tidak wajib |
   | Konversi | Diisi angka<br><br>Hanya diisi apabila terdapat satuan konversi atau jika kolom UOM_2 diisi | Tidak wajib |
   | Kode Master Sumber Daya | Harus diisi sebanyak 3 karakter<br><br>Pastikan isi kode sudah sesuai dengan Master Kode Sumber Daya Nasional WIKA<br><br>Kode master harus sesuai dengan jenis sumber daya di kolom kode sumber daya, kesalahan input dapat mengakibatkan kesalahan rekap nilai laporan biaya<br><br>Contoh isi =  AF1 (untuk material Besi Beton) | Wajib diisi |
   | Harga RKP | Diisi angka harga satuan per sumber daya<br><br>Tidak diperbolehkan merubah harga RKP saat input adendum RAB<br><br>Nominal tidak diinput menggunakan separator rupiah<br><br>Contoh isi = 8150 | Wajib diisi |
   | Harga Review | Diisi angka harga satuan per sumber daya<br><br>Nominal diisi sama dengan nominal kolom Harga RKP apabila belum adendum RAB<br><br>Nominal tidak diinput menggunakan separator rupiah<br><br>Contoh isi = 8150 | Wajib diisi |

   > Catatan:
   > - Semua kolom wajib berformat general/text

4. Untuk proses upload, tekan tombol `Browse` kemudian pilih dokumen.

   <img src="../assets/pmcs/drawio_upllem1.svg" alt="gbr-menu-lembar1"/>

5. Tekan tombol `Simpan`.

## Notifikasi Gagal Upload

Lorem ipsum dolor sir amet.

### `Kode Error #001`

>   #### Contoh Sampel Notifikasi
>   Maaf, file yang dipilih bukan bertipe `.xls` Excel 97-2003 Workbook.
>
>   #### Apa artinya?
>   File yang Anda pilih saat `Browse` dokumen salah.
>
>   #### Apa yang harus dilakukan?
>   Ulangi proses pemilihan dokumen, pastikan tipe dokumen yang di upload adalah Microsoft Excel 97-2003 Worksheet berformat `.xls`.
>
>   #### Catatan
>   Mengapa laptop Saya tidak menampilkan tipe dokumen seperti gambar di atas? Googling dulu [cara memunculkan tipe file pada explorer](http://lmgtfy.com/?q=cara+memunculkan+tipe+file+pada+explorer).

### `Kode Error #002`

>   #### Contoh Sampel Notifikasi
>   Maaf, Anda belum memilih proyek di Dashboard. Otomatis diarahkan menuju dashboard.
>
>   #### Apa artinya?
>   Jangan lupa pilih proyek sebelum upload data.
>
>   #### Apa yang harus dilakukan?
>   Pada menu `Dashboard`, pilih Kode SPK (Project), klik tombol `Pilih`. Lanjutkan upload data.

### `Kode Error #007`

>   #### Contoh Sampel Notifikasi
>   Kode Sumber Daya : A200028 memiliki 7 karakter. Kode tidak boleh lebih dari 6 karakter. [#007]
>
>   #### Apa artinya?
>   Jumlah karakter kode tersebut melebihi batas maksimal.
>
>   #### Apa yang harus dilakukan?
>   1. Buka template excel
>   2. Cek kolom **Kode Sumber Daya**
>   3. Cari kode yang ditunjuk
>   4. Periksa jumlah karakter
>   5. Ubah kode
>
>   #### Catatan
>   Bagaimana cara cek jumlah karakter? Googling dulu [cara cek jumlah karakter pada excel](http://lmgtfy.com/?q=cara+cek+jumlah+karakter+pada+excel).

### `Kode Error #009`

>   #### Contoh Sampel Notifikasi
>   Nama Sumber Daya untuk kode : A10001 memiliki 252 karakter. Nama tidak boleh lebih dari 200 karakter. [#009]
>
>   #### Apa artinya?
>   Jumlah karakter nama sumber daya tersebut melebihi batas maksimal.
>
>   #### Apa yang harus dilakukan?
>   1. Buka template excel
>   2. Cek kolom **Nama Sumber Daya**
>   3. Cari berdasarkan kode yang ditunjuk
>   4. Periksa jumlah karakter
>   5. Ubah nama

### `Kode Error #013`

>   #### Contoh Sampel Notifikasi
>   Nama Sumber Daya untuk kode : A10002 tidak boleh menggunakan karakter simbol. Contoh: Diameter Ø. [#013]
>
>   #### Apa artinya?
>   Nama sumber daya tersebut memiliki karakter simbol sehingga ditolak sistem.
>
>   #### Apa yang harus dilakukan?
>   1. Buka template excel
>   2. Cek kolom **Nama Sumber Daya**
>   3. Cari berdasarkan kode yang ditunjuk
>   4. Periksa apakah ada simbol
>   5. Ubah nama

### `Kode Error #015`

>   #### Contoh Sampel Notifikasi
>   Satuan Sumber Daya untuk kode : A10006 tidak boleh menggunakan karakter simbol. Contoh: Meter kubik m³. [#015]
>
>   #### Apa artinya?
>   Satuan sumber daya tersebut memiliki karakter simbol sehingga ditolak sistem.
>
>   #### Apa yang harus dilakukan?
>   1. Buka template excel
>   2. Cek kolom `UOM`
>   3. Cari berdasarkan kode yang ditunjuk
>   4. Periksa apakah ada simbol
>   5. Ubah satuan

### `Kode Error #018`

>   #### Contoh Sampel Notifikasi
>   Kode Sumber Daya : A2C004 tidak bisa mapping ke Kode Master E22 apabila jenis sumber daya berbeda. [#018]
>
>   #### Apa artinya?
>   Ditolak sistem karena jenis sumber daya berbeda, kode E hanya untuk sumber daya Subkon. Identifikasi jenis sumber daya berdasarkan karakter awal pada kode, perhatikan tabel.
>
> <img src="../assets/pmcs/drawio_kodeawalsbd.svg" alt="gbr-identifikasi-sbd"/>
>
>   #### Apa yang harus dilakukan?
>   1. Buka template excel
>   2. Cek kolom **Kode Master**
>   3. Cari berdasarkan kode sumber daya yang ditunjuk
>   4. Ubah kode master menyesuaikan jenis sumber daya

### `Kode Error #026`

>   #### Contoh Sampel Notifikasi
>   Satuan Sumber Daya untuk kode : A10008 tidak boleh kosong. Satuan wajib diisi. [#026]
>
>   #### Apa artinya?
>   Anda belum mengisi kolom satuan sumber daya sehingga ditolak sistem.
>
>   #### Apa yang harus dilakukan?
>   1. Buka template excel
>   2. Cek kolom `UOM`
>   3. Cari berdasarkan kode sumber daya yang ditunjuk
>   4. Isi satuan

*[PMCS]: Project Monitoring & Control System
