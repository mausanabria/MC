<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Martial Challenge</title>
    <link rel="stylesheet" href="style.css"> <!-- Enlace al archivo CSS -->
    <link rel="stylesheet" href="fonts.css"> <!-- Enlace al archivo font -->
</head>
<body>

<!-- PARTE 1 INICIO-->
<!-- Contenedor principal que ocupa el 80% del ancho de la página -->
<div class="contenido_seccion_menuyservicios">
    
    <!-- Header con imagen a la izquierda y secciones a la derecha -->
    <header>
        <div class="logo">
            <img src="martial.jpeg" alt="Logo"> <!-- Aquí puedes cambiar por tu imagen -->
        </div>
        <nav class="navbar">
            <ul>
                <li><a href="#Torneos">Torneos</a></li>
                <li><a href="#Nosotros">Nosotros</a></li>
                <li><a href="#Precios">Precios</a></li>
                <li><a href="#Servicio">Servicio</a></li>
                <li><a href="#Contacto">Contacto</a></li>
            </ul>
        </nav>
    </header>

    <!-- Sección del carrusel -->
    <section class="servicios_carrusel_seccion_completa">
        <!-- Imagen grande destacada -->
        <div class="imagen_principal_carrusel">
            <img id="featured-image" src="Metropolitano 2024.jpeg" alt="Imagen destacada">
        </div>
        <!-- Carrusel de miniaturas -->
        <div class="servicios-carrusel">
            <div class="servicios" onclick="changeImage('MC2.jpeg')">
                <img src="MC2.jpeg" alt="Miniatura 2">
            </div>
            <div class="servicios" onclick="changeImage('Examen1.jpeg')">
                <img src="Examen1.jpeg" alt="Miniatura 1"> 
            </div>
            <div class="servicios" onclick="changeImage('MC4.jpeg')">
                <img src="MC4.jpeg" alt="Miniatura 3">
            </div>

        <script>
            // Función para cambiar la imagen destacada al hacer clic en una miniatura
            function changeImage(imageSrc) {
            document.getElementById('featured-image').src = imageSrc;
            }
        </script>
        </div> 
    </section>

</div> 
<!-- PARTE 1 FIN-->

<h2 class="subtitulo">Servicios</h2>
<section class="imagensobretexto">
    
    <div class="gallery-container">
        <div class="gallery-item">
            <div class="image-container">
                <img src="MC3.jpeg" alt="Imagen 2">
                <div class="overlay">
                <p class="textoservicio">Gestion de Examenes</p>
                </div>
            </div>
        </div>
        <div class="gallery-item">
            <div class="image-container">
                <img src="Examen2.jpeg" alt="Imagen 1">
                <div class="overlay">
                <p class="textoservicio">Sistema de Puntuacion</p>
                </div>
            </div>
        </div>
        <div class="gallery-item">
            <div class="image-container">
            <img src="MC1.jpeg" alt="Imagen 3">
                <div class="overlay">
                <p class="textoservicio">Organizacion de Torneos</p>
                </div>
            </div>
        </div>
    </div>
</section>


<!-- PARTE 2 FIN-->
    <div class="contenido_menu">   
            <h2 class="subtitulo">Torneos</h2>
        <div class="carousel-container">
            <div class="carousel-images">
                <!-- Agrega tus imágenes aquí -->
                <img src="ITA 2024.jpeg" alt="Imagen 1">
                <img src="Nacional 2024.jpeg" alt="Imagen 2">
                <img src="Metropolitano 2024.jpeg" alt="Imagen 3">
                <img src="ITA 2023.jpeg" alt="Imagen 4">
                <img src="Nacional 2023.jpeg" alt="Imagen 5">
                <img src="Metropolitano 2024.jpeg" alt="Imagen 6">
            </div>

            <!-- Botones para navegar -->
            <button class="prev" onclick="moveSlide(-1)">&#10094;</button>
            <button class="next" onclick="moveSlide(1)">&#10095;</button>
        </div>
    

    <script>
        let currentIndex = 0;

        function moveSlide(direction) {
            const images = document.querySelectorAll('.carousel-images img');
            const totalImages = images.length;
            currentIndex += direction;

            if (currentIndex < 0) {
                currentIndex = totalImages - 1;
            } else if (currentIndex >= totalImages) {
                currentIndex = 0;
            }

            const newTransformValue = -(currentIndex * (images[0].width + 20)); // 20 es el margen entre las imágenes
            document.querySelector('.carousel-images').style.transform = `translateX(${newTransformValue}px)`;
        }
    </script>
    </div>
<!-- PARTE 2 FIN-->

<!-- PARTE 3 INICIO-->

    <h2 class="subtitulo">Quienes Somos</h2>
        <p class="quienes-somos">
        Martial Challenge es una herramienta de software orientada a brindar apoyo en eventos deportivos masivos, como torneos, exámenes, cursos, etc. Brindando al usuario una experiencia agradable, dinámica e intuitiva. El principal beneficio es la automatización del proceso del evento y la eficiencia de los tiempos, tanto para los organizadores, colaboradores, competidores, alumnos, acompañantes y público en general.
        </p>
<div class="secciones-container">
    <div class="seccion">
        <h3>Administracion y Gestion</h3>
        <p>Nuestro sofware brinda a los organizadores e instructores una herramienta dinámica, y eficiente, mejorando la experiencia de llevar adelante eventos deportivos, orientada a la administración, gestión y organización de los eventos y de la logística interna y detrás de escena de dichos eventos. Es por esto que nuestro especialista dentro del staff es <b>Lic. Administración de empresas.</b></p>
    </div>
    <div class="seccion">
        <h3>Orientado al Competidor </h3>
        <p>Buscamos brindarles a nuestros clientes la mejor experiencia haciendo foco en garantizar la calidad del evento y que los competidores o alumno sean los verdaderos protagonistas cuidando al detalle la comodidad y el alto desempeño del competidor. Es por esto que un Integrante del staff es <b>Lic. Ed. Fisica y deportes & Magister en Formación y Desarrollo del Rendimiento deportivo.</b></p>
    </div>
    <div class="seccion">
        <h3>Software y Seguridad</h3>
        <p>Nuestra prioridad es el desarrollo de un software a medida, diseñado con versatilidad y adaptabilidad a cada instructor, escuela, asociación o federación, llevado adelante con la mejor calidad de herramientas de programación, sin dejar de lado la importancia de la seguridad informatica, Martial Challenge cuenta con un <b>Lic. Informatica & Diplomado en seguridad informatica.</b></p>
    </div>
</div>

<!-- PARTE 3 FIN-->

</body>
</html>

