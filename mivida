<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Para ti ❤️</title>

    <style>

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            height: 100vh;
            overflow: hidden;

            background: linear-gradient(
                135deg,
                #ffb6c1,
                #ff69b4,
                #ff1493
            );

            font-family: Arial, sans-serif;

            display: flex;
            justify-content: center;
            align-items: center;
        }


        /* CORAZONES DEL FONDO */

        .corazones {
            position: fixed;
            inset: 0;
            pointer-events: none;
        }

        .corazon-fondo {
            position: absolute;

            color: rgba(255,255,255,0.7);

            font-size: 25px;

            animation: flotar 6s linear infinite;
        }

        @keyframes flotar {

            0% {
                transform: translateY(110vh) rotate(0deg);
                opacity: 0;
            }

            20% {
                opacity: 1;
            }

            100% {
                transform: translateY(-120vh) rotate(360deg);
                opacity: 0;
            }
        }


        /* CAJA PRINCIPAL */

        .contenedor {
            position: relative;
            z-index: 10;

            text-align: center;

            background: rgba(255,255,255,0.18);

            padding: 45px;

            border-radius: 25px;

            backdrop-filter: blur(8px);

            box-shadow:
                0 10px 40px rgba(0,0,0,0.2);
        }


        h1 {
            color: white;

            font-size: 38px;

            margin-bottom: 35px;

            text-shadow:
                0 3px 10px rgba(150,0,60,0.4);
        }


        /* BOTONES */

        .botones {
            display: flex;

            justify-content: center;

            gap: 25px;
        }

        button {
            border: none;

            padding: 14px 40px;

            border-radius: 30px;

            font-size: 20px;

            cursor: pointer;

            transition: 0.3s;
        }

        #si {
            background: #ff1744;

            color: white;
        }

        #no {
            background: white;

            color: #ff1744;
        }

        button:hover {
            transform: scale(1.1);
        }


        /* CORAZÓN GRANDE */

        #corazonGrande {
            display: none;

            position: fixed;

            top: 50%;
            left: 50%;

            transform: translate(-50%, -50%);

            z-index: 20;

            text-align: center;
        }


        .corazon {
            position: relative;

            width: 220px;
            height: 220px;

            margin: auto;

            transform: rotate(-45deg);

            background: #ff1744;

            opacity: 0;

            animation: crearCorazon 5s forwards;

            box-shadow:
                0 0 40px #ff1744,
                0 0 80px rgba(255,0,80,0.6);
        }

        .corazon::before,
        .corazon::after {
            content: "";

            position: absolute;

            width: 220px;
            height: 220px;

            background: #ff1744;

            border-radius: 50%;
        }

        .corazon::before {
            top: -110px;
            left: 0;
        }

        .corazon::after {
            top: 0;
            left: 110px;
        }


        @keyframes crearCorazon {

            0% {
                opacity: 0;
                transform:
                    rotate(-45deg)
                    scale(0);
            }

            30% {
                opacity: 0.3;
            }

            60% {
                opacity: 0.7;
                transform:
                    rotate(-45deg)
                    scale(0.7);
            }

            100% {
                opacity: 1;
                transform:
                    rotate(-45deg)
                    scale(1);
            }
        }


        /* TEXTO */

        #mensaje {
            position: absolute;

            top: 50%;
            left: 50%;

            transform:
                translate(-50%, -50%)
                rotate(0deg);

            width: 250px;

            color: white;

            font-size: 24px;

            font-weight: bold;

            text-shadow:
                0 2px 8px #99002b;

            opacity: 0;

            animation: aparecerTexto 1.5s 5s forwards;
        }

        @keyframes aparecerTexto {

            from {
                opacity: 0;
            }

            to {
                opacity: 1;
            }
        }

    </style>
</head>

<body>


    <!-- CORAZONES DEL FONDO -->

    <div class="corazones">

        <span class="corazon-fondo" style="left:5%; animation-delay:0s;">❤️</span>
        <span class="corazon-fondo" style="left:15%; animation-delay:2s;">💗</span>
        <span class="corazon-fondo" style="left:25%; animation-delay:4s;">💕</span>
        <span class="corazon-fondo" style="left:35%; animation-delay:1s;">❤️</span>
        <span class="corazon-fondo" style="left:45%; animation-delay:3s;">💖</span>
        <span class="corazon-fondo" style="left:55%; animation-delay:5s;">❤️</span>
        <span class="corazon-fondo" style="left:65%; animation-delay:2s;">💗</span>
        <span class="corazon-fondo" style="left:75%; animation-delay:4s;">💕</span>
        <span class="corazon-fondo" style="left:85%; animation-delay:1s;">❤️</span>
        <span class="corazon-fondo" style="left:95%; animation-delay:3s;">💖</span>

    </div>


    <!-- PREGUNTA -->

    <div class="contenedor" id="pregunta">

        <h1>
            ¿Me amas? ❤️
        </h1>

        <div class="botones">

            <button id="si" onclick="decirSi()">
                Sí ❤️
            </button>

            <button id="no" onclick="decirNo()">
                No
            </button>

        </div>

    </div>


    <!-- CORAZÓN FINAL -->

    <div id="corazonGrande">

        <div class="corazon"></div>

        <div id="mensaje">
            Te amo muchísimo,<br>
            mi chonguita ❤️
        </div>

    </div>


    <script>

        function decirSi() {

            document.getElementById("pregunta").style.display = "none";

            document.getElementById("corazonGrande").style.display = "block";

        }


        function decirNo() {

            const boton =
                document.getElementById("no");

            boton.style.position = "absolute";

            boton.style.left =
                Math.random() * 80 + "%";

            boton.style.top =
                Math.random() * 80 + "%";

        }

    </script>

</body>
</html>
