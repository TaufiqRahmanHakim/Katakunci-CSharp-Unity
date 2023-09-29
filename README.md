# Rangkuman Kata Kunci C# dalam Pemrograman Berorientasi Objek

Berikut adalah rangkuman dari beberapa kata kunci C# yang penting dalam pemrograman berorientasi objek.

## Access Modifiers

- **public**: Dapat diakses oleh semua orang.
- **private**: Hanya dapat diakses di dalam kelas itu sendiri.
- **protected**: Dapat diakses di dalam kelas itu sendiri dan kelas 'anak'nya.
- **internal**: Dapat diakses di dalam program yang sama.

## Storage Modifiers

- **static**: Milik kelas, bukan milik kelas 'anak'.
- **const**: Nilainya tetap dan tidak dapat diubah.
- **readonly**: Mirip dengan const, tetapi dapat diatur di awal.

## Kata Kunci untuk Pewarisan & Polimorfisme

- **virtual**: Dapat diubah di kelas 'anak'.
- **override**: Mengubah implementasi dari fungsi di kelas 'induk'.
- **abstract**: Kelas yang tidak dapat diinstansiasi sendiri, harus diwariskan terlebih dahulu.
- **sealed**: Kelas yang tidak dapat diwariskan lagi.

## Lain-lain

- **new**: Membuat versi baru dari fungsi atau variabel.
- **base**: Memanggil fungsi dari kelas 'induk'.
- **this**: Merujuk ke objek saat ini.
- **params**: Menerima banyak argumen.
- **ref**, **out**: Mengirim variabel sebagai referensi.
- **interface**: Mirip 'kontrak' untuk kelas lain.
- **enum**: Kumpulan nilai konstan.
- **delegate**: Menyimpan fungsi untuk dipanggil nanti.
- **event**: Mirip alarm untuk kode lain.


Instantiate : digunakan untuk membuat salinan dari suatu objek yang sudah ada. Ini bisa berupa GameObject, prefab, atau komponen lainnya.
Quaternion : berurusan dengan rotasi
Coroutine : Digunakan untuk eksekusi kode yang bisa 'pause' dan 'resume', sangat berguna untuk timing dalam animasi.

## Kata Kunci dan Fungsi yang Mendukung IEnumerator:
- **yield return null**: Menunda eksekusi sampai frame berikutnya.
- **yield return new WaitForSeconds(x)**: Menunda eksekusi selama x detik.
- **yield return StartCoroutine(anotherCoroutine())**: Menunggu sampai Coroutine lain selesai dijalankan.
- **StartCoroutine**: Fungsi untuk memulai Coroutine.
- **StopCoroutine**: Fungsi untuk menghentikan Coroutine.
- **StopAllCoroutines**: Fungsi untuk menghentikan semua Coroutine yang berjalan pada GameObject tersebut.
- **WaitForEndOfFrame**: Menunda eksekusi sampai semua rendering dan update selesai.
- **WaitForFixedUpdate**: Menunda eksekusi sampai FixedUpdate berikutnya dijalankan.
- **OnEnable/OnDisable**: Kadang digunakan untuk memulai atau menghentikan Coroutine ketika GameObject diaktifkan atau dinonaktifkan.
- **IEnumerator**: Tipe data yang harus kamu gunakan untuk mendefinisikan Coroutine.
- **yield break**: Mengakhiri Coroutine sebelum ia selesai.


## Kata Kunci dan Fungsi yang Mendukung Quartenion:
- **Quaternion.Angle**: Mengukur seberapa "jauh" antara dua posisi rotasi.
- **Quaternion.AngleAxis**: Membuat putaran berdasarkan sumbu (misalnya, sumbu Y) dan sudut (misalnya, 90 derajat).
- **Quaternion.Euler**: Membuat rotasi dari sudut-sudut yang biasa kita kenal, seperti memiringkan kepala ke atas atau ke bawah.
- **Quaternion.FromToRotation**: Membuat rotasi yang mengubah arah satu objek ke arah objek lain.
- **Quaternion.Inverse**: Membalik rotasi. Misalnya, jika objek terbalik, ini akan membalikkannya kembali.
- **Quaternion.Lerp**: Menggabungkan dua rotasi dengan cara yang lebih "kasar" atau cepat.
- **Quaternion.Slerp**: Menggabungkan dua rotasi dengan cara yang lebih "halus" atau akurat.
- **Quaternion.LookRotation**: Membuat objek "melihat" ke arah tertentu, seperti kamera mengikuti karakter.
- **Quaternion.RotateTowards**: Memutar objek ke arah tertentu dengan kecepatan yang bisa diatur.
- **Quaternion.Set**: Menentukan rotasi dengan angka-angka spesifik.
- **Quaternion.SetFromToRotation**: Sama seperti FromToRotation, tapi langsung mengubah rotasi objek.
- **Quaternion.SetLookRotation**: Sama seperti LookRotation, tapi langsung mengubah rotasi objek.

## Kata Kunci dan Fungsi yang Mendukung Random:
- **Random.Range**: Menghasilkan angka acak antara dua angka. Misalnya, untuk mendapatkan angka antara 1 dan 10.
- **Random.value**: Menghasilkan angka float acak antara 0 dan 1. Bisa digunakan untuk probabilitas.
- **Random.ColorHSV**: Menghasilkan warna acak dalam format HSV.
- **Random.InitState**: Mengatur "seed" untuk generator angka acak, sehingga kamu bisa mendapatkan urutan angka acak yang sama setiap kali.
- **Random.insideUnitCircle**: Menghasilkan titik acak dalam lingkaran dengan radius 1.
- **Random.insideUnitSphere**: Menghasilkan titik acak dalam bola dengan radius 1.
- **Random.onUnitSphere**: Menghasilkan titik acak di permukaan bola dengan radius 1.

## Kata Kunci dan Fungsi yang Mendukung Raycast:
Physics.Raycast: Metode utama untuk melakukan raycasting. Ini akan mengirimkan "ray" (sinar) dan memberi tahu kamu apakah sinar tersebut mengenai sesuatu.

Physics.RaycastAll: Mirip dengan Raycast, tapi ini akan mengembalikan semua objek yang terkena sinar.

Physics.SphereCast: Seperti Raycast, tapi menggunakan bola, bukan sinar. Berguna untuk deteksi yang lebih luas.

Physics.BoxCast: Seperti Raycast, tapi menggunakan kotak.

Physics.CapsuleCast: Seperti Raycast, tapi menggunakan kapsul.

Physics.RaycastNonAlloc: Versi lebih efisien dari Raycast yang tidak mengalokasikan memori baru.
