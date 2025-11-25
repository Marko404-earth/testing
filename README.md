<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Wonders of Cavite</title>
  <style>
    :root { --sidebar-width: 220px; --accent: #4DA8DA; --bg: #7A7A73; --header-h: 60px; }
    html, body { height: 100%; margin: 0; font-family: Arial, sans-serif; background: var(--bg); color: #111; }
    /* top horizontal header */
    .topbar {
      position: fixed;
      top: 0;
      left: 0;
      right: 0;
      height: var(--header-h);
      background: #111; /* header background color */
      color: #fff;
      display: flex;
      align-items: center;
      padding: 0 16px;
      box-sizing: border-box;
      z-index: 40;
    }
    .topbar .logo { font-weight: 700; font-size: 18px; margin-right: 12px; }
    .topbar .site-title { font-size: 16px; }
    /* sidebar vertical nav placed under header */
    .sidebar {
      position: fixed;
      top: var(--header-h);
      left: 0;
      width: var(--sidebar-width);
      height: calc(100vh - var(--header-h));
      background: var(--accent);
      color: #fff;
      display: flex;
      flex-direction: column;
      gap: 12px;
      padding: 18px 12px;
      box-sizing: border-box;
      z-index: 30;
      overflow-y: auto;
    }
    .sidebar h1 { font-size: 16px; margin: 0 0 6px 0; }
    .sidebar nav ul { list-style: none; padding: 0; margin: 6px 0 0 0; display:flex; flex-direction:column; gap:8px; }
    .sidebar nav a {
      display: block;
      color: #fff;
      text-decoration: none;
      padding: 8px 10px;
      border-radius: 6px;
    }
    .sidebar nav a:hover,
    .sidebar nav a:focus { background: rgba(255,255,255,0.12); outline: none; }
    /* main content sits to the right and below the header */
    .content {
      margin-left: var(--sidebar-width);
      margin-top: var(--header-h);
      padding: 28px;
      box-sizing: border-box;
      min-height: calc(100vh - var(--header-h));
    }
    /* Responsive: collapse sidebar below header on small screens */
    @media (max-width: 720px) {
      :root { --sidebar-width: 100%; }
      .sidebar {
        position: relative;
        top: 0;
        width: 100%;
        height: auto;
        flex-direction: row;
        align-items: center;
        gap: 10px;
        padding: 10px;
      }
      .sidebar nav ul { flex-direction: row; gap: 8px; margin: 0; }
      .content { margin-left: 0; margin-top: calc(var(--header-h) + 12px); padding: 16px; }
    }
    .video-wrap iframe {
      width: 80%;
      max-width: 900px;
      height: 480px;
      border: 0;
      display:block;
      border-radius: 8px;
      box-shadow: 0 8px 20px rgba(0,0,0,0.25);
    }
  </style>
</head>
<body>
  <header class="topbar" role="banner">
    <div class="logo">🌴</div>
    <div class="site-title"><h1>Wonders of Cavite</h1></div>
  </header>
  <aside class="sidebar" aria-label="Main navigation">
    <div class="brand">
      <h1>Explore</h1>
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
  <main class="content" role="main">
    <section id="home" class="video-wrap">
      <iframe src="https://www.youtube.com/embed/ol_76rcb9wA" allowfullscreen title="Wonders of Cavite"></iframe>
    </section>
  </main>
</body>
</html>
