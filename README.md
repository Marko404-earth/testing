<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Wonders of Cavite</title>
  <link rel="stylesheet" href="styles.css">
  <style>
    /* layout */
    :root { --sidebar-width: 220px; --accent: #4DA8DA; --bg: #7A7A73; }
    html, body { height: 100%; margin: 0; font-family: Arial, sans-serif; background: var(--bg); color: #111; }
    /* sidebar */
    .sidebar {
      position: fixed;
      top: 0;
      left: 0;
      width: var(--sidebar-width);
      height: 100vh;
      background: var(--accent);
      color: #fff;
      display: flex;
      flex-direction: column;
      gap: 18px;
      padding: 20px 16px;
      box-sizing: border-box;
    }
    .sidebar .brand { margin-bottom: 6px; }
    .sidebar h1 { font-size: 18px; margin: 0; line-height: 1.1; }
    .sidebar nav ul { list-style: none; padding: 0; margin: 12px 0 0 0; display:flex; flex-direction:column; gap:8px; }
    .sidebar nav a {
      display: block;
      color: #fff;
      text-decoration: none;
      padding: 8px 10px;
      border-radius: 6px;
    }
    .sidebar nav a:hover,
    .sidebar nav a:focus {
      background: rgba(255,255,255,0.12);
      outline: none;
    }
    /* main content area */
    .content {
      margin-left: var(--sidebar-width);
      padding: 28px;
      box-sizing: border-box;
      min-height: 100vh;
    }
    /* keep iframe responsive */
    .video-wrap iframe {
      width: 100%;
      max-width: 900px;
      height: 480px;
      border: 0;
      display:block;
      border-radius: 8px;
      box-shadow: 0 8px 20px rgba(0,0,0,0.25);
    }
    /* responsive: collapse sidebar to top bar on small screens */
    @media (max-width: 720px) {
      .sidebar {
        position: relative;
        width: 100%;
        height: auto;
        flex-direction: row;
        align-items: center;
        gap: 12px;
        padding: 12px;
      }
      .sidebar nav ul { flex-direction: row; gap: 8px; margin: 0; }
      .content { margin-left: 0; padding: 16px; }
      .video-wrap iframe { height: 320px; }
    }
  </style>
</head>
<body>
  <aside class="sidebar" aria-label="Main navigation">
    <div class="brand">
      <h1>Wonders of Cavite</h1>
    </div>
    <nav aria-label="Primary">
      <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#cities">Cities</a></li>
        <li><a href="#food">Food</a></li>
        <li><a href="#religions">Religions</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </aside>
  <main class="content">
    <section id="home" class="video-wrap">
      <iframe src="https://www.youtube.com/embed/ol_76rcb9wA" allowfullscreen title="Wonders of Cavite"></iframe>
    </section>
    <section id="cities">
      <h2>Cities</h2>
      <p></p>
    </section>
    <section id="food">
      <h2>Food</h2>
      <p></p>
    </section>
    <section id="religions">
      <h2>Religions</h2>
      <p></p>
    </section>
    <section id="contact">
      <h2>Contact</h2>
      <p></p>
    </section>
  </main>
</body>
</html>
