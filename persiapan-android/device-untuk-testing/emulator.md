# Emulator

Android Emulator adalah mesin android virtual atau biasa disebut AVD (Android Virtual Device) yang merepresentasikan suatu perangkat android tertentu di komputer anda tanpa harus memiliki perangkat aslinya.

## Membuat & Mengelola Android Emulator di Android Studio

Android Studio sudah menyediakan sebuah tool yang mana kita dapat membuat atau mengelola Android Emulator, tool tersebut ialah Android Virtual Device(AVD). Terdapat 3 cara membuka AVD di Android Studio. 

Pertama melalui Welcome Wizard Android Studio, di bagian Configure pilih AVD Manager

![Melalui Welcome Wizard Android Studio](https://user-images.githubusercontent.com/52988155/109598864-bf2c1400-7b4c-11eb-9469-ac9cb3287655.png) 

Kedua melalui menu Tools pada halaman Project Android Studio, Tools > AVD Manager

![Melalui Menu Tools](https://user-images.githubusercontent.com/52988155/109599203-6315bf80-7b4d-11eb-8bf5-1a35f7fae1ab.png)

Ketiga melalui Toolbar Android Studio, AVD Manager berada di nomor empat dari sebelah kanan toolbar

![Melalui Toolbar](https://user-images.githubusercontent.com/52988155/109599563-fa7b1280-7b4d-11eb-924a-646fe4bd6661.png)

Setelah masuk pada AVD Manager, akan ditampilkan daftar emulator yang pernah dibuat. Pada bagian awal akan ditampilkan satu buah emulator yang mana emulator tersebut dibuat ketika proses penginstallan Android Studio. 

![AVD Manager](https://user-images.githubusercontent.com/52988155/109599704-39a96380-7b4e-11eb-80ac-310b448a60a7.png)

Kita dapat menggunakan emulator yang sudah ada pada AVD Manager atau jika ingin membuat emulator baru bisa mengikuti langkah - langkah berikut:
* Klik tombol Create Virtual Device yang ada di bagian kiri bawah

![Klik Create Virtual Device](https://user-images.githubusercontent.com/52988155/109600262-627e2880-7b4f-11eb-8d82-ded9a7cc89e1.png)

* Pilih hardware yang dibutuhkan. Terdapat berbagai macam hardware dan tipe hardware yang sudah disediakan oleh Android Studio, mulai dari TV, Phone, Wear OS, Tablet dan Automotive.

![Pilih Hardware](https://user-images.githubusercontent.com/52988155/109600483-c7d21980-7b4f-11eb-9041-91b497e36d8f.png)

* Jika tidak menemukan hardware yang sesuai, kita bisa membuat hardware sendiri dengan spesifikasi keinginan kita. Caranya adalah dengan klik tombol New Hardware Profile dan mengisi spesifikasi emulator yang kita inginkan.

![Custom Hardware](https://user-images.githubusercontent.com/52988155/109600870-7b3b0e00-7b50-11eb-91d2-0900e4d4a3db.png)

* Setelah memilih hardware yang sesuai, akan diarahkan untuk memilih System Image atau Android yang akan ditanamkan pada hardware. Jika System Image yang akan dipilih maka silahkan download terlebih dahulu dengan klik Download

![Pilih Android System](https://user-images.githubusercontent.com/52988155/109601066-d3721000-7b50-11eb-802f-4cbe4a74ddc5.png)

* Selanjutnya akan ditampilkan hasil konfigurasi yang telah kita lakukan sebelumnya, di bagian ini kita bisa mengganti nama emulator sesuai keinginan. Dan jika semuanya sudah sesuai silahkan klik Finish.

![Verify Configuration](https://user-images.githubusercontent.com/52988155/109601826-2ac4b000-7b52-11eb-95c2-5f8c61365c78.png)

* Setelah proses pembuatan selesai, maka emulator akan muncul di halaman awal AVD Manager

![Emulator selesai dibuat](https://user-images.githubusercontent.com/52988155/109601953-5f386c00-7b52-11eb-859e-a5456b6964c3.png)

* Untuk menjalankan emulator bisa klik tombol Play yang terdapat pada kolom Actions, dan berikut hasil ketika emulator berhasil dijalankan

![Menjalankan Emulator](https://user-images.githubusercontent.com/52988155/109602380-97d84580-7b52-11eb-9538-41ba3acaf7a8.png)


## Menjalankan Aplikasi dengan Android Emulator

Untuk menjalankan Aplikasi yang sudah dibuat menggunakan Android Emulator, silahkan buka project Android menggunakan Android Studio, kemudian pada bagian toolbar pilih emulator yang akan digunakan untuk menjalankan Aplikasi.

![Memilih Android Emulator](https://user-images.githubusercontent.com/52988155/109602655-1a610500-7b53-11eb-95f6-5eb49ad5fd99.png)

Setelah memilih Android Emulator yang akan digunakan, klik tombol Play yang berada tepat di sebelah kanan toolbar untuk memilih emulator. And Congratulations... Your App will running on Android Emulator. 😄
