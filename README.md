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
        <a onclick="showSection('multipurpose')">Education</a>
        <a onclick="showSection('coder')">Coder Stuff</a>
        <a onclick="showSection('credits')">Credits</a>
        <a onclick="showSection('proxy')">Make a Proxy</a>
    </div>

<div id="home" class="main-content active">
        <h1>Welcome to LINKED!</h1>
        <p>Select a category from the sidebar to get started.</p>
    </div>

 <div id="proxies" class="main-content">
        <h1>Proxies</h1>
        <button class="accordion">Rammerhead</button>
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

</div>

<div id="games" class="main-content">
        <h1>Games</h1>
        <button class="accordion">Extreme math</button>
        <div class="panel">
            <a href="https://tutoring4free.org/">Extreme math Link 1</a>
            <a href="https://easytutoring.app/">Extreme math link 2</a>
            <a href="https://extrememath.dev/">Extreme math link 3</a>
            <a href="https://simply-history.xyz/#google_vignette">Extreme math link 4</a>
            <a href="https://extrememath.org/">Extreme math link 5</a>
            <a href="https://simple-education.xyz/#google_vignette">Extreme math link 6</a>
        </div>
        <button class="accordion">Minecraft</button>
        <div class="panel">
            <a href="https://g.deev.is/">Minecraft link 1</a>
            <a href="https://eaglercraft.q13x.com/">Minecraft link 2</a>
            <a href="https://ubg100.github.io/eaglercraft.html">Minecraft link 3</a>
            <a href="https://burritoedition.github.io/emu/Minecraft/web/index.html">Minecraft link 4</a>
            <a href="https://reslauncher.vercel.app/">Minecraft link 5</a>
            <a href="https://sd592g.github.io/zj684od4lfg/">Minecraft link 6</a>
            <a href="https://eagler.almondnet.cn/Nebula.html">Minecraft link 7</a>
            <a href="https://mess.eu.org/">Minecraft link 8</a>
            <a href="https://precisionclient-88k.pages.dev/">Minecraft link 9</a>
        </div>
        <button class="accordion">Google sites</button>
        <div class="panel">
    <a href="https://sites.google.com/site/tyronesgameshack/">Tyrones games link 1</a>
    <a href="https://sites.google.com/site/unblockedgames66ez/">Unblocked games 66 link 2</a>
    <a href="https://sites.google.com/site/unblockedgame76/">Unblocked games 76 link 3</a>
    <a href="https://sites.google.com/view/games-unblockedd/">games unblocked link 4</a>
    <a href="https://sites.google.com/site/classroom6x/unblockedgames">Classroom6x link 5</a>
    <a href="https://sites.google.com/view/games-unblocked/">games unblocked2 link 6</a>
    <a href="https://sites.google.com/site/thegamecompilation/home?authuser=0">unblocked games world link 7</a>
        </div>
</div>

<div id="movies" class="main-content">
        <h1>Movies</h1>
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
        <h1>Educations</h1>
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

