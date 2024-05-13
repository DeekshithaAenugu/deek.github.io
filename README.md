-HTML-
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Deekshitha's Portfolio</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <aside>
        <h1>Aenugu Deekshitha</h1>
        <img src="DK .jpg" alt="dk">
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#portfolio">Portfolio</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </aside>

    <main>
        <section id="home" class="card">
            <h2>Welcome</h2>
             <p>Welcome to my professional portfolio. Discover the projects I've worked on and my journey through the world of Electronics and Communication Engineering, blending technical prowess with a passion for innovation.</p>

        </section>

        <section id="about" class="card">
            <h2>About Me</h2>
            <p>Currently enhancing my skills in Computer Science at Sacred Heart University, I am Aenugu Deekshitha, a dedicated and driven professional aiming to leverage my technical knowledge and certifications in AI and Electric Power Systems to solve real-world problems. With a solid foundation in C, Java, and Python, I am eager to apply my abilities in a challenging environment while continuing to grow and learn.</p>

        </section>

        <section id="portfolio" class="card">
            <h2>Work's</h2>
            <article class="project">
                <h3>Smart Campus Energy Monitoring</h3>
    <p>Developed an IoT-based energy monitoring system designed to optimize and reduce electricity usage across college campuses. This project involved the integration of sensor data with a centralized Python-based analytics platform to monitor and analyze energy consumption patterns.</p>
  </article>
            <article class="project">
                <h3>Automated Home Gardens</h3>
    <p>Engineered a microcontroller-driven system to automate garden watering based on soil moisture levels, which significantly improves plant health by applying precise watering protocols. The system uses C and Java for control logic and operational efficiency.</p>

            </article>
            <article class="project">
                <h3>Virtual Bake Sale Platform</h3>
    <p>Initiated and developed an online platform to host virtual bake sales, facilitating community engagement and fundraising. The platform features a user-friendly interface developed using HTML, CSS, and JavaScript to allow users to participate in or host bake sales from the comfort of their homes.</p>

            </article>
        </section>

        <section id="contact" class="card">
    <h2>Contact Me</h2>
    <form>
        <div class="form-group">
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" placeholder="Your Name" required>
        </div>
        <div class="form-group">
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" placeholder="Your Email" required>
        </div>
        <div class="form-group">
            <label for="message">Message:</label>
            <textarea id="message" name="message" placeholder="Your Message" required></textarea>
        </div>
        <button type="submit">Send</button>
    </form>
</section>

    </main>

    <footer>
        <a href="">LinkedIn</a>
        <p>© 2024 Aenugu Deekshitha. All rights are reserved.</p>
    </footer>
</body>
</html>
-CSS-
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    scroll-behavior: smooth;
}

body {
    font-family: 'Arial', sans-serif;
    display: flex;
    min-height: 100vh;
    background-color: #fff8e1; 
}

aside {
    background-color: #ffab40; 
    color: #ffffff;
    padding: 20px;
    width: 250px;
    height: 100vh;
    position: fixed;
    overflow: auto;
}

aside h1 {
    font-size: 24px;
    margin-bottom: 20px;
}

nav ul {
    list-style-type: none;
}

nav a {
    color: #ffffff;
    text-decoration: none;
    display: block;
    padding: 10px;
    transition: background-color 0.3s;
}

nav a:hover {
    background-color: #ffd54f; 
}

main {
    margin-left: 250px;
    flex-grow: 1;
    padding: 20px;
}

.card {
    background: #ffffff; 
    margin-bottom: 20px;
    padding: 20px;
    border-radius: 10px;
    box-shadow: 0 2px 5px rgba(0,0,0,0.1);
}

.section-intro {
    background-color: #ffe0b2; 
}

.section-work {
    background-color: #e0f7fa; 
}

.project {
    margin-top: 10px;
    background: #f5f5f5; 
    padding: 10px;
    border-radius: 5px;
}

footer {
    background-color: #ffab40; 
    color: #ffffff;
    text-align: center;
    padding: 10px;
    position: fixed;
    bottom: 0;
    width: calc(100% - 250px);
    margin-left: 250px;
}

footer a {
    color: #b2dfdb; 
    text-decoration: none;
}

@media (max-width: 768px) {
    aside {
        width: 100%;
        height: auto;
        position: relative;
    }

    main {
        margin-left: 0;
    }

    footer {
        width: 100%;
        margin-left: 0;
    }
}
#contact {
    background-color: #f5f5f5; 
    padding: 20px;
    border-radius: 10px;
    box-shadow: 0 2px 5px rgba(0,0,0,0.1);
}

#contact h2 {
    color: #333;
    margin-bottom: 20px;
}

.form-group {
    display: grid;
    grid-template-columns: 1fr 3fr; 
    gap: 10px;
    margin-bottom: 15px;
    align-items: center;
}

.form-group label {
    justify-self: end;
    font-weight: bold;
    color: #555;
}

.form-group input,
.form-group textarea {
    width: 100%;
    padding: 8px;
    border-radius: 4px;
    border: 1px solid #ccc;
    background: #ffffff;
}

.form-group textarea {
    height: 100px; 
}

button {
    width: auto;
    padding: 10px 20px;
    background-color: #ffab40;
    color: white;
    border: none;
    cursor: pointer;
    border-radius: 4px;
    align-self: start;
    justify-self: end;
    grid-column: 2 / 3;
}

@media (max-width: 600px) {
    .form-group {
        grid-template-columns: 1fr; 
    }

    .form-group label {
        justify-self: start; 
    }

    button {
        width: 100%;
        justify-self: stretch; 
    }
}
