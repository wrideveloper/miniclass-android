# Activity Lifecycle

Developer yang baik harus mengetahui secara detail tentang _life cycle_ sebuah activity. Terutama untuk melakukan aksi yang tepat, saat terjadi perubahan _state_ activity. _Callback methods_ yang ada dapat digunakan untuk melakukan beragam proses terkait state dari activity. ****Misalnya melakukan semua inisialisasi komponen di `onCreate()`, melakukan _disconnect_ terhadap koneksi ke _server_ pada `onStop()`atau `onDestroy()`dan lain sebagainya.

Pemahaman yang baik tentang daur hidup _activity_ akan membuat implementasi rancangan aplikasi Kamu menjadi lebih baik. Hal ini juga akan meminimalisir terjadinya _error_ /_bug_/_force_ _close_ yang tidak diinginkan.

![Daur Hidup atau Lifecycle dari sebuah Activity](../.gitbook/assets/image.png)

* `onCreate()` adalah kondisi awal saat _Activity_ baru diciptakan, biasanya dilakukan inisialisasi pada tahapan ini.
* `onStart()` adalah saat _Activity_ dimulai
* `onResume()` adalah saat _Activity_ dibuka kembali, biasanya dieksekusi setelah `onPause()`
* `onPause()` akan dipanggil saat ada _Activity_ lain yang terbuka.
* `onStop()` adalah kondisi saat _Activity_ tidak ditampilkan dilayar \(biasanya saat pengguna menekan tombol Home\).
* `onRestart()` adalah kondisi saat _Activity_ kembali dibuka oleh pengguna.
* `onDestroy()` adalah kondisi saat _Activity_ dihancurkan pada memori.

**Stack\(Last In, First Out \(LIFO\)\) Pada Activity**

Perpindahan _Activity_ menggunakan konsep _Stack_ atau Tumpukan yang ada pada Struktur Data. Konsepnya sama seperti Tumpukan pada dunia nyata.

Misalnya Kamu sedang melakukan kegiatan bersih-bersih halaman rumahmu, Kamu diminta untuk menyusun ulang Batako-batako yang ada di halaman rumahmu. Tentu saja untuk menghemat ruang, batako tersebut akan Kamu susun secara bertumpuk. Ketika Kamu sedang menumpuk batako, operasi pada _Stack_ yang Kamu lakukan adalah **`Push`**, yaitu meletakkan batako baru di tumpukan batako yang sudah ada. Sedangkan ketika Kamu ingin mengambil atau mengeluarkan batako, pastinya yang akan Kamu ambil adalah yang **paling atas** terlebih dahulu. Operasi tersebut, jika pada _Stack_ disebut **`Pop`**.

Konsep itulah yang digunakan di _Activity_ Android. Untuk penjelasan lebih lengkapnya, Kamu bisa melihat ilustrasi di bawah ini:

![](../.gitbook/assets/image%20%283%29.png)

<table>
  <thead>
    <tr>
      <th style="text-align:left"><b>Gambar 1</b>
      </th>
      <th style="text-align:left">Gambar 2</th>
      <th style="text-align:left">Gambar 3</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">
        <p>Aktif: Activity 1</p>
        <p><b>onCreate()</b> &#x2192; <b>onStart()</b> &#x2192; <b>onResume()</b>
        </p>
      </td>
      <td style="text-align:left">
        <p>Aktif: Activity 2</p>
        <p>Stack append: Activity 2 [ <b>onCreate()</b> &#x2192; <b>onStart()</b> &#x2192; <b>onResume() </b>]</p>
      </td>
      <td style="text-align:left">
        <p>Activity 1</p>
        <p><b>onStart()</b> &#x2192; <b>onRestart()</b> &#x2192; <b>onResume()</b>
        </p>
      </td>
    </tr>
    <tr>
      <td style="text-align:left">Aksi: Klik Button1 (Pindah)</td>
      <td style="text-align:left">Aksi: Klik Hardware Back Button</td>
      <td style="text-align:left">Aktif: Activity 1</td>
    </tr>
    <tr>
      <td style="text-align:left">Stack push: Activity 1 [ <b>onPause() </b>&#x2192; <b>onStop() </b>]</td>
      <td
      style="text-align:left">Stack pop: Activity 2: [ <b>onPause() </b>&#x2192; <b>onStop()</b>&#x2192; <b>onDestroy()  </b>]</td>
        <td
        style="text-align:left"></td>
    </tr>
  </tbody>
</table>

