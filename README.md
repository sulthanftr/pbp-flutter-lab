## *Stateless widget* dan *Stateful widget*
| _Stateless widget_ | _Stateful widget_ |
|--|--|
| Suatu _widget_ dikatakan _stateless_ jika _widget_ tersebut tidak dapat berubah sama sekali meskipun dilakukan interaksi terhadapnya. | Sementara, suatu _widget_ dikatakan _stateful_ jika _widget_ tersebut dapat berubah (tampilan, warna, dll.) ketika sesuatu terjadi seperti sebuah interaksi oleh user.

## Daftar _Widget_ yang Digunakan pada Proyek ini beserta Fungsinya
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

## Method `setState()`
Digunakan untuk mengubah _state_ internal dari sebuah objek sekaligus memperbarui tampilan. Jika perubahan _state_ tidak menggunakan `setState()`, perubahan tidak langsung diperbarui pada tampilan aplikasi.
## Perbedaan antara `const` dan `final`
Kedua variabel ini tidak dapat diubah setelah diinisialisasikan. value dari `const` harus diketahui pada _compile-time_, semetara value dari `final` harus diketahui pada _run-time_

## Implementasi Tugas

 1. Menambahkan 2 variabel pada `_MyHomePageState`
	 - `_condition` untuk menyimpan string sifat angka ("GENAP" atau "GANJIL")
	 - `_color` untuk menyimpan warna string `_condition`
2. Membuat fungsi `_decrementCounter()` untuk mengurangi `_counter` dengan 1. Jika `_counter` = 0, tidak melakukan apa-apa
3. Membuat fungsi `_changeCondition()`
	- Jika `_counter` genap atau 0,
		- `_condition = "GENAP"`
		- `_color = Colors.red`
	- Jika ganjil,
		- `_condition = "GANJIL"`
		- `_color = Colors.blue`
4. Tambahkan `FloatingActionButton` yang memanggil `_decrementCounter()` dan terletak di pojok kanan bawah tampilan aplikasi
5. Tambahkan _widget_ `Visibility` yang menyembunyikan tombol pada step sebelumnya jika `_counter` < 1
