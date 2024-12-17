# 362358302106_Fitri ayu wulan sari

### Soal 3
1. Jelaskan fungsi keyword yield* pada kode tersebut!
Answer : Penjelasan Fungsi yield*:
Keyword yield* dalam Dart digunakan untuk mendelegasikan pengembalian elemen dari iterable atau stream lain. Artinya, jika Anda menggunakan yield* untuk sebuah iterable atau stream, maka semua elemen dari iterable atau stream tersebut akan dipancarkan (dikirim) satu per satu ke luar fungsi generator.

Dengan kata lain, yield* membiarkan hasil dari iterable atau stream lain "diteruskan" sebagai bagian dari fungsi generator.

2. Apa maksud isi perintah kode tersebut?
Answer : 

1. **`Stream.periodic`**  
   Fungsi ini membuat *stream* yang memancarkan (menghasilkan) nilai pada interval tertentu.  
   - Argumen pertama: `const Duration(seconds: 1)` menyatakan bahwa nilai akan dipancarkan setiap 1 detik.  
   - Argumen kedua: Sebuah fungsi yang menerima waktu `t` (jumlah pemanggilan periodik) dan menghasilkan nilai tertentu.

2. **`t % colors.length`**  
   Ini adalah operasi modulus (`%`) yang memastikan bahwa nilai `t` akan diubah menjadi **index** dalam rentang `[0, colors.length - 1]`. Jika `t` bertambah terus, maka nilai index akan "berputar" kembali ke awal saat mencapai panjang `colors`.

3. **`colors[index]`**  
   Fungsi tersebut akan mengambil elemen dari list `colors` berdasarkan nilai index yang telah dihitung.

4. **`yield*`**  
   Keyword `yield*` digunakan untuk **meneruskan hasil stream** yang dibuat oleh `Stream.periodic`. Jadi, setiap hasil dari `Stream.periodic` akan dikirimkan ke luar fungsi generator, satu per satu, setiap detik.

### Soal 5
1. Jelaskan perbedaan menggunakan listen dan await for 
Answer: 
Gunakan listen jika:
Membutuhkan kontrol lebih (seperti pause/resume stream).
Ingin menangani error atau selesai stream dengan callback terpisah.

Gunakan await for jika Anda:
Membutuhkan cara sederhana untuk membaca stream sampai selesai.
Ingin menulis kode yang lebih bersih dan mudah dibaca.


A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://docs.flutter.dev/cookbook)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.
