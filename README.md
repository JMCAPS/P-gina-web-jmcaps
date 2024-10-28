# P-gina-web-jmcaps
Código HTML y archivos 

Hola 
Mostrar texto citado
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="JM CAPS - Bolsos únicos para cada momento. Descubre nuestra colección de bolsos elegantes y clásicos.">
    <title>JM CAPS</title>
    <style>
        /* Estilos generales */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Arial', sans-serif;
        }

        body {
            color: #333;
            background-color: #111;
        }

        .gold-texture {
            background: linear-gradient(135deg, #D4AF37, #FFD700, #C9A52D);
            background-clip: text;
            color: transparent;
            -webkit-background-clip: text;
            font-weight: bold;
        }

        /* Navegación */
        .navbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 15px 30px;
            background-color: #000;
            color: #FFD700;
        }

        .navbar a {
            color: #FFD700;
            text-decoration: none;
            margin: 0 15px;
            font-weight: bold;
            transition: color 0.3s ease;
        }

        .navbar a:hover {
            color: #D4AF37;
        }

        /* Estilo del logo */
        .navbar img {
            width: 150px; /* Ajuste del tamaño del logo */
            height: auto;
            transition: transform 0.5s ease-in-out, opacity 0.5s ease-in-out;
            opacity: 0;
            transform: scale(0.9);
        }

        .navbar img.loaded {
            opacity: 1;
            transform: scale(1);
        }

        /* Sección Hero */
        .hero {
            background-image: linear-gradient(to right, rgba(0, 0, 0, 0.8), rgba(0, 0, 0, 0.5)), url('https://example.com/imagen-bolsos.jpg');
            background-size: cover;
            background-position: center;
            height: 80vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            color: white;
            text-align: center;
        }

        .hero h1 {
            font-size: 4rem;
            font-weight: 700;
            margin-bottom: 20px;
            color: #FFD700;
            background: linear-gradient(135deg, #FFD700, #D4AF37, #FFD700);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            text-transform: uppercase;
        }

        .hero p {
            font-size: 1.5rem;
            margin-bottom: 30px;
            color: #f2f2f2;
        }

        .hero button {
            padding: 12px 25px;
            font-size: 1.2rem;
            color: #111;
            background-color: #FFD700;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s ease;
            font-weight: bold;
        }

        .hero button:hover {
            background-color: #D4AF37;
        }

        /* Productos Destacados */
        .featured-products {
            padding: 60px 30px;
            text-align: center;
            background-color: #111;
        }

        .featured-products h2 {
            font-size: 2.5rem;
            font-weight: 700;
            margin-bottom: 40px;
            color: #FFD700;
        }

        /* Contenedor del carrusel */
        .carousel-container {
            display: flex;
            overflow: hidden;
            white-space: nowrap;
            position: relative;
        }

        /* Movimiento del carrusel */
        @keyframes scroll {
            0% { transform: translateX(0); }
            100% { transform: translateX(-100%); }
        }

        /* Configuración del carrusel */
        .carousel {
            display: flex;
            animation: scroll 20s linear infinite;
        }

        .product-card {
            width: 250px;
            padding: 20px;
            box-shadow: 0px 4px 15px rgba(255, 215, 0, 0.2);
            border-radius: 10px;
            text-align: center;
            background-color: #222;
            transition: transform 0.3s ease;
            border: 1px solid #FFD700;
            margin-right: 20px;
        }

        .product-card:hover {
            transform: translateY(-10px);
            border-color: #D4AF37;
        }

        .product-card img {
            width: 100%;
            height: auto;
            border-radius: 5px;
            margin-bottom: 15px;
        }

        .product-card h3 {
            font-size: 1.2rem;
            font-weight: bold;
            margin: 10px 0;
            color: #FFD700;
        }

        .product-card p {
            color: #999;
            font-size: 1rem;
            margin-bottom: 10px;
        }

        .product-card button {
            padding: 8px 16px;
            background-color: #FFD700;
            color: #111;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s ease;
            font-weight: bold;
        }

        .product-card button:hover {
            background-color: #D4AF37;
        }

        /* Pie de página */
        .footer {
            padding: 20px;
            text-align: center;
            background-color: #000;
            color: #FFD700;
        }

        .social-media {
            margin-top: 20px;
        }

        .social-media a {
            margin: 0 10px;
            color: #FFD700;
            font-size: 1.5rem;
            text-decoration: none;
        }
    </style>
</head>
<body>

    <!-- Barra de navegación -->
    <header class="navbar">
        <div>
            <a href="#" class="gold-texture">JM CAPS</a>
        </div>
        <img src="LOGO.jpeg" alt="Logo JM CAPS" id="logo">
        <nav>
            <a href="#">Inicio</a>
            <a href="#">Productos</a>
            <a href="#">Sobre Nosotros</a>
            <a href="#">Contacto</a>
        </nav>
    </header>

    <!-- Sección Hero -->
    <section class="hero">
        <div>
            <h1>Exprésate con Estilo</h1>
            <p>Bolsos únicos para cada momento</p>
            <button>Descubre Ahora</button>
        </div>
    </section>

    <!-- Productos Destacados -->
    <section class="featured-products">
        <h2>Descubre Nuestros Productos</h2>
        <div class="carousel-container">
            <div class="carousel">
                <!-- Modelos del 1 al 15 -->
                <div class="product-card">
                    <img src="MODELO1.jpeg" alt="Bolso Modelo 1">
                    <h3>Modelo 1</h3>
                    <p>$499</p>
                    <button>Ver Más</button>
                </div>
                <div class="product-card">
                    <img src="MODELO2.jpeg" alt="Bolso Modelo 2">
                    <h3>Modelo 2</h3>
                    <p>$499</p>
                    <button>Ver Más</button>
                </div>
                <div class="product-card">
                    <img src="MODELO3.jpeg" alt="Bolso Modelo 3">
                    <h3>Modelo 3</h3>
                    <p>$499</p>
                    <button>Ver Más</button>
                </div>
                <div class="product-card">
                    <img src="MODELO4.jpeg" alt="Bolso Modelo 4">
                    <h3>Modelo 4</h3>
                    <p>$499</p>
                    <button>Ver Más</button>
                </div>
                <div class="product-card">
                    <img src="MODELO5.jpeg" alt="Bolso Modelo 5">
                    <h3>Modelo 5</h3>
                    <p>$499</p>
                    <button>Ver Más</button>
                </div>
                <div class="product-card">
                    <img src="MODELO6.jpeg" alt="Bolso Modelo 6">
                    <h3>Modelo 6</h3>
                    <p>$499</p>
                    <button>Ver Más</button>
                </div>
                <div class="product-card">
                    <img src="MODELO7.jpeg" alt="Bolso Modelo 7">
                    <h3>Modelo 7</h3>
                    <p>$499</p>
                    <button>Ver Más</button>
                </div>
                <div class="product-card">
                    <img src="MODELO8.jpeg" alt="Bolso Modelo 8">
                    <h3>Modelo 8</h3>
                    <p>$499</p>
                    <button>Ver Más</button>
                </div>
                <div class="product-card">
                    <img src="MODELO9.jpeg" alt="Bolso Modelo 9">
                    <h3>Modelo 9</h3>
                    <p>$499</p>
                    <button>Ver Más</button>
                </div>
                <div class="product-card">
                    <img src="MODELO10.jpeg" alt="Bolso Modelo 10">
                    <h3>Modelo 10</h3>
                    <p>$499</p>
                    <button>Ver Más</button>
                </div>
                <div class="product-card">
                    <img src="MODELO11.jpeg" alt="Bolso Modelo 11">
                    <h3>Modelo 11</h3>
                    <p>$499</p>
                    <button>Ver Más</button>
                </div>
                <div class="product-card">
                    <img src="MODELO12.jpeg" alt="Bolso Modelo 12">
                    <h3>Modelo 12</h3>
                    <p>$499</p>
                    <button>Ver Más</button>
                </div>
                <div class="product-card">
                    <img src="MODELO13.jpeg" alt="Bolso Modelo 13">
                    <h3>Modelo 13</h3>
                    <p>$499</p>
                    <button>Ver Más</button>
                </div>
                <div class="product-card">
                    <img src="MODELO14.jpeg" alt="Bolso Modelo 14">
                    <h3>Modelo 14</h3>
                    <p>$499</p>
                    <button>Ver Más</button>
                </div>
                <div class="product-card">
                    <img src="MODELO15.jpeg" alt="Bolso Modelo 15">
                    <h3>Modelo 15</h3>
                    <p>$499</p>
                    <button>Ver Más</button>
                </div>
            </div>
        </div>
    </section>

    <!-- Redes Sociales -->
    <section class="social-media">
        <h2>Síguenos en nuestras redes sociales</h2>
        <a href="https://www.instagram.com/invites/contact/?igsh=feflm7etwaf7&utm_content=w2kp31e" target="_blank">Instagram</a>
        <a href="https://www.tiktok.com/@jm_caps_oficial?_t=8qskgyISbPZ&_r=1" target="_blank">TikTok</a>
        <a href="https://wa.me/5215544759776?text=Hola,%20me%20interesa%20saber%20más%20sobre%20sus%20productos!" target="_blank">WhatsApp</a>
    </section>

    <!-- Pie de página -->
    <footer class="footer">
        <p>&copy; 2024 JM CAPS. Todos los derechos reservados.</p>
    </footer>

    <script>
        // Efecto de carga del logo
        window.addEventListener('load', function() {
            const logo = document.getElementById('logo');
            logo.classList.add('loaded');
        });
    </script>

</body>
</html>

Mostrar texto citado
