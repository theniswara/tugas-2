# Penjelasan

```java

public class OperasiMatriks {
// Mendefinisikan kelas dengan nama OperasiMatriks 

    public static void main(String[] args) {
    // Mendefinisikan main method, Method yang akan dieksekusi pertama kali ketika program dijalankan


        // Program operasi matriks
        int[][] matriksA = {
            {1, 2, 3},
            {4, 5, 6}
        };
        // Mendeklerasikan dan menginisiasi array 2D dengan nama matriksA, memiliki 2 baris dan 3 kolom

        int[][] matriksB = {
            {7, 8, 9},
            {10, 11, 12}
        };
        // Mendeklarasikan dan menginisiasi array 2d dengan nama matriksB.

        // Penjumlahan matriks
        int[][] hasil = new int[2][3];
        // Mendeklarasikan array 2D dengan nama hasil, digunakan untuk menyimpan panjulahan matriksA dan matriksB

        for (int i = 0; i < matriksA.length; i++) {
        // Menggunakan nested loop untuk penjumlahan matriksA dan matriksB, mengiterasi setiap baris dari matriks
        
            for (int j = 0; j < matriksA[0].length; j++) {
            // Mengiterasi setiap kolom dari matriks.

                hasil[i][j] = matriksA[i][j] + matriksB[i][j];
                // Melakukan penjumlahan elemen matriks matriksA dan matriksB pada baris i dan kolom j, dan menyimpan hasilnya dalam matriks hasil.
            }
      

        }

        // Menampilkan hasil
        System.out.println("Hasil penjumlahan matriks:");
        // Mencetak teks "Hasil penjumlahan matriks:"

        for (int[] baris : hasil) {
        // Mengiterasi setiap baris dari matriks hasil.

            for (int nilai : baris) {
            // Mengiterasi setiap nilai dalam baris tersebut.

                System.out.print(nilai + " ");
                // Mencetak setiap nilai diikuti dengan spasi.

            }
            System.out.println();
            // Mencetak baris baru setelah semua nilai dalam satu baris matriks dicetak.
        }
    }
}

```