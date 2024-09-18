<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Multiplicador de Números</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
        }
        input, button {
            padding: 10px;
            margin-top: 10px;
        }
    </style>
</head>
<body>
    <h1>Multiplicador de Números</h1>
    <label for="numero">Ingresa un número:</label>
    <input type="number" id="numero" placeholder="Número a multiplicar" />
    
    <label for="multiplicador">Ingresa el multiplicador:</label>
    <input type="number" id="multiplicador" placeholder="Multiplicador" />
    
    <button onclick="multiplicar()">Multiplicar</button>

    <h2 id="resultado"></h2>

    <script>
        function multiplicar() {
            const numero = document.getElementById('numero').value;
            const multiplicador = document.getElementById('multiplicador').value;
            const resultado = numero * multiplicador;
            document.getElementById('resultado').innerText = `Resultado: ${resultado}`;
        }
    </script>
</body>
</html>
