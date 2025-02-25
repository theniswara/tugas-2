# Penjelasan

```java
public class StatistikArray {
// Mendefinisikan class bernama Stas    `

    public static void main(String[] args) {
    // Mendefinisikan main method, Method yang akan dieksekusi pertama kali ketika program dijalankan
    

        // Program menghitung statistik nilai siswa
        int[] nilai = {75, 80, 65, 90, 85, 70, 95, 88};
        // Mendeklarasi dan menginisiasi array bernama nilai yang berisi 8 elemen bertipe int

        // Mencari nilai tertinggi dan terendah
        int tertinggi = nilai[0];
        // Mendeklarasi dan inisialisasi variabel nilai dengan elemen pertama array, digunakan untuk menyimpan nilai tertinggi dalam array

        int terendah = nilai[0];
        // Mendeklarasi dan inisialisasi variabel nilai dengan elemen pertama array, digunakan untuk menyimpan nilai terendah dalam array

        int total = nilai[0];
        // Mendeklarasi dan inisialisasi variabel nilai dengan elemen pertama array, digunakan untuk menyimpan nilai total dalam array


        for (int i = 1; i < nilai.length; i++) {
        // Menggunakan perulangan for untuk mengterasi array nilai dari indeks 1 higga akhir array

            if (nilai[i] > tertinggi) tertinggi = nilai[i];
            // Jika elemen array pada index i lebih besar dari nilai tertinggi, jika ya tertinggi diudate dengan nilai itu
            
            if (nilai[i] < terendah) terendah = nilai[i];   
            // Jika elemen array pada index i lebih kecil dari nilai terendah, jika ya terendah diudate dengan nilai itu
             
            total += nilai[i];
            // Menambahkan nilai array pada indeks i ke variabel total
        }

        double rataRata = (double) total / nilai.length;
        // Menghitung rata - rata dari semua nilay array.

        System.out.println("Nilai tertinggi: " + tertinggi);
        // Mencetak nilai tertinggi

        System.out.println("Nilai terendah: " + terendah);
        // Mencetak nilai terendah

        System.out.println("Rata-rata: " + rataRata);
        // Mencetak nilai terendah
    }
}

```