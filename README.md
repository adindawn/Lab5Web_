# PRAKTIKUM 5: JAVASCRIPT

# PENGENALAN JAVASCRIPT

```
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Mengenal JavaScript</title>
</head>
<body>
    <h1>Pengenalan JavaScript</h1>
    <h3>Contoh document.write dan console.log</h3>
    <script>
    document.write("Hello World");
    console.log("Hello World");
    </script>
</body>
</html>
```


  Membuat file di VSCode dengan nama ```lab5_javascript.html```. Pada file ini memperkenalkan JAVASCRIPT dasar didalamnya terdapat dua perintah utama: 
  * ```document.write("Hello World")``` perintah ini untuk menampilkan teks langsung di halaman web.
  * ```console.log("Hello World")``` perintah ini untuk menampilkan teks di console  browser.
Tujuan dari perintah ini untuk menunjukkan cara Javascript berinteraksi dengan halaman web dam console.


   Berikut hasil pada Browser

<img width="483" height="278" alt="Screenshot 2025-10-24 052859" src="https://github.com/user-attachments/assets/c0aa62bd-ac85-4727-802c-946bb7d51ec4" />



# JAVASCRIPT DASAR 

```
script>
        // Pemakaian Alert
        alert("Halo! Ini contoh penggunaan alert di JavaScript.");

        // Pemakaian Prompt
        let nama = prompt("Siapa namamu?");
        document.write("Halo, " + nama + "!<br>");

        // Membuat fungsi
        function salam(nama) {
            return "Selamat datang, " + nama + "!";
        }

        // Memanggil fungsi
        let hasil = salam(nama);
        document.write(hasil);
    </script>
```


  Membuat file di VSCode dengan nama ```dasar_javascript.html```. Pada file ini menampilkan perintah ```altert``` sebagai pesan awal, dan ```prompt``` untuk meminta input nama pengguna. Ketika dijalanka  di Browser, pengguna akan diminta memasukkan nama, lalu Javascript akan menampilkan sapaan di halaman Browser "Selamat datang [nama]!. 


   Berikut hasil pada Browser 

<img width="431" height="249" alt="Screenshot 2025-10-24 054532" src="https://github.com/user-attachments/assets/73c15561-79d6-463c-8000-9c518f47ed71" />



# PEMROGRAMAN DASAR DI JAVASCRIPT 

```
<script>
        // --- Operasi Aritmatika ---
        let a = 10;
        let b = 5;

        document.write("<h3>Operasi Aritmatika</h3>");
        document.write("a = " + a + ", b = " + b + "<br>");
        document.write("Penjumlahan (a + b) = " + (a + b) + "<br>");
        document.write("Pengurangan (a - b) = " + (a - b) + "<br>");
        document.write("Perkalian (a * b) = " + (a * b) + "<br>");
        document.write("Pembagian (a / b) = " + (a / b) + "<br>");
        document.write("Sisa bagi (a % b) = " + (a % b) + "<br><br>");

        // --- Seleksi Kondisi if..else ---
        document.write("<h3>Seleksi Kondisi if..else</h3>");
        let nilai = prompt("Masukkan nilai ujianmu:");
        if (nilai >= 75) {
            document.write("Selamat, kamu lulus!<br>");
        } else {
            document.write("Maaf, kamu belum lulus.<br>");
        }

        // --- Operator Switch ---
        document.write("<h3>Seleksi Kondisi switch</h3>");
        let grade = prompt("Masukkan grade (A/B/C/D):");
        switch (grade) {
            case "A":
                document.write("Nilai kamu sangat baik!<br>");
                break;
            case "B":
                document.write("Nilai kamu baik.<br>");
                break;
            case "C":
                document.write("Nilai kamu cukup.<br>");
                break;
            case "D":
                document.write("Nilai kamu kurang.<br>");
                break;
            default:
                document.write("Grade tidak valid!<br>");
        }
    </script>
```


  Membuat file di VSCode dengan nama ```dasar_pemrograman.html```. Pada file ini membantu memahami cara kerja perhitungan, logika pengambilan keputusan, dan interaksi dengan pengguna menggunakan ```prompt```, untuk melakukan operasi aritmatika atau koleksi kondisi menggunakan struktur sebagai berikut: 
  * Struktur Seleksi kondisi ```if..else``` pengguna diminta memasukkan nilai ujian melalui ```prompt()```. Jika nilai lebih besar dari 75, maka akan muncul pesan "Selamat, kamu lulus!". dan jika kurang dari 75 akan muncul "Maaf, kamu belum lulu!".
  * Struktur Seleksi kondisi ```switch``` program meminta pengguna memasukkan grade (A/B/C/D) berdasarkan input Javascript memampilakan pesan yang sesuai:
    - A: Nilai sangat baik
    - B: Nilai baik
    - C: Nilai cukup
    - D: Nilai kurang
  Jika input tidak sesuai, muncul pesan "Grade tidak valid".


    Berikut hasil pada Browser

<img width="740" height="364" alt="Screenshot 2025-10-24 060724" src="https://github.com/user-attachments/assets/36b0c3ea-ca68-46e5-a4b6-060ed1ad7f69" />

<img width="745" height="377" alt="Screenshot 2025-10-24 060738" src="https://github.com/user-attachments/assets/f2de3387-11d9-4693-849e-88d8d1545bf4" />

<img width="520" height="592" alt="Screenshot 2025-10-24 060752" src="https://github.com/user-attachments/assets/07c79f8e-8639-455f-b55f-d529d9745a8d" />

