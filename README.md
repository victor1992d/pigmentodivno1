<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>J&H'S Pigmento Divino</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" integrity="sha512-9usAa10IRO0HhonpyAIVpjrylPvoDwiPUiKdWk5t3PyolY1cOd4DSE0Ga+ri4AuTroPR5aQvXU9xC6qOPnzFeg==" crossorigin="anonymous" referrerpolicy="no-referrer" />
    <style>
        :root {
            --black: #222;
            --white: #fff;
            --pink: #ff69b4;
            --fuchsia: #ff00ff;
            --light-pink: #ffb6c1;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Arial', sans-serif;
        }

        body {
            background: var(--white);
            color: var(--black);
            line-height: 1.6;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }

        /* Header */
        header {
            background: var(--black);
            color: var(--white);
            padding: 20px 0;
            text-align: center;
            position: relative;
        }

        header h1 {
            font-size: 2.5em;
            margin-bottom: 5px;
            color: var(--pink);
        }

        header .logo {
            font-size: 1.5em;
            color: var(--fuchsia);
            font-family: 'Times New Roman', serif;
            margin-top: 0;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        header .logo img {
            max-height: 50px;
            margin-left: 10px;
        }

        header p {
            font-size: 1.1em;
            opacity: 0.8;
        }

        .logo {
            font-size: 2.5em;
            font-weight: bold;
            color: var(--fuchsia);
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .logo span {
            margin-left: 10px;
            font-size: 0.6em;
            color: var(--white);
        }

        .logo img {
            max-height: 50px;
            margin-right: 10px;
        }

        /* Navigation */
        nav {
            background: var(--light-pink);
            padding: 15px 0;
            text-align: center;
        }

        nav a {
            color: var(--black);
            text-decoration: none;
            margin: 0 15px;
            font-weight: bold;
            transition: color 0.3s ease;
        }

        nav a:hover {
            color: var(--fuchsia);
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(to right, var(--pink), var(--fuchsia));
            color: var(--white);
            padding: 80px 0;
            text-align: center;
            border-radius: 20px;
            margin: 30px 0;
            position: relative;
            overflow: hidden;
        }

        .hero img {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            object-fit: cover;
            opacity: 0.3;
            z-index: 0;
        }

        .hero h2,
        .hero p {
            position: relative;
            z-index: 1;
        }

        .hero h2 {
            font-size: 3em;
            margin-bottom: 20px;
        }

        .hero p {
            font-size: 1.2em;
            max-width: 800px;
            margin: 0 auto;
        }

        /* Services Section */
        .services {
            padding: 50px 0;
        }

        .service-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }

        .service-card {
            background: var(--light-pink);
            border-radius: 15px;
            padding: 25px;
            text-align: center;
            transition: transform 0.3s ease;
        }

        .service-card:hover {
            transform: translateY(-5px);
        }

        .service-card h3 {
            font-size: 1.8em;
            margin-bottom: 15px;
            color: var(--fuchsia);
        }

        .service-card p {
            font-size: 1.1em;
        }

        /* Micropigmentation & Microblading Sections */
        .micropigmentation,
        .microblading {
            padding: 50px 0;
        }

        .section-title {
            font-size: 2.5em;
            text-align: center;
            margin-bottom: 30px;
            color: var(--pink);
        }

        .image-gallery {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 15px;
        }

        .gallery-item {
            width: 250px;
            height: 250px;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }

        .gallery-item img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            transition: transform 0.3s ease;
        }

        .gallery-item:hover img {
            transform: scale(1.1);
        }

        /* Contact Section */
        .contact {
            background: var(--black);
            color: var (--white);
            padding: 50px 0;
            text-align: center;
        }

        .contact h2 {
            font-size: 2.5em;
            margin-bottom: 20px;
            color: var(--pink);
        }

        .contact-info {
            font-size: 1.2em;
            margin-bottom: 15px;
        }

        .contact-info a {
            color: var(--white);
            text-decoration: none;
            transition: color 0.3s ease;
        }

        .contact-info a:hover {
            color: var(--fuchsia);
        }

        /* Footer */
        footer {
            background: var (--black);
            color: var (--white);
            text-align: center;
            padding: 20px 0;
            font-size: 0.9em;
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <h1>J&H'S</h1>
            <div class="logo">
                <h2 style="font-weight: normal;">Pigmento Divino</h2>
                <img id="header-background" src=" https://mail.google.com/mail/u/0?ui=2&ik=79970a0255&attid=0.12&permmsgid=msg-a:r-9201921208579153125&th=194f7c09ecad064f&view=att&disp=safe&realattid=194f7c06ed3fd3a2e7ad&zw         " alt="Header Background">
            </div>
            <p>Realzando tu belleza natural con arte y precisión</p>
        </div>
    </header>

    <nav>
        <div class="container">
            <a href="#micropigmentacion">Micropigmentación</a>
            <a href="#microblading">Microblading</a>
            <a href="#estetica">Estética</a>
            <a href="#contacto">Contacto</a>
        </div>
    </nav>

    <section class="hero">
        <img id="hero-background" src="https://i.imgur.com/Vt00iR2.jpeg" alt="Background Image">
        <div class="container">
            <h2>Descubre el arte de la belleza permanente</h2>
            <p>En J&H'S Pigmento Divino, transformamos tu rostro con técnicas avanzadas de micropigmentación y microblading. ¡Realza tu belleza y simplifica tu rutina diaria!</p>
        </div>
    </section>

    <section class="services">
        <div class="container">
            <h2 class="section-title">Nuestros Servicios</h2>
            <div class="service-grid">
                <div class="service-card">
                    <h3>Micropigmentación de Cejas</h3>
                    <p>Define y da forma a tus cejas con resultados naturales y duraderos.</p>
                </div>
                <div class="service-card">
                    <h3>Micropigmentación de Labios</h3>
                    <p>Realza el color y la forma de tus labios para una sonrisa perfecta.</p>
                </div>
                <div class="service-card">
                    <h3>Micropigmentación de Líneas de Ojos</h3>
                    <p>Define tu mirada con un delineado permanente que resalta tus ojos.</p>
                </div>
                <div class="service-card">
                    <h3>Microblading</h3>
                    <p>Técnica manual para crear trazos finos que imitan el vello natural de las cejas.</p>
                </div>
                <div class="service-card">
                    <h3>Microlady</h3>
                    <p>Tratamiento innovador para rejuvenecer y revitalizar la piel.</p>
                </div>
                <div class="service-card">
                    <h3>Depilación</h3>
                    <p>Eliminación del vello no deseado con métodos suaves y efectivos.</p>
                </div>
                <div class="service-card">
                    <h3>Lifting de Pestañas</h3>
                    <p>Realza y curva tus pestañas para una mirada más abierta y atractiva.</p>
                </div>
                <div class="service-card">
                    <h3>Limpieza de Cutis</h3>
                    <p>Tratamiento profundo para limpiar, exfoliar e hidratar tu piel.</p>
                </div>
            </div>
        </div>
    </section>

    <section id="micropigmentacion" class="micropigmentacion">
        <div class="container">
            <h2 class="section-title">Micropigmentación</h2>
            <p style="text-align: center; font-size: 1.2em; margin-bottom: 20px;">Descubre la magia de la micropigmentación: cejas perfectas, labios definidos y una mirada impactante. ¡Resultados duraderos y naturales!</p>
            <div class="image-gallery" id="micropigmentacion-gallery">
                <!-- La imagen se agrega aquí -->
                <div class="gallery-item">
                    <img src="https://mail.google.com/mail/u/0?ui=2&ik=79970a0255&attid=0.9&permmsgid=msg-a:r-9201921208579153125&th=194f7c09ecad064f&view=att&disp=safe&realattid=194f7c06ed3fbf611e3a&zw          " alt="Imagen de micropigmentación 1">
                </div>
                <!-- La imagen se agrega aquí -->
                <div class="gallery-item">
                    <img src="https://mail.google.com/mail/u/0?ui=2&ik=79970a0255&attid=0.24&permmsgid=msg-a:r-9201921208579153125&th=194f7c09ecad064f&view=att&disp=safe&realattid=194f7c06ed3fd2c16f9b&zw       " alt="Imagen de micropigmentación 2">
                </div>
                <!-- La imagen se agrega aquí -->
                <div class="gallery-item">
                    <img src="https://mail.google.com/mail/u/0?ui=2&ik=79970a0255&attid=0.34&permmsgid=msg-a:r-9201921208579153125&th=194f7c09ecad064f&view=att&disp=safe&realattid=194f7c06ed3fd728c7e15&zw   " alt="Imagen de micropigmentación 3">
                </div>
            </div>
        </div>
    </section>

    <section id="microblading" class="microblading">
        <div class="container">
            <h2 class="section-title">Microblading</h2>
            <p style="text-align: center; font-size: 1.2em; margin-bottom: 20px;">Logra unas cejas perfectas con nuestra técnica de microblading. ¡Trazos precisos que imitan el vello natural para un look impecable!</p>
            <div class="image-gallery" id="microblading-gallery">
                <!-- La imagen se agrega aquí -->
                <div class="gallery-item">
                    <img src="https://mail.google.com/mail/u/0?ui=2&ik=79970a0255&attid=0.42&permmsgid=msg-a:r-9201921208579153125&th=194f7c09ecad064f&view=att&disp=safe&realattid=194f7c06ed3f6bb5904c&zw      " alt="Imagen de microblading 1">
                </div>
                <!-- La imagen se agrega aquí -->
                <div class="gallery-item">
                    <img src="https://mail.google.com/mail/u/0?ui=2&ik=79970a0255&attid=0.19&permmsgid=msg-a:r-9201921208579153125&th=194f7c09ecad064f&view=att&disp=safe&realattid=194f7c06ed3fd565d7c5&zw     " alt="Imagen de microblading 2">
                </div>
                <!-- La imagen se agrega aquí -->
                <div class="gallery-item">
                    <img src="https://mail.google.com/mail/u/0?ui=2&ik=79970a0255&attid=0.9&permmsgid=msg-a:r-9201921208579153125&th=194f7c09ecad064f&view=att&disp=safe&realattid=194f7c06ed3fbf611e3a&zw         " alt="Imagen de microblading 3">
                </div>
            </div>
        </div>
    </section>

    <section id="estetica" class="estetica">
        <div class="container">
            <h2 class="section-title">Otros Servicios de Estética</h2>
            <p style="text-align: center; font-size: 1.2em; margin-bottom: 20px;">Explora nuestra gama de servicios de estética: depilación, lifting de pestañas, limpieza de cutis y mucho más. ¡Consiéntete y realza tu belleza natural!</p>
            <div class="image-gallery" id="estetica-gallery">
                <!-- La imagen se agrega aquí -->
                <div class="gallery-item">
                    <img src=" https://mail.google.com/mail/u/0?ui=2&ik=79970a0255&attid=0.23&permmsgid=msg-a:r-9201921208579153125&th=194f7c09ecad064f&view=att&disp=safe&realattid=194f7c06ed4f9de94bd26&zw       " alt="Imagen de estética 1">
                </div>
                <!-- La imagen se agrega aquí -->
                <div class="gallery-item">
                    <img src="https://mail.google.com/mail/u/0?ui=2&ik=79970a0255&attid=0.11&permmsgid=msg-a:r-9201921208579153125&th=194f7c09ecad064f&view=att&disp=safe&realattid=194f7c06ed3f80d8d1c12&zw     " alt="Imagen de estética 2">
                </div>
                <!-- La imagen se agrega aquí -->
                <div class="gallery-item">
                    <img src="https://mail.google.com/mail/u/0?ui=2&ik=79970a0255&attid=0.23&permmsgid=msg-a:r-9201921208579153125&th=194f7c09ecad064f&view=att&disp=safe&realattid=194f7c06ed4f9de94bd26&zw       " alt="Imagen de estética 3">
                  
                </div>
            </div>
        </div>
     <section id="contacto" class="contact">
        <div class="container">
            <h2>Contacto</h2>
            <p class="contact-info">¡Contáctanos para agendar tu cita y transformar tu belleza!</p>
            <p class="contact-info">Teléfono: <a href="tel:+34665970550">+34 665 97 05 50</a></p>
            <p class="contact-info">Email: <a href="mailto:info@pigmentodivino.com">info@pigmentodivino.com</a></p>
            <p class="contact-info">Dirección: España, Barcelona          M dirección es Carrer de les torres 29 local 4  c.p 08042 Barcelona</p>
            <p class="contact-info">Horario: Lunes a domingo 9:00 AM - 22 PM</p>
        </div>
    </section>

    <footer>
        <div class="container">
            <p>&copy; 2024 J&H'S Pigmento Divino. Todos los derechos reservados.</p>
        </div>
    </footer>

        <div class="container">
            <p>&copy; 2024 J&H'S Pigmento Divino. Todos los derechos reservados.</p>
        </div>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', () => {
            loadImages('micropigmentacion');
            loadImages('microblading');
            loadImages('estetica');
            loadBackground();
        });

        function loadImages(category) {
            const images = JSON.parse(localStorage.getItem(category)) || [];
            images.forEach(imageUrl => {
                addImageToGallery(category, imageUrl);
            });
        }

        function addImageToGallery(category, imageUrl) {
            const gallery = document.getElementById(`${category}-gallery`);
            const galleryItem = document.createElement('div');
            galleryItem.className = 'gallery-item';
            const imgElement = document.createElement('img');
            imgElement.src = imageUrl;
            imgElement.alt = 'Imagen subida';
            galleryItem.appendChild(imgElement);
            gallery.appendChild(galleryItem);
        }

        function loadBackground() {
            const imageUrl = localStorage.getItem('heroBackground');
            if (imageUrl) {
                setBackground(imageUrl);
                setHeaderBackground(imageUrl);
            }
        }

        function setBackground(imageUrl) {
            document.getElementById('hero-background').src = imageUrl;
        }

        function setHeaderBackground(imageUrl) {
            document.getElementById('header-background').src = imageUrl;
        }
    </script>
</body>
</html>
     


