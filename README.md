<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="css/stylenya.css">
    <link rel="website icon" type="png"
    href="gambar/LOGOOOJ.png">
</head>
<body>
    <header>
        <nav> 
            <img src="gambar/logoo.png" alt="logo">
        </nav>
        <h1>AGRITOUREZ</h1>
        <nav>
            <ul>
                <li><a href="#home">Beranda</a></li>
                <li><a href="#products">Produk</a></li>
                <li><a href="#cart">Keranjang</a></li>
            </ul>
        </nav>
    </header>

    <section id="home">
        <h2>Selamat Datang di Toko Sayuran Segar dan berbagai olahan susu</h2>
        <p> Kami menjual berbagai macam sayuran segar langsung dari petani pangalengan, serta olahan olahan susu khas pangalengan.</p>
        <img src="gambar/ilustrasi sayur.jpg" alt="Sayuran Segar">
    </section>

    <section id="products">
        <h2>Produk Kami</h2>
        <div class="product">
            <img src="gambar/kentang.jpeg" alt="kentang">
            <h3>kentang</h3>
            <p>Rp 20.000/kg</p>
            <button onclick="addToCart('kentang', 20000)">Tambah ke Keranjang</button>
        </div>
        <div class="product">
            <img src="gambar/Tomato_je.jpg" alt="Tomat">
            <h3>Tomat</h3>
            <p>Rp 8.000/kg</p>
            <button onclick="addToCart('Tomat', 8000)">Tambah ke Keranjang</button>
        </div>
        <div class="product">
            <img src="gambar/wortel.png" alt="Wortel">
            <h3>Wortel</h3>
            <p>Rp 12.000/kg</p>
            <button onclick="addToCart('Wortel', 12000)">Tambah ke Keranjang</button>
        </div>
        <div class="product">
            <img src="gambar/kol.webp" alt="kol">
            <h3>kol</h3>
            <p>Rp 15.000/kg</p>
            <button onclick="addToCart('kol',15000 )"> Tambah ke keranjang</button> 
        </div>

    
        <!-- Tambahkan produk lainnya di sini -->
    </section>

    <section id="product">
    <h2>produk olahan susu</h2>
       <div class="product">
        <img src="gambar/susu.jpeg" alt="susu murni">
        <h3>susu murni</h3>
        <p>Rp 12.000/liter</p>
        <button onclick="addToCart('susu murni', 12000)"> Tambah ke keranjang </button>
    </div>
    <div class="product">
        <img src="gambar/permen susu.jpeg" alt="permen susu">
        <h3>permen susu</h3>
        <p>Rp 10.000/bungkus</p>
        <button onclick="addToCart('permen susu', 10000)"> Tambah ke keranjang </button>
    </div>


    </section>

    <section id="cart">
        <h2>Keranjang Belanja</h2>
        <ul id="cartItems"></ul>
        <p>Total: Rp <span id="totalAmount">0</span></p>
        <button id="buyButton" onclick="buyItems()">Beli Sekarang</button>
        <button id="clearButton" onclick="clearCart()">Batalkan Pesanan</button>
    </section>

    
    <footer>
        <p>&copy; 2024 AGRITOUREZ. untuk informasi lebih lanjut bisa hubungi, email surya, no hp : 0001 </p>
    </footer>

    <script src="java/sistemnya.js"></script>
</body>
</html>
