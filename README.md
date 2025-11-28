<h1>My Portifolio </h1> 
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>GameHub - Notícias e Rankings de Games</title>
  <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
  <style>
    /* Reset e estilos básicos */
    * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Roboto', sans-serif; }
    body { background-color: #121212; color: #f5f5f5; }
    a { text-decoration: none; color: inherit; }
    header { background-color: #1f1f1f; padding: 20px; display: flex; align-items: center; justify-content: space-between; }
    header h1 { font-size: 2rem; color: #ff3c3c; cursor: pointer; }
    nav a { margin-left: 20px; font-weight: bold; color: #f5f5f5; }
    
    /* Banner */
    .banner { position: relative; height: 400px; background: url('https://source.unsplash.com/1600x400/?gaming') center/cover no-repeat; display: flex; align-items: center; justify-content: center; }
    .banner h2 { font-size: 3rem; background-color: rgba(0,0,0,0.6); padding: 20px; border-radius: 10px; }

    /* Seções */
    section { padding: 40px 20px; max-width: 1200px; margin: auto; }
    h2.section-title { font-size: 2rem; margin-bottom: 20px; border-left: 5px solid #ff3c3c; padding-left: 10px; }

    /* Notícias e Cards */
    .cards { display: grid; grid-template-columns: repeat(auto-fit, minmax(280px, 1fr)); gap: 20px; }
    .card { background-color: #1f1f1f; border-radius: 10px; overflow: hidden; transition: transform 0.3s; cursor: pointer; }
    .card:hover { transform: translateY(-5px); }
    .card img { width: 100%; height: 180px; object-fit: cover; }
    .card-content { padding: 15px; }
    .card-content h3 { font-size: 1.2rem; margin-bottom: 10px; }
    .card-content p { font-size: 0.9rem; color: #cccccc; }

    /* Footer */
    footer { background-color: #1f1f1f; padding: 20px; text-align: center; color: #888; }
  </style>
</head>
<body>

  <!-- Header -->
  <header>
    <h1 id="logo">GameHub</h1>
    <nav>
      <a href="#noticias">Notícias</a>
      <a href="#rankings">Rankings</a>
      <a href="#lancamentos">Lançamentos</a>
      <a href="#comunidade">Comunidade</a>
    </nav>
  </header>

  <!-- Banner -->
  <div class="banner">
    <h2>As Últimas Novidades do Mundo dos Games</h2>
  </div>

  <!-- Notícias -->
  <section id="noticias">
    <h2 class="section-title">Últimas Notícias</h2>
    <div class="cards">
      <div class="card">
        <img src="https://source.unsplash.com/400x200/?game" alt="Notícia 1">
        <div class="card-content">
          <h3>Clair Obscur: Expedition 33 é GOTY 2025</h3>
          <p>O jogo indie que conquistou o mundo e ganhou diversos prêmios...</p>
        </div>
      </div>
      <div class="card">
        <img src="https://source.unsplash.com/400x200/?gaming-console" alt="Notícia 2">
        <div class="card-content">
          <h3>Gamescom 2025 traz grandes anúncios</h3>
          <p>Novos jogos revelados e datas de lançamento confirmadas para 2026...</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Rankings -->
  <section id="rankings">
    <h2 class="section-title">Top Jogos da Semana</h2>
    <div class="cards">
      <div class="card">
        <img src="https://source.unsplash.com/400x200/?rpg-game" alt="Ranking 1">
        <div class="card-content">
          <h3>1. Clair Obscur: Expedition 33</h3>
          <p>RPG épico com narrativa imersiva e arte incrível.</p>
        </div>
      </div>
      <div class="card">
        <img src="https://source.unsplash.com/400x200/?fps-game" alt="Ranking 2">
        <div class="card-content">
          <h3>2. Valor Mortis</h3>
          <p>Soulslike histórico com combate desafiador e gráficos de tirar o fôlego.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Lançamentos -->
  <section id="lancamentos">
    <h2 class="section-title">Próximos Lançamentos</h2>
    <div class="cards">
      <div class="card">
        <img src="https://source.unsplash.com/400x200/?console" alt="Lançamento 1">
        <div class="card-content">
          <h3>Warhammer 40K: Dawn of War 4</h3>
          <p>Previsto para 2026 em PC e consoles.</p>
        </div>
      </div>
      <div class="card">
        <img src="https://source.unsplash.com/400x200/?videogame" alt="Lançamento 2">
        <div class="card-content">
          <h3>Denshattack!</h3>
          <p>Game indie inovador ainda sem data definida.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Comunidade -->
  <section id="comunidade">
    <h2 class="section-title">O que a galera tá falando</h2>
    <div class="cards">
      <div class="card">
        <div class="card-content">
          <h3>@gamerbr_01</h3>
          <p>“Clair Obscur merece o GOTY! Arte e narrativa sensacionais.”</p>
        </div>
      </div>
      <div class="card">
        <div class="card-content">
          <h3>@levelupplayer</h3>
          <p>“Ansioso por Valor Mortis! A jogabilidade parece incrível.”</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer>
    &copy; 2025 GameHub. Todos os direitos reservados.
  </footer>

  <script>
    // Animação simples na logo
    const logo = document.getElementById('logo');
    logo.addEventListener('mouseover', () => {
      logo.style.transform = 'scale(1.2)';
      logo.style.transition = 'transform 0.3s';
    });
    logo.addEventListener('mouseout', () => {
      logo.style.transform = 'scale(1)';
    });
  </script>
</body>
</html>
