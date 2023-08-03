<!DOCTYPE html>
<html>
<head>
    <title>Ayúdame.</title>
    <style>
        h1 {
            color: blue;
            font-size: 24px;
        }
        .red-colon {
            color: red;
        }
    </style>
</head>
<body>
    <h1>Sálid nos va a matar :( <span class="red-colon">:</span></h1>
    <p>De todas formas, ¿de qué sirve lograr todo?</p>

    <button onclick="salvame()">Sálvame</button>
    <button onclick="matame()">Mátame</button>

    <script>
        function showMessage(message) {
            return confirm(message);
        }

        function redirectTo(url) {
            window.location.href = url;
        }

        function salvame() {
            var message = "Mucha suerte. Tu estabilidad emocional es lo más importante. Si sigues esforzándote, estarás muy bien.";
            alert(message);
            redirectTo("https://youtu.be/zeJyACD5DWM");
        }

        function matame() {
            var confirmacion = showMessage("¿Estás seguro de esto?");
            if (confirmacion) {
                confirmacion = showMessage("Ya respondiste dos veces. ¿Estás con seguridad de que quieres terminar todo?");
                if (confirmacion) {
                    alert("¡Cobarde, sufrirás vivo!");
                    redirectTo("https://youtu.be/GZ9Cg4iydWg");
                } else {
                    var message = "Por favor, no le hagas caso. ¿Aceptas salvarte?";
                    confirmacion = showMessage(message);
                    if (confirmacion) {
                        message = "Mucha suerte. Tu estabilidad emocional es lo más importante. Si sigues esforzándote, estarás muy bien.";
                        alert(message);
                        redirectTo("https://youtu.be/zeJyACD5DWM");
                    } else {
                        message = "Nos estamos entendiendo. No escuches al imbécil que interfirió en lo que estamos haciendo. Reconfirma que quieres irte. Me gusta escuchar cuando lo dicen.";
                        confirmacion = showMessage(message);
                        if (confirmacion) {
                            message = "Sufrirás viviendo. No vas a morir. :)";
                            alert(message);
                            redirectTo("https://youtu.be/GZ9Cg4iydWg");
                        } else {
                            message = "Gracias por apreciarte. Recuerda cuidar tu salud mental. Si sigues esforzándote, estarás muy bien. Nunca dejes que las voces de tu cabeza te hagan daño";
                            alert(message);
                            redirectTo("https://youtu.be/zeJyACD5DWM");
                        }
                    }
                }
            }
        }
    </script>
</body>
</html>
