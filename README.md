<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Twig's Utilities</title>
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
        <h2>Twig's Utilities</h2>
        <a onclick="showSection('home')">Home</a>
        <a onclick="showSection('proxies')">Pr0x1es</a>
        <a onclick="showSection('blocked')">Pr0x1es if the first is blocked</a>
        <a onclick="showSection('games')">Games Links</a>
        <a onclick="showSection('movies')">Movies/TV+Music</a>
        <a onclick="showSection('multipurpose')">Multi Purpose Pages</a>
        <a onclick="showSection('coder')">Coder Stuff</a>
        <a onclick="showSection('credits')">Credits</a>
        <a onclick="showSection('proxy')">Make a Proxy</a>
    </div>

<div id="home" class="main-content active">
        <h1>Welcome to Twig's Utilities</h1>
        <p>Select a category from the sidebar to get started.</p>
    </div>

 <div id="proxies" class="main-content">
        <h1>Proxies</h1>
        <button class="accordion">RammerHead</button>
        <div class="panel">
            <a href="#">Link 1 for RammerHead</a>
            <a href="#">Link 2 for RammerHead</a>
        </div>
        <button class="accordion">Interstellar</button>
        <div class="panel">
            <a href="#">Link 1 for Interstellar</a>
            <a href="#">Link 2 for Interstellar</a>
        </div>
</div>

<div id="blocked" class="main-content">
        <h1>Pr0x1es if the first one is blocked</h1>
        <button class="accordion">Alternative Proxy 1</button>
        <div class="panel">
            <a href="#">Link 1 for Alternative Proxy 1</a>
        </div>
        <button class="accordion">Alternative Proxy 2</button>
        <div class="panel">
            <a href="#">Link 1 for Alternative Proxy 2</a>
        </div>
</div>

<div id="games" class="main-content">
        <h1>Games Links</h1>
        <button class="accordion">Popular Games</button>
        <div class="panel">
            <a href="#">Game Link 1</a>
            <a href="#">Game Link 2</a>
        </div>
        <button class="accordion">New Games</button>
        <div class="panel">
            <a href="#">Game Link 1</a>
        </div>
</div>

<div id="movies" class="main-content">
        <h1>Movies/TV+Music</h1>
        <button class="accordion">Movies</button>
        <div class="panel">
            <a href="#">Movie Link 1</a>
        </div>
        <button class="accordion">TV Shows</button>
        <div class="panel">
            <a href="#">TV Show Link 1</a>
        </div>
</div>

<div id="multipurpose" class="main-content">
        <h1>Multi Purpose Pages</h1>
        <button class="accordion">Tools</button>
        <div class="panel">
            <a href="#">Tool Link 1</a>
        </div>
</div>

<div id="coder" class="main-content">
        <h1>Coder Stuff</h1>
        <button class="accordion">Coding Resources</button>
        <div class="panel">
            <a href="#">Resource Link 1</a>
        </div>
</div>

<div id="credits" class="main-content">
        <h1>Credits</h1>
        <button class="accordion">Acknowledgements</button>
        <div class="panel">
            <a href="#">Credit Link 1</a>
        </div>
    </div>

<div id="proxy" class="main-content">
        <h1>Make a Proxy</h1>
        <button class="accordion">Proxy Instructions</button>
        <div class="panel">
            <a href="#">Step 1</a>
            <a href="#">Step 2</a>
        </div>
    </div>

<footer>
        <p>&copy; 2024 Twig's Utilities | All Rights Reserved</p>
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
        for (var i = 0; i < acc.length; i++) {
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

