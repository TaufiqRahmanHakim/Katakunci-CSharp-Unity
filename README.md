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
