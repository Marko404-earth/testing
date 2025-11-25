<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>Wonders of Cavite</title>
  <style>
    :root { --sidebar-width: 220px; --accent: #4DA8DA; --bg: #7A7A73; --header-h: 60px; }
    html, body { 
    height: 100%; 
    margin: 0; 
    font-family: Arial, sans-serif; 
    background: var(--bg); 
    color: #111; 
    }
    .topbar { 
    position: fixed; 
    top: 0; 
    left: 0; 
    right: 0; 
    height: var(--header-h); 
    background: #4DA8DA; 
    color: #7A7A73; 
    display: flex; 
    align-items: center; 
    padding: 0 16px; 
    box-sizing: 
    border-box; 
    z-index: 40; 
    }
    .topbar .logo { 
    font-weight: 700; 
    font-size: 18px; 
    margin-right: 12px; 
    }
    .topbar .site-title { 
    font-size: 16px; 
    }
    .sidebar { 
    font-weight: bold; 
    position: fixed; 
    top: var(--header-h); 
    left: 0; 
    width: var(--sidebar-width); 
    height: calc(100vh - var(--header-h)); 
    background: var(--accent); 
    color: #7A7A73; 
    display: flex; 
    flex-direction: column; 
    gap: 12px; 
    padding: 18px 12px; 
    box-sizing: border-box; 
    z-index: 30; 
    overflow-y: auto; 
    }
    .sidebar h1 { 
    font-size: 16px; 
    margin: 0 0 6px 0; 
    }
    .sidebar nav ul {
    list-style: none; 
    padding: 0; 
    margin: 6px 0 0 0; 
    display: flex; 
    flex-direction: column; 
    gap:8px; 
    }
    .sidebar nav a { 
    display: block; 
    color: #7A7A73; 
    text-decoration: none; 
    padding: 8px 10px; 
    border-radius: 6px; 
    font-size: 18px;
    }
    .sidebar nav a:hover, .sidebar nav a:focus { 
    background: rgba(255,255,255,0.12); 
    outline: none; 
    }
    .content {
    margin-left: var(--sidebar-width); 
    margin-top: var(--header-h); 
    padding: 28px; 
    box-sizing: border-box; 
    min-height: calc(100vh - var(--header-h)); 
    }
    .video-wrap { 
    width: 100%; 
    display: block; 
    margin-bottom: 24px; 
    }
    .video-wrap iframe {
      width: 100%;
      height: calc( (100vw - var(--sidebar-width)) * 0.5625 ); /* 16:9 responsive */
      max-height: 650px;
      border: 0;
      display: block;
      border-radius: 15px;
      box-shadow: 0 8px 20px rgba(0,0,0,0.25);
    }
    .info { 
    max-width: 100%; 
    background: rgba(255,255,255,0.04); 
    padding: 18px; 
    border-radius: 10px; 
    color: #4DA8DA; 
    }
    .info h2 { 
    margin-top: 0; 
    color: #4DA8DA; 
    }
    .info p { 
    color: #4DA8DA; 
    line-height: 1.6; 
    }
    @media (max-width: 900px) {
      .video-wrap iframe { height: 56.25vw; } /* maintain 16:9 */
    }
    @media (max-width: 720px) {
      :root { --sidebar-width: 100%; }
      .content { 
      margin-left: 0; 
      margin-top: calc(var(--header-h) + 12px); 
      padding: 16px; 
      }
      .video-wrap iframe { 
      height: 56.25vw; 
      max-height: 420px; 
      }
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
      .sidebar nav ul { 
      flex-direction: row; 
      gap: 8px; margin: 0; 
      }
    }
  </style>
</head>
<body>
  <header class="topbar" role="banner">
    <div class="site-title"><h1 style="margin:0;" style="color: #7A7A73">Wonders of Cavite</h1></div>
  </header>
  <aside class="sidebar" aria-label="Main navigation">
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
    <section id="home" class="video-wrap" aria-label="Featured video">
      <iframe src="https://www.youtube.com/embed/ol_76rcb9wA" allowfullscreen title="Wonders of Cavite"></iframe>
    </section>
    <section class="info" id="overview">
      <h2>General Information (Times New Roman)</h2>
      <br>
      <p>Cavite is a historic, populous, and rapidly industrializing province in the CALABARZON region of the Philippines. It is known as the "Historical Capital of the Philippines" for its crucial role in the country's fight for independence from Spain.</p>
      <br>
      <p><strong>Geography:</strong> Located on the southern shores of Manila Bay, Cavite is bordered by Metro Manila to the northeast, Laguna to the east, and Batangas to the south.</p>
      <br>
      <p><strong>Capital:</strong> The provincial capital is Imus, while the seat of the provincial government is in Trece Martires. The province is composed of 8 cities and 15 municipalities. While Tagalog is the most widely spoken language, a Spanish-based creole called Chavacano is also spoken in some areas, particularly Cavite City and Ternate.</p>
      <br>
      <h2>History (Times New Roman)</h2>
      <br>
      <p><strong>Spanish colonial period:</strong> Spanish colonizers established a port in Cavite in 1571, and it became a vital trading hub for the Manila-Acapulco Galleon Trade.</p>
      <br>
      <p><strong>Philippine Revolution:</strong> Cavite was a significant center of the Philippine Revolution in the late 1800s. Key events include the Cavite Mutiny of 1872 and the proclamation of Philippine independence by Emilio Aguinaldo in Kawit on June 12, 1898.</p>
      <br>
      <p><strong>American colonial period:</strong> Following the Spanish-American War, the US established a major naval base at Sangley Point in Cavite City, which operated until 1941.</p>
      <br>
      <p><strong>World War II:</strong> During the Japanese occupation, guerrilla forces in Cavite fought against the Japanese Imperial forces. American and Filipino forces liberated the province in January 1945.</p>
    </section>
  </main>
</body>
</html>
