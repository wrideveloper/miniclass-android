# Android Manifest

Android Manifest merupakan salah satu yang otomatis akan dibuat ketika membuat project baru dengan Android Studio. Di dalam Android manifest sendiri menjelaskan informasi - informasi penting tentang aplikasi Android yang dibuat ke fitur build Android, sistem operasi Android, dan Google Play. Informasi - informasi tersebut di antaranya ialah:
<ul>
  <li>
    Nama paket aplikasi, yang biasanya menyesuaikan namespace kode. Fitur build Android menggunakan ini untuk menentukan lokasi entitas kode saat membuat project Anda. Saat mengemas aplikasi, fitur build akan mengganti nilai ini dengan ID aplikasi dari file build Gradle, yang digunakan sebagai identifier aplikasi di sistem dan Google Play.
  </li>
  <li>
    Komponen aplikasi, yang meliputi seluruh aktivitas, layanan, penerima siaran, dan penyedia materi. Tiap komponen harus menentukan properti dasar seperti nama Kotlin atau class Java. Komponen tersebut juga mendeklarasikan kemampuan seperti konfigurasi perangkat yang bisa ditangani, dan filter intent yang menjelaskan cara komponen bisa dimulai.
  </li>
  <li>
    Izin yang diperlukan aplikasi untuk mengakses bagian sistem atau aplikasi lain yang dilindungi. Ini juga mendeklarasikan semua izin yang harus dimiliki aplikasi jika mereka ingin mengakses materi dari aplikasi ini.
  </li>
  <li>
    Fitur hardware dan software yang diperlukan aplikasi, yang memengaruhi perangkat mana yang bisa menginstal aplikasi dari Google Play.
  </li>
</ul>
