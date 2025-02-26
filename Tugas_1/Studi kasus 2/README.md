# Penjelasan

```java 
public class TicTacToe {
// Mendefinisikan sebuah kelas dengan nama TicTacToe.

    public static void main(String[] args) {
    // Mendefinisikan main method, Method yang akan dieksekusi pertama kali ketika program dijalankan

        char[][] papan = new char[3][3];
        // Mendeklarasikan dan menginisialisasi array 2D dengan nama papan yang berukuran 3x3, yang digunakan untuk papan Tic Tac Toe.

        // Inisialisasi papan kosong
        for (int i = 0; i < 3; i++) {
        // Mengiterasi setiap baris.

            for (int j = 0; j < 3; j++) {
            // Mengiterasi setiap kolom

                papan[i][j] = '-';
                // Mengisi setiap kotak dengan karakter '-'
            }
        }

        // Simulasi beberapa langkah
        papan[0][0] = 'X';
        //  Menempatkan 'X' di baris 0, kolom 0
        papan[1][1] = 'O';
        // Menempatkan 'O' di baris 1, kolom 1.
        papan[2][2] = 'X';
        // Menempatkan 'X' di baris 2, kolom 2.

        // Tampilkan papan
        System.out.println("Status Papan:");
        // Mencetak teks "Status Papan:"

        tampilkanPapan(papan);
        // Memanggil method tampilkanPapan untuk menampilkan isi papan
    }

    public static void tampilkanPapan(char[][] papan) {
    // Method ini digunakan untuk menampilkan isi papan ke konsol

        for (int i = 0; i < 3; i++) {
        // Mengiterasi setiap baris.
            
            for (int j = 0; j < 3; j++) {
            // Mengiterasi setiap kolom. 

                System.out.print(papan[i][j] + " ");
                // Mencetak nilai setiap kotak diikuti dengan spasi
            }
            System.out.println();
            // Mencetak baris baru setelah semua kotak dalam satu baris dicetak.
        }
    }
}

```