# Proyek Materi React Fundamental dicoding.

Silahkan Mengecek Branch



V2
---
New Criteria :



----------------------------

V1
---
Criteria

# Proyek Materi React Fundamental dicoding.

## Kriteria Utama 1: Minimal terdapat 2 halaman yang berbeda
Berikut detail dari kriterianya.

Halaman 1: menampilkan daftar catatan.
Halaman 2: menampilkan detail catatan atau catatan secara tunggal.


## Kriteria Utama 2: Daftar catatan
Berikut detail dari kriterianya.

Menampilkan daftar catatan dengan data awal (initial data) yang kami sediakan.
Data yang ditampilkan pada daftar catatan adalah
judul catatan (title),
waktu pembuatan (createdAt), dan
isi catatan (body).
Terdapat conditional rendering di mana bila tidak terdapat data catatan, UI menampilkan pesan “Tidak ada catatan” atau pesan apa pun yang mengindikasikan data catatan kosong.


## Kriteria Utama 3: Detail catatan
Berikut detail dari kriterianya.

Menampilkan catatan tunggal yang dipilih pengguna dari daftar catatan aktif atau diarsipkan.
Menggunakan id catatan sebagai path parameter dalam menampilkan halaman detail catatan.
Catatan yang tampil harus sesuai dengan id yang terdapat pada path parameter.
Halaman Detil Catatan harus dapat diakses langsung dengan menggunakan URL.


## Kriteria Utama 4: Menambahkan catatan baru
Aplikasi mampu menambahkan catatan baru dengan kriteria berikut.

Memanfaatkan controlled component dalam membuat form input.
Data catatan disimpan cukup pada memori saja (akan hilang jika browser di-refresh). Kami sarankan untuk memanfaatkan fungsi menyimpan catatan yang disediakan.
Data catatan yang disimpan merupakan objek JavaScript dengan struktur berikut:
{
  id: string,
  title: string,
  body: string,
  archived: boolean, 
  createdAt: string,
}
Berikut contoh data riilnya:
{
  id: 'notes-1',
  title: "Babel",
  body: "Babel merupakan tools open-source yang digunakan untuk mengubah sintaks ECMAScript 2015+ menjadi sintaks yang didukung oleh JavaScript engine versi lama. Babel sering dipakai ketika kita menggunakan sintaks terbaru termasuk sintaks JSX.",
  archived: false,
  createdAt: '2022-04-14T04:27:34.572Z'
}
Catatan tambahan
Properti id pada tiap catatan yang disimpan haruslah unik. Tips dalam menetapkan nilai untuk adalah Anda bisa memanfaatkan nilai timestamp. Untuk mendapatkan nilai timestamp di JavaScript cukup mudah, cukup dengan menuliskan expressions +new Date().
Fungsi tambah catatan bisa ditampilkan pada halaman terpisah. Contohnya, pada URL /notes/new.


## Kriteria Utama 5: Menghapus catatan
Aplikasi mampu menghapus catatan yang tersimpan. Berikut detailnya.

Aplikasi harus menyediakan tombol hapus untuk menghapus data catatan yang disimpan.
Tombol hapus boleh diletakkan di mana saja, tetapi pastikan pengguna dapat mengaksesnya dengan baik. Sebagai contoh, Anda bisa menampilkan pada halaman detail catatan dan/atau daftar catatan.


## Kriteria Utama 6: Memvalidasi properti
Berikut detail dari kriterianya.

Memvalidasi seluruh masukkan (props) yang diterima komponen menggunakan PropTypes.
Sebelum mengirimkan submission, pastikan tidak ada warning terkait validasi komponen.


Selain kriteria utama, terdapat kriteria opsional yang yang dapat Anda penuhi agar mendapat nilai yang lebih tinggi.



## Kriteria Opsional 1: Arsip Catatan
Berikut detail dari kriterianya.

Catatan terarsip adalah catatan yang properti archived bernilai true.
Menyediakan halaman baru untuk menampilkan daftar catatan yang terarsip.
Data yang ditampilkan pada daftar catatan adalah
judul catatan (title),
waktu pembuatan (createdAt), dan
isi catatan (body).
Terdapat conditional rendering di mana bila tidak terdapat data catatan, maka UI menampilkan pesan “Arsip kosong” atau pesan apa pun yang mengindikasikan data catatan terarsip kosong.
Mengarsipkan catatan.
Aplikasi harus menyediakan tombol arsip dan batal arsip untuk mengarsipkan dan memindahkan catatan dari arsip.
Tombol arsip dan batal arsip bisa diletakkan di mana saja, tetapi pastikan pengguna dapat mengaksesnya dengan baik. Sebagai contoh, Anda bisa menampilkan pada halaman detail catatan dan/atau daftar catatan.


## Kriteria Opsional 2: Pencarian catatan
Berikut detail dari kriterianya.

Aplikasi memiliki fitur pencarian catatan berdasarkan kata kunci yang dimasukkan, dengan ketentuan:
Jika kolom pencarian tidak kosong, maka aplikasi hanya menampilkan daftar catatan yang judulnya mengandung kata kunci yang dimasukkan.
Jika kolom pencariannya kosong, maka aplikasi menampilkan seluruh catatan.
Memanfaatkan search parameter agar pencarian bersifat shareable melalui URL.
Memanfaatkan controlled component dalam membangun input pencarian.


## Kriteria Opsional 3: 404 Pages
Aplikasi menyediakan halaman khusus bila pengguna mengakses URL aplikasi dengan alamat yang tidak diketahui/diharapkan.

