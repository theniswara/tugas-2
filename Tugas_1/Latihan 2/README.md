# Penjelasan

```java
public class PencarianArray {
// Mendefenisikan kelas dengan nama PencarianArray

    public static void main(String[] args) {
    // Mendefinisikan main method, Method yang akan dieksekusi pertama kali ketika program dijalankan

        // Program mencari nilai dalam array
        int[] nilai = {75, 80, 65, 90, 85, 70, 95, 88};
        // Mendeklarasi dan inisiasi array dengan nama nilai bertipe int yang berisi 8 elemen

        int cari = 90;
        // Mendeklarasi dan inisialisasi variabel cari tipe int, dengan nilai 90

        boolean ketemu = false; 
        // Mendeklarasi variabel ketemu dengan tipe boolean dan menginisiasi dengan nilai false

        int indeks = -1;
        // Mendeklarasi variabel indeks tipe int dengan inisiasi dengan nilai -1

        // Mencari nilai
        for (int i = 0; i < nilai.length; i++) {
        // Menggunakan perulangan for untuk mencari nilai cari dalam array nilai, i dimulai dari 0 dan berjalan hingga kurang dari panjang array

            if (nilai[i] == cari) {
            // Memeriksa apakah elemen array pada index i sama dengan nilai yang dicari

                ketemu = true;
                // Jika ditemukan, ketemu berubah menjadi true

                indeks = i;
                // indeks diisi dengan nilai i 

                break;
                // Perulangan dihentikan
            }
        }

        // Menampilkan hasil
        if (ketemu) {
            System.out.println("Nilai " + cari + " ditemukan pada indeks " + indeks);
        // Jike ketemu bernilai true, program mencetak pesan beserta indeksnya

        } else {
            System.out.println("Nilai " + cari + " tidak ditemukan");
        // Jika ketemu bernilai false, program mencetak nilai tidak ditemukan.

        }
    }
}

```