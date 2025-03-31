<!DOCTYPE html>
<html>
<head>
    <title>Henni's Theken-Challenge</title>
    <style>
        body { font-family: Arial; background: #f5e9dc; text-align: center; }
        h1 { color: #d4a017; }
        .rules { background: white; padding: 20px; margin: 20px; border-radius: 10px; }
    </style>
</head>
<body>
    <h1>🍻 Willkommen zur Henni's Theken-Challenge!</h1>
    <div class="rules">
        <h2>Regeln:</h2>
        <p>1. Jeder Spieler würfelt virtuell (Button unten).</p>
        <p>2. Bei einer 1-3: Du trinkst einen Schluck!</p>
        <p>3. Bei einer 4-6: Du bestimmst, wer trinkt!</p>
        <button onclick="rollDice()">Würfeln!</button>
        <p id="result"></p>
    </div>
    <script>
        function rollDice() {
            const dice = Math.floor(Math.random() * 6) + 1;
            document.getElementById("result").innerText = "Du hast eine " + dice + " gewürfelt!";
        }
    </script>
</body>
</html>
