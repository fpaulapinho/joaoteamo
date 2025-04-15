# joaoteamo
baitolices para meu amado 
<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PaulinhaGatinha.Com</title>
    <style>
        body {
            background-color: #bd88a8;
            text-align: center;
            font-family: Arial, sans-serif;
        }

        .container {
            padding: 20px;
        }

        h1 {
            color: hsl(345, 63%, 37%);
        }

        .heart {
            font-size: 50px;
            color: hsl(342, 54%, 19%);
            cursor: pointer;
        }

        #nao {
            font-size: 24px;
            color: #333;
            background-color: #a1303d;
            border: none;
            cursor: pointer;
            position: absolute;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Para o melhor namorado do mundo!!</h1>
        <p>Boa noite meu Amor❤️,</p>
        <p>você é a pessoa mais especial da minha vidinha, amo te ter!.</p>
        <p>quer passar todos os dias da vida comigo?</p>
        <div class="gallery">
            <img
              src="imagens/joaoeeu.jpg"
              alt="breakfast"
              class="image"
              alt="A gallery image"
              width="500"
        height="500"

            />
          </div>
        <p class="heart" onclick="mostrarResposta()">Te Amo❤️</p>
        <button id="nao" onmouseover="mudarPosicao()">Não</button>
        <p id="resposta" style="display: none;"></p>
    </div>
    <script>
        function mostrarResposta() {
            document.getElementById('resposta').style.display = 'block';
            document.getElementById('resposta').innerHTML = 'tmj lindo!!❤️';
        }

        function mudarPosicao() {
            const buttonNao = document.getElementById('nao');
            const randomX = Math.floor(Math.random() * window.innerWidth);
            const randomY = Math.floor(Math.random() * window.innerHeight);
            buttonNao.style.left = `${randomX}px`;
            buttonNao.style.top = `${randomY}px`;
        }
    </script>
</body>
</html>
