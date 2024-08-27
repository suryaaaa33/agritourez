<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Toko Sayuran Segar</title>
    <link rel="stylesheet" href="styles.css">
  <style>
  body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f4f4f4;
}

header {
    background-color: #4CAF50;
    color: white;
    padding: 15px 0;
    text-align: center;
}

header h1 {
    margin: 0;
}

nav ul {
    list-style-type: none;
    padding: 0;
}

nav ul li {
    display: inline;
    margin: 0 10px;
}

nav ul li a {
    color: white;
    text-decoration: none;
    font-weight: bold;
}

section {
    padding: 20px;
    margin: 20px auto;
    max-width: 1000px;
    background-color: white;
    border-radius: 10px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

section h2 {
    color: #333;
}

section#home img {
    width: 100%;
    border-radius: 10px;
    margin-top: 20px;
}

.product {
    display: inline-block;
    width: 30%;
    text-align: center;
    margin: 10px;
    padding: 10px;
    border: 1px solid #ddd;
    border-radius: 10px;
    background-color: #fafafa;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

.product img {
    width: 100%;
    border-radius: 10px;
}

.product h3 {
    color: #4CAF50;
}

.product p {
    color: #555;
}

.product button {
    background-color: #4CAF50;
    color: white;
    border: none;
    padding: 10px;
    cursor: pointer;
    border-radius: 5px;
    transition: background-color 0.3s ease;
}

.product button:hover {
    background-color: #45a049;
}

footer {
    background-color: #4CAF50;
    color: white;
    text-align: center;
    padding: 10px 0;
    margin-top: 20px;
}

footer p {
    margin: 0;
}

#cart-animation {
    position: fixed;
    bottom: 20px;
    right: 20px;
    background-color: #4CAF50;
    color: white;
    padding: 10px 20px;
    border-radius: 5px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.3);
    opacity: 0;
    transition: opacity 0.5s ease;
    z-index: 1000;
}

#cart-animation.visible {
    opacity: 1;
}

#cart-animation.hidden {
    opacity: 0;
}
  </style>
</head>
<body>
    <header>
        <h1>Toko Sayuran Segar</h1>
        <nav>
            <ul>
                <li><a href="#home">Beranda</a></li>
                <li><a href="#products">Produk</a></li>
                <li><a href="#contact">Kontak</a></li>
            </ul>
        </nav>
    </header>

    <section id="home">
        <h2>Selamat Datang di Toko Sayuran Segar</h2>
        <p>Kami menyediakan berbagai macam sayuran segar langsung dari petani lokal.</p>
        <img src="sayuran.jpeg" alt="Sayuran Segar">
    </section>

    <section id="products">
        <h2>Produk Kami</h2>
        <div class="product">
            <img src="bayamm.jpeg" alt="Bayam">
            <h3>Bayam</h3>
            <p>Rp 10.000/kg</p>
            <button onclick="addToCart(this)">Tambah ke Keranjang</button>
        </div>
        <div class="product">
            <img src="Tomato_je.jpg" alt="Tomat">
            <h3>Tomat</h3>
            <p>Rp 8.000/kg</p>
            <button onclick="addToCart(this)">Tambah ke Keranjang</button>
        </div>
        <div class="product">
            <img src="wortel.png" alt="Wortel">
            <h3>Wortel</h3>
            <p>Rp 12.000/kg</p>
            <button onclick="addToCart(this)">Tambah ke Keranjang</button>
        </div>
        <!-- Tambahkan produk lainnya di sini -->
    </section>

    <section id="contact">
        <h2>Kontak Kami</h2>
        <p>Untuk pemesanan atau informasi lebih lanjut, hubungi kami di:</p>
        <p>Email: info@toko-sayuran.com</p>
        <p>Telepon: 0812-3456-7890</p>
    </section>

    <footer>
        <p>&copy; 2024 Toko Sayuran Segar. Semua hak cipta dilindungi.</p>
    </footer>

    <div id="cart-animation" class="hidden">✔ Ditambahkan ke Keranjang</div>

    <script>
        function addToCart(button) {
            var cartAnimation = document.getElementById("cart-animation");
            cartAnimation.classList.remove("hidden");
            cartAnimation.classList.add("visible");

            setTimeout(function() {
                cartAnimation.classList.remove("visible");
                cartAnimation.classList.add("hidden");
            }, 2000);
        }
    </script>
</body>
</html>
