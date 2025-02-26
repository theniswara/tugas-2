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
        // Menggunakan perulangan for untuk menghitung rata-rata nilai setiap siswa. Mengiterasi setiap siswa

            double total = 0;
            // Mendeklarasikan variabel total untuk menyimpan jumlah nilai seorang siswa.

            for (int n : nilai[i]) {
            // Mengiterasi setiap nilai mata pelajaran siswa tersebut

                total += n;
                // Menambahkan nilai mata pelajaran ke variabel total.
            }
            double rataSiswa = total / nilai[i].length;
            // Menghitung rata-rata nilai siswa dengan membagi total dengan jumlah mata pelajaran

            System.out.printf("%s: %.2f\\n", namaSiswa[i], rataSiswa);
            // Mencetak nama siswa dan rata-rata nilainya dengan format 2 angka desimal.

        }

        // Menghitung rata-rata per mata pelajaran
        System.out.println("\\nRata-rata nilai per mata pelajaran:");
        // Mencetak teks "Rata-rata nilai per mata pelajaran:"

        for (int j = 0; j < nilai[0].length; j++) {
        // Menggunakan perulangan for untuk menghitung rata-rata nilai setiap mata pelajaran. mengiterasi setiap mata pelajaran (kolom dalam array nilai).

            double total = 0;
            // Mendeklarasikan variabel total untuk menyimpan jumlah nilai semua siswa untuk satu mata pelajaran.

            for (int i = 0; i < nilai.length; i++) {
            // Mengiterasi setiap siswa untuk mata pelajaran tersebut.

                total += nilai[i][j];
                // Menambahkan nilai siswa ke variabel total.
            }
            double rataMapel = total / nilai.length;
            //  Menghitung rata-rata nilai mata pelajaran dengan membagi total dengan jumlah siswa
            
            System.out.printf("%s: %.2f\\n", mapel[j], rataMapel);
            // Mencetak nama mata pelajaran dan rata-rata nilainya dengan format 2 angka desimal.
        }
    }
}


```