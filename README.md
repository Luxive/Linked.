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
        <h2>Twig's Utilities</h2>
        <a onclick="showSection('home')">Home</a>
        <a onclick="showSection('proxies')">Prox1es</a>
        <a onclick="showSection('games')">Games</a>
        <a onclick="showSection('movies')">Movies</a>
        <a onclick="showSection('multipurpose')">Educations</a>
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
        <h1>Pr0x1es if the first one is blocked</h1>
        <button class="accordion">Backup Proxy 1</button>
        <div class="panel">
            <a href="#">Link 1 for Backup Proxy 1</a>
            <a href="#">Link 2 for Backup Proxy 1</a>
        </div>

<button class="accordion">Backup Proxy 2</button>
        <div class="panel">
            <a href="#">Link 1 for Backup Proxy 2</a>
            <a href="#">Link 2 for Backup Proxy 2</a>
        </div>
    </div>

<div id="games" class="main-content">
        <h1>Games Links</h1>
        <button class="accordion">Action Games</button>
        <div class="panel">
            <a href="#">Link 1 for Action Games</a>
            <a href="#">Link 2 for Action Games</a>
        </div>

<button class="accordion">Puzzle Games</button>
        <div class="panel">
            <a href="#">Link 1 for Puzzle Games</a>
            <a href="#">Link 2 for Puzzle Games</a>
        </div>
</div>

<div id="movies" class="main-content">
        <h1>Movies/TV+Music</h1>
        <button class="accordion">Movies</button>
        <div class="panel">
            <a href="#">Link 1 for Movies</a>
            <a href="#">Link 2 for Movies</a>
        </div>

<button class="accordion">TV Shows</button>
        <div class="panel">
            <a href="#">Link 1 for TV Shows</a>
            <a href="#">Link 2 for TV Shows</a>
        </div>

<button class="accordion">Music</button>
        <div class="panel">
            <a href="#">Link 1 for Music</a>
            <a href="#">Link 2 for Music</a>
        </div>
    </div>

<div id="multipurpose" class="main-content">
        <h1>Multi Purpose Pages</h1>
        <button class="accordion">Page 1</button>
        <div class="panel">
            <a href="#">Link 1 for Page 1</a>
            <a href="#">Link 2 for Page 1</a>
        </div>

<button class="accordion">Page 2</button>
        <div class="panel">
            <a href="#">Link 1 for Page 2</a>
            <a href="#">Link 2 for Page 2</a>
        </div>
    </div>

<div id="coder" class="main-content">
        <h1>Coder Stuff</h1>
        <button class="accordion">HTML/CSS Resources</button>
        <div class="panel">
            <a href="#">Link 1 for HTML/CSS</a>
            <a href="#">Link 2 for HTML/CSS</a>
        </div>

<button class="accordion">JavaScript Resources</button>
        <div class="panel">
            <a href="#">Link 1 for JavaScript</a>
            <a href="#">Link 2 for JavaScript</a>
        </div>
    </div>

<div id="credits" class="main-content">
        <h1>Credits</h1>
        <button class="accordion">Contributors</button>
        <div class="panel">
            <a href="#">Link 1 for Contributors</a>
            <a href="#">Link 2 for Contributors</a>
        </div>
    </div>

<div id="proxy" class="main-content">
        <h1>Make a Proxy</h1>
        <button class="accordion">Proxy Setup Guide</button>
        <div class="panel">
            <a href="#">Link 1 for Proxy Guide</a>
            <a href="#">Link 2 for Proxy Guide</a>
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
        var
