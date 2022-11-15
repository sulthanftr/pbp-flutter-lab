## Perbedaan `Navigator.push` dan `Navigator.pushReplacement`.
| `Navigator.push` | `Navigator.pushReplacement` |
|--|--|
| Sebuah method untuk _push_ sebuah route ke stack Navigator	| Mengganti route yang saat ini ditampilkan dengan sebuah route baru dan _push_ route baru ke stack Navigator

## Daftar _Widget_ yang Digunakan pada Proyek ini beserta Fungsinya
- Navigator
	- Widget yang mengelola sekumpulan widget _child_ dengan struktur stack.
 - Expanded
	 - Widget yang memperluas _child_ dari Row, Column, atau Flex sehingga mengisi ruang yang tersedia.
 - Text
	 - Menampilkan tulisan dengan satu _style_
 - Column
	 - Menampilkan susunan isi _widget_ / _children_ secara vertikal
 - Center
	 - Menengahkan posisi _children_ dalam tampilan
 - Row
	 - Menampilkan susunan _children_ secara horizontal
 - Visibility
	 - Menampilkan atau menyembunyikan suatu _child_
 - Container
	 - Penampung berbagai _widget_ untuk menerapkan posisi, ukuran, dan _property_ lainnya secara seragam
 - MainAxisAlignment
	 - Menempatkan _children_ sepanjang sumbu utama dalam sebuah layout _flex_
 - EdgeInsets
	 - Memberikan _Offset_ pada 4 arah kardinal yang bersifat _immutable_

## Jenis-jenis _event_ yang ada pada Flutter
- `onPressed()`
- `onChanged()`
- `onSaved()`

## Cara `Navigator` "mengganti" halaman dari aplikasi Flutter.
Navigator bekerja menggunaan struktur data _stack_. Setiap tampilan halaman atau _route_ di _push_ ke stack Navigator untuk ditampilkan. _Route_ yang berada di paling atas _stack_ menjadi _route_ yang ditampilkan saat ini. Navigator mengganti halaman dengan operasi _pop_ atau _push_ pada route saat ini stack.

## Implementasi Tugas
1. Buat komponen Drawer untuk menavigasi ke _route_ lain.
2. Buat halaman form untuk membuat Budget baru. Form berisi field judul budget, nominal budget, dan jenis.
3. Buat TextField untuk judul dan nominal, sementara buat DropdownButtonFormField untuk jenis. Pilihan pada _dropdown_ terdiri dari 'Pengeluaran' dan 'Pemasukan'
4. Buat tombol untuk menyimpan input pada form budget dengan TextButton. pastikan semua field terisi saat akan tersimpan dengan menambahkan `validator` pada masing-masing field.
5. Buat sebuah list kosong global untuk menyimpan setiap data budget yang didapat dari submisi form.
6. Buat halaman list budget untuk menampilkan setiap data budget dalam bentuk _cards_
7. Impor file .dart dari halaman form untuk mengakses list budget
8. Buat tampilan untuk setiap elemen pada list menggunakan builder `ListView.builder()`
9. Tetapkan value `itemCount` dari builder sebagai panjang list budget
10. Buat widget `Card` yang menampilkan judul, nominal, dan jenis suatu budget, lalu tetapkan widget tersebut sebagai `itemBuilder` dari builder
