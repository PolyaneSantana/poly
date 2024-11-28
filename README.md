# Os Guardiões do Arco-Íris

## Descrição
"Os Guardiões do Arco-Íris" é uma página web fictícia que apresenta uma aventura mágica e colorida. O projeto utiliza HTML e CSS para criar uma experiência visualmente envolvente e responsiva. Ideal para explorar conceitos de design e estruturação de páginas na web.

## Funcionalidades
- *Design Responsivo:* Layout adaptável para diferentes dispositivos.
- *Temática Mágica:* Utilização de cores, imagens e tipografia para criar uma atmosfera imersiva.
- *Componentes de História:*
  - *Introdução:* Apresenta a Terra das Cores e o início da aventura.
  - *Personagens:* Destaque para os Guardiões (Luna, Bolt e Ziggy).
  - *Aventura:* Detalhes sobre a missão principal e os desafios enfrentados.

## Estrutura de Arquivos
- *index.html:* Página principal contendo o conteúdo HTML.
- *style.css:* (Integrado no index.html) Define o estilo visual da página.
- *README.md:* Este arquivo com informações sobre o projeto.

## Tecnologias Utilizadas
- *HTML5:* Para a estruturação da página.
- *CSS3:* Para estilização avançada, incluindo efeitos visuais e responsividade.

## Instruções de Uso
1. Faça o download ou clone este repositório:
   ```bash
   git clone https://github.com/seu-usuario/os-guardioes-do-arco-iris.git
 <!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Os Guardiões do Arco-Íris</title>
  <style>
    /* Estilos Globais */
    body {
      margin: 0;
      font-family: 'Arial', sans-serif;
      background-image: url('https://via.placeholder.com/1920x1080?text=Background+Colorido');
      background-size: cover;
      background-attachment: fixed;
      background-repeat: no-repeat;
      color: white;
      text-shadow: 1px 1px 2px #000;
    }

    header {
      text-align: center;
      padding: 40px;
      background: rgba(0, 0, 0, 0.6);
    }

    header h1 {
      font-size: 3em;
      margin: 0;
    }

    header p {
      font-size: 1.5em;
    }

    main {
      padding: 20px;
      background: rgba(0, 0, 0, 0.7);
      border-radius: 15px;
      margin: 20px auto;
      max-width: 1200px;
      box-shadow: 0 0 15px rgba(0, 0, 0, 0.5);
    }

    .introducao, .guardioes, .aventura {
      margin-bottom: 40px;
    }

    .introducao img, .aventura img {
      width: 100%;
      border-radius: 15px;
      margin-top: 20px;
    }

    .guardioes {
      display: flex;
      justify-content: space-around;
      flex-wrap: wrap;
    }

    .personagem {
      text-align: center;
      margin: 20px;
      background: rgba(255, 255, 255, 0.2);
      padding: 20px;
      border-radius: 15px;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.3);
      flex: 1 1 30%;
    }

    .personagem img {
      max-width: 150px;
      border-radius: 10px;
      margin-bottom: 15px;
    }

    .aventura img {
      max-width: 100%;
      border-radius: 15px;
      margin: 20px 0;
    }

    .voltar-topo {
      display: block;
      text-align: center;
      margin: 40px auto;
      padding: 15px 30px;
      background-color: #f8d90f;
      color: #000;
      font-weight: bold;
      text-decoration: none;
      border-radius: 10px;
      box-shadow: 0 5px 10px rgba(0, 0, 0, 0.3);
    }

    footer {
      text-align: center;
      padding: 20px;
      background: rgba(0, 0, 0, 0.8);
      color: #f8d90f;
    }

    footer a {
      color: #f8d90f;
      text-decoration: none;
    }

    footer a:hover {
      text-decoration: underline;
    }
  </style>
</head>
<body>
  <header>
    <h1>Os Guardiões do Arco-Íris</h1>
    <p>Uma aventura cheia de cores, amizade e magia!</p>
  </header>

  <main>
    <section class="introducao">
      <h2>Bem-vindo à Terra das Cores</h2>
      <p>Na Terra das Cores, a harmonia sempre reinou graças ao Arco-Íris Mágico, que traz felicidade e vida a todos. Mas algo sombrio começou a acontecer: as cores começaram a desaparecer misteriosamente. Os Guardiões foram convocados para proteger o reino e restaurar o equilíbrio!</p>
      <img src="https://img.freepik.com/fotos-gratis/um-arco-iris-de-sonho-num-campo_23-2151625173.jpg?semt=ais_hybrid<"?semt=ais_hybrid?text=Paisagem+Colorida" alt="Arco-Íris sobre a vila">
    </section>

    <section class="guardioes">
      <h2>Conheça os Guardiões</h2>
      <div class="personagem">
        <img src="https://via.placeholder.com/200x200?text=Luna" alt="Luna">
        <h3>Luna</h3>
        <p>Com suas asas de cristal, Luna espalha luz e esperança por onde passa. Ela é a líder destemida do grupo.</p>
      </div>
      <div class="personagem">
        <img src="https://via.placeholder.com/200x200?text=Bolt" alt="Bolt">
        <h3>Bolt</h3>
        <p>Bolt é o mais rápido do grupo e usa seus poderes elétricos para enfrentar desafios e iluminar o caminho.</p>
      </div>
      <div class="personagem">
        <img src="https://via.placeholder.com/200x200?text=Ziggy" alt="Ziggy">
        <h3>Ziggy</h3>
        <p>Ziggy é o coração do time. Com seu dom de cura, ele ajuda a manter todos unidos e prontos para a ação.</p>
      </div>
    </section>

    <section class="aventura">
      <h2>A Grande Aventura</h2>
      <p>Os Guardiões descobriram que *Sombróx*, um espírito das trevas, roubou as cores para mergulhar o mundo na escuridão eterna. Para derrotá-lo, eles precisam coletar as Essências do Arco-Íris espalhadas por terras misteriosas.</p>
      <img src="https://via.placeholder.com/800x400?text=Os+Guardiões+em+ação" alt="Os Guardiões em Ação">
      <p>A jornada é repleta de desafios: desfiladeiros mágicos, florestas encantadas e labirintos de cristal. Em cada lugar, eles enfrentam perigos e aprendem lições sobre coragem, trabalho em equipe e o poder da amizade.</p>
    </section>

    <a href="#header" class="voltar-topo">Voltar ao topo</a>
  </main>

  <footer>
    <p>&copy; 2024 Os Guardiões do Arco-Íris</p>
    <p>Explore mais histórias mágicas em <a href="#">nosso site oficial</a>.</p>
  </footer>
</body>
</html>
