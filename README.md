<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PaulinhaGatinha.Com</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Pacifico&family=Roboto:wght@300;500;700&display=swap');

    body {
        margin: 0;
        overflow: hidden;
        background: linear-gradient(135deg, #ffc0cb, #ff4d4d, #ffe6e6, #ff0000);
        background-size: 400% 400%;
        animation: gradientBG 15s ease infinite;
        font-family: 'Roboto', sans-serif;
        text-align: center;
        color: #fff;
    }

    @keyframes gradientBG {
        0% { background-position: 0% 50%; }
        50% { background-position: 100% 50%; }
        100% { background-position: 0% 50%; }
    }

    
    .container {
        padding: 40px 20px;
        position: relative;
        z-index: 10;
        animation: fadeIn 2s ease;
    }

    
    @keyframes fadeIn {
        0% { opacity: 0; transform: translateY(30px); }
        100% { opacity: 1; transform: translateY(0); }
    }

    h1 {
        font-family: 'Pacifico', cursive;
        font-size: 42px;
        color: #ffe5f9;
        text-shadow: 2px 2px 10px #00000066;
    }

    p {
        font-size: 20px;
        margin: 10px 0;
        text-shadow: 1px 1px 4px rgba(0, 0, 0, 0.3);
    }

    .heart {
        font-size: 60px;
        color: #ff3366;
        cursor: pointer;
        transition: transform 0.3s ease, text-shadow 0.3s;
        animation: pulse 2s infinite;
    }

    .heart:hover {
        transform: scale(1.3);
        text-shadow: 0 0 20px #ff6b81;
    }

    @keyframes pulse {
        0%, 100% { transform: scale(1); }
        50% { transform: scale(1.1); }
    }

    #nao {
        font-size: 24px;
        color: #fff;
        background-color: #a1303d;
        border: none;
        cursor: pointer;
        position: absolute;
        padding: 10px 20px;
        border-radius: 10px;
    }

    #floating-hearts {
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        pointer-events: none;
        overflow: hidden;
        z-index: 1;
    }

    .floating-heart {
        position: absolute;
        font-size: 24px;
        color: #ff99cc;
        animation: float 5s linear infinite;
        opacity: 0.7;
    }

    @keyframes float {
        0% {
            transform: translateY(100vh) scale(1);
            opacity: 0;
        }
        50% {
            opacity: 1;
        }
        100% {
            transform: translateY(-10vh) scale(1.5);
            opacity: 0;
        }
    }
</style>
</head>
<body>

    <div class="floating-heart" style="left:5%; animation-delay: 0s;">❤</div>
    <div class="floating-heart" style="left:15%; animation-delay: 1s;">❤</div>
    <div class="floating-heart" style="left:25%; animation-delay: 2s;">❤</div>
    <div class="floating-heart" style="left:35%; animation-delay: 3s;">❤</div>
    <div class="floating-heart" style="left:45%; animation-delay: 4s;">❤</div>
    <div class="floating-heart" style="left:55%; animation-delay: 5s;">❤</div>
    <div class="floating-heart" style="left:65%; animation-delay: 6s;">❤</div>
    <div class="floating-heart" style="left:75%; animation-delay: 2.5s;">❤</div>
    <div class="floating-heart" style="left:85%; animation-delay: 3.5s;">❤</div>
    <div class="floating-heart" style="left:95%; animation-delay: 1.5s;">❤</div>

    
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
              width="250"
        height="250"

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
