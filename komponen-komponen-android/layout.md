# Layout pada Android

Layout adalah suatu tampilan tata letak di android studio untuk mengatur penempatan text/gambar yang sudah terkonsep. Jadi layout di sini adalah bagian terpenting untuk memperindah tampilan pada aplikasi yang kita buat nyaman di lihat bagi pengguna. 

Terdapat 5 jenis layout pada android studio yang bisa digunakan untuk merancang tampilan aplikasi semenarik mungkin, yaitu:

## Linear Layout

Linear Layout merupakan jenis layout yang menyejajarkan semua komponen yang akan digunakan dalam satu arah, yaitu horizontal atau vertikal. Linear Layout dibuka dengan tag ```<LinearLayout>``` dan ditutup dengan tag ```</LinearLayout>```. Untuk menentukan arah (horizontal atau vertikal) dari Linear Layout yaitu dengan menambahkan atribut ```android:orientation``` pada tag pembuka Linear Layout.

Contoh implementasinya adalah sebagai berikut:


## Relative Layout

Relative Layout merupakan jenis layout yang mana untuk pengaturan layoutnya secara relative (bebas) sehingga tidak sebatas horizontal atau vertikal saja. Untuk kode xml dari Relative Layout sendiri dibuka dengan tag ```<RelativeLayout>``` dan ditutup dengan tag ```</RelativeLayout>```.

Contoh implementasinya adalah sebagai berikut:


## Table Layout

Table Layout merupakan jenis layout yang digunakan untuk merancang tampilan menyerupai tabel yang mana terdiri dari baris dan kolom. Meskipun namanya Table Layout, layout ini tidak akan menampilkan garis kolom, baris, atau sel. Layout ini dibuka dengan tag ```<TableLayout>``` dan ditutup dengan tag ```</TableLayout>```.

Contoh implementasinya adalah sebagai berikut:


## Frame Layout

Frame Layout merupakan jenis layout yang dipergunakan jika menginginkan tampilan dengan komponen tumpang tindih. Misalnya ialah memasukkan komponen Button pada komponen Image. Tag pembuka dari layout ini yaitu ```<FrameLayout>``` dan penutupnya adalah ```</FrameLayout>```.

Contoh implementasinya adalah sebagai berikut:


## Constraint Layout

Constraint Layout adalah jenis layout terbaru di android studio. Constraint Layout sendiri merupakan pengembangan dari Linear Layout. Dengan menggunakan layout ini kita dapat membuat sebuah tampilan aplikasi yang lebih responsif dan powerfull. Lebih resposif dan powerfull dikarenakan cara kerja layout ini adalah dengan saling bergantungan antar komponen.

Contoh implementasinya adalah sebagai berikut:
