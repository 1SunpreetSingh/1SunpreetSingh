<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cool Website</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            font-family: 'Arial', sans-serif;
            overflow: hidden;
        }

        header {
            position: fixed;
            top: 0;
            width: 100%;
            background-color: rgba(0, 0, 0, 0.8);
            z-index: 1000;
        }

        nav {
            display: flex;
            justify-content: space-around;
            align-items: center;
            height: 50px;
            color: white;
        }

        section {
            height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 2em;
            color: white;
        }

        #home {
            background: url('https://source.unsplash.com/random') no-repeat center center/cover;
        }

        #about {
            background-color: #3498db;
        }

        #contact {
            background-color: #e74c3c;
        }

        footer {
            text-align: center;
            padding: 20px;
            background-color: #2c3e50;
            color: white;
        }
    </style>
</head>
<body>
    <header>
        <nav>
            <a href="#home">Home</a>
            <a href="#about">About</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>

    <section id="home">
        <h1>Welcome to the Cool Website!</h1>
    </section>

    <section id="about">
        <h1>About Us:</h1>
        <p>This is the about section. We are an awesome team doing cool things.</p>
    </section>

    <section id="contact">
        <h1>Contact Us:</h1>
        <p>Feel free to reach out to us. We would love to hear from you!</p>
    </section>

    <footer>
        &copy; 2023 Cool Website. All rights reserved.
    </footer>

    <script>
        // Smooth scrolling
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();

                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
    </script>
</body>
</html>
