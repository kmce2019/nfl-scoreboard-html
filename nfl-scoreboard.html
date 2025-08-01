<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>NFL Scoreboard</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #111;
      color: #fff;
      margin: 0;
      padding: 20px;
    }
    h1 {
      text-align: center;
      margin-bottom: 10px;
    }
    .game {
      border: 1px solid #444;
      border-radius: 8px;
      padding: 10px;
      margin-bottom: 10px;
      background: #222;
    }
    .team {
      display: flex;
      justify-content: space-between;
      font-size: 1.2em;
    }
    .status {
      text-align: center;
      color: #ccc;
      margin-top: 5px;
      font-size: 0.9em;
    }
  </style>
</head>
<body>
  <h1>Live NFL Scores</h1>
  <div id="scoreboard">Loading...</div>

  <script>
    async function fetchScores() {
      try {
        const res = await fetch('https://site.api.espn.com/apis/site/v2/sports/football/nfl/scoreboard');
        const data = await res.json();
        const games = data.events || [];

        let html = "";
        games.forEach(event => {
          const comp = event.competitions[0];
          const home = comp.competitors.find(t => t.homeAway === "home");
          const away = comp.competitors.find(t => t.homeAway === "away");

          html += `
            <div class="game">
              <div class="team"><span>${away.team.displayName}</span><span>${away.score}</span></div>
              <div class="team"><span>${home.team.displayName}</span><span>${home.score}</span></div>
              <div class="status">${comp.status.type.shortDetail}</div>
            </div>
          `;
        });

        document.getElementById("scoreboard").innerHTML = html || "<p>No games found.</p>";
      } catch (e) {
        document.getElementById("scoreboard").innerHTML = `<p>Error loading scores</p>`;
      }
    }

    fetchScores();
    setInterval(fetchScores, 60000); // Refresh every 60 seconds
  </script>
</body>
</html>
