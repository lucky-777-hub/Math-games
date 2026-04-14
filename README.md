# Math-games
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GNN-Math | Retro Math Games</title>
    <link rel="stylesheet" href="css/styles.css">
</head>
<body>
    <div id="app">
        <!-- Main Menu -->
        <div id="mainMenu" class="screen">
            <h1>🎮 GNN-MATH 🎮</h1>
            <p class="subtitle">RETRO MATH GAMES ARCADE</p>
            <div class="menu-grid" id="gameMenu"></div>
            <div class="stats">
                <p>Total Score: <span id="totalScore">0</span></p>
            </div>
        </div>

        <!-- Game Screen -->
        <div id="gameScreen" class="screen hidden">
            <div class="game-header">
                <h2 id="gameName"></h2>
                <div class="game-controls">
                    <label>Level: 
                        <select id="levelSelect" onchange="changeLevel(this.value)">
                            <option value="easy">Easy</option>
                            <option value="medium" selected>Medium</option>
                            <option value="hard">Hard</option>
                            <option value="expert">Expert</option>
                        </select>
                    </label>
                    <button onclick="backToMenu()" class="btn-back">← Back</button>
                </div>
            </div>
            <div id="gameContainer" class="game-container"></div>
            <div class="game-stats">
                <p>Score: <span id="gameScore">0</span></p>
                <p>Time: <span id="gameTimer">0</span>s</p>
                <p>Streak: <span id="gameStreak">0</span></p>
            </div>
        </div>
    </div>

    <script src="js/main.js"></script>
</body>
</html>
