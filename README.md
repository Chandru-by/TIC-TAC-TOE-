<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tic Tac Toe Game</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="main-menu">
        <h1>Tic Tac Toe</h1>
        <button id="playVsFriendBtn">Play vs Friend</button>
        <button id="playVsComputerBtn">Play vs Computer</button>
        <div class="settings">
            <button id="settingsBtn">⚙️ Settings</button>
            <div id="settingsPanel" class="settings-panel hidden">
                <label for="soundEffects">Sound Effects:</label>
                <input type="checkbox" id="soundEffects" checked>
                <label for="winningMusic">Winning Music:</label>
                <input type="checkbox" id="winningMusic" checked>
            </div>
        </div>
    </div>

    <div id="difficulty-popup" class="popup hidden">
        <div class="popup-content">
            <h2>Choose Difficulty</h2>
            <button id="easyBtn">Easy</button>
            <button id="mediumBtn">Medium</button>
            <button id="hardBtn">Hard</button>
        </div>
    </div>

    <div id="game-container" class="hidden">
        <div id="game-board" class="game-board"></div>
        <div class="message-area">
            <p id="status-message"></p>
        </div>
    </div>

    <div id="game-over-popup" class="popup hidden">
        <div class="popup-content">
            <h2 id="winning-message"></h2>
            <button id="restartBtn">Restart Game</button>
        </div>
    </div>

    <audio id="winningSound" src="winning.mp3" preload="auto"></audio>
    <audio id="clickSound" src="click.mp3" preload="auto"></audio>

    <script src="script.js"></script>
</body>
</html>
