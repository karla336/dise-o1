<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Karla Aguilar | Diseñadora Gráfica</title>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=DM+Sans:ital,opsz,wght@0,9..40,100..1000;1,9..40,100..1000&family=Playfair+Display:ital,wght@0,400..900;1,400..900&display=swap" rel="stylesheet">
    <style>
        /* --- Variables de Colores Pastel --- */
        :root {
            --bg-principal: #f9f6f0;
            --pastel-rosa: #ffd6d6;
            --pastel-lila: #e8dbfc;
            --pastel-verde: #d2e7df;
            --texto-oscuro: #2b2b2b;
            --texto-secundario: #6e6e6e;
            --blanco: #ffffff;
        }

        /* --- Estilos Generales --- */
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            font-family: 'DM Sans', sans-serif;
            background-color: var(--bg-principal);
            color: var(--texto-oscuro);
            line-height: 1.6;
        }

        .container {
            max-width: 1100px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* --- Navbar --- */
        header {
            padding: 30px 0;
        }

        .nav-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-family: 'Playfair Display', serif;
            font-size: 1.8rem;
            font-weight: 700;
            letter-spacing: -0.5px;
        }

        .btn-contacto {
            background-color: var(--texto-oscuro);
            color: var(--blanco);
            text-decoration: none;
            padding: 12px 24px;
            border-radius: 50px;
            font-weight: 500;
            font-size: 0.9rem;
            transition: all 0.3s ease;
        }

        .btn-contacto:hover {
            transform: translateY(-2px);
            opacity: 0.9;
        }

        /* --- Hero Section --- */
        .hero {
            padding: 80px 0 60px 0;
            text-align: center;
        }

        .hero h1 {
            font-family: 'Playfair Display', serif;
            font-size: 3.5rem;
            line-height: 1.2;
            margin-bottom: 24px;
            font-weight: 600;
        }

        .hero p {
            font-size: 1.2rem;
            color: var(--texto-secundario);
            max-width: 600px;
            margin: 0 auto;
        }

        /* --- Servicios --- */
        .servicios {
            padding: 80px 0;
            background-color: var(--blanco);
            border-radius: 40px 40px 0 0;
        }

        .servicios-titulo {
            text-align: center;
            font-family: 'Playfair Display', serif;
            font-size: 2.5rem;
            margin-bottom: 50px;
        }

        .grid-servicios {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }

        .card {
            padding: 40px;
            border-radius: 24px;
            transition: transform 0.3s ease;
        }

        .card:hover {
            transform: translateY(-5px);
        }

        .card-1 { background-color: var(--pastel-rosa); }
        .card-2 { background-color: var(--pastel-lila); }
        .card-3 { background-color: var(--pastel-verde); }

        .card h3 {
            font-family: 'Playfair Display', serif;
            font-size: 1.6rem;
            margin-bottom: 15px;
        }

        .card p {
            color: var(--texto-oscuro);
            opacity: 0.8;
            font-size: 1rem;
        }

        /* --- Sección de Contacto (Formulario) --- */
        .contacto-section {
            padding: 80px 0;
            background-color: var(--bg-principal);
            text-align: center;
        }

        .contacto-section h2 {
            font-family: 'Playfair Display', serif;
            font-size: 2.5rem;
            margin-bottom: 40px;
        }

        .form-contacto {
            max-width: 500px;
            margin: 0 auto;
            background: var(--blanco);
            padding: 40px;
            border-radius: 24px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.03);
            text-align: left;
        }

        .form-contacto label {
            display: block;
            margin-bottom: 20px;
            font-weight: 500;
            font-size: 0.95rem;
            color: var(--texto-oscuro);
        }

        .form-contacto input[type="email"],
        .form-contacto textarea {
            width: 100%;
            padding: 14px;
            margin-top: 8px;
            border: 1px solid #e2e2e2;
            border-radius: 12px;
            background-color: #fafafa;
            font-family: 'DM Sans', sans-serif;
            font-size: 1rem;
            transition: all 0.3s ease;
            outline: none;
        }

        .form-contacto input[type="email"]:focus,
        .form-contacto textarea :focus {
            border-color: var(--pastel-lila);
            background-color: var(--blanco);
            box-shadow: 0 0 0 4px rgba(232, 219, 252, 0.4);
        }

        .form-contacto textarea {
            height: 120px;
            resize: none;
        }

        .form-contacto button[type="submit"] {
            width: 100%;
            background-color: var(--pastel-lila);
            color: var(--texto-oscuro);
            border: none;
            padding: 16px;
            border-radius: 50px;
            font-size: 1.1rem;
            font-weight: 600;
            cursor: pointer;
            box-shadow: 0 4px 14px rgba(232, 219, 252, 0.4);
            transition: all 0.3s ease;
            margin-top: 10px;
        }

        .form-contacto button[type="submit"]:hover {
            transform: translateY(-2px);
            box-shadow: 0 6px 20px rgba(232, 219, 252, 0.6);
        }

        /* --- Footer --- */
        footer {
            background-color: var(--blanco);
            text-align: center;
            padding: 40px 0;
            font-size: 0.9rem;
            color: var(--texto-secundario);
            border-top: 1px solid #f0f0f0;
        }

        /* Responsive */
        @media (max-width: 768px) {
            .hero h1 { font-size: 2.5rem; }
            .grid-servicios { grid-template-columns: 1fr; }
            .form-contacto { padding: 30px 20px; }
        }
    </style>
</head>
<body>

    <header>
        <div class="container nav-container">
            <div class="logo">karla aguilar.</div>
            <a href="#contacto" class="btn-contacto">Hablemos</a>
        </div>
    </header>

    <section class="hero">
        <div class="container">
            <h1>Llevo la identidad de tu marca al siguiente nivel en redes sociales</h1>
            <p>Diseño soluciones visuales estéticas, modernas y estratégicas para que tu negocio destaque en el feed de tus clientes.</p>
        </div>
    </section>

    <section class="servicios">
        <div class="container">
            <h2 class="servicios-titulo">Mis Servicios</h2>
            
            <div class="grid-servicios">
                <div class="card card-1">
                    <h3>Diseño de Feeds</h3>
                    <p>Estructuración visual armónica y atractiva para que tu perfil de Instagram cuente una historia coherente a primera vista.</p>
                </div>
                
                <div class="card card-2">
                    <h3>Diseño de Posts</h3>
                    <p>Contenido diario optimizado e impactante: carruseles, publicaciones estáticas y plantillas personalizadas que generan engagement.</p>
                </div>
                
                <div class="card card-3">
                    <h3>Stories & Highlights</h3>
                    <p>Diseño de portadas para historias destacadas y layouts dinámicos para tus historias diarias, manteniendo siempre la estética de tu marca.</p>
                </div>
            </div>
        </div>
    </section>

    <section class="contacto-section" id="contacto">
        <div class="container">
            <h2>¿Trabajamos juntos?</h2>
            
            <form class="form-contacto" action="https://formspree.io/f/mnjkozrw" method="POST">
                <label>
                    Tu email:
                    <input type="email" name="email" placeholder="ejemplo@correo.com" required>
                </label>
                <label>
                    Tu mensaje:
                    <textarea name="message" placeholder="Cuéntame un poco sobre tu proyecto..." required></textarea>
                </label>
                <button type="submit">Enviar</button>
            </form>

        </div>
    </section>

    <footer>
        <div class="container">
            <p>&copy; 2026 Karla Aguilar. Todos los derechos reservados.</p>
        </div>
    </footer>

</body>
</html>
