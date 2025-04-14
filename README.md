<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <title>Pour Mathilde</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    /* RESET + STYLES GÉNÉRAUX */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }
    body {
      font-family: 'Helvetica Neue', sans-serif;
      background-color: #fff;
      color: #111;
      line-height: 1.6;
      overflow-x: hidden;
    }
    a {
      text-decoration: none;
      color: inherit;
    }

    /* ACCUEIL */
    .hero {
      height: 100vh;
      display: flex;
      justify-content: center;
      align-items: center;
      text-align: center;
      padding: 2rem;
    }
    .hero h1 {
      font-size: 3rem;
      font-weight: 300;
    }

    /* SECTION HISTOIRE */
    .section {
      padding: 6rem 2rem;
      max-width: 800px;
      margin: auto;
    }
    .section h2 {
      font-size: 2rem;
      margin-bottom: 1rem;
      font-weight: 400;
      text-align: center;
    }
    .timeline {
      margin-top: 2rem;
    }
    .timeline p {
      margin-bottom: 1rem;
      opacity: 0.8;
    }

    /* GALERIE */
    .gallery {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 1rem;
      margin-top: 2rem;
    }
    .gallery div {
      background-color: #f0f0f0;
      height: 200px;
      display: flex;
      align-items: center;
      justify-content: center;
      font-style: italic;
      color: #666;
    }

    /* LETTRE */
    .letter {
      margin-top: 2rem;
      font-style: italic;
      text-align: center;
      opacity: 0.9;
    }

    /* SURPRISE */
    .surprise {
      text-align: center;
      margin-top: 3rem;
    }
    .btn {
      padding: 0.8rem 1.5rem;
      background-color: #111;
      color: #fff;
      border: none;
      cursor: pointer;
      transition: 0.3s ease;
    }
    .btn:hover {
      background-color: #444;
    }
    .secret {
      display: none;
      margin-top: 2rem;
      font-size: 1.2rem;
      animation: fadeIn 1s ease forwards;
    }
    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(10px); }
      to { opacity: 1; transform: translateY(0); }
    }
  </style>
</head>
<body>

  <section class="hero">
    <h1>Pour Mathilde,<br>mon cœur, ma lumière, mon évidence.</h1>
  </section>

  <section class="section">
    <h2>Notre histoire</h2>
    <div class="timeline">
      <p>— Le jour où je t’ai rencontrée, tout a changé.</p>
      <p>— Nos fous rires, nos silences, nos regards… tout est précieux.</p>
      <p>— Chaque moment avec toi est une page de bonheur écrite à deux.</p>
    </div>
  </section>

  <section class="section">
    <h2>Nos souvenirs</h2>
    <div class="gallery">
      <div>“Ton sourire ce jour-là…”</div>
      <div>“Notre premier voyage”</div>
      <div>“Juste toi et moi”</div>
      <div>“Un regard, et tout est dit”</div>
    </div>
  </section>

  <section class="section">
    <h2>Une lettre pour toi</h2>
    <div class="letter">
      <p>Mathilde,</p>
      <p>Tu es la plus belle des surprises que la vie m’ait offerte. Ce site n’est qu’un petit reflet de tout ce que je ressens. Merci d’être toi. Je t’aime.</p>
    </div>
  </section>

  <section class="section surprise">
    <button class="btn" onclick="showSecret()">Clique ici</button>
    <div class="secret" id="secret">Un jour, ce site s'appellera "notre histoire pour toujours".</div>
  </section>

  <script>
    function showSecret() {
      document.getElementById("secret").style.display = "block";
    }
  </script>

</body>
</html>
