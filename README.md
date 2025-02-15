<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Vivienda Vacacional</title>
    <link rel="stylesheet" href="styles.css"> <!-- Aquí puedes incluir tus estilos CSS -->
    <script src="script.js" defer></script> <!-- Si tienes un archivo JS -->
    <style>
        /* Estilos básicos para la página */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }
        header {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 1rem;
        }
        header h1 {
            margin: 0;
        }
        .banner {
            background-image: url('banner.jpg');
            background-size: cover;
            color: white;
            text-align: center;
            padding: 100px 0;
        }
        .section {
            padding: 2rem;
            text-align: center;
        }
        .gallery img {
            width: 100%;
            max-width: 300px;
            margin: 10px;
            border-radius: 8px;
        }
        .availability-calendar {
            margin-top: 2rem;
        }
        .contact-form input, .contact-form textarea {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: 1px solid #ddd;
            border-radius: 4px;
        }
        .contact-form button {
            background-color: #333;
            color: white;
            padding: 12px 20px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
        }
        .contact-form button:hover {
            background-color: #555;
        }
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 1rem;
            position: fixed;
            width: 100%;
            bottom: 0;
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <h1>Vivienda Vacacional</h1>
    </header>

    <!-- Banner -->
    <div class="banner">
        <h2>Bienvenidos a nuestro paraíso vacacional</h2>
        <p>Disfruta de una estancia única en la mejor ubicación</p>
    </div>

    <!-- Información de la propiedad -->
    <section class="section">
        <h2>Detalles de la Propiedad</h2>
        <p>Hermosa casa de 3 habitaciones, 2 baños, con vistas espectaculares y todos los servicios para que te sientas como en casa.</p>

        <div class="gallery">
            <h3>Galería de Imágenes</h3>
            <img src="room1.jpg" alt="Habitación 1">
            <img src="room2.jpg" alt="Habitación 2">
            <img src="view.jpg" alt="Vista desde la propiedad">
        </div>
    </section>

    <!-- Motor de reservas (básico) -->
    <section class="section">
        <h2>Reserva Ahora</h2>
        <form action="reservar.php" method="POST">
            <label for="check-in">Fecha de entrada:</label>
            <input type="date" id="check-in" name="check_in" required>

            <label for="check-out">Fecha de salida:</label>
            <input type="date" id="check-out" name="check_out" required>

            <label for="guests">Número de personas:</label>
            <input type="number" id="guests" name="guests" min="1" required>

            <button type="submit">Confirmar Reserva</button>
        </form>
    </section>

    <!-- Calendario de disponibilidad (básico) -->
    <section class="section availability-calendar">
        <h2>Calendario de Disponibilidad</h2>
        <p>Aquí estará el calendario donde puedes ver las fechas disponibles.</p>
        <p><i>(Puedes integrar un calendario interactivo más avanzado aquí)</i></p>
    </section>

    <!-- Página de contacto -->
    <section class="section">
        <h2>Contacto</h2>
        <form class="contact-form" action="contactar.php" method="POST">
            <input type="text" name="name" placeholder="Tu nombre" required>
            <input type="email" name="email" placeholder="Tu correo electrónico" required>
            <textarea name="message" placeholder="Tu mensaje" required></textarea>
            <button type="submit">Enviar Mensaje</button>
        </form>
    </section>

    <!-- Pie de página -->
    <footer>
        <p>&copy; 2025 Vivienda Vacacional. Todos los derechos reservados.</p>
    </footer>
</body>
</html>
