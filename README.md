<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <meta name="description" content="MA Agency - The most dangerous nexus of the dark web.">
    <meta name="author" content="MA Agency">
    <meta property="og:title" content="MA Agency - Dark Nexus">
    <meta property="og:description" content="Blood marks every corner of this domain. Dare to enter?">
    <meta property="og:image" content="https://yourimagepath.com/preview.jpg">
    <meta property="og:url" content="https://yourwebsite.com">
    <title>MA Agency - Dark Nexus</title>
    <style>
        /* General Styles */
        body {
            font-family: 'Arial', sans-serif;
            background-color: #000;
            color: #c00;
            margin: 0;
            padding: 0;
            scroll-behavior: smooth;
            background: linear-gradient(to bottom, #000, #111);
        }
        h1, h2, h3, p {
            margin: 0;
        }
        a {
            text-decoration: none;
        }

        /* Header */
        header {
            text-align: center;
            padding: 50px 20px;
            background: radial-gradient(circle, rgba(34, 34, 34, 0.9), #000);
            color: white;
            box-shadow: 0 5px 10px rgba(0, 0, 0, 0.8);
        }
        header h1 {
            font-size: 3.5rem;
            letter-spacing: 4px;
            text-shadow: 0 0 15px #c00, 0 0 30px black;
        }
        header p {
            font-size: 1.2rem;
            color: #888;
            text-shadow: 0 0 10px #c00;
        }

        /* Navigation */
        nav {
            display: flex;
            justify-content: center;
            gap: 20px;
            padding: 15px;
            background-color: #111;
            position: sticky;
            top: 0;
            z-index: 1000;
        }
        nav a {
            color: #c00;
            font-size: 1.2rem;
            font-weight: bold;
            text-transform: uppercase;
            transition: all 0.3s ease;
        }
        nav a:hover {
            color: white;
            transform: scale(1.1);
        }

        /* Hero Section */
        .hero {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            text-align: center;
            color: white;
            background: url('https://yourimagepath.com/dark-hero-bg.jpg') no-repeat center center/cover;
            box-shadow: inset 0 0 50px rgba(255, 0, 0, 0.5);
        }
        .hero h2 {
            font-size: 4rem;
            text-shadow: 0 0 20px #c00, 0 0 40px black;
            animation: pulse 2s infinite;
        }
        .hero p {
            font-size: 1.5rem;
            margin: 20px 0;
        }

        /* Agents Section */
        #agents {
            padding: 50px 20px;
            background-color: #111;
            color: white;
            text-align: center;
        }
        #agents h2 {
            font-size: 2.5rem;
            color: #c00;
        }
        #agents ul {
            list-style: none;
            padding: 0;
        }
        #agents li {
            margin: 20px 0;
            font-size: 1.5rem;
            color: #fff;
        }

        /* Complaints Section */
        #complaints {
            padding: 50px 20px;
            background-color: #111;
            color: white;
            text-align: center;
        }
        #complaints h2 {
            font-size: 2.5rem;
            color: #c00;
        }
        #complaints input {
            width: 80%;
            padding: 10px;
            margin: 10px 0;
            font-size: 1rem;
            border: 1px solid #c00;
            background: #222;
            color: white;
            border-radius: 5px;
        }
        #complaints button {
            padding: 10px 20px;
            font-size: 1rem;
            background-color: #c00;
            color: white;
            border: none;
            cursor: pointer;
            border-radius: 5px;
            transition: background-color 0.3s;
        }
        #complaints button:hover {
            background-color: #900;
        }
        #complaints ul {
            list-style: none;
            padding: 0;
            margin-top: 20px;
        }
        #complaints li {
            background: #222;
            color: white;
            margin: 10px 0;
            padding: 10px;
            border: 1px solid #c00;
            border-radius: 5px;
        }

        /* Jumpscare */
        #jumpscare {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.95);
            z-index: 9999;
            justify-content: center;
            align-items: center;
            animation: fadein 1s;
        }
        #jumpscare img {
            max-width: 80%;
            max-height: 80%;
        }
        @keyframes fadein {
            from {
                opacity: 0;
            }
            to {
                opacity: 1;
            }
        }

        /* Footer */
        footer {
            padding: 20px;
            text-align: center;
            background-color: #111;
            color: #888;
            font-size: 0.9rem;
        }
    </style>
</head>
<body>

<header>
    <h1>MA Agency</h1>
    <p>The Most Dangerous Nexus of the Dark Web</p>
</header>

<nav>
    <a href="#about">About</a>
    <a href="#agents">Agents</a>
    <a href="#complaints">Complaints</a>
</nav>

<section class="hero">
    <div>
        <h2>Where Shadows Reign</h2>
        <p>Blood marks every corner of this domain. Dare to enter?</p>
    </div>
</section>

<section id="agents">
    <h2>Our Elite Agents</h2>
    <ul>
        <li><strong>Leads Agent 47</strong><br>Phone: 01308769690 or 01989747850</li>
        <li><strong>Information Collector Agent 7</strong></li>
        <li><strong>Agent 37 and 27</strong></li>
    </ul>
</section>

<section id="complaints">
    <h2>Complaint Board</h2>
    <input type="text" id="complaintInput" placeholder="Write your complaint here">
    <button onclick="submitComplaint()">Submit</button>
    <ul id="complaintList"></ul>
</section>

<!-- Jumpscare -->
<div id="jumpscare" onclick="hideJumpscare()">
    <img src="https://yourimagepath.com/scary-image.jpg" alt="Scary Image">
</div>

<footer>
    © 2025 MA Agency - All Rights Reserved. Dare to enter the shadows?
</footer>

<script>
    // Complaints Logic
    function submitComplaint() {
        const input = document.getElementById('complaintInput');
        const list = document.getElementById('complaintList');

        if (input.value.trim() !== '') {
            const li = document.createElement('li');
            li.textContent = input.value;
            list.appendChild(li);
            input.value = '';
        } else {
            alert('Please write a complaint before submitting.');
        }
    }

    // Jumpscare Logic
    function showJumpscare() {
        document.getElementById('jumpscare').style.display = 'flex';
    }

    function hideJumpscare() {
        document.getElementById('jumpscare').style.display = 'none';
    }

    // Automatically show jumpscare after 5 seconds
    setTimeout(showJumpscare, 5000);
</script>

</body>
</html>
