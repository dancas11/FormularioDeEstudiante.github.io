<html lang="en">


<head>
    <link rel="shortcut icon" type="image/x-icon" href="educacion-a-distancia-04.png">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Formulario de estudiante</title>
    <style>
        body {
            background: #000;
            color: #fff;
            font-family: 'Trebuchet MS', sans-serif;
            text-align: center;
            margin: 0;
            padding: 0;
        }

        .header {
            background: linear-gradient(90deg, #ff00cc, #00ccff);
            padding: 20px;
        }

        h1 {
            font-size: 36px;
            letter-spacing: 3px;
        }

        .container {
            margin: 20px;
        }

        .content {
            background-color: rgba(0, 0, 0, 0.8);
            padding: 20px;
            border-radius: 20px;
            box-shadow: 0px 0px 20px 0px rgba(255, 255, 255, 0.2);
        }

        .footer {
            background: linear-gradient(90deg, #ff00cc, #00ccff);
            padding: 10px;
            position: fixed;
            bottom: 0;
            width: 100%;
        }

        form {
            margin-top: 20px;
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        input[type="text"], input[type="email"], input[type="submit"] {
            padding: 15px;
            margin: 10px;
            border: none;
            border-radius: 20px;
            width: 250px;
            font-size: 18px;
            text-align: center;
            background: rgba(255, 255, 255, 0.1);
            color: #fff;
        }

        input[type="submit"] {
            background: linear-gradient(90deg, #ff00cc, #00ccff);
            cursor: pointer;
            transition: background 0.3s ease;
        }

        input[type="submit"]:hover {
            background: linear-gradient(90deg, #00ccff, #ff00cc);
        }

        @keyframes neon {
            0% {
                text-shadow: 0 0 5px #ff00cc, 0 0 10px #ff00cc, 0 0 15px #ff00cc;
            }

            50% {
                text-shadow: 0 0 10px #00ccff, 0 0 20px #00ccff, 0 0 30px #00ccff;
            }

            100% {
                text-shadow: 0 0 5px #ff00cc, 0 0 10px #ff00cc, 0 0 15px #ff00cc;
            }
        }

        .neon-text {
            font-size: 24px;
            animation: neon 1.5s infinite;
        }
    </style>
</head>

<body>
    <div class="header">
        <h1 class="neon-text">FORMULARIO DE ESTUDIANTE</h1>
    </div>

    <div class="container">
        <div class="content">
            <h2><img src="textanim-TDrKm.gif"></h2>
            <p>¡Hola estudiante! Tu opinión nos importa y deseamos saber más de ti para aconsejarte y guiarte en el mundo académico.</p>
            <img src="manos-hacia-arriba-enchufe.gif" alt="estudiante" height="150">


    <div class="container">
        <form id="formulario">
            <label for="nombre">Nombre y Apellido:</label>
            <input type="text" id="nombre" name="nombre" required>
            
            <label for="email">Correo Electrónico:</label>
            <input type="text" id="email" name="email" required>
            
        <label for="edad">Edad:</label>
        <input type="number" id="edad" name="edad" required>
            
            <label for="sexo">Sexo:</label>
            <select id="sexo" name="sexo" required>
                <option value="femenino">Femenino</option>
                <option value="masculino">Masculino</option>
                <option value="otro">Otro</option>
            </select>
            
            <label for="colegio">Colegio al que perteneces:</label>
            <input type="text" id="colegio" name="colegio" required>
            
            <label for="carrera">¿Qué quieres estudiar?</label>
            <input type="text" id="carrera" name="carrera" required>
            
            <label for="universidad">¿Dónde quieres estudiar?</label>
            <input type="text" id="universidad" name="universidad" required>
            
            <label for="razon">¿Por qué quieres estudiar esa carrera?</label>
            <input type="text" id="razon" name="razon" required>
            
            <label for="duracion">Duración de la carrera:</label>
            <input type="text" id="duracion" name="duracion" required>
            
            <label for="conforme">¿Te sientes conforme con el plan de estudio de la carrera que elegiste?</label>
            <input type="checkbox" id="Sí" name="afirmativo" value="Sí">
        <label for="Sí">Sí</label>
        <input type="checkbox" id="No" name="negativo" value="No">
        <label for="No">No</label>
            
            <label for="preparado">¿Te sientes preparado con la educación virtual recibida?</label>
        <input type="checkbox" id="Sí" name="afirmativo" value="Sí">
        <label for="Sí">Sí</label>
        <input type="checkbox" id="No" name="negativo" value="No">
        <label for="No">No</label>
            
            <label for="mejoras">¿Cómo se puede mejorar la calidad educativa de tu país?</label>
            <input type="text" id="mejoras" name="mejoras" required>
            
            <input type="submit" value="Enviar" class="blink-text">
        </form>
    </div>

    <script>
        document.getElementById("formulario").addEventListener("submit", function(event) {
            
            var edad = document.getElementById("edad").value;
            if (isNaN(edad)) {
                alert("La edad debe ser un número válido.");
                event.preventDefault(); // Evitar que se envíe el formulario
            }
            </script>
