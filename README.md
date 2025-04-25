# QuevePec-REPORDUCCION DE PESCADOS Y VENTAS
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Quevepec | Reproducción de Peces y Venta de Productos</title>
  <style>
    body { font-family: Arial, sans-serif; margin: 0; padding: 0; background-color: #f8f9fa; color: #333; }
    header { background-color: #006D6F; color: white; padding: 40px 20px; text-align: center; }
    header h1 { font-size: 3em; margin: 0; }
    header p { font-size: 1.2em; }
    nav { background-color: #004f4f; display: flex; justify-content: center; gap: 30px; padding: 15px; }
    nav a { color: white; text-decoration: none; font-weight: bold; font-size: 1.1em; }
    section { padding: 40px 20px; }
    .hero { background: url('https://source.unsplash.com/featured/?fishing,water') no-repeat center/cover; color: white; padding: 100px 20px; text-align: center; }
    .hero h2 { font-size: 2.5em; margin-bottom: 20px; }
    .productos, .portafolio { display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 30px; }
    .card { background: white; padding: 20px; border-radius: 10px; box-shadow: 0 2px 10px rgba(0,0,0,0.1); }
    .card img { width: 100%; height: 250px; object-fit: cover; border-radius: 8px; }
    footer { background-color: #006D6F; color: white; text-align: center; padding: 20px; margin-top: 40px; }
    form input, form textarea { width: 100%; margin: 10px 0; padding: 12px; border: 1px solid #ccc; border-radius: 5px; }
    form button { background-color: #004f4f; color: white; padding: 12px 25px; border: none; border-radius: 5px; cursor: pointer; }
    .testimonios { background-color: #f2f2f2; padding: 30px 20px; border-radius: 8px; }
    .testimonio-card { background-color: white; padding: 20px; border-radius: 8px; box-shadow: 0 2px 10px rgba(0,0,0,0.1); }
    .testimonio-card p { font-style: italic; }
  </style>
</head>
<body>
  <header>
    <h1>Quevepec</h1>
    <p>Reproducción de Peces y Venta de Productos de Pesca</p>
  </header>
  <nav>
    <a href="#inicio">Inicio</a>
    <a href="#sobre-nosotros">Sobre Nosotros</a>
    <a href="#reproduccion">Reproducción de Peces</a>
    <a href="#tienda">Tienda</a>
    <a href="#contacto">Contacto</a>
  </nav>

  <section class="hero" id="inicio">
    <h2>Bienvenidos a Quevepec</h2>
    <p>Impulsando la pesca responsable con productos de calidad y conocimiento sobre reproducción de peces.</p>
  </section>

  <section id="sobre-nosotros">
    <h2>Sobre Nosotros</h2>
    <p>En Quevepec, nuestra misión es promover la pesca sostenible a través de productos innovadores y un profundo conocimiento en la reproducción de especies acuáticas.</p>
  </section>

  <section id="reproduccion">
    <h2>Reproducción de Peces</h2>
    <p>Nos especializamos en la cría y reproducción de peces para asegurar especies saludables, ayudando tanto a la industria pesquera como a la conservación ambiental.</p>
    <img src="https://source.unsplash.com/featured/?fish-farming" alt="Reproducción de peces" />
  </section>

  <section id="tienda">
    <h2>Nuestros Productos</h2>
    <div class="productos">
      <div class="card">
        <img src="https://source.unsplash.com/featured/?fishing-rod" alt="Caña de Pesca">
        <h3>Caña de Pesca Profesional</h3>
        <p>Ideal para todo tipo de pesca, diseño ergonómico y durabilidad garantizada.</p>
        <p><strong>$79.99</strong></p>
      </div>
      <div class="card">
        <img src="https://source.unsplash.com/featured/?fishing-accessories" alt="Accesorios de Pesca">
        <h3>Kit Completo de Accesorios</h3>
        <p>Todo lo que necesitas para mejorar tu experiencia de pesca.</p>
        <p><strong>$59.99</strong></p>
      </div>
    </div>
  </section>

  <section id="testimonios">
    <h2>Testimonios</h2>
    <div class="testimonios">
      <div class="testimonio-card">
        <p>“Los productos de Quevepec son excelentes. La caña de pesca es súper resistente y los accesorios son de primera.”</p>
        <p><strong>- Juan Pérez</strong></p>
      </div>
      <div class="testimonio-card">
        <p>“Conocí Quevepec por sus conocimientos sobre la reproducción de peces. ¡Una marca que entiende lo que hace!”</p>
        <p><strong>- Marta López</strong></p>
      </div>
    </div>
  </section>

  <section id="contacto">
    <h2>Contacto</h2>
    <form>
      <input type="text" placeholder="Tu nombre" required>
      <input type="email" placeholder="Tu correo" required>
      <textarea placeholder="Tu mensaje" rows="5" required></textarea>
      <button type="submit">Enviar</button>
    </form>
  </section>

  <footer>
    <p>&copy; 2025 Quevepec. Todos los derechos reservados.</p>
  </footer>
</body>
</html>
