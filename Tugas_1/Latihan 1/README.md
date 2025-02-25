# Penjelasan 

```java
public class LatihanArray1 {
// Mendefinisikan kelas dengan nama LatihanArray1

    public static void main(String[] args) {    
    // Mendefinisikan main method, Method yang akan dieksekusi pertama kali ketika program dijalankan

        int[] bilanganGenap = new int[10];      
        // Deklarasi & inisiasi array bernama bilanganGenap, tipe int & menampung 10 elemen
        
        int jumlah = 0;                         
        // Deklarasi & inisiasi variabel tipe int dengan nilai 0


        for (int i = 0; i < bilanganGenap.length; i++) {    
        // Perulangan for untuk mengisi array bilanganGenap dg bilangan genap. i dimulai  dari 0 dan berjalan hingga i kurang dari panjang array

            bilanganGenap[i] = (i + 1) * 2;     
            // Setiap elemen diisi nilai ini yang menghasilkan bilangan genap
        }

        System.out.println("Isi array:");       
        // Mencetak teks "Isi Array"

        for (int bilangan : bilanganGenap) {    
        // Mengiterasi setiap elemen dalam array bilanganGenap 

            System.out.print(bilangan + " ");   
            // Mencetak setiap elemen array + spasi.

            jumlah += bilangan;                 
            // Menambahkan nilai setiap elemen array ke variabel jumlah.
        }

        System.out.println("\nJumlah semua elemen: " + jumlah); 
        // Mencetak teks "Jumlah semua elemen " diikuti dengan variabel jumlah. \n digunakkan untuk membuat baris baru
    }
}
```