<!doctype html>
<html lang="pt-br">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Fluxograma - Jornada da Moana</title>
    <style>
      /* Fundo geral */
      body {
        margin: 0;
        padding: 0;
        font-family: Arial, sans-serif;
        color: #fff;
        background-image: url('https://wallpapercave.com/wp/wp2578911.jpg'); /* Imagem tropical */
        background-size: cover;
        background-repeat: no-repeat;
        background-attachment: fixed;
      }

      /* Cabeçalho */
      .header-container {
        width: 100%;
        background-color: rgba(0, 0, 0, 0.7);
        padding: 20px;
        text-align: center;
      }

      .logo {
        font-size: 2.5em;
        font-weight: bold;
        text-shadow: 2px 2px 5px rgba(0, 0, 0, 0.8);
        color: #ffd700; /* Dourado */
      }

      /* Fluxograma */
      .fluxograma {
        display: flex;
        flex-direction: column;
        align-items: center;
        margin-top: 20px;
        padding-bottom: 50px;
      }

      /* Caixas de etapas */
      .caixa {
        background-color: rgba(0, 0, 128, 0.7); /* Azul-marinho translúcido */
        padding: 20px;
        border-radius: 15px;
        margin: 15px;
        width: 80%;
        max-width: 500px;
        text-align: center;
        box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.3);
        transition: transform 0.3s ease;
      }

      .caixa:hover {
        transform: scale(1.05); /* Leve zoom ao passar o mouse */
      }

      .caixa img {
        width: 100%;
        height: auto;
        border-radius: 10px;
      }

      /* Setas */
      .seta {
        font-size: 2.5em;
        color: #ffd700; /* Dourado */
        text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.6);
      }

      /* Detalhes */
      .detalhes {
        background-color: rgba(0, 0, 0, 0.8);
        color: #fff;
        padding: 20px;
        border-radius: 10px;
        box-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
        display: none;
        position: fixed;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        width: 80%;
        max-width: 400px;
        z-index: 1000;
      }

      .detalhes h3 {
        color: #ffd700; /* Dourado */
        margin-top: 0;
      }

      .detalhes img {
        width: 100%;
        margin-top: 15px;
        border-radius: 10px;
      }

      .fechar {
        display: inline-block;
        background-color: #ff4500; /* Laranja vibrante */
        color: #fff;
        padding: 10px 20px;
        margin-top: 20px;
        border: none;
        border-radius: 5px;
        cursor: pointer;
        text-align: center;
      }

      .fechar:hover {
        background-color: #cc3700; /* Laranja escuro */
      }
    </style>
  </head>
  <body>
    <div class="header-container">
      <div class="logo">A Jornada de Moana</div>
    </div>

    <div class="fluxograma">
      <!-- Etapa 1 -->
      <div class="caixa" onclick="mostrarDetalhes(1)">
        <img src="https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEglUKOAZ1cFnlGL31RcdRygxobxETw210MF3aZ1Fws1gYQeDQCjxPC1aLXJP60xUj6OjuwpkVqg6d4BlxeW_T_2fh8iRKeeXe6rkxp1bY3t5NVz7005xNOtLUObu0ktvm3yPvLNMtKHbNI/s1600/%255D.jpg" alt="Moana criança" />
        <p>Moana descobre seu amor pelo mar desde pequena.</p>
      </div>

      <div class="seta">↓</div>

      <!-- Etapa 2 -->
      <div class="caixa" onclick="mostrarDetalhes(2)">
        <img src="https://static.wikia.nocookie.net/disneyprincesas/images/f/fd/Motunui_%28Moana_-_2016%29.png/revision/latest?cb=20170307202548&path-prefix=pt-br" alt="Ilha de Motunui" />
        <p>A ilha de Motunui começa a sofrer com a escassez de recursos.</p>
      </div>

      <div class="seta">↓</div>

      <!-- Etapa 3 -->
      <div class="caixa" onclick="mostrarDetalhes(3)">
        <img src="https://static.wixstatic.com/media/98d3de_acd27a88bb834372ae077f0461e26c27~mv2.jpg/v1/fill/w_568,h_238,al_c,q_80,usm_0.66_1.00_0.01,enc_auto/98d3de_acd27a88bb834372ae077f0461e26c27~mv2.jpg" alt="Moana e Maui" />
        <p>Moana parte para encontrar Maui e restaurar o coração de Te Fiti.</p>
      </div>

      <div class="seta">↓</div>

      <!-- Etapa 4 -->
      <div class="caixa" onclick="mostrarDetalhes(4)">
        <img src="https://static.wikia.nocookie.net/disney/images/f/fb/Moana-87.jpg/revision/latest?cb=20161025201030&path-prefix=pt-br" alt="Te Fiti" />
        <p>Com coragem, Moana enfrenta Te Kā e devolve o coração a Te Fiti.</p>
      </div>

      <div class="seta">↓</div>

      <!-- Etapa 5 -->
      <div class="caixa" onclick="mostrarDetalhes(5)">
        <img src="https://disneyplusbrasil.com.br/wp-content/uploads/2024/10/Moana-e-Maui-em-Moana-2.jpg" alt="Motunui restaurada" />
        <p>Moana retorna para Motunui, trazendo vida e equilíbrio à ilha.</p>
      </div>
    </div>

    <!-- Caixa de Detalhes -->
    <div class="detalhes" id="detalhesCaixa1">
      <h3>Moana criança</h3>
      <p>Desde pequena, Moana sente uma conexão especial com o oceano, mas seu pai a proíbe de navegar.</p>
      <img src="https://i.imgur.com/TpJTSHr.jpg" alt="Moana criança" />
      <button class="fechar" onclick="fecharDetalhes()">Fechar</button>
    </div>

    <!-- Outros detalhes aqui para as etapas 2 a 5 -->

    <script>
      function mostrarDetalhes(etapa) {
        document.querySelectorAll('.detalhes').forEach(function (detalhe) {
          detalhe.style.display = 'none';
        });
        var detalhesCaixa = document.getElementById('detalhesCaixa' + etapa);
        detalhesCaixa.style.display = 'block';
      }

      function fecharDetalhes() {
        document.querySelectorAll('.detalhes').forEach(function (detalhe) {
          detalhe.style.display = 'none';
        });
      }
    </script>
  </body>
</html>
