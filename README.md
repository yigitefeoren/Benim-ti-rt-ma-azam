<!-- signup.html dosyasını düzenle -->
<h2>Kayıt Ol</h2>
<form id="signup-form">
    <label for="email">E-posta:</label>
    <input type="email" id="email" name="email" required>

    <label for="password">Şifre:</label>
    <input type="password" id="password" name="password" required>

    <button type="submit">Kayıt Ol</button>
</form>
/* style.css dosyasını düzenle */
body {
    font-family: Arial, sans-serif;
    background-color: #f4f4f9;
}

.form-container {
    width: 100%;
    max-width: 400px;
    margin: 50px auto;
    padding: 20px;
    background-color: white;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    border-radius: 8px;
}<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tişört Satışı</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>Tişört Mağazamıza Hoş Geldiniz!</h1>

        <nav>
            <ul>
                <li><a href="signup.html">Kayıt Ol</a></li>
                <li><a href="login.html">Giriş Yap</a></li>
            </ul>
        </nav>
    </header>
    
    <section class="main-content">
        <h2>En Popüler Tişörtler</h2>
        <p>Burada en popüler tişörtlerimiz var. İstediğini seçip satın alabilirsin!</p>
        <!-- Burada tişört ürünlerini listelemek için HTML öğeleri ekleyebilirsin. -->
    </section>

    <footer>
        <p>&copy; 2025 Tişört Mağazası</p>
    </footer>
</body>
</html><!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Giriş Yap</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>Giriş Yap</h1>
    </header>

    <section class="form-container">
        <form id="login-form">
            <label for="email">E-posta:</label>
            <input type="email" id="email" name="email" required>

            <label for="password">Şifre:</label>
            <input type="password" id="password" name="password" required>

            <button type="submit">Giriş Yap</button>
        </form>
    </section>

    <footer>
        <p>&copy; 2025 Tişört Mağazası</p>
    </footer>
</body>
</html>// Bu script dosyası, form doğrulama işlemleri veya diğer etkileşimler için kullanılabilir.
document.getElementById('signup-form').addEventListener('submit', function(event) {
    event.preventDefault();
    
    let email = document.getElementById('email').value;
    let password = document.getElementById('password').value;

    // Kayıt verilerini buraya ekleyebilirsin. (Örneğin, Firebase ile entegrasyon)
    alert(`Kayıt Başarılı: ${email}`);
});

document.getElementById('login-form').addEventListener('submit', function(event) {
    event.preventDefault();
    
    let email = document.getElementById('email').value;
    let password = document.getElementById('password').value;

    // Giriş doğrulama işlemi yapılabilir. (Örneğin, Firebase veya başka bir backend ile)
    alert(`Giriş Başarılı: ${email}`);
});<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ürün Ekle</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>Ürün Ekle</h1>
    </header>

    <section class="form-container">
        <form id="product-form">
            <label for="product-name">Ürün Adı:</label>
            <input type="text" id="product-name" name="product-name" required>

            <label for="product-description">Ürün Açıklaması:</label>
            <textarea id="product-description" name="product-description" required></textarea>

            <label for="product-price">Ürün Fiyatı (TL):</label>
            <input type="number" id="product-price" name="product-price" required>

            <label for="product-image">Ürün Resmi URL:</label>
            <input type="url" id="product-image" name="product-image">

            <button type="submit">Ürünü Ekle</button>
        </form>
    </section>

    <footer>
        <p>&copy; 2025 Tişört Mağazası</p>
    </footer>
</body>
</html><!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ürünler</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>Tüm Ürünler</h1>
    </header>

    <section class="product-list">
        <div class="product">
            <img src="product-image-url.jpg" alt="Ürün Resmi" />
            <h3>Ürün Adı</h3>
            <p>Ürün Açıklaması</p>
            <p><strong>Fiyat:</strong> 100 TL</p>
            <button>Sepete Ekle</button>
        </div>
        <!-- Ürünler burada listelenecek. Dinamik olarak ekleyebilirsin. -->
    </section>

    <footer>
        <p>&copy; 2025 Tişört Mağazası</p>
    </footer>
</body>
</html><!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sepetim</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>Sepetim</h1>
    </header>

    <section class="cart-container">
        <div class="cart-item">
            <img src="product-image-url.jpg" alt="Ürün Resmi" />
            <h3>Ürün Adı</h3>
            <p>Ürün Açıklaması</p>
            <p><strong>Fiyat:</strong> 100 TL</p>
            <button>Sil</button>
        </div>
        <!-- Sepetteki ürünler burada listelenecek. -->
    </section>

    <footer>
        <p>&copy; 2025 Tişört Mağazası</p>
    </footer>
</body>
</html><!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tişört Mağazası</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>Tişört Mağazamıza Hoş Geldiniz!</h1>
        <nav>
            <ul>
                <li><a href="signup.html">Kayıt Ol</a></li>
                <li><a href="login.html">Giriş Yap</a></li>
            </ul>
        </nav>
    </header>
    
    <section class="main-content">
        <h2>En Popüler Tişörtler</h2>
        <p>Burada en popüler tişörtlerimiz var. İstediğini seçip satın alabilirsin!</p>
        <a href="view-products.html" class="button">Ürünleri Gör</a>
    </section>

    <footer>
        <p>&copy; 2025 Tişört Mağazası</p>
    </footer>
</body>
</html>body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f4f4f9;
}

header {
    background-color: #4CAF50;
    color: white;
    padding: 10px 0;
    text-align: center;
}

header nav ul {
    list-style-type: none;
    padding: 0;
}

header nav ul li {
    display: inline;
    margin: 0 15px;
}

header nav ul li a {
    color: white;
    text-decoration: none;
    font-size: 18px;
}

footer {
    background-color: #4CAF50;
    color: white;
    text-align: center;
    padding: 10px 0;
    position: fixed;
    width: 100%;
    bottom: 0;
}

.form-container {
    width: 100%;
    max-width: 400px;
    margin: 50px auto;
    padding: 20px;
    background-color: white;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    border-radius: 8px;
}

.form-container input,
.form-container button {
    width: 100%;
    padding: 10px;
    margin: 10px 0;
    border: 1px solid #ccc;
    border-radius: 4px;
}

.form-container button {
    background-color: #4CAF50;
    color: white;
    border: none;
    cursor: pointer;
}

.form-container button:hover {
    background-color: #45a049;
}

.product-list .product {
    width: 100%;
    max-width: 300px;
    margin: 20px auto;
    padding: 10px;
    background-color: white;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
    border-radius: 8px;
    text-align: center;
}

.product-list/* Yazma kodlarını gizle */
.writing-code {
    display: none;
}

/* Çelenkleri göster */
.wreath {
    display: block;
}<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tişört Mağazası</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>Tişört Mağazamıza Hoş Geldiniz!</h1>
        <nav>
            <ul>
                <li><a href="signup.html">Kayıt Ol</a></li>
                <li><a href="login.html">Giriş Yap</a></li>
            </ul>
        </nav>
    </header>

    <section class="main-content">
        <h2>En Popüler Tişörtler</h2>
        <p>Burada en popüler tişörtlerimiz var. İstediğini seçip satın alabilirsin!</p>
        <a href="view-products.html" class="button">Ürünleri Gör</a>
    </section>

    <footer>
        <p>&copy; 2025 Tişört Mağazası</p>
    </footer>
</body>
</html><pre
    Kodlar burada olacak...
</pre><pre>
    Kodlar burada olacak...
</pre><pre style="display:none;">
    Kodlar burada olacak...
</pre><code style="display:none;">
    Kodlar burada olacak...
</code>body {
    background-color: #f0f8ff; /* Açık mavi bir arka plan */
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
}

header {
    background-color: #4CAF50;
    color: white;
    padding: 10px 0;
    text-align: center;
}body {
    background-color: #f0f8ff; /* Açık mavi bir arka plan */
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
}

header {
    background-color: #4CAF50;
    color: white;
    padding: 10px 0;
    text-align: center;
}#00f