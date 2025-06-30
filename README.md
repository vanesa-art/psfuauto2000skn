```html
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sistem PSFU AUTO2000 SUKUN</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            margin: 0;
            padding: 20px;
        }
        .container {
            max-width: 600px;
            margin: auto;
            background: white;
            padding: 20px;
            border-radius: 5px;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
        }
        button {
            background-color: #e44336;
            color: white;
            border: none;
            padding: 10px;
            cursor: pointer;
            transition: background-color 0.3s ease;
        }
        button:hover {
            background-color: #c7352e;
        }
        input[type="text"], input[type="password"], select {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: 1px solid #ddd;
            border-radius: 5px;
        }
        h2 {
            text-align: center;
        }
    </style>
</head>
<body>

    <!-- Halaman Login -->
    <div class="container" id="login">
        <h2>Sistem PSFU AUTO2000 SUKUN</h2>
        <input type="text" id="username" placeholder="Username" />
        <input type="password" id="password" placeholder="Password" />
        <button onclick="login()">Login</button>
    </div>

    <!-- Halaman Pilihan -->
    <div class="container" id="options" style="display:none;">
        <h2>Pilih Opsi</h2>
        <button onclick="showForm()">Masuk sebagai Pengisi Hasil PSFU</button>
        <button onclick="viewData()">Lihat Data Hasil PSFU per SA</button>
    </div>

    <!-- Form Pengisian Hasil PSFU -->
    <div class="container" id="form" style="display:none;">
        <h2>Isi Hasil PSFU</h2>
        <input type="text" placeholder="Nama Customer" />
        <input type="text" placeholder="No HP Customer" />
        <input type="text" placeholder="Nopol" />
        <select>
            <option value="">Pilih Tipe Mobil</option>
            <option value="Toyota Avanza">Toyota Avanza</option>
            <option value="Toyota Innova">Toyota Innova</option>
            <option value="Toyota Yaris">Toyota Yaris</option>
            <option value="Toyota Camry">Toyota Camry</option>
            <!-- Tambahkan tipe mobil lainnya disini -->
        </select>
        <input type="date" placeholder="Tanggal Terakhir Service" />
        <input type="number" min="1" max="10" placeholder="Nilai (1-10)" />
        <textarea placeholder="Penjabaran Penilaian"></textarea>
        <select>
            <option value="">Pilih Service Advisor</option>
            <option value="Eko M aries">Eko M aries</option>
            <option value="Merza ghoelam machmud">Merza ghoelam machmud</option>
            <option value="Fendi indra kristiawan">Fendi indra kristiawan</option>
            <option value="Wardjito">Wardjito</option>
            <option value="Ahmad fiqih">Ahmad fiqih</option>
        </select>
        <select>
            <option value="">Pilih SA Bengkel atau Body Repaint</option>
            <option value="Bengkel">SA Bengkel</option>
            <option value="Body Repaint">SA Body Repaint</option>
        </select>
        <button onclick="submitForm()">OK</button>
    </div>

    <script>
        function login() {
            // Implementasi login (dummy)
            document.getElementById('login').style.display = 'none';
            document.getElementById('options').style.display = 'block';
        }

        function showForm() {
            document.getElementById('options').style.display = 'none';
            document.getElementById('form').style.display = 'block';
        }

        function viewData() {
            alert('Fitur ini belum tersedia.');
        }

        function submitForm() {
            alert('Form berhasil dikirim!');
            // Implementasi penyimpanan data (dummy)
        }
    </script>

</body>
</html>
```
