# -Souskal3011.github.io.<!DOCTYPE html>
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
// Detecteer toetsenbordtype en pas de besturing aan
function changeKeyboardLayout() {
  const layout = document.getElementById('keyboard-type').value;
  if (layout === 'azerty') {
    // Stel AZERTY besturing in (bijvoorbeeld ZQSD)
    console.log('AZERTY layout ingesteld');
  } else {
    // Stel QWERTY besturing in (WASD)
    console.log('QWERTY layout ingesteld');
  }
}

// Functie om spellen te starten (gebruik cloud gaming services zoals Parsec)
function startGame(game) {
  alert('Je hebt ' + game + ' gekozen! Je kunt het nu in je browser spelen.');
  // Hier kun je een link naar de cloud gaming service toevoegen
}
body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
  background-color: #f0f8ff;
  color: #333;
}

header {
  background-color: #00bcd4;
  color: white;
  padding: 20px;
  text-align: center;
}

main {
  padding: 20px;
}

h1, h2 {
  font-size: 2em;
  color: #0288d1;
}

button {
  background-color: #0288d1;
  color: white;
  border: none;
  padding: 10px 20px;
  font-size: 1.2em;
  cursor: pointer;
}

button:hover {
  background-color: #039be5;
}

footer {
  text-align: center;
  padding: 10px;
  background-color: #0288d1;
  color: white;
}
// Detecteer controller input
window.addEventListener("gamepadconnected", (e) => {
  console.log(`Controller connected: ${e.gamepad.id}`);
});
