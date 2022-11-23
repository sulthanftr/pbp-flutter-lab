
###  Apakah bisa kita melakukan pengambilan data JSON tanpa membuat model terlebih dahulu?
- Bisa, tetapi hanya baik dilakukan jika data JSON kecil. Jika ukuran data JSON sedang atau besar, disarankan untuk membuat model terlebih dahulu untuk menjaga kejelasan kode, kemudahan *refactoring*, dan efisiensi
	

###  Sebutkan widget apa saja yang kamu pakai di proyek kali ini dan jelaskan fungsinya.
- Stack: Memposisikan *children* relatif terhadap tepi-tepi kotak.
- Center: Menengahkan posisi _children_ dalam tampilan
- Text: Menampilkan tulisan dengan satu _style_
- TextSpan: Menampilkan teks *immutable* secara merentang
- SizedBox: Menampilkan sebuah box dengan ukuran tertentu
- RichText: Menampilkan berbagai teks yang menggunakan berbagai *style* berbeda.
- Container: Penampung berbagai _widget_ untuk menerapkan posisi, ukuran, dan _property_ lainnya secara seragam
- FutureBuilder: Widget yang membangun tampilan dirinya sendiri. Berguna untuk menampilkan berbagai widget yang sama dengan data yang berbeda.
- Column: Menampilkan susunan isi _widget_ / _children_ secara vertikal
- Row: Menampilkan susunan _children_ secara horizontal
 - MainAxisAlignment: Menempatkan _children_ sepanjang sumbu utama dalam sebuah layout _flex_
- EdgeInsets: Memberikan _Offset_ pada 4 arah kardinal yang bersifat _immutable_
###   Jelaskan mekanisme pengambilan data dari JSON hingga dapat ditampilkan pada Flutter.
1. Serialisasikan JSON secara manual atau automatis menggunakan *code generation*
2. Buat data JSON atau ambil data dari suatu *network*
3. Serialisasikan data JSON, simpan data kedalam suatu *query* atau *list*
4. Tampilkan data beserta atribut-atribut nya menggunakan sebuah *Widget*

###   Jelaskan bagaimana cara kamu mengimplementasikan  _checklist_  di atas.
1. Tambahkan dependensi HTTP pada proyek flutter agar dapat mengambil data dari internet
2. Buat model serialisasi data JSON dari MyWatchlist
3. Fetch data MyWatchlist secara asynchronous dari website heroku Tugas 3, kemudian serialisasi data tersebut
4. Buat halaman yang menampilkan berbentuk list dari objek-objek watchlist menggunakan data yang telah diserialisasi
5. Wrap setiap objek sebagai tombol dengan *routing* ke halaman detail watchlist
6. Buat halaman detail watchlist yang menampilkan atribut-atribut dari suatu objek MyWatchlist
