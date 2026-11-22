# blog.page
<!doctype html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Wander Notes</title>
  <style>
    :root {
      --ink: #1f2924;
      --muted: #69736d;
      --paper: #f7f5ef;
      --line: #dedfd7;
      --accent: #d66b4d;
    }

    * { box-sizing: border-box; }

    body {
      margin: 0;
      background: var(--paper);
      color: var(--ink);
      font-family: Georgia, "Times New Roman", serif;
    }

    header {
      max-width: 1100px;
      margin: auto;
      padding: 28px 24px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      border-bottom: 1px solid var(--line);
    }

    .brand {
      font-size: 22px;
      font-weight: 700;
      letter-spacing: -0.5px;
    }

    nav a {
      margin-left: 24px;
      color: var(--ink);
      text-decoration: none;
      font-family: Arial, sans-serif;
      font-size: 14px;
    }

    main {
      max-width: 1100px;
      margin: auto;
      padding: 48px 24px;
    }

    .hero {
      display: grid;
      grid-template-columns: 1.25fr 0.75fr;
      gap: 48px;
      align-items: end;
      margin-bottom: 64px;
    }

    .hero img {
      width: 100%;
      height: 430px;
      object-fit: cover;
    }

    .hero h1 {
      margin: 12px 0 18px;
      font-size: clamp(42px, 6vw, 76px);
      line-height: 0.95;
      letter-spacing: -3px;
    }

    .meta {
      color: var(--muted);
      font-family: Arial, sans-serif;
      font-size: 13px;
    }

    .intro {
      max-width: 480px;
      color: var(--muted);
      font-size: 18px;
      line-height: 1.6;
    }

    .posts {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 28px;
    }

    article {
      border-top: 1px solid var(--line);
      padding-top: 18px;
    }

    article img {
      width: 100%;
      height: 220px;
      object-fit: cover;
      margin-bottom: 18px;
    }

    article h2 {
      margin: 8px 0;
      font-size: 25px;
      line-height: 1.15;
    }

    article p {
      color: var(--muted);
      line-height: 1.55;
    }

    footer {
      max-width: 1100px;
      margin: auto;
      padding: 32px 24px 48px;
      border-top: 1px solid var(--line);
      color: var(--muted);
      font-family: Arial, sans-serif;
      font-size: 13px;
    }

    @media (max-width: 700px) {
      nav a:not(:first-child) { display: none; }
      .hero, .posts { grid-template-columns: 1fr; }
      .hero { gap: 24px; }
      .hero img { height: 300px; }
      .hero h1 { letter-spacing: -2px; }
    }
  </style>
</head>
<body>
  <header>
    <div class="brand">Wander Notes</div>
    <nav>
      <a href="#">Stories</a>
      <a href="#">Places</a>
      <a href="#">About</a>
    </nav>
  </header>

  <main>
    <section class="hero">
      <img src="https://images.unsplash.com/photo-1500530855697-b586d89ba3ee?auto=format&fit=crop&w=1400&q=85" alt="Mountain landscape">
      <div>
        <div class="meta">The Dolomites · Italy</div>
        <h1>Days Above the Clouds</h1>
        <p class="intro">A quiet journey through alpine villages, winding trails, and mornings shaped by mountain light.</p>
      </div>
    </section>

    <section class="posts">
      <article>
        <img src="https://images.unsplash.com/photo-1533105079780-92b9be482077?auto=format&fit=crop&w=900&q=85" alt="Greek island">
        <div class="meta">Travel guide · Greece</div>
        <h2>A Slow Weekend in Naxos</h2>
        <p>Whitewashed streets, hidden coves, and long lunches beneath the shade of olive trees.</p>
      </article>

      <article>
        <img src="https://images.unsplash.com/photo-1528127269322-539801943592?auto=format&fit=crop&w=900&q=85" alt="Boat in Vietnam">
        <div class="meta">Field notes · Vietnam</div>
        <h2>Life Along the Mekong</h2>
        <p>Following the river through floating markets, sleepy towns, and emerald-green fields.</p>
      </article>

      <article>
        <img src="https://images.unsplash.com/photo-1470770841072-f978cf4d019e?auto=format&fit=crop&w=900&q=85" alt="Lake and mountains">
        <div class="meta">Photo diary · Switzerland</div>
        <h2>Still Mornings in the Alps</h2>
        <p>Three peaceful days around lakes so clear they seemed to hold the sky itself.</p>
      </article>
    </section>
  </main>

  <footer>© 2026 Wander Notes · Travel slowly, leave lightly.</footer>
</body>
</html>
