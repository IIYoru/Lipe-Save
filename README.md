# Lipe-Save

!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Feliz Aniversário!</title>
  <style>
    /* Estilos gerais */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Arial', sans-serif;
      background-color: #f0f8ff;
      color: #333;
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      text-align: center;
      flex-direction: column;
      position: relative;
      overflow: hidden; /* Impede que animações saiam da tela */
    }

    /* Container */
    .container {
      max-width: 90%;
      padding: 20px;
      background-color: #ffffff;
      border-radius: 10px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
      z-index: 10;
    }

    h1 {
      font-size: 2.5em;
      color: #b14330;
      margin-bottom: 10px;
    }

    .mensagem {
      font-size: 1.2em;
      color: #555;
      margin-bottom: 20px;
    }

    .imagem {
      max-width: 100%;
      height: auto;
      border-radius: 10px;
    }

    /* Foguetes animados */
    .foguetes {
      position: absolute;
      top: 0;
      left: 50%;
      transform: translateX(-50%);
      z-index: 0;
    }

    .foguete {
      position: absolute;
      bottom: -100px; /* Começo fora da tela */
      width: 30px;
      height: 60px;
      background-color: #ff6347;
      border-radius: 50%;
      animation: subir 4s ease-in-out infinite;
    }

    .foguete1 {
      left: 10%;
      animation-delay: 0s;
    }

    .foguete2 {
      left: 45%;
      animation-delay: 1s;
    }

    .foguete3 {
      left: 80%;
      animation-delay: 2s;
    }

    /* Animação de subida */
    @keyframes subir {
      0% {
        bottom: -100px;
        transform: scale(0.5) rotate(0deg);
      }
      50% {
        bottom: 50%;
        transform: scale(1) rotate(180deg);
      }
      100% {
        bottom: 100%;
        transform: scale(1.5) rotate(360deg);
      }
    }

    /* Confetes caindo */
    .confetes {
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      pointer-events: none;
      z-index: 5;
    }

    .confete {
      position: absolute;
      width: 10px;
      height: 10px;
      background-color: #ff6347;
      opacity: 0;
      animation: cair 3s infinite;
      border-radius: 50%;
    }

    /* Efeito de confete caindo */
    @keyframes cair {
      0% {
        transform: translateY(-100px) rotate(0deg);
        opacity: 1;
      }
      100% {
        transform: translateY(100vh) rotate(360deg);
        opacity: 0;
      }
    }

    /* Confetes com cores diferentes */
    .confete:nth-child(1) {
      background-color: #e97d6a;
      animation-duration: 3s;
      animation-delay: 0s;
    }

    .confete:nth-child(2) {
      background-color: #ff0;
      animation-duration: 3.5s;
      animation-delay: 1s;
    }

    .confete:nth-child(3) {
      background-color: #32cd32;
      animation-duration: 4s;
      animation-delay: 2s;
    }

    .confete:nth-child(4) {
      background-color: #1e90ff;
      animation-duration: 3.5s;
      animation-delay: 0.5s;
    }

    /* Responsividade para dispositivos móveis */
    @media (max-width: 600px) {
      h1 {
        font-size: 2em;
      }

      .mensagem {
        font-size: 1em;
      }
    }
  </style>
</head>
<body>
  <div class="container">
    <h1>Feliz Aniversário Mainha!</h1>
    <p class="mensagem">Mainha do meu coração, neste dia tão especial  queria te enviar um abraço bem apertado através dessa pequena pagina, a saudade aperta meu peito, sinto muito sua falta, de tudo que vc sempre me proporcionou como um abraço apertado, conselhos duvidosos, risadas sinceras e acima de tudo o carinho enorme. Sendo breve te desejo toda a felicidade do mundo pois vc merece ela e muito mais, só lembrando que não importa a distancia, ao final do dia vc sempre estará cmg no meu coração.</p>
   <h2>EU TE AMO</h2> <img src="iamgem.png" alt="Feliz Aniversário" class="imagem">
  </div>

  <!-- Foguetes Animados -->
  <div class="foguetes">
    <div class="foguete foguete1"></div>
    <div class="foguete foguete2"></div>
    <div class="foguete foguete3"></div>
  </div>

  <!-- Confetes Animados -->
  <div class="confetes">
    <div class="confete"></div>
    <div class="confete"></div>
    <div class="confete"></div>
    <div class="confete"></div>
    <div class="confete"></div>
    <div class="confete"></div>
    <div class="confete"></div>
    <div class="confete"></div>
    <div class="confete"></div>
    <div class="confete"></div>
  </div>
</body>
</html>
