# innovation-from-hikmah
innovation of biological educational gask
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pembelajaran Biologi Mencit</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #FAF3E0; /* warna krem */
            color: #3E2723; /* warna coklat tua */
        }

        header {
            background-color: #D7CCC8; /* coklat susu */
            padding: 1em;
            text-align: center;
        }

        header h1 {
            color: #4E342E; /* coklat biasa */
        }

        nav a {
            margin: 0 10px;
            color: #3E2723;
            text-decoration: none;
        }

        .login-section, section {
            background-color: #FFFFFF; /* putih */
            padding: 20px;
            margin: 10px auto;
            width: 80%;
            border-radius: 8px;
        }

        button {
            background-color: #8D6E63; /* warna coklat */
            color: white;
            padding: 10px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }

        button:hover {
            background-color: #6D4C41; /* lebih gelap saat hover */
        }
    </style>
</head>
<body>
    <!-- Beranda -->
    <header>
        <h1>Selamat Datang di Pembelajaran Biologi Mencit</h1>
        <nav>
            <a href="#login">Login</a>
            <a href="#materi">Materi Anatomi Mencit</a>
            <a href="#task">Tugas Anatomi</a>
        </nav>
    </header>
    
    <section id="beranda">
        <h2>Media Belajar Biologi</h2>
        <p>Website ini merupakan media belajar tentang anatomi dan fisiologi mencit.</p>
    </section>

    <!-- Halaman Login -->
    <section id="login" class="login-section">
        <h2>Login untuk Siswa</h2>
        <form onsubmit="navigateToMateri(event)">
            <label for="name">Nama:</label>
            <input type="text" id="name" name="name" required>
            
            <label for="nim">NIM:</label>
            <input type="text" id="nim" name="nim" required>
            
            <button type="submit">Login</button>
        </form>
    </section>

    <!-- Halaman Materi -->
    <section id="materi">
        <h2>Materi Anatomi Mencit</h2>
        <p>Pilih bagian anatomi untuk mempelajari lebih lanjut.</p>
        <a href="#task">Kerjakan Task Anatomi</a>
    </section>

    <!-- Halaman Task -->
    <section id="task">
        <h2>Tugas Anatomi Mencit</h2>
        <p>Unggah gambar anatomi mencit dan jawab pertanyaan terkait.</p>
        <form>
            <label for="upload-image">Unggah Gambar:</label>
            <input type="file" id="upload-image" accept="image/*">
            
            <label for="answer">Jawaban Anda:</label>
            <textarea id="answer" name="answer" required></textarea>
            
            <button type="submit">Kirim</button>
        </form>
    </section>

    <script>
        function navigateToMateri(event) {
            event.preventDefault();
            // Pindah ke bagian materi setelah login
            document.getElementById("materi").scrollIntoView({ behavior: 'smooth' });
        }
    </script>
</body>
</html>
