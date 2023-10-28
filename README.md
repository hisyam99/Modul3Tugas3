# Aplikasi Menghitung Deret Fibonacci Menggunakan Konsep Iteratif

**FibonacciIterative** adalah kelas Java yang dibuat untuk menghitung deret Fibonacci secara iteratif. Deret Fibonacci adalah urutan angka di mana setiap angka adalah jumlah dari dua angka sebelumnya. Kelas ini menyediakan metode untuk menghitung deret Fibonacci hingga suatu nilai tertentu dan juga menyertakan contoh penggunaan dalam metode `main`. Dokumentasi ini akan menjelaskan cara menggunakan kelas FibonacciIterative dan memberikan informasi tentang struktur kode.

## Pengantar

Deret Fibonacci adalah urutan angka yang dimulai dengan 0 dan 1, di mana setiap angka berikutnya adalah penjumlahan dari dua angka sebelumnya. Dalam kelas `FibonacciIterative`, deret Fibonacci dihitung secara iteratif menggunakan perulangan.

## Penggunaan

Untuk menggunakan kelas `FibonacciIterative`, kita perlu mengikuti langkah-langkah berikut:

1. **Instansiasi Objek FibonacciIterative**: Buat objek `FibonacciIterative` dengan menyediakan nilai yang ingin Anda hitung dalam deret Fibonacci.

   ```java
   FibonacciIterative fibonacci = new FibonacciIterative(nilai);
   ```

   Gantilah `nilai` dengan nilai yang ingin Anda hitung dalam deret Fibonacci.

2. **Hitung Deret Fibonacci**: Panggil metode `calculate()` pada objek `FibonacciIterative` yang telah kita buat tadi untuk menghitung deret Fibonacci hingga nilai yang telah ditentukan.

   ```java
   long result = fibonacci.calculate();
   ```

   Hasil perhitungan deret Fibonacci akan disimpan dalam variabel `result`.

3. **Pengukuran Waktu Eksekusi**: Kode ini juga mencatat waktu yang diperlukan untuk menghitung deret Fibonacci. Hasil pengukuran waktu akan ditampilkan dalam milidetik.

4. **Menampilkan Hasil**: Kita dapat menampilkan hasil perhitungan deret Fibonacci dan waktu eksekusi dengan menggunakan perintah berikut:

   ```java
   System.out.println("Iteratif: Hasil = " + result + ", Waktu = " + duration + " ms");
   ```

## Contoh Penggunaan

Contoh penggunaan dalam metode `main` yang menghitung deret Fibonacci untuk beberapa nilai yang berbeda.

```java
int[] numbers = {100, 1000, 5000, 10000};

for (int nilai : numbers) {
    FibonacciIterative fibonacci = new FibonacciIterative(nilai);
    double startTime = System.currentTimeMillis();
    long result = fibonacci.calculate();
    double endTime = System.currentTimeMillis();
    double duration = endTime - startTime; // durasi dalam milidetik

    System.out.println("nilai = " + nilai);
    System.out.println("Iteratif: Hasil = " + result + ", Waktu = " + duration + " ms");
    System.out.println();
}
```

Kode diatas menghitung deret Fibonacci untuk nilai-nilai yang berbeda dan melihat hasil perhitungannya.

## Lisensi

Kode dalam proyek ini dilisensikan di bawah [Lisensi MIT](LICENSE).