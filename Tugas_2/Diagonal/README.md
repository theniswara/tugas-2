
```java
public class MenentukanDiagonal {
    public static void main(String[] args) {
        // Matriks persegi 3x3
        int[][] matriks = {
            {1, 2, 3},
            {4, 5, 6},
            {7, 8, 9}
        };

        System.out.println("Matriks:");
        printMatriks(matriks);

        System.out.println("\nDiagonal Utama:");
        int[] diagonalUtama = getDiagonalUtama(matriks);
        printArray(diagonalUtama);

        System.out.println("\nDiagonal Samping:");
        int[] diagonalSamping = getDiagonalSamping(matriks);
        printArray(diagonalSamping);
    }

    // Metode untuk mendapatkan diagonal utama
    public static int[] getDiagonalUtama(int[][] matriks) {
        int n = matriks.length;
        int[] diagonal = new int[n]; // Array untuk menyimpan diagonal utama

        for (int i = 0; i < n; i++) {
            diagonal[i] = matriks[i][i]; // Elemen diagonal utama: matriks[i][i]
        }

        return diagonal;
    }

    // Metode untuk mendapatkan diagonal samping
    public static int[] getDiagonalSamping(int[][] matriks) {
        int n = matriks.length;
        int[] diagonal = new int[n]; // Array untuk menyimpan diagonal samping

        for (int i = 0; i < n; i++) {
            diagonal[i] = matriks[i][n - 1 - i]; // Elemen diagonal samping: matriks[i][n-1-i]
        }

        return diagonal;
    }

    // Metode untuk mencetak matriks
    public static void printMatriks(int[][] matriks) {
        for (int[] baris : matriks) {
            for (int nilai : baris) {
                System.out.print(nilai + " ");
            }
            System.out.println();
        }
    }

    // Metode untuk mencetak array
    public static void printArray(int[] array) {
        for (int nilai : array) {
            System.out.print(nilai + " ");
        }
        System.out.println();
    }
}
```