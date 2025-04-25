# QuevePec-REPORDUCCION DE PESCADOS Y VENTAS
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Quevepec | Tienda y Portafolio Profesional</title>
  <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;700&display=swap" rel="stylesheet">
  <style>
    :root {
      --primary-color: #000;
      --secondary-color: #fff;
      --accent-color: #f2f2f2;
      --hover-color: #e5e5e5;
      --text-dark: #1a1a1a;
      --text-light: #fff;
    }
    * {margin: 0; padding: 0; box-sizing: border-box;}
    body {
      font-family: 'Roboto', sans-serif;
      background-color: var(--secondary-color);
      color: var(--text-dark);
    }
    header, footer {
      background: var(--primary-color);
      color: var(--text-light);
      padding: 20px 40px;
      text-align: center;
    }
    nav a {
      margin: 0 15px;
      color: var(--text-light);
      text-decoration: none;
      font-weight: bold;
    }
    .hero {
      background: url('https://source.unsplash.com/1600x500/?fish,aquaculture') center/cover no-repeat;
      padding: 80px 20px;
      text-align: center;
      color: var(--text-light);
    }
    .hero h1 {
      font-size: 3em;
      text-transform: uppercase;
      margin-bottom: 10px;
    }
    .hero p {
      font-size: 1.2em;
      max-width: 700px;
      margin: auto;
    }
    .section {
      padding: 60px 40px;
      max-width: 1200px;
      margin: auto;
    }
    .section h2 {
      font-size: 2em;
      margin-bottom: 30px;
      text-align: center;
      text-transform: uppercase;
    }
    .products, .portfolio, .team, .testimonials {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 30px;
    }
    .card {
      background: #fff;
      border: 1px solid #ddd;
      padding: 20px;
      transition: 0.3s;
    }
    .card:hover {
      box-shadow: 0 4px 15px rgba(0,0,0,0.1);
      transform: translateY(-5px);
    }
    .card img {
      width: 100%;
      height: 200px;
      object-fit: cover;
      margin-bottom: 15px;
    }
    .card h3 {
      margin-bottom: 10px;
    }
    .price {
      color: green;
      font-weight: bold;
    }
    .testimonial {
      background: #fafafa;
      border-left: 4px solid var(--primary-color);
      padding: 20px;
    }
    .map {
      width: 100%;
      height: 400px;
      border: none;
      margin-top: 30px;
    }
    .contact-form input, .contact-form textarea {
      width: 100%;
      margin-bottom: 15px;
      padding: 10px;
      border: 1px solid #ccc;
    }
    .contact-form button {
      background: var(--primary-color);
      color: var(--text-light);
      border: none;
      padding: 10px 20px;
      font-weight: bold;
      cursor: pointer;
    }
    footer .footer-links {
      margin-top: 15px;
    }
    footer .footer-links a {
      color: #aaa;
      margin: 0 10px;
      text-decoration: none;
      font-size: 0.9em;
    }
  </style>
</head>
<body>
  <header>
    <h1>Quevepec</h1>
    <nav>
      <a href="#">Inicio</a>
      <a href="#productos">Productos</a>
      <a href="#portafolio">Portafolio</a>
      <a href="#equipo">Equipo</a>
      <a href="#testimonios">Testimonios</a>
      <a href="#contacto">Contacto</a>
    </nav>
  </header>

  <div class="hero">
    <h1>Innovación en Acuicultura</h1>
    <p>Reproducción y comercialización de pescado con tecnología y pasión por la sostenibilidad.</p>
  </div>

  <section class="section" id="productos">
    <h2>Productos Destacados</h2>
    <div class="products">
      <div class="card">
        <img src="https://source.unsplash.com/400x300/?fish" alt="Tilapia">
        <h3>Tilapia Premium</h3>
        <p>Pescado fresco, criado en condiciones controladas y saludables.</p>
        <p class="price">S/ 25.00 x Kg</p>
      </div>
      <div class="card">
        <img src="https://source.unsplash.com/400x300/?fisherman" alt="Crianza">
        <h3>Asesoría de Crianza</h3>
        <p>Consultoría especializada en reproducción y cultivo de peces.</p>
        <p class="price">Desde S/ 150.00</p>
      </div>
      <div class="card">
        <img src="https://source.unsplash.com/400x300/?aquarium" alt="Sistema">
        <h3>Sistemas de Acuicultura</h3>
        <p>Equipos modernos para mejorar tu producción piscícola.</p>
        <p class="price">Desde S/ 500.00</p>
      </div>
    </div>
  </section>

  <section class="section" id="portafolio">
    <h2>Proyectos Realizados</h2>
    <div class="portfolio">
      <div class="card">
        <img src="https://source.unsplash.com/400x300/?pond" alt="Estanque">
        <h3>Instalación de Estanques</h3>
        <p>Diseño y ejecución de estanques eficientes.</p>
      </div>
      <div class="card">
        <img src="https://source.unsplash.com/400x300/?tank" alt="Tanques">
        <h3>Tanques de Recirculación</h3>
        <p>Implementación de sistemas para recirculación de agua.</p>
      </div>
    </div>
  </section>

  <section class="section" id="equipo">
    <h2>Nuestro Equipo</h2>
    <div class="team">
      <div class="card">
        <img src="https://source.unsplash.com/400x300/?person,ceo" alt="CEO">
        <h3>Juan Pérez</h3>
        <p>Fundador y experto en ingeniería acuícola.</p>
      </div>
      <div class="card">
        <img src="https://source.unsplash.com/400x300/?woman,scientist" alt="Bio">
        <h3>María Gómez</h3>
        <p>Bióloga marina, responsable de calidad.</p>
      </div>
    </div>
  </section>

  <section class="section" id="testimonios">
    <h2>Testimonios</h2>
    <div class="testimonials">
      <div class="testimonial">
        <p>“Gracias a Quevepec, mejoramos nuestra producción en un 40%. ¡Excelente servicio!”</p>
        <strong>- Cooperativa Pesquera Sur</strong>
      </div>
      <div class="testimonial">
        <p>“La calidad del pescado es excelente y el equipo muy profesional.”</p>
        <strong>- Restaurante Marino El Anzuelo</strong>
      </div>
    </div>
  </section>

  <section class="section" id="contacto">
    <h2>Contacto</h2>
    <form class="contact-form">
      <input type="text" placeholder="Nombre" required>
      <input type="email" placeholder="Correo electrónico" required>
      <textarea rows="5" placeholder="Mensaje"></textarea>
      <button type="submit">Enviar</button>
    </form>
    <iframe class="map" src="https://maps.google.com/maps?q=peru&z=6&output=embed"></iframe>
  </section>

  <footer>
    <p>© 2025 Quevepec. Todos los derechos reservados.</p>
    <div class="footer-links">
      <a href="#">Términos</a>
      <a href="#">Privacidad</a>
      <a href="#">Soporte</a>
    </div>
  </footer>
</body>
</html>
