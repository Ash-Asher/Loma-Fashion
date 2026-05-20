<!DOCTYPE html>
<html lang="de">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Loma Fashion</title>
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap" rel="stylesheet">
    <style>
        /* Grundlegendes Styling */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Montserrat', sans-serif;
        }

        body {
            background-color: #f5f1ea; /* Beige Hintergrund */
            color: #333;
            line-height: 1.6;
        }

        a {
            text-decoration: none;
            color: inherit;
        }

        /* Header */
        header {
            background-color: #8b5e3c; /* Dunkelbraun */
            color: white;
            padding: 1rem 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        header h1 {
            font-size: 2rem;
        }

        nav ul {
            list-style: none;
            display: flex;
            gap: 1.5rem;
        }

        nav ul li a {
            color: white;
            font-weight: 600;
            transition: color 0.3s;
        }

        nav ul li a:hover {
            color: #d9b89a; /* Helleres Braun für Hover */
        }

        /* Hero-Sektion */
        .hero {
            background: url('https://images.unsplash.com/photo-1593032457861-3cf45d768da1?auto=format&fit=crop&w=1400&q=80') no-repeat center center/cover;
            height: 70vh;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            color: white;
            position: relative;
        }

        .hero::after {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(139, 94, 60, 0.5); /* Braun Overlay */
        }

        .hero-content {
            position: relative;
            max-width: 700px;
        }

        .hero-content h2 {
            font-size: 2.5rem;
            margin-bottom: 1rem;
        }

        .hero-content p {
            font-size: 1.2rem;
        }

        /* Sektionen */
        section {
            padding: 4rem 2rem;
        }

        .section-title {
            text-align: center;
            margin-bottom: 2rem;
            font-size: 2rem;
            color: #8b5e3c; /* Dunkelbraun Akzent */
        }

        .products {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
        }

        .product-card {
            background-color: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: transform 0.3s;
        }

        .product-card:hover {
            transform: scale(1.05);
        }

        .product-card img {
            width: 100%;
            height: 300px;
            object-fit: cover;
        }

        .product-card h3 {
            padding: 1rem;
            font-size: 1.2rem;
            color: #8b5e3c;
        }

        /* Footer */
        footer {
            background-color: #8b5e3c;
            color: white;
            text-align: center;
            padding: 2rem;
        }

        footer p {
            margin-bottom: 0.5rem;
        }

        footer a {
            color: #d9b89a;
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <h1>Loma Fashion</h1>
        <nav>
            <ul>
                <li><a href="#trends">Trends</a></li>
                <li><a href="#about">Über Uns</a></li>
                <li><a href="#contact">Kontakt</a></li>
            </ul>
        </nav>
    </header>

    <!-- Hero-Sektion -->
    <section class="hero">
        <div class="hero-content">
            <h2>Neue Trends, Neuer Style</h2>
            <p>Jeder Look ein neues Teil</p>
        </div>
    </section>

    <!-- Produkt-Sektion -->
    <section id="trends">
        <h2 class="section-title">Unsere neuesten Trends</h2>
        <div class="products">
            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1618354691003-8a3f6f57f9f1?auto=format&fit=crop&w=800&q=80" alt="Produkt 1">
                <h3>Sommer Kleid</h3>
            </div>
            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1593032465174-d5cbf0479b4b?auto=format&fit=crop&w=800&q=80" alt="Produkt 2">
                <h3>Casual Jacke</h3>
            </div>
            <div class="product-card">
                <img src="https://images.unsplash.com/photo-1521335629791-ce4aec67dd52?auto=format&fit=crop&w=800&q=80" alt="Produkt 3">
                <h3>Stylische Sneakers</h3>
            </div>
        </div>
    </section>

    <!-- Über Uns -->
    <section id="about">
        <h2 class="section-title">Über Loma Fashion</h2>
        <p style="max-width: 700px; margin: 0 auto; text-align: center;">
            Loma Fashion steht für frische Styles, aktuelle Trends und Looks, die auffallen. Wir glauben daran, dass Mode Spaß machen und jeden Tag besonders machen sollte.
        </p>
    </section>

    <!-- Kontakt -->
    <section id="contact">
        <h2 class="section-title">Kontakt</h2>
        <p style="text-align: center;">Schreibe uns an: <a href="mailto:info@lomafashion.de">info@lomafashion.de</a></p>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2026 Loma Fashion</p>
        <p>Folge uns auf <a href="#">Instagram</a> & <a href="#">Facebook</a></p>
    </footer>
</body>
</html>
