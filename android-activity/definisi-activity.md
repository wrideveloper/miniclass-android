# Activity

Activity  merupakan salah satu komponen penting Android yang berfungsi untuk menampilkan _user interface_ ke layar pengguna. Ini seperti pada saat Kamu melihat daftar percakapan pada aplikasi _chat_ atau daftar _email_ pada aplikasi Gmail di ponsel Android Kamu. Di dalamnya Kamu dapat berinteraksi dengan aplikasi Kamu, baik dengan menekan tombol atau menampilkan _list_.

Bila dibandingkan dengan aplikasi web dan desktop, _Activity_ sama seperti halaman dan _form_.

| Android | Web | Desktop |
| :--- | :--- | :--- |
| Activity | Page | Form |

Seperti ketika Kamu membuat project baru di Android Studio, biasanya akan ada dua berkas yang sudah tercipta, yaitu **MainActivity** dan **activity\_main.xml.** MainActivity ini disebut sebagai class Activity karena mewarisi \(_extends_\) _superclass_ Activity. Tugasnya yaitu menampilkan layout activity\_main.xml dan mengelola interaksi yang ada di dalamnya.  
  
Umumnya dalam sebuah aplikasi terdapat lebih dari satu activity ****yang saling terhubung dengan tugas yang berbeda-beda. Yang perlu diperhatikan yaitu setiap Activity harus terdaftar di **AndroidManifest.xml**_**.**_  Secara _default_, ia akan didaftarkan jika Kamu membuat Activity baru dengan cara otomatis. Caranya yaitu klik kanan pada nama package → New →  Activity →  pilih template Activity yang tersedia.

## Praktik: Aplikasi Penghitung Penggunaan Listrik Sederhana dengan Mengimplementasikan Activity

Pada materi sebelumnya, Kamu sudah belajar bagaimana cara melakukan _layouting_ pada Android. Sekarang, saatnya Kamu mencoba untuk membuat _layout_ tersebut menjadi fungsional dan bisa dioperasikan menggunakan Activity.

Aplikasi yang ingin dibuat adalah Aplikasi untuk menghitung Penggunaan Listrik Harian di Rumah sederhana. 

### Gambaran __Aplikasi

![Contoh layout aplikasi yang ingin dibuat](../.gitbook/assets/image%20%281%29.png)

* Terdapat **3 EditText** yang terdiri dari **Lampu, Televisi, AC, Kulkas** yang digunakan untuk memasukan jumlah penggunaan listrik\(dalam satuan watt**\)** dan **1 EditText** yang digunakan untuk memasukkan **Biaya Penggunaan Listrik per Watt**-nya.
* Terdapat **1 Button** yang digunakan untuk menghitung biaya penggunaan listrik.
* Terdapat **1** **TextView** yang digunakan untuk menampilkan hasil perhitungan biaya penggunaan listrik
* Untuk menghitung biaya penggunaan listrik, Kamu bisa menggunakan rumus:

```text
total = (lampu + televisi + kulkas + AC) * Biaya per watt
```

### _Flow_ Aplikasi

* Masukkan jumlah penggunaan listrik pada **Lampu, Televisi, AC, Kulkas** dan **Biaya Penggunaan Listrik per Watt**-nya.
* Setelah itu, tekan tombol **Hitung,** hasil akan perhitungan menggunakan rumus di atas akan tampil pada **TextView.**

