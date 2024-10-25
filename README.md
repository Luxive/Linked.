<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Unblocked Games</title>
    <style>
        body {
            font-family: 'Arial', sans-serif;
            background-color: #282828;
            color: white;
            margin: 0;
            padding: 0;
        }

header {
            background-color: #1abc9c;
            padding: 20px;
            text-align: center;
        }

header h1 {
            font-size: 3rem;
            color: white;
            text-transform: uppercase;
            letter-spacing: 2px;
        }

.games-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 15px;
            padding: 30px;
            margin: 0;
        }

.game-card {
            background-color: #34495e;
            border-radius: 8px;
            padding: 15px;
            text-align: center;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.3);
            transition: transform 0.2s;
        }

.game-card:hover {
            transform: translateY(-10px);
        }

.game-card img {
            width: 100%;
            height: 150px;
            border-radius: 8px;
            object-fit: cover;
        }

.game-card h3 {
            margin: 10px 0;
            font-size: 1.5rem;
        }

.play-btn {
            background-color: #e74c3c;
            color: white;
            padding: 10px 15px;
            border: none;
            border-radius: 5px;
            text-decoration: none;
            display: inline-block;
            font-size: 1rem;
            transition: background-color 0.3s ease;
        }

.play-btn:hover {
            background-color: #c0392b;
        }

footer {
            text-align: center;
            padding: 20px;
            background-color: #1abc9c;
            position: fixed;
            width: 100%;
            bottom: 0;
        }

footer p {
            margin: 0;
            color: white;
        }
    </style>
</head>
<body>

<header>
        <h1>Unblocked Games</h1>
</header>

<section class="games-grid">
        <div class="game-card">
            <img src="https://via.placeholder.com/200x150" alt="Game 1">
            <h3>Game 1</h3>
            <a href="https://yourgame1link.com" class="play-btn" target="_blank">Play Now</a>
        </div>

<div class="game-card">
            <img src="https://via.placeholder.com/200x150" alt="Game 2">
            <h3>Game 2</h3>
            <a href="https://yourgame2link.com" class="play-btn" target="_blank">Play Now</a>
        </div>

<div class="game-card">
            <img src="https://via.placeholder.com/200x150" alt="Game 3">
            <h3>Game 3</h3>
            <a href="https://yourgame3link.com" class="play-btn" target="_blank">Play Now</a>
        </div>

<div class="game-card">
            <img src="https://via.placeholder.com/200x150" alt="Game 4">
            <h3>Game 4</h3>
            <a href="https://yourgame4link.com" class="play-btn" target="_blank">Play Now</a>
        </div>
    </section>

<footer>
        <p>© 2024 Unblocked Games</p>
    </footer>

</body>
</html>
