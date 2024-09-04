<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Professional Website</title>
    <link rel="stylesheet" href="style.css">
    <style>
        /* Simple CSS to hide and show sections */
        section {
            display: none;
        }
        section.active {
            display: block;
        }
    </style>
</head>
<body>
    <header>
        <h1>Welcome to My Professional Website</h1>
        <nav>
            <ul>
                <li><a href="#" onclick="showSection('home')">Home</a></li>
                <li><a href="#" onclick="showSection('about')">About</a></li>
                <li><a href="#" onclick="showSection('contact')">Contact</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <!-- Home Section -->
        <section id="home" class="active">
            <h2>Introduction</h2>
            <p>This is the home page of my professional website. Here, you will find information about me and how to contact me.</p>
        </section>

        <!-- About Section -->
        <section id="about">
            <h2>About Me</h2>
            <p>I am a professional in [your field] with several years of experience. I specialize in [your expertise].</p>
        </section>

        <!-- Contact Section -->
        <section id="contact">
            <h2>Contact Me</h2>
            <p>If you would like to reach out, feel free to contact me via email at [your-email@example.com].</p>
        </section>
    </main>

    <footer>
        <p>&copy; 2024 Professional Website. All rights reserved.</p>
    </footer>

    <script>
        function showSection(sectionId) {
            // Hide all sections
            const sections = document.querySelectorAll('section');
            sections.forEach(section => section.classList.remove('active'));

            // Show the selected section
            document.getElementById(sectionId).classList.add('active');
        }
    </script>
</body>
</html>
