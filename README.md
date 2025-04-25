# QuevePec-REPORDUCCION DE PESCADOS Y VENTAS
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Quevepec | Tienda Profesional</title>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }
    body { font-family: 'Inter', sans-serif; background: #f9f9f9; color: #222; }
    header { background: #0e3c3d; color: white; padding: 20px 40px; display: flex; justify-content: space-between; align-items: center; }
    header h1 { font-size: 1.8em; }
    nav a { margin-left: 25px; color: white; text-decoration: none; font-weight: 600; }
    .hero { background: url('https://source.unsplash.com/1600x600/?fish,fishing') center/cover no-repeat; color: white; padding: 100px 40px; text-align: center; }
    .hero h2 { font-size: 3em; margin-bottom: 15px; }
    .hero p { font-size: 1.2em; }
    .section { padding: 60px 40px; max-width: 1200px; margin: auto; }
    .section h2 { font-size: 2em; margin-bottom: 30px; color: #0e3c3d; }
    .products, .portfolio-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 30px; }
    .card { background: white; border-radius: 10px; overflow: hidden; box-shadow: 0 4px 12px rgba(0,0,0,0.1); transition: transform .3s; cursor: pointer; }
    .card:hover { transform: translateY(-5px); }
    .card img { width: 100%; height: 200px; object-fit: cover; }
    .card-body { padding: 20px; }
    .card-body h3 { margin-bottom: 10px; font-size: 1.2em; }
    .card-body p { font-size: 0.95em; color: #444; }
    .card-body .price { font-weight: bold; margin-top: 10px; color: #0e3c3d; }
    .portfolio-modal { display: none; position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: rgba(0,0,0,0.7); align-items: center; justify-content: center; }
    .modal-content { background: white; padding: 30px; max-width: 600px; width: 90%; border-radius: 10px; position: relative; }
    .modal-content img { width: 100%; border-radius: 10px; margin-bottom: 20px; }
    .modal-close { position: absolute; top: 10px; right: 20px; font-size: 1.5em; cursor: pointer; }
    footer { background: #0e3c3d; color: white; padding: 40px; text-align: center; margin-top: 60px; }
    .footer-links { margin-top: 20px; }
    .footer-links a { margin: 0 15px; color: #ccc; text-decoration: none; font-size: 0.95em; }
    @media (max-width: 768px) {
      header { flex-direction: column; align-items: flex-start; }
      nav a { margin: 10px 10px 0 0; display: inline-block; }
    }
  </style>
</head>
<body>
  <header>
    <h1>Quevepec</h1>
    <nav>
      <a href="#inicio">Inicio</a>
      <a href="#productos">Productos</a>
      <a href="#portafolio">Portafolio</a>
      <a href="#empresa">Nosotros</a>
      <a href="#contacto">Contacto</a>
    </nav>
  </header>

  <section class="hero" id="inicio">
    <h2>La tienda oficial de Quevepec</h2>
    <p>Expertos en reproducción de peces y productos de calidad para la pesca</p>
  </section>

  <section class="section" id="productos">
    <h2>Productos Destacados</h2>
    <div class="products">
      <div class="card">
        <img src="https://source.unsplash.com/400x300/?fishing-rod" alt="Caña de Pesca">
        <div class="card-body">
          <h3>Caña de Pesca Pro</h3>
          <p>Diseño ergonómico, resistente, ideal para pesca deportiva y comercial.</p>
          <p class="price">$85.00</p>
        </div>
      </div>
      <div class="card">
        <img src="https://source.unsplash.com/400x300/?fishing-net" alt="Red de Pesca">
        <div class="card-body">
          <h3>Red de Pesca Eco</h3>
          <p>Redes de bajo impacto ambiental, seguras para la fauna marina.</p>
          <p class="price">$39.00</p>
        </div>
      </div>
      <div class="card">
        <img src="https://source.unsplash.com/400x300/?aquaculture" alt="Tanque de Cría">
        <div class="card-body">
          <h3>Tanque de Cría Profesional</h3>
          <p>Tanques especiales para reproducción de peces, alta eficiencia y durabilidad.</p>
          <p class="price">$299.00</p>
        </div>
      </div>
    </div>
  </section>

  <section class="section" id="portafolio">
    <h2>Portafolio de Proyectos</h2>
    <div class="portfolio-grid">
      <div class="card" onclick="showModal('Proyecto de cría intensiva', 'https://source.unsplash.com/600x400/?fish-tank', 'Instalación moderna de tanques para reproducción de tilapia en ambientes controlados.')">
        <img src="https://source.unsplash.com/600x400/?fish-tank" alt="Cría intensiva">
        <div class="card-body">
          <h3>Cría Intensiva</h3>
          <p>Proyecto de cría de peces de alto rendimiento en ambientes controlados.</p>
        </div>
      </div>
      <div class="card" onclick="showModal('Estanque ecológico', 'https://source.unsplash.com/600x400/?pond-fish', 'Diseño de estanques sostenibles para reproducción natural de especies locales.')">
        <img src="https://source.unsplash.com/600x400/?pond-fish" alt="Estanque ecológico">
        <div class="card-body">
          <h3>Estanque Ecológico</h3>
          <p>Modelo autosustentable de reproducción en ecosistemas controlados.</p>
        </div>
      </div>
      <div class="card" onclick="showModal('Centro de reproducción de truchas', 'https://source.unsplash.com/600x400/?trout-farm', 'Infraestructura para la reproducción técnica de truchas en zonas de altura.')">
        <img src="https://source.unsplash.com/600x400/?trout-farm" alt="Reproducción de truchas">
        <div class="card-body">
          <h3>Centro de Truchas</h3>
          <p>Reproducción técnica y monitoreo automatizado de truchas.</p>
        </div>
      </div>
    </div>
  </section>

  <div class="portfolio-modal" id="portfolioModal">
    <div class="modal-content">
      <span class="modal-close" onclick="closeModal()">&times;</span>
      <img id="modalImg" src="" alt="">
      <h3 id="modalTitle"></h3>
      <p id="modalDesc"></p>
    </div>
  </div>

  <section class="section" id="empresa">
    <h2>Sobre Quevepec</h2>
    <p>Somos una marca dedicada a la innovación en la reproducción de peces y el desarrollo de productos para la pesca responsable. Nuestro compromiso es ofrecer soluciones sustentables que ayuden tanto a pequeños pescadores como a grandes productores acuícolas.</p>
  </section>

  <section class="section" id="contacto">
    <h2>Contacto</h2>
    <p>¿Tienes preguntas? Escríbenos:</p>
    <form>
      <input type="text" placeholder="Nombre completo" required style="width:100%;padding:10px;margin:10px 0;">
      <input type="email" placeholder="Correo electrónico" required style="width:100%;padding:10px;margin:10px 0;">
      <textarea rows="5" placeholder="Mensaje" required style="width:100%;padding:10px;margin:10px 0;"></textarea>
      <button type="submit" style="padding: 12px 30px; background-color: #0e3c3d; color: white; border: none; border-radius: 5px;">Enviar</button>
    </form>
  </section>

  <footer>
    <p>&copy; 2025 Quevepec. Todos los derechos reservados.</p>
    <div class="footer-links">
      <a href="#">Facebook</a>
      <a href="#">Instagram</a>
      <a href="#">YouTube</a>
    </div>
  </footer>

  <script>
    function showModal(title, imgSrc, desc) {
      document.getElementById('modalTitle').textContent = title;
      document.getElementById('modalImg').src = imgSrc;
      document.getElementById('modalDesc').textContent = desc;
      document.getElementById('portfolioModal').style.display = 'flex';
    }
    function closeModal() {
      document.getElementById('portfolioModal').style.display = 'none';
    }
  </script>
</body>
</html>
