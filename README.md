<!DOCTYPE html>
<html lang="pt-br">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Date Misterioso</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            background-color: #f8f9fa;
        }

        #conteudo {
            background: #ffffff;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            padding: 20px;
            text-align: center;
        }

        h2 {
            color: #007bff;
            font-size: 24px;
            margin-bottom: 20px;
        }

        p {
            color: #333;
            font-size: 16px;
            margin-bottom: 20px;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            line-height: 1.5;
        }

        .btn {
            background-color: #007bff;
            color: #fff;
            border: none;
            padding: 10px 20px;
            font-size: 16px;
            cursor: pointer;
            border-radius: 5px;
            transition: background-color 0.3s ease;
        }

        .btn:hover {
            background-color: #0056b3;
        }

        .btn:focus {
            outline: none;
        }
    </style>
</head>

<body>
    <div id="conteudo">
        <h2>Aceita se aventurar em um date comigo?</h2>
        <p>E ai, gatinha! O que acha de ir para um date comigo? Posso proporcionar piadinhas ruins, maconha e beijos intensos, aceitas?</p>
        <button class="btn" onclick="sim()">SIM</button>
        <button class="btn" onclick="desvia(this)" onmouseover="desvia(this)">NÃO</button>
    </div>

    <script>
        function sim() {
            alert("Você aceitou! :)");
            // redireciona para um URL após clicar no SIM
            location.href = "https://music.youtube.com/watch?v=izGwDsrQ1eQ";
        }

        function desvia(btn) {
            btn.style.position = 'absolute';
            btn.style.bottom = geraPosicao(10, 90);
            btn.style.left = geraPosicao(10, 90);
            console.log('opa, desviei...');
        }

        function geraPosicao(min, max) {
            return (Math.random() * (max - min) + min) + "%";
        }
    </script>
</body>

</html>
