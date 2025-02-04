#portfolio
<!DOCTYPE html> 
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Portfolio</title>
    <link rel="stylesheet" href="styles.css">
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css" rel="stylesheet">
    <script src="https://kit.fontawesome.com/a076d05399.js"></script>
</head>

<body>
    <header>
        <div class="container">
            
            <nav>
                <label class="logo">Donaboina Hasini</label>
                <input type="checkbox" id="check">
                <label for="check" class="checkbtn"><i class="fas fa-bars"></i></label>
                <ul>
                    <li><a class="active" href="#about">About</a></li>
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
                
                <div class="panel">
                    <p>Developed and launched the BVC Cafeteria app, optimizing the student cafeteria experience by providing real-time updates on available items, prices, and stock levels. Designed and implemented a user-friendly interface and integrated real-time data systems to enhance transparency and reduce wait times. The app’s seamless design and practical functionality were recognized by a company that offered to publish it on the Play Store at no cost.</p>
                    <a href="https://github.com/Dunaboinsvenkatasaihasini/BVC-Cafeteria" target="_blank">View Project</a>
                </div>
            </div>
            <div class="project">
                <h3>Project 2: My Portfolio</h3>

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










