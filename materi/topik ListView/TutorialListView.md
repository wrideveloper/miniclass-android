# Menerapkan ListView pada Android Studio
Pada tutorial kali ini, kita akan mengisi Fragment yang telah dibuat pada tutorial sebelumnya dengan ListView.

## Pengertian ListView
ListView adalah View Group yang ditampilkan secara list dan dapat digulung(scrollable). Konten yang terdapat pada ListView, ditambahkan secara automatis menggunakan Adapter yang tugasnya mengambil konten dari beberapa sumber seperti Array atau Database, dan diubah(convert) menjadi ListView secara berurutan.

## Menyiapkan Layout yang digunakan
1. Pada tutorial fragment sebelumnya kita sudah membuat beberapa layout kosong. Sehingga kita akan menggunakan **HomeFragment dan mengisinya dengan listview.**
2. Buka layout **fragment_home.xml** `res/layout/fragment_home.xml` dan isi XML tersebut dengan kode dibawah :
  ```xml
  <?xml version="1.0" encoding="utf-8"?>
<FrameLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".HomeFragment">
  
    <ListView
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:id="@+id/listView1"
        />

</FrameLayout>
```
  Elemen `<ListView/>` pada *preview design* akan terlihat seperti gambar dibawah ini : 
  ((Gambar1))
  
3. Selanjutnya, buat XML baru dengan nama `list_layout.xml`, dengan target seperti :
((Gambar2))

Berikut kode yang dapat diisikan pada XML anda : 
  ```xml
  <?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    android:orientation="horizontal"
    android:layout_width="match_parent"
    android:layout_height="wrap_content"
    android:layout_margin="16dp"
    tools:context="com.example.fragmentandlistview.HomeFragment">
    <ImageView
        android:id="@+id/image"
        android:layout_width="90dp"
        android:layout_height="90dp"
        android:src="@drawable/ic_launcher_background"/>
    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:orientation="vertical"
        android:layout_marginLeft="9dp">
        <TextView
            android:id="@+id/textTitle"
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:text="Items"
            android:textSize="24sp"/>
        <TextView
            android:id="@+id/textDescription"
            android:layout_width="match_parent"
            android:layout_height="fill_parent"
            android:text="Description"
            android:layout_marginRight="12dp"
            android:maxLines="4"
            android:lines="4"
            android:textSize="16sp"/>
    </LinearLayout>
</LinearLayout>
  ```
  
