<!DOCTYPE html>
<html lang="nl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Veilige Gaming en Media Platform - Beskan</title>
  <link rel="stylesheet" href="style.css">
  <script src="script.js"></script>
</head>
<body>
  <header>
    <h1>Welkom bij Beskan - Veilige Gaming en Media</h1>
    <p>Speel gratis games, kijk films en video's, en gebruik je favoriete controller!</p>
  </header>

  <main>
    <section id="cloud-gaming">
      <h2>Speel Je Favoriete Spellen Online</h2>
      <p>Kies je game en speel deze direct in je browser!</p>
      <button onclick="startGame('Fortnite')">Speel Fortnite</button>
      <button onclick="startGame('Minecraft')">Speel Minecraft</button>
    </section>

    <section id="media">
      <h2>Gratis Films en Video's</h2>
      <p>Bekijk educatieve en leuke video's, en films geschikt voor 12+.</p>
      <ul>
        <li><a href="https://www.example-movie.com" target="_blank">Educatieve Film 1</a></li>
        <li><a href="https://www.example-movie.com" target="_blank">Leuke Film 2</a></li>
      </ul>
    </section>

    <section id="controller-settings">
      <h2>Controller Instellingen</h2>
      <label for="keyboard-type">Kies je toetsenbordtype:</label>
      <select id="keyboard-type" onchange="changeKeyboardLayout()">
        <option value="qwerty">QWERTY</option>
        <option value="azerty">AZERTY</option>
      </select>
    </section>
  </main>

  <footer>
    <p>&copy; 2025 Beskan - Alle rechten voorbehouden.</p>
  </footer>
</body>
</html>
