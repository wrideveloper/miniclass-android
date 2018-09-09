#  Android Lifecycle
![Android lifecycle](lifecycle.png)

## Activity Lifecycle
Berikut penjelasan fungsi dari tiap method di atas :
* **onCreate()**

         Di-method ini Activity sudah dimulai tapi belum terlihat oleh pengguna.
* **onStart()**

         Activity sudah terlihat tapi belum bisa berinteraksi.   
- **onResume()**

         Activity sudah terlihat dan pengguna sudah dapat berinteraksi.
- **onPause()**

         Activity sudah akan bersiap-siap meninggalkan layar (masih terlihat) dan sudah tidak berinteraksi dengan pengguna. 
- **onStop()**

         Kebalikan dari **onStart()** Activity sudah tidak terlihat.
- **onDestroy()**

         Kebalikan dari **onCreate()**. Method ini dapat terpanggil karena memanggil method **finish()** atau karena sistem membutuhkan memori lebih. Di dalam **onDestroy()** kita biasanya membersihkan proses-proses yang ada di belakang layar. Misalnya pengunduhan data dari internet yang mungkin masih berjalan jika tidak dihentikan di **onDestroy()**.    
- **onRestart()**            
         Dipanggil saat activity sudah melalui **onStop()** tapi akan diaktifkan lagi. Method ini jarang di implementasi. 

**Selengkapnya tentang Android -** https://www.codepolitan.com/memahami-activity-lifecycle-di-android-598d779a83dbf