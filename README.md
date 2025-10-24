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
Tujuan dari perintah ini untuk menunjukkan cara Javascript berinteraksi dengan halaman web dan console.


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



# PEMBUATAN FORMULIR DAN TOMBOL 

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Pembuatan Form dan Button</title>
    <script>
        // Fungsi untuk menampilkan hasil input
        function tampilkanNama() {
            let nama = document.getElementById("nama").value;
            document.getElementById("hasil").innerHTML = "Halo, " + nama + "!";
        }
    </script>
</head>
<body>
    <h2>Form Input dan Button</h2>

    <!-- Form Input -->
    <form>
        <label for="nama">Nama:</label>
        <input type="text" id="nama" placeholder="Masukkan nama kamu">
        <button type="button" onclick="tampilkanNama()">Tampilkan</button>
    </form>

    <!-- Hasil tampil di sini -->
    <p id="hasil"></p>
</body>
</html>
```


  Membuat file di VSCode dengan nama ```form_button.html```. Pada file ini halaman HTML sederhana yang berisi form(input teks + tombol) dan skrip Javascript di elemen ```<head>```. File ini terdapat dua elemen yaitu: 
  * elemen ```<input type="text">``` untuk meminta pengguna memasukkan nama, di dalam elemen ini terdapat atribut ```id="nama"``` digunakan agar javascript bisa mengambil nilainya.
  * eleme ```<button>``` memiliki atribut ```onclick="tampilkanNama()", yang berarti saat tombol di klik, fungsi ```tampilanNama()" akan dijalankan.


    Berikut hasil pada Browser

<img width="534" height="279" alt="Screenshot 2025-10-24 063800" src="https://github.com/user-attachments/assets/db6d13b5-02e0-4fe1-bb6d-b25d067d3bd8" />

<img width="535" height="316" alt="Screenshot 2025-10-24 063859" src="https://github.com/user-attachments/assets/ab38c4e2-7c07-4210-924b-26a7313df1a3" />



# HTML DOM (KOTAK CEKLIS OTOMATIS) 

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Perhitungan Otomatis dengan Checkbox</title>
    <script>
        function hitungTotal() {
            let total = 0;

            // Ambil semua checkbox
            let item1 = document.getElementById("item1");
            let item2 = document.getElementById("item2");
            let item3 = document.getElementById("item3");

            // Cek apakah dipilih
            if (item1.checked) total += parseInt(item1.value);
            if (item2.checked) total += parseInt(item2.value);
            if (item3.checked) total += parseInt(item3.value);

            // Tampilkan hasil
            document.getElementById("total").innerHTML = "Total harga: Rp " + total.toLocaleString();
        }
    </script>
</head>
<body>
    <h2>Perhitungan Otomatis (Checkbox)</h2>

    <form>
        <input type="checkbox" id="item1" value="10000" onclick="hitungTotal()"> Nasi Goreng (Rp 10.000)<br>
        <input type="checkbox" id="item2" value="8000" onclick="hitungTotal()"> Mie Ayam (Rp 8.000)<br>
        <input type="checkbox" id="item3" value="12000" onclick="hitungTotal()"> Ayam Geprek (Rp 12.000)<br><br>
    </form>

    <p id="total">Total harga: Rp 0</p>
</body>
</html>
```


  Membuat file di VSCode dengan nama ```checkbox_total``` pada file ini menampilkan daftar menu makanan dengan checkbox dan menghitung total harga otomatis setiap kali pengguna mencentang atau menghapus pilihan. Perhitungan ini dilakukan menggunakan Javascript tanpa perlu menekan tombol apapun. Di file ini terdapat elemen ```<input type="checkbox">``` setiap makanan memiliki nilai harga di atribut ```value```. Event ```onclick="hitungTotal()"``` digunakan agar fungsi dijalankan setiap kali checkbox diklik. 


    Berikut hasil pada Browser 

<img width="449" height="290" alt="Screenshot 2025-10-24 065729" src="https://github.com/user-attachments/assets/03011fa9-f889-4645-926b-42c6d2c667f7" />

<img width="473" height="307" alt="Screenshot 2025-10-24 065743" src="https://github.com/user-attachments/assets/53b4718f-6763-44c6-a379-68ce46a44375" />



# PERTANYAAN DAN TUGAS 

1. Buat script untuk melakukan validasi pada isian form

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Validasi Form</title>
    <script>
        function validasiForm() {
            let nama = document.getElementById("nama").value;
            let email = document.getElementById("email").value;
            let password = document.getElementById("password").value;

            // Mengecek apakah kolom kosong
            if (nama == "" || email == "" || password == "") {
                alert("Semua kolom harus diisi!");
                return false;
            }

            // Validasi format email
            let polaEmail = /^[^ ]+@[^ ]+\.[a-z]{2,3}$/;
            if (!email.match(polaEmail)) {
                alert("Format email tidak valid!");
                return false;
            }

            // Validasi panjang password
            if (password.length < 6) {
                alert("Password harus minimal 6 karakter!");
                return false;
            }

            alert("Form berhasil dikirim!");
            return true;
        }
    </script>
</head>
<body>
    <h2>Form Registrasi (Validasi dengan JavaScript)</h2>

    <form onsubmit="return validasiForm()">
        <label for="nama">Nama:</label><br>
        <input type="text" id="nama" placeholder="Masukkan nama kamu"><br><br>

        <label for="email">Email:</label><br>
        <input type="text" id="email" placeholder="contoh@email.com"><br><br>

        <label for="password">Password:</label><br>
        <input type="password" id="password" placeholder="Minimal 6 karakter"><br><br>

        <input type="submit" value="Kirim">
    </form>
</body>
</html>
```


  Berikut hasil pada Browser 

<img width="578" height="401" alt="Screenshot 2025-10-24 072049" src="https://github.com/user-attachments/assets/55f32097-8c3d-4847-aa2f-34e23d433443" />

<img width="585" height="444" alt="Screenshot 2025-10-24 072230" src="https://github.com/user-attachments/assets/de7f32cf-a219-496f-8d08-542bd814deb1" />

<img width="1177" height="451" alt="Screenshot 2025-10-24 072302" src="https://github.com/user-attachments/assets/8b86bdaf-548e-44a3-b3b8-a06c2b850d8a" />







