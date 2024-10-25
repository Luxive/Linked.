<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>LINKED!</title>
    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
            background-color: #1e1e1e;
            color: white;
        }
        .sidebar {
            height: 100vh;
            width: 250px;
            position: fixed;
            background-color: #2c2c2c;
            padding: 20px;
        }
        .sidebar h2 {
            color: #f1f1f1;
            margin-bottom: 40px;
            font-size: 1.8rem;
        }
        .sidebar a {
            display: block;
            color: white;
            padding: 10px 0;
            text-decoration: none;
            font-size: 1.1rem;
            cursor: pointer;
        }
        .sidebar a:hover {
            background-color: #444;
        }
        .main-content {
            margin-left: 260px;
            padding: 20px;
            background-color: #262626;
            min-height: 100vh;
            display: none;
        }
        .main-content.active {
            display: block;
        }
        .main-content h1 {
            font-size: 2.5rem;
            color: #e5e5e5;
        }
        .main-content a {
            color: #1abc9c;
            text-decoration: none;
        }
        .main-content a:hover {
            text-decoration: underline;
        }
        .accordion {
            width: 100%;
            background-color: #333;
            border: none;
            color: white;
            padding: 18px;
            text-align: left;
            font-size: 18px;
            cursor: pointer;
            transition: background-color 0.4s ease;
        }
        .accordion:hover {
            background-color: #444;
        }
        .accordion:after {
            content: '\002B';
            font-size: 20px;
            float: right;
        }
        .accordion.active:after {
            content: "\2212";
        }
        .panel {
            padding: 0 18px;
            background-color: #1e1e1e;
            display: none;
            overflow: hidden;
            border-top: 1px solid #444;
        }
        .panel a {
            display: block;
            color: #1abc9c;
            margin: 10px 0;
            text-decoration: none;
        }
        .panel a:hover {
            text-decoration: underline;
        }
        footer {
            margin-top: 40px;
            text-align: center;
            color: #ccc;
        }
    </style>
</head>
<body>
    <div class="sidebar">
        <h2>LINKED!</h2>
        <a onclick="showSection('home')">Home</a>
        <a onclick="showSection('proxies')">Prox1es</a>
        <a onclick="showSection('games')">Games</a>
        <a onclick="showSection('movies')">Movies</a>
        <a onclick="showSection('multipurpose')">Educational</a>
        <a onclick="showSection('coder')">Coder Stuff</a>
        <a onclick="showSection('credits')">Credits</a>
        <a onclick="showSection('proxy')">Make a Proxy</a>
    </div>

   <div id="home" class="main-content active">
        <h1>Welcome to Linked!</h1>
        <p>Join Discord or gay.</p>
    </div>

<div id="proxies" class="main-content">
        <h1>Games</h1>
        <button class="accordion">=</button>
        <div class="panel">
            <a href="#">Link 1 for RammerHead</a>
            <a href="#">Link 2 for RammerHead</a>
            <a href="#">Link 3 for RammerHead</a>
        </div>
 <h1>Proxies</h1>
        <button class="accordion"</button>
        <div class="panel">
            <a href="#">Link 1 for RammerHead</a>
            <a href="#">Link 2 for RammerHead</a>
            <a href="#">Link 3 for RammerHead</a>
        </div>
<button class="accordion">Interstellar</button>
<div class="panel">
            <a href="#">Link 1 for Interstellar</a>
            <a href="#">Link 2 for Interstellar</a>
            <a href="#">Link 3 for Interstellar</a>
        </div>
    </div>

<div id="blocked" class="main-content">
        <h1>Prox1es</h1>
        <p>Links to alternative proxies.</p>
</div>

<div id="games" class="main-content">
        <h1>Games</h1>
        <p>Links to games coming soon...</p>
    </div>

<div id="movies" class="main-content">
        <h1>Movies</h1>
        <p>Links to movies, TV shows, and music coming soon...</p>
    </div>

 <div id="multipurpose" class="main-content">
        <h1>Educational</h1>
        <p>Links coming soon</p>
    </div>

<div id="coder" class="main-content">
        <h1>Coder Stuff</h1>
        <p>Resources for coders.</p>
    </div>

<div id="credits" class="main-content">
        <h1>Credits</h1>
        <p>Credit to all contributors.</p>
    </div>

<div id="proxy" class="main-content">
        <h1>Make a Proxy</h1>
        <p>How to make your own proxy coming soon...</p>
    </div>

<footer>
        <p>&copy; 2024 LINKED! | All Rights Reserved</p>
    </footer>

<script>
        function showSection(sectionId) {
            var sections = document.getElementsByClassName("main-content");
            for (var i = 0; i < sections.length; i++) {
                sections[i].classList.remove("active");
            }
            document.getElementById(sectionId).classList.add("active");
        }

        var acc = document.getElementsByClassName("accordion");
        var i;

        for (i = 0; i < acc.length; i++) {
            acc[i].addEventListener("click", function() {
                this.classList.toggle("active");
                var panel = this.nextElementSibling;
                if (panel.style.display === "block") {
                    panel.style.display = "none";
                } else {
                    panel.style.display = "block";
                }
            });
        }
    </script>
</body>
</html>
