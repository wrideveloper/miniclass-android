---
description: >-
  Mengenal List pada aplikasi Android dan komponen RecyclerView untuk
  membuatnya.
---

# List & RecyclerView

## List dalam Aplikasi Android

Pada dasarnya interaksi umum antara pengguna dengan aplikasi dalam menampilkan data dengan jumlah yang banyak adalah dengan menggunakan list yang bisa di-_scroll_ .

Jika kamu menggunakan berbagai macam aplikasi di HP Androidmu, tentu saja ada banyak sekali jenis-jenis _list_ yang kamu temukan dengan bentuk yang berbeda-beda. Ada yang bisa di _scroll_ dari atas ke bawah atau kiri ke kanan, Ada yang hanya berisi teks dan ada juga yang berisi gambar.

![Aplikasi Instagram yang menggunakan RecyclerView untuk menampilkan Detail Foto dan Highlight Stories.](../.gitbook/assets/ezgif.com-gif-maker-4-.gif)

## RecyclerView untuk Menampilkan List

Sebenarnya, Listview menjadi komponen pertama yang mengakomodasi penampilan List pada Aplikasi Android. Namun semenjak Google meluncurkan pendekatan Material Design, RecyclerView menjadi pilihan pertama yang harus digunakan. Kamu masih bisa menggunakan kedua komponen tersebut secara berdampingan dalam satu aplikasi.

RecyclerView adalah sebuah komponen tampilan _\(widget\)_ yang lebih canggih ketimbang pendahulunya ListView. Gambar di bawah menunjukkan perbedaan ListView dan RecyclerView, jika Kamu menggunakan ListView objek dari tiap item akan dibuat semuanya dari awal sampai akhir. Sedangkan jika Kamu menggunakan RecyclerView, objek yang dibuat hanya sebatas ukuran layar dan beberapa di atas dan di bawahnya saja. Selanjutnya ia menggunakan kembali item yang sudah tidak terlihat.

![Ilustrasi perbedaan ListView dan RecyclerView. Sumber: Dicoding](../.gitbook/assets/image%20%287%29.png)

Dampaknya sangat signifikan apabila data yang ditampilan berjumlah sangat banyak. Misalnya ada 1000 data yang akan ditampilkan, makan penggunaan RecyclerView akan lebih ramah memori.

## Ilustrasi Penerapan RecyclerView

![Ilustrasi penggunaan RecyclerView. Sumber: Dicoding](../.gitbook/assets/image%20%2812%29.png)

Penjelasan:

* Datasoure: Merupakan kumpulan data yang ingin ditampilkan. Biasanya data disimpan dalam sebuah `ArrayList`.
* Layout Item: Sebuah _file_ XML berisi tampilan dari setiap _item_. Kamu bisa melakukan kostumisasi tampilan sesuka hati dengan menambahkan berbagai Komponen View.
* Adapter: Merupakan sebuah komponen yang mengatur bagaimana data akan ditampilkan dan sebagai jembatan antara Layout Item dan RecyclerView. Untuk membuat Adapater, diperlukan untuk membuat sebuah _class_ khusus. ViewHolder di dalam Adapter berfungsi untuk melakukan _binding_ dan memasukan data ke dalam komponen di Layout Item.
* Layout manager: Berfungsi untuk mengatur posisi dari _list_ yang akan ditampilkan. Apakah dalam bentuk _list, grid_, atau _staggered_\(Grid dengan ukuran berbeda-beda, seperti pada _tab_ Explore Instagram\).

Sumber:

[Dicoding.com](https://www.dicoding.com/)

