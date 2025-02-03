# My-portfolio
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Portfolio</title>
    <link rel="stylesheet" href="styles.css">
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css" rel="stylesheet">
    <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.6.0/jquery.min.js"></script>
</head>

<body>
    <header>

        <div class="container">
            <h1>Donaboina Hasini</h1>
            <nav>
                <ul>
                    <li><a href="#about">About</a></li>
                    <li><a href="#Skillssection">Skills</a></li>
                    <li><a href="#projects">Projects</a></li>
                    <li><a href="#internshipsection">Internships</a></li>
                    <li><a href="#certificatesection">Certificates</a></li>
                    <li><a href="#contact">Contact</a></li>
                </ul>
            </nav>
        </div>
    </header>

    <section id="about" class="section">
        <div class="container">
            <h2>About Me</h2>
            <p><i>Enthusiastic and adaptable fresher ready to embark on a successful career journey with a hunger for learning and growth.
                Eager to contribute and learn in a dynamic work environment.<br>
                I’m excited to bring my energy, creativity, and problem-solving mindset to every opportunity. My goal is to keep learning, improve as a developer, and contribute to meaningful projects.
            </i></p>
        </div>

        <div class="social-links">
            <a href="mailto:21h41a4521@bvcits.edu.in"><i class="fa-regular fa-envelope email"></i> E-mail</a>
            <a href="https://www.linkedin.com/in/donaboina-venkata-sai-hasini-09735a278"><i class="fab fa-linkedin"></i> LinkedIn</a><br>
            <a href="https://web.whatsapp.com/8d7979ed-cd33-46fb-9a61-777c574fc0a5" download="" class="resume"><i class="fa-regular fa-circle-down"></i> Download Resume</a>
        </div>
    </section>

    <section id="Skillssection" class="section">
        <div class="container">
            <h2>Skills</h2>
            <ul class="skillset">

                <li>SQL</li>
                <li>HTML</li>
                <li>CSS</li>
                <li>Java</li>
            </ul>
        </div>
    </section>

    <section id="projects" class="section">
        <div class="container">
            <h2>My Projects</h2>
            <div class="project">
                <h3>Project 1: BVC Cafeteria - App Development</h3>
                <button class="accordion">View Details</button>
                <div class="panel">
                    <p>Developed and launched the BVC Cafeteria app, optimizing the student cafeteria experience by providing real-time updates on available items, prices, and stock levels. Designed and implemented a user-friendly interface and integrated real-time data systems to enhance transparency and reduce wait times. The app’s seamless design and practical functionality were recognized by a company that offered to publish it on the Play Store at no cost.</p>
                    <a href="https://github.com/Dunaboinsvenkatasaihasini/BVC-Cafeteria" target="_blank">View Project</a>
                </div>
            </div>
            <div class="project">
                <h3>Project 2: My Portfolio</h3>
                <button class="accordion">View Details</button>
                <div class="panel">
                    <p>I developed a professional portfolio using HTML and CSS, focusing on creating responsive and user-friendly web designs. This project helped me gain proficiency in front-end web development, allowing me to showcase my personal projects and skills effectively.</p>
                    <a href="#">View Project</a>
                </div>
            </div>
        </div>
    </section>

    <section id="internshipsection" class="section">
        <div class="container">
            <h2>Internships</h2>
            <div class="internship">
                <p><strong>1. Front-end Development Intern</strong> at HQLEdutech Pvt Ltd
                Gained a foundational understanding of HTML5, CSS, and web design principles. Focused on enhancing user interface design for mobile apps and websites. Received a certificate from HQL EDUTECH.</p>
                <p><strong>2. Data Analytics & Visualization Intern</strong> at Accenture
                Worked on cleaning and analyzing datasets to derive business insights. Completed a virtual internship successfully on July 28, 2024.</p>
            </div>
        </div>
    </section>

    <section id="certificatesection" class="section">
        <div class="container">
            <h2>Certificates</h2>
            <ul class="certificates-list">
                <li><a href="https://www.hackerrank.com/certificates/03dad880ef06" target="_blank">SQL - HackerRank</a></li>
                <li><a href="https://www.hackerrank.com/certificates/1785d65a44ad" target="_blank">JavaScript - HackerRank</a></li>
                <li>Java Fundamentals - Oracle</li>
                <li>HTML - Infosys Springboard</li>
                <li>CSS - Bitslab</li>
            </ul>
        </div>
    </section>

    <section id="contact" class="section">
        <div class="container">
            <h2>Contact</h2>
            <form>
                <label for="name">Your Name</label>
                <input type="text" id="name" name="name" required>

                <label for="email">Your Email</label>
                <input type="email" id="email" name="email" required>

                <label for="message">Message</label>
                <textarea id="message" name="message" rows="4" required></textarea>

                <button type="submit">Send Message</button>
            </form>
        </div>
    </section>

    <footer>
        <div class="container">
            <p>&copy; 2025 Donaboina VS Hasini. All rights reserved.</p>
        </div>
    </footer>

    <script>
        // Smooth scrolling for navigation links
        $(document).ready(function () {
            $("a").on('click', function (event) {
                if (this.hash !== "") {
                    event.preventDefault();
                    var hash = this.hash;
                    $('html, body').animate({
                        scrollTop: $(hash).offset().top
                    }, 800, function () {
                        window.location.hash = hash;
                    });
                }
            });
        });

        // Accordion for project details
        var acc = document.getElementsByClassName("accordion");
        for (var i = 0; i < acc.length; i++) {
            acc[i].addEventListener("click", function () {
                this.classList.toggle("active");
                var panel = this.nextElementSibling;
                if (panel.style.maxHeight) {
                    panel.style.maxHeight = null;
                } else {
                    panel.style.maxHeight = panel.scrollHeight + "px";
                }
            });
        }
    </script>
</body>

</html>











/* Global Styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    transition: all 0.3s ease-in-out;
}

body {
    font-family: 'Arial', sans-serif;
    background-color: #f4f4f4;
    color: #333;
}

.container {
    width: 80%;
    margin: 0 auto;
}

h1, h2, h3 {
    text-align: center;
    margin-bottom: 1rem;
    font-weight: bold;
    color: #1f0606;
    position: relative;
}

p {
    margin-bottom: 1rem;
    font-size: 1.1rem;
    color: #555;
}

a {
    text-decoration: none;
}

/* Header Section */
header {
    background-color:gray;
    color: white;
    padding: 1rem 0;
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.2);
    position: fixed;
    width: 100%;
    top: 0;
    left: 0;
    z-index: 100;
}

header h1 {
    font-size: 2.5rem;
    margin-bottom: 0.5rem;
}

nav ul {
    display: flex;
    justify-content: center;
    list-style: none;
}

nav ul li {
    margin: 0 1.5rem;
}

nav ul li a {
    color: white;
    text-decoration: none;
    font-size: 1.1rem;
    font-weight: bold;
    text-transform: uppercase;
    transition: color 0.3s, transform 0.3s ease;
}

nav ul li a:hover {
    color: #f0f0f0;
    transform: scale(1.1);
}

/* About Section */
#about {
    background-color:lightcyan;
    padding: 4rem 0;
    margin-top: 70px; /* to avoid overlap with fixed header */
}

#about p {
    font-size: 1.2rem;
    color: #666;
}

.social-links {
    display: flex;
    justify-content: center;
    gap: 2rem;
    margin-top: 1rem;
}

.social-links a {
    color: #5e25fc;
    font-size: 1.5rem;
    transition: color 0.3s, transform 0.3s ease;
}

.social-links a:hover {
    color: #6a11cb;
    transform: scale(1.2);
}

.resume {
    background-color: #25bbfc;
    color: white;
    padding: 0.7rem 2rem;
    border: none;
    border-radius: 5px;
    font-size: 1.1rem;
    text-decoration: none;
    transition: background-color 0.3s, transform 0.3s ease;
}

.resume:hover {
    background-color: #6a11cb;
    transform: translateY(-5px);
}

/* Skills Section */
#Skillssection {
    padding: 4rem 0;
    background-color: #dfedfb;
}

.skillset {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 2rem;
    font-size: 1.2rem;
    list-style: none;
    font-weight: bold;
}

.skillset li {
    background-color: #2575fc;
    color: white;
    padding: 0.7rem 1.5rem;
    border-radius: 20px;
    transition: background-color 0.3s, transform 0.3s ease;
}

.skillset li:hover {
    background-color: #6a11cb;
    transform: translateY(-5px);
}

/* Projects Section */
#projects {
    background-color: #f2f2f2;
    padding: 4rem 0;
}

.project {
    background-color: #fff;
    padding: 2rem;
    margin-bottom: 2rem;
    border-radius: 8px;
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
    transition: box-shadow 0.3s, transform 0.3s ease;
}

.project:hover {
    box-shadow: 0 10px 20px rgba(0, 0, 0, 0.15);
    transform: translateY(-10px);
}

.project a {
    color: #2575fc;
    text-decoration: none;
    font-weight: bold;
    transition: color 0.3s ease;
}

.project a:hover {
    color: #6a11cb;
}

/* Internship Section */
#internshipsection {
    padding: 4rem 0;
    background-color: #fdf2f2;
}

.internship {
    font-size: 1.2rem;
    line-height: 1.8;
    margin-bottom: 2rem;
}

.internship p {
    margin-bottom: 1rem;
}

.internship strong {
    font-size: 1.3rem;
    color: #2575fc;
}

/* Certificates Section */
#certificatesection {
    padding: 4rem 0;
    background-color: #e2e2e2;
}

.certificates-list {
    font-size: 1.2rem;
    list-style: none;
    margin: 0;
    padding: 0;
}

.certificates-list li {
    margin-bottom: 1rem;
    transition: transform 0.3s ease;
}

.certificates-list li:hover {
    transform: scale(1.05);
}

.certificates-list a {
    color: #2575fc;
    text-decoration: none;
    font-weight: bold;
    transition: color 0.3s ease;
}

.certificates-list a:hover {
    color: #6a11cb;
}

/* Contact Section */
#contact {
    padding: 4rem 0;
    background-color: #f9f9f9;
}

form {
    display: flex;
    flex-direction: column;
    gap: 1.5rem;
}

form label {
    font-size: 1.1rem;
    color: #333;
}

form input, form textarea {
    padding: 0.8rem;
    font-size: 1.1rem;
    border: 1px solid #ccc;
    border-radius: 5px;
    transition: border-color 0.3s ease;
}

form input:focus, form textarea:focus {
    border-color: #2575fc;
}

form button {
    background-color: #25cafc;
    color: white;
    padding: 0.8rem 1.5rem;
    border: none;
    border-radius: 5px;
    font-size: 1.2rem;
    cursor: pointer;
    transition: background-color 0.3s, transform 0.3s ease;
}

form button:hover {
    background-color: #2111cb;
    transform: translateY(-5px);
}

/* Footer Section */
footer {
    background-color:gray;
    color: white;
    padding: 1rem 0;
    text-align: center;
    position: relative;
    bottom: 0;
    width: 100%;
    font-size: 1rem;
}

/* Media Queries for Responsiveness */
@media (max-width: 768px) {
    .container {
        width: 90%;
    }

    nav ul {
        flex-direction: column;
        gap: 1rem;
    }

    .social-links {
        flex-direction: column;
        gap: 1rem;
    }

    .skillset {
        flex-direction: column;
        gap: 1.5rem;
    }

    .certificates-list {
        font-size: 1rem;
    }

    .project {
        padding: 1.5rem;
    }

    .project a {
        font-size: 1rem;
    }

    .resume {
        font-size: 1rem;
        padding: 0.5rem 1.5rem;
    }

    form input, form textarea {
        padding: 0.8rem;
        font-size: 1rem;
    }
}

