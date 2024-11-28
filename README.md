# *A Jornada de Moana - Fluxograma Interativo*

Este projeto apresenta a jornada da personagem Moana de forma interativa por meio de um fluxograma. Ele utiliza *HTML, **CSS* e *JavaScript* para criar uma experiência visual imersiva e intuitiva.

---

## *Recursos Principais*

- *Fluxograma Visual*: 
  - Exibe a sequência de eventos da história de Moana com caixas interativas conectadas por setas.
  - Cada caixa contém uma imagem e uma breve descrição.

- *Interação com Pop-ups*:
  - Ao clicar em uma etapa do fluxograma, é exibida uma janela pop-up com mais detalhes e uma imagem ampliada.

- *Design Temático*:
  - Fundo tropical inspirado no tema da história.
  - Cores vibrantes, efeitos de hover e transições suaves para uma interface moderna.

---

## *Como Funciona*

1. *Estrutura do Fluxograma*:
   - Cada etapa é uma caixa clicável com uma imagem e texto.
   - As etapas estão conectadas por setas indicando a ordem dos eventos.

2. *Pop-ups de Detalhes*:
   - Cada caixa possui um pop-up associado, que exibe mais informações ao ser clicada.
   - O botão "Fechar" retorna ao fluxograma principal.

---

## *Tecnologias Utilizadas*

- *HTML*: Estruturação do conteúdo.
- *CSS*: Estilização e efeitos visuais.
- *JavaScript*: Gerenciamento das interações.

---

## *Como Executar o Projeto*

1. Clone ou baixe este repositório.
2. Abra o arquivo index.html em qualquer navegador web.
3. Explore o fluxograma clicando nas caixas para obter mais detalhes.

---

## *Possíveis Melhorias*

1. Tornar o layout mais responsivo para dispositivos móveis.
2. Adicionar animações suaves ao abrir e fechar os pop-ups.
3. Criar uma navegação mais avançada, com botões "Próximo" e "Anterior".

---

## *Licença*

Este projeto foi desenvolvido apenas para fins educacionais e não tem fins lucrativos. As imagens utilizadas pertencem aos seus respectivos proprietários.

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
        <img src="https://i.imgur.com/TpJTSHr.jpg" alt="Moana criança" />
        <p>Moana descobre seu amor pelo mar desde pequena.</p>
      </div>

      <div class="seta">↓</div>

      <!-- Etapa 2 -->
      <div class="caixa" onclick="mostrarDetalhes(2)">
        <img src="https://i.imgur.com/Uuvk2LY.jpg" alt="Ilha de Motunui" />
        <p>A ilha de Motunui começa a sofrer com a escassez de recursos.</p>
      </div>

      <div class="seta">↓</div>

      <!-- Etapa 3 -->
      <div class="caixa" onclick="mostrarDetalhes(3)">
        <img src="https://i.imgur.com/s21hL2M.jpg" alt="Moana e Maui" />
        <p>Moana parte para encontrar Maui e restaurar o coração de Te Fiti.</p>
      </div>

      <div class="seta">↓</div>

      <!-- Etapa 4 -->
      <div class="caixa" onclick="mostrarDetalhes(4)">
        <img src="https://i.imgur.com/5DfNdeJ.jpg" alt="Te Fiti" />
        <p>Com coragem, Moana enfrenta Te Kā e devolve o coração a Te Fiti.</p>
      </div>

      <div class="seta">↓</div>

      <!-- Etapa 5 -->
      <div class="caixa" onclick="mostrarDetalhes(5)">
        <img src="https://i.imgur.com/zZ3xVvb.jpg" alt="Motunui restaurada" />
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
