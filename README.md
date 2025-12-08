<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aura Jewelry — Pura Esencia</title>

    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;700&display=swap" rel="stylesheet">

    <style>
        :root {
            --color-principal: #1a1a1a;
            --color-secundario: #555;
            --color-fondo: #fff;
            --fuente: 'Roboto', sans-serif;
            --max-width: 1000px;
        }

        body {
            margin: 0;
            font-family: var(--fuente);
            background: var(--color-fondo);
            color: var(--color-principal);
            line-height: 1.6;
            font-weight: 300;
        }

        a {
            text-decoration: none;
            color: var(--color-principal);
            transition: .2s;
        }
        a:hover { color: var(--color-secundario); }

        .container {
            max-width: var(--max-width);
            margin: 0 auto;
            padding: 0 20px;
        }

        
        header {
            background: var(--color-fondo);
            padding: 25px 0;
            border-bottom: 1px solid #eee;
        }
        nav ul {
            list-style: none;
            display: flex;
            justify-content: center;
            gap: 40px;
            margin: 0;
            padding: 0;
        }
        nav a {
            font-weight: 400;
            font-size: 15px;
            text-transform: uppercase;
        }

        
        .hero-banner {
            min-height: 70vh;
            background-size: cover;
            background-position: center;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            color: var(--color-fondo);
            position: relative;
        }
        .hero-banner::before {
            content: '';
            position: absolute;
            inset: 0;
            background: rgba(0,0,0,.4);
            z-index: 1;
        }
        .hero-content {
            position: relative;
            z-index: 2;
            padding: 20px;
        }
        .hero-content h1 {
            font-size: 3.5rem;
            margin-bottom: 15px;
            font-weight: 700;
        }
        .hero-content p {
            font-size: 1.2rem;
            max-width: 700px;
            margin: 0 auto 40px;
        }
        .btn {
            background: var(--color-fondo);
            color: var(--color-principal);
            padding: 12px 30px;
            font-weight: 700;
            border: 1px solid var(--color-fondo);
        }
        .btn:hover {
            background: transparent;
            color: var(--color-fondo);
        }

        
        section { padding: 80px 0; text-align: center; }
        h2 {
            font-size: 2rem;
            margin-bottom: 50px;
            text-transform: uppercase;
            font-weight: 700;
        }

        
        .grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 40px;
        }
        .card img {
            width: 100%;
            height: 300px;
            object-fit: cover;
            border: 1px solid #eee;
            margin-bottom: 20px;
        }
        .card h3 { font-size: 1.2rem; font-weight: 700; }
        .precio { color: var(--color-secundario); margin-bottom: 15px; }

        
        .about p {
            max-width: 800px;
            margin: auto;
            font-size: 1.1rem;
            color: var(--color-secundario);
        }

        
        .formulario { background: #f8f8f8; }
        form {
            max-width: 500px;
            margin: auto;
            background: #fff;
            padding: 40px;
            border: 1px solid #eee;
            display: grid;
            gap: 15px;
        }
        label { font-size: 14px; font-weight: 700; text-align: left; }
        input, select, textarea {
            padding: 12px;
            border: 1px solid #ccc;
            font-size: 15px;
        }
        button {
            background: var(--color-principal);
            color: #fff;
            padding: 14px;
            border: none;
            font-weight: 700;
            cursor: pointer;
        }
        button:hover { background: var(--color-secundario); }

        
        footer {
            text-align: center;
            padding: 30px;
            font-size: 14px;
            color: var(--color-secundario);
            border-top: 1px solid #eee;
        }

        @media(max-width:768px) {
            .hero-content h1 { font-size: 2.4rem; }
            .hero-content p { font-size: 1rem; }
            h2 { font-size: 1.6rem; }
        }
    </style>
</head>

<body>

    <header>
        <nav class="container">
            <ul>
                <li><a href="#inicio">Inicio</a></li>
                <li><a href="#productos">Colección</a></li>
                <li><a href="#about">Marca</a></li>
                <li><a href="#contacto">Contacto</a></li>
            </ul>
        </nav>
    </header>

   
    <section id="inicio" class="hero-banner" style="background-image: url('https://coletta.mx/cdn/shop/files/new_jewellery.webp?v=1720909888&width=2000');">
        <div class="hero-content">
            <h1>Aura</h1>
            <p>Simplicidad que ilumina. Joyería que realza tu esencia.</p>
            <a class="btn" href="#productos">Explorar</a>
        </div>
    </section>

    <section id="productos" class="productos">
        <div class="container">
            <h2>Colección</h2>

            <div class="grid">

                <div class="card">
                    <img src="https://image3.nihaojewelry.com/fit-in/0x0/filters:quality(80)/filters:format(webp)/product/2025/7/24/1948306919433310208/Collar-Largo-Ajustable-Acero-Inoxidable-Pintado-De-Oro-18K-Cadena-De-Su-ter-Elegante-Para-Mujer-Accesorio-De-Joyer-a-Para-Todas-Las-Estaciones.jpg" alt="Collar">
                    <h3>Collar Minimal Oro</h3>
                    <p class="precio">$1,299 MXN</p>
                </div>

                <div class="card">
                    
                    <img src="https://resources.sears.com.mx/medios-plazavip/mkt/6368690ad6614_020r01mjpg.jpg?scale=500&qlty=75" alt="Anillo">
                    <h3>Anillo Pura Plata</h3>
                    <p class="precio">$899 MXN</p>
                </div>

                <div class="card">
                    
                    <img src="https://i5.walmartimages.com/asr/2f186496-8f2e-4abb-8767-185b2fbd77ab.425efc411a652b5a8277d56b66d06963.jpeg?odnHeight=612&odnWidth=612&odnBg=FFFFFF" alt="Pulsera">
                    <h3>Pulsera Brillo Sutil</h3>
                    <p class="precio">$1,050 MXN</p>
                </div>

                <div class="card">
                 
                    <img src="https://m.media-amazon.com/images/I/51z-Ii6HxcL._AC_SY1000_.jpg" alt="Aretes">
                    <h3>Aretes Geométricos</h3>
                    <p class="precio">$750 MXN</p>
                </div>

            </div>
        </div>
    </section>

    <section id="about" class="about">
        <div class="container">
            <h2>Nuestra Marca</h2>
            <p>
                En Aura creemos en la belleza minimalista, la elegancia sutil y las piezas que hablan por sí mismas.
                Cada joya está diseñada para acompañarte toda la vida.
            </p>
        </div>
    </section>

    <section id="contacto" class="formulario">
        <div class="container">
            <h2>Contáctanos</h2>

             <form id="padelForm"> 
        <fieldset>
            <legend></legend>
            
            <label for="nombre">Nombre:</label>
            <input type="text" id="nombre" name="usuario_nombre" placeholder="Nombre (s)">
            <br><br>
            
            <label for="correo">Correo electrónico:</label>
            <input type="email" id="correo" name="correo" placeholder="ejemplo@.com" required>
            <br><br>
            
            <label for="telefono">Teléfono:</label>
            <input type="tel" id="telefono" name="telefono" placeholder="12-223-2987" required>
        </fieldset>
        <br><br>
        <button type="submit">Enviar Formulario</button>
    </form>
</div>

<script>
    // URL de tu Google Apps Script
    const scriptURL = ['https://script.google.com/macros/s/AKfycbz1moelb5M4-2j6tKIH2FPpIQMgLp15zp6_6xJKOJ6oOYIFi7M6qwEhX5qqWF2R-jUCVg/exec'](https://script.google.com/macros/s/AKfycbz1moelb5M4-2j6tKIH2FPpIQMgLp15zp6_6xJKOJ6oOYIFi7M6qwEhX5qqWF2R-jUCVg/exec);
    
    // Obtenemos el formulario por su ID
    const form = document.getElementById('padelForm');

    form.addEventListener('submit', e => {
        e.preventDefault(); // Detiene el envío normal (para que no te redirija)
        
        // Desactivamos el botón y mostramos un mensaje temporal
        const submitButton = form.querySelector('button[type="submit"]');
        submitButton.disabled = true;
        submitButton.textContent = 'Enviando...';
        
        // Enviamos los datos usando Fetch API
        fetch(scriptURL, { method: 'POST', body: new FormData(form)})
            .then(response => {
                // El script devuelve JSON con {"result": "success"}
                if (response.ok) {
                    // Si es exitoso, mostramos una alerta y limpiamos el formulario.
                    alert('¡Gracias! Por unirte a la Familia.');
                    form.reset(); 
                } else {
                    alert('Error: No se pudo conectar con el servidor de Google.');
                }
            })
            .catch(error => {
                alert('Ocurrió un error al enviar: ' + error.message);
                console.error('Error!', error.message);
            })
            .finally(() => {
                // Restauramos el botón después de la operación
                submitButton.disabled = false;
                submitButton.textContent = 'Enviar Formulario';
            });
    });
</script>

<footer>
    <p style="background-color:floralwhite">©️ 2025 AURA. Todos los derechos reservados.</p>
</footer>
</body>
</html>
