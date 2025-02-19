# 3x3-Tournament
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>3x3 Tournament</title>
  <style>
    /* Reset básico */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      font-family: Arial, sans-serif;
      background-color: #fff;
      color: #333;
      line-height: 1.6;
    }
    header {
      background-color: #000;
      color: #fff;
      padding: 10px 20px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      flex-wrap: wrap;
    }
    header .logo {
      display: flex;
      align-items: center;
    }
    header .logo img {
      width: 50px;
      height: auto;
      margin-right: 10px;
    }
    header nav ul {
      list-style: none;
      display: flex;
      flex-wrap: wrap;
    }
    header nav ul li {
      margin-left: 20px;
    }
    header nav ul li a {
      color: #fff;
      text-decoration: none;
      font-weight: bold;
    }
    .banner {
      background: url('banner.jpg') no-repeat center center/cover;
      height: 300px;
      display: flex;
      align-items: center;
      justify-content: center;
      position: relative;
    }
    .banner h1 {
      color: #fff;
      font-size: 3em;
      text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.7);
    }
    section {
      padding: 40px 20px;
    }
    .intro {
      text-align: center;
    }
    .intro h2 {
      font-size: 2.5em;
      color: #ff6600; /* Naranja */
      margin-bottom: 20px;
    }
    .intro p {
      max-width: 800px;
      margin: 0 auto;
      font-size: 1.2em;
    }
    .events {
      background-color: #f4f4f4;
    }
    .events h2 {
      text-align: center;
      font-size: 2.5em;
      color: #ff6600;
      margin-bottom: 20px;
    }
    .event-container {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
    }
    .event {
      background-color: #fff;
      border: 1px solid #ddd;
      border-radius: 5px;
      margin: 10px;
      width: 300px;
      overflow: hidden;
      box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    }
    .event img {
      width: 100%;
      height: 200px;
      object-fit: cover;
    }
    .event-details {
      padding: 15px;
    }
    .event-details h3 {
      margin-bottom: 10px;
      font-size: 1.5em;
      color: #333;
    }
    .event-details p {
      font-size: 1em;
      color: #555;
    }
    .contact {
      text-align: center;
    }
    .contact h2 {
      font-size: 2.5em;
      color: #ff6600;
      margin-bottom: 20px;
    }
    .contact form {
      max-width: 600px;
      margin: 0 auto;
    }
    .contact form input,
    .contact form textarea {
      width: 100%;
      padding: 10px;
      margin-bottom: 10px;
      border: 1px solid #ccc;
      border-radius: 3px;
      font-size: 1em;
    }
    .contact form button {
      background-color: #ff6600;
      color: #fff;
      border: none;
      padding: 10px 20px;
      font-size: 1em;
      border-radius: 3px;
      cursor: pointer;
    }
    .social {
      margin-top: 20px;
    }
    .social a {
      color: #000;
      text-decoration: none;
      font-size: 1.2em;
      margin: 0 10px;
    }
    footer {
      background-color: #000;
      color: #fff;
      text-align: center;
      padding: 20px;
    }
    @media(max-width: 768px) {
      header {
        flex-direction: column;
      }
      header nav ul {
        flex-direction: column;
        margin-top: 10px;
      }
      .banner h1 {
        font-size: 2.5em;
      }
    }
  </style>
</head>
<body>
  <!-- Encabezado con logotipo y menú de navegación -->
  <header>
    <div class="logo">
      <img src="logo.png" alt="3x3 Tournament Logo">
      <h1>3x3 Tournament</h1>
    </div>
    <nav>
      <ul>
        <li><a href="#intro">Inicio</a></li>
        <li><a href="#events">Eventos</a></li>
        <li><a href="#contact">Contacto</a></li>
      </ul>
    </nav>
  </header>

  <!-- Banner principal -->
  <div class="banner">
    <h1>¡Bienvenido a 3x3 Tournament!</h1>
  </div>

  <!-- Sección de Introducción -->
  <section id="intro" class="intro">
    <h2>Acerca de Nosotros</h2>
    <p>
      En 3x3 Tournament nos apasiona el baloncesto. Organizamos torneos 3x3 de alto nivel donde se une la emoción, el deporte y la competencia. Únete a nosotros y forma parte de la experiencia deportiva más dinámica.
    </p>
  </section>

  <!-- Sección de Eventos -->
  <section id="events" class="events">
    <h2>Próximos Eventos</h2>
    <div class="event-container">
      <div class="event">
        <img src="evento1.jpg" alt="Evento 1">
        <div class="event-details">
          <h3>Torneo de Verano</h3>
          <p>Fecha: 15 de Agosto 2025<br>Ubicación: Ciudad Deportiva</p>
        </div>
      </div>
      <div class="event">
        <img src="evento2.jpg" alt="Evento 2">
        <div class="event-details">
          <h3>Torneo de Otoño</h3>
          <p>Fecha: 10 de Octubre 2025<br>Ubicación: Estadio Central</p>
        </div>
      </div>
      <!-- Agrega más eventos aquí si lo deseas -->
    </div>
  </section>

  <!-- Sección de Contacto -->
  <section id="contact" class="contact">
    <h2>Contacto</h2>
    <form action="https://example.com/send" method="post">
      <input type="text" name="nombre" placeholder="Tu nombre" required>
      <input type="email" name="email" placeholder="Tu email" required>
      <textarea name="mensaje" rows="5" placeholder="Tu mensaje" required></textarea>
      <button type="submit">Enviar</button>
    </form>
    <div class="social">
      <a href="https://instagram.com/tu_cuenta" target="_blank">Instagram</a>
    </div>
  </section>

  <!-- Pie de página -->
  <footer>
    <p>&copy; 2025 3x3 Tournament. Todos los derechos reservados.</p>
  </footer>
</body>
</html>
