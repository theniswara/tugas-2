# Penjelasan

```java
public class SistemNilai {
//  Mendefinisikan kelas dengan nama SistemNilai

    public static void main(String[] args) {
    // Mendefinisikan main method, Method yang akan dieksekusi pertama kali ketika program dijalankan

        // Data siswa
        String[] namaSiswa = {"Ani", "Budi", "Cici", "Dodi", "Edi"};
        // Mendeklarasikan dan menginisialisasi array namaSiswa yang berisi nama-nama siswa. Array ini memiliki 5 elemen bertipe String
        
        int[][] nilai = {
            {80, 85, 90}, // Nilai Ani
            {75, 70, 85}, // Nilai Budi
            {85, 80, 88}, // Nilai Cici
            {90, 85, 95}, // Nilai Dodi
            {70, 75, 80}  // Nilai Edi
        };
        // Mendeklarasikan dan menginisialisasi array 2D nilai yang berisi nilai-nilai siswa untuk setiap mata pelajaran.

        String[] mapel = {"Matematika", "Bahasa Inggris", "IPA"};
        // Mendeklarasikan dan menginisialisasi array mapel yang berisi nama-nama mata pelajaran. Array ini memiliki 3 elemen bertipe String.

        // Menghitung rata-rata per siswa
        System.out.println("Rata-rata nilai per siswa:");
        // Mencetak teks "Rata-rata nilai per siswa:" ke konsol.

        for (int i = 0; i < nilai.length; i++) {
            double total = 0;
            for (int n : nilai[i]) {
                total += n;
            }
            double rataSiswa = total / nilai[i].length;
            System.out.printf("%s: %.2f\\n", namaSiswa[i], rataSiswa);
        }

        // Menghitung rata-rata per mata pelajaran
        System.out.println("\\nRata-rata nilai per mata pelajaran:");
        for (int j = 0; j < nilai[0].length; j++) {
            double total = 0;
            for (int i = 0; i < nilai.length; i++) {
                total += nilai[i][j];
            }
            double rataMapel = total / nilai.length;
            System.out.printf("%s: %.2f\\n", mapel[j], rataMapel);
        }
    }
}

```