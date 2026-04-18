# Portfolio-
Random 
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Portfolio</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Arial, sans-serif;
        }

        body {
            background: #0f172a;
            color: white;
        }

        header {
            display: flex;
            justify-content: space-between;
            padding: 20px 50px;
            background: #020617;
            position: sticky;
            top: 0;
        }

        header h1 {
            color: #38bdf8;
        }

        nav a {
            margin-left: 20px;
            text-decoration: none;
            color: white;
            transition: 0.3s;
        }

        nav a:hover {
            color: #38bdf8;
        }

        section {
            padding: 60px 50px;
        }

        .hero {
            height: 90vh;
            display: flex;
            align-items: center;
            justify-content: space-between;
        }

        .hero-text h2 {
            font-size: 40px;
        }

        .hero-text span {
            color: #38bdf8;
        }

        button {
            margin-top: 20px;
            padding: 10px 20px;
            border: none;
            background: #38bdf8;
            color: black;
            cursor: pointer;
            border-radius: 5px;
        }

        .projects {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }

        .card {
            background: #1e293b;
            padding: 20px;
            border-radius: 10px;
            transition: 0.3s;
        }

        .card:hover {
            transform: scale(1.05);
        }

        footer {
            text-align: center;
            padding: 20px;
            background: #020617;
        }

        /* Responsive */
        @media(max-width: 768px){
            .hero {
                flex-direction: column;
                text-align: center;
            }
        }
    </style>
</head>

<body>

<header>
    <h1>MyPortfolio</h1>
    <nav>
        <a href="#home">Home</a>
        <a href="#projects">Projects</a>
        <a href="#contact">Contact</a>
    </nav>
</header>

<section class="hero" id="home">
    <div class="hero-text">
        <h2>Hello, I'm <span>George</span></h2>
        <p>A beginner web developer learning cool stuff 🚀</p>
        <button onclick="scrollToProjects()">View Projects</button>
    </div>
</section>

<section id="projects">
    <h2>My Projects</h2>
    <br>

    <div class="projects">
        <div class="card">
            <h3>Project 1</h3>
            <p>Simple calculator using JavaScript.</p>
        </div>

        <div class="card">
            <h3>Project 2</h3>
            <p>Form validation project.</p>
        </div>

        <div class="card">
            <h3>Project 3</h3>
            <p>Student management system in C.</p>
        </div>
    </div>
</section>

<section id="contact">
    <h2>Contact Me</h2>
    <br>
    <p>Email: your@email.com</p>
</section>

<footer>
    <p>© 2026 My Portfolio</p>
</footer>

<script>
    function scrollToProjects() {
        document.getElementById("projects").scrollIntoView({
            behavior: "smooth"
        });
    }
</script>

</body>
</html>
