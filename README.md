# Nama : Muhammad Fauzan
# NPM  : 2406496302

# Readme Tugas 7

- [x] Membuat sebuah program Flutter baru dengan tema Football shop yang sesuai dengan tugas-tugas sebelumnya.
- [x] Membuat tiga tombol sederhana dengan ikon dan teks untuk product kamu:
    - [x] All Products
    - [x] My Products
    - [x] Create Product
- [x] Mengimplementasikan warna-warna yang berbeda untuk setiap tombol:
    - [x] Warna biru untuk tombol All Products
    - [x] Warna hijau untuk tombol My Products
    - [x] Warna merah untuk tombol Create Product
- [x] Memunculkan Snackbar dengan tulisan:
    - [x] "Kamu telah menekan tombol All Products" ketika tombol All Products ditekan.
    -[x] "Kamu telah menekan tombol My Products" ketika tombol My Products ditekan.
    -[x] "Kamu telah menekan tombol Create Product" ketika tombol Create Product ditekan.
- [x] Jawab pertanyaan-pertanyaan berikut di file README.md pada folder root:
    - [x] Jelaskan apa itu widget tree pada Flutter dan bagaimana hubungan parent-child (induk-anak) bekerja antar widget.
    - Widget tree pada Flutter adalah struktur hierarki yang menggambarkan bagaimana setiap widget saling berhubungan dalam membentuk tampilan aplikasi. Setiap widget di Flutter memiliki peran sebagai parent (induk) atau child (anak), di mana parent widget bertanggung jawab untuk mengatur tata letak, posisi, dan perilaku dari child widget di dalamnya. Misalnya, widget Scaffold bisa menjadi induk dari AppBar dan Body, sedangkan di dalam Body bisa terdapat Column yang memiliki beberapa anak seperti Text dan Button. Hubungan ini membuat Flutter bekerja secara deklaratif — perubahan pada data atau struktur widget akan menyebabkan rebuild pada bagian pohon yang terdampak, sehingga tampilan selalu sesuai dengan kondisi terkini aplikasi.
    - [x] Sebutkan semua widget yang kamu gunakan dalam proyek ini dan jelaskan fungsinya.
    - Widget yang digunakan dalam proyek ini antara lain Scaffold, AppBar, Text, Padding, Column, Row, SizedBox, Center, GridView.count, Card, Container, Material, InkWell, Icon, dan SnackBar.Masing-masing berfungsi membentuk tampilan antarmuka aplikasi: Scaffold menjadi kerangka utama layar, AppBar menampilkan judul di bagian atas, Column dan Row mengatur tata letak vertikal dan horizontal, Card serta Container menampilkan konten dengan batas dan jarak tertentu, GridView.count menampilkan daftar item dalam bentuk grid, Material dan InkWell memberikan efek klik interaktif, sedangkan SnackBar menampilkan notifikasi saat item ditekan.
    - [x] Apa fungsi dari widget MaterialApp? Jelaskan mengapa widget ini sering digunakan sebagai widget root.
    - Widget MaterialApp berfungsi sebagai kerangka utama aplikasi Flutter yang menerapkan gaya dan prinsip desain Material Design dari Google. Widget ini menyediakan pengaturan global seperti tema warna (theme), judul aplikasi (title), navigasi antar halaman (routes, navigator), serta pengelolaan status aplikasi. Karena fungsinya yang menyatukan seluruh konfigurasi inti aplikasi, MaterialApp hampir selalu digunakan sebagai widget root, agar semua widget di bawahnya dapat mewarisi tampilan, tema, dan perilaku yang konsisten sesuai standar Material Design.
    - [x] Jelaskan perbedaan antara StatelessWidget dan StatefulWidget. Kapan kamu memilih salah satunya?
    StatelessWidget adalah widget yang tidak memiliki state atau data yang bisa berubah selama aplikasi berjalan; tampilannya hanya bergantung pada data yang diberikan saat pertama kali dibuat. Contohnya seperti teks, ikon, atau tombol yang tidak berubah.Sedangkan StatefulWidget adalah widget yang memiliki state dinamis, artinya tampilannya bisa berubah seiring waktu, misalnya saat pengguna berinteraksi, menekan tombol, atau data diperbarui. Kamu memilih StatelessWidget ketika tampilan bersifat tetap dan tidak perlu pembaruan, sedangkan StatefulWidget digunakan saat tampilan harus merespons perubahan data atau input pengguna.
    - [x] Apa itu BuildContext dan mengapa penting di Flutter? Bagaimana penggunaannya di metode build?
    - BuildContext adalah objek yang merepresentasikan posisi atau lokasi sebuah widget di dalam widget tree. Objek ini penting karena memungkinkan widget untuk berinteraksi dengan lingkungan sekitarnya—misalnya mengakses theme, media query (ukuran layar), atau ancestor widget seperti Scaffold dan Navigator. Dalam metode build(), BuildContext digunakan untuk membangun tampilan berdasarkan konteksnya, misalnya memanggil Theme.of(context) untuk mengambil warna tema atau ScaffoldMessenger.of(context) untuk menampilkan SnackBar. Tanpa BuildContext, widget tidak akan tahu di mana posisinya berada di dalam hierarki aplikasi Flutter.
    - [x] Jelaskan konsep "hot reload" di Flutter dan bagaimana bedanya dengan "hot restart".
    - Hot reload di Flutter adalah fitur yang memungkinkan pengembang melihat hasil perubahan kode secara instan tanpa kehilangan state aplikasi yang sedang berjalan, seperti data input atau posisi halaman saat ini. Flutter hanya memperbarui bagian kode yang diubah, sehingga prosesnya sangat cepat dan efisien untuk iterasi desain dan logika UI. Sedangkan hot restart akan memulai ulang seluruh aplikasi dari awal, artinya semua variabel, state, dan data sementara akan hilang — mirip seperti menjalankan ulang aplikasi dari nol. Jadi, perbedaannya: hot reload mempertahankan state, sedangkan hot restart mengulang aplikasi sepenuhnya.
- [x] Melakukan add-commit-push ke suatu repositori baru di GitHub.