# intive-and-love
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Carta Romántica</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            overflow: hidden;
            font-family: 'Arial', sans-serif;
            background-image: url('https://www.w3schools.com/w3images/tulips.jpg'); /* Fondo de tulipanes */
            background-size: cover;
            background-position: center;
            height: 100vh;
        }
        .carta {
            position: relative;
            background-color: rgba(255, 255, 255, 0.8);
            padding: 40px;
            max-width: 600px;
            margin: 50px auto;
            border-radius: 15px;
            text-align: center;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);
        }
        h1 {
            color: #ff69b4;
            font-size: 2.5em;
            margin-bottom: 20px;
        }
        p {
            font-size: 1.5em;
            color: #333;
            margin-bottom: 30px;
        }
        .firma {
            font-style: italic;
            color: #ff69b4;
        }
        /* Estilo de las mariposas */
        .butterfly {
            position: absolute;
            width: 50px;
            height: 50px;
            background-image: url('https://img.icons8.com/ios/452/butterfly.png'); /* Mariposa */
            background-size: contain;
            background-repeat: no-repeat;
            animation: fly 10s linear infinite;
        }
        /* Animación de vuelo de las mariposas */
        @keyframes fly {
            0% {
                top: 0;
                left: 0;
                transform: rotate(0deg);
            }
            100% {
                top: 90%;
                left: 100%;
                transform: rotate(360deg);
            }
        }
    </style>
</head>
<body>
    <div class="carta">
        <h1>Hola querida Luciana,</h1>
        <p>Quería saber si tendría el honor de poder ir a tomar la media tarde con vos.</p>
        <p class="firma">Con cariño,</p>
        <p class="firma">[Tu nombre]</p>
    </div>
    <!-- JavaScript para generar mariposas -->
    <script>
        function generarMariposas() {
            for (let i = 0; i < 10; i++) { // Generar 10 mariposas
                let butterfly = document.createElement('div');
                butterfly.classList.add('butterfly');
                butterfly.style.top = Math.random() * 100 + '%'; // Posición aleatoria vertical
                butterfly.style.left = Math.random() * 100 + '%'; // Posición aleatoria horizontal
                butterfly.style.animationDuration = (Math.random() * 5 + 5) + 's'; // Duración aleatoria para cada mariposa
                document.body.appendChild(butterfly);
            }
        }
        // Llamar a la función para generar las mariposas al cargar la página
        window.onload = generarMariposas;
    </script>

</body>
</html>
