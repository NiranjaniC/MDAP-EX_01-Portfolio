# MDAP-EX_01-Portfolio
## Date:11/08/2025

## AIM
To create a Portfolio using HTML and CSS.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for introduction, about, projects, and contact details.

### STEP 5
Define global styles for fonts, colors, and layout.

### STEP 6
Style the header, navigation bar, and sections.

### STEP 7
Use Flexbox or CSS Grid for layout design.

### STEP 8
Add hover effects and transitions for interactivity.

### STEP 9
Add Images and Media.

### STEP 10
Use optimized images for a professional look.

### STEP 11
Open the HTML file in a browser to check layout and functionality.

### STEP 12
Fix styling issues and refine content placement.

### STEP 13
Deploy the Portfolio.

### STEP 14
Upload to GitHub Pages for free hosting.

## PROGRAM
## index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Portfolio - Dark Theme</title>
    <link rel="stylesheet" href="index.css">
</head>
<body>
    <!-- Header and Navigation -->
    <header>
        <nav class="navbar">
            <div class="logo">MyPortfolio</div>
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#skills">Skills</a></li>
                <li><a href="#certifications">Certifications</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <!-- Home Section -->
    <section id="home" class="home-section">
        <div class="intro">
            <h1>Hello, I'm <span>Niranjani.C</span></h1>
            <p>Aspiring Data Analyst</p>
            <a href="#projects" class="btn">View My Work</a>
        </div>
        <div class="intro-img">
            <img src="images/profile.jpg" alt="Profile Photo">
        </div>
    </section>

    <!-- About Section -->
    <section id="about" class="about-section">
        <h2>About Me</h2>
        <p>I am a passionate IT student specializing in cloud computing and data analytics. I enjoy building solutions that are both efficient and visually appealing.</p>
    </section>

    <!-- Skills Section -->
    <section id="skills" class="skills-section">
        <h2>Skills</h2>
        <div class="skills-grid">
            <div class="skill-card">C programming</div>
            <div class="skill-card">Python</div>
            <div class="skill-card">Data Analytics</div>
            <div class="skill-card">Cloud Computing (AWS)</div>
            <div class="skill-card">SQL</div>
        </div>
    </section>

    <!-- Certifications Section -->
    <section id="certifications" class="certifications-section">
        <h2>Certifications</h2>
        <ul class="cert-list">
            <li>Google Data Analytics Professional Certificate</li>
            <li>AWS Cloud Practitioner Essentials</li>
            <li>Python for Everybody - Coursera</li>
            <li>Introduction to Data Science - IBM</li>
        </ul>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="projects-section">
        <h2>Projects</h2>
        <div class="project-grid">
            <div class="project-card">
                <img src="images/project1.png" alt="Project 1">
                <h3>Cloud Cost Tracker</h3>
                <p>Tracks AWS cost budget monthly using Lambda and Budgets API.</p>
            </div>
            <div class="project-card">
                <img src="images/project2.png" alt="Project 2">
                <h3>Data Visualization Dashboard</h3>
                <p>Interactive charts built with Python and Plotly.</p>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="contact-section">
        <h2>Contact Me</h2>
        <p>Email: <a href="mailto:niranjanichandrasekaren03@gmail.com">niranjanichandrasekaren03@gmail.com</a></p>
        <p>LinkedIn: <a href="#">linkedin.com/in/Niranjani</a></p>
    </section>

    <footer>
        <p>© 2025 Niranjani. All Rights Reserved.</p>
    </footer>
</body>
</html>
```
## index.css
```
/* Global Styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
body {
    font-family: Arial, sans-serif;
    color: #eaeaea;
    background-color: #121212;
    line-height: 1.6;
}
a {
    text-decoration: none;
    color: inherit;
}

/* Navbar */
.navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1rem 2rem;
    background-color:  #00249c;
    color: #eaeaea;
}
.nav-links {
    display: flex;
    gap: 1.5rem;
    list-style: none;
}
.nav-links a {
    color: #eaeaea;
    transition: color 0.3s ease;
}
.nav-links a:hover {
    color: #0635d0;
}

/* Home Section */
.home-section {
    display: flex;
    align-items: center;
    justify-content: space-around;
    padding: 2rem;
    background: #1e1e1e;
}
.home-section .intro {
    max-width: 50%;
}
.home-section h1 span {
    color:  #0635d0;
}
.btn {
    display: inline-block;
    margin-top: 1rem;
    padding: 0.7rem 1.5rem;
    background:  #0635d0;
    color: #121212;
    border-radius: 5px;
    font-weight: bold;
    transition: background 0.3s ease, transform 0.2s ease;
}
.btn:hover {
    background: #0635d0;
    transform: scale(1.05);
}
.intro-img img {
    width: 150px;
    border-radius: 50%;
    border: 3px solid #0635d0;
}

/* Section Base Styles */
.about-section, .skills-section, .certifications-section, .projects-section, .contact-section {
    padding: 3rem 2rem;
    text-align: center;
    background: #1e1e1e;
    margin-top: 1rem;
    border-radius: 8px;
}
.about-section p {
    max-width: 600px;
    margin: auto;
}

/* Skills Section */
.skills-grid {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 1rem;
    margin-top: 1.5rem;
}
.skill-card {
    background: #0635d0;
    color: #eaeaea;
    padding: 0.8rem 1.2rem;
    border-radius: 8px;
    box-shadow: 0 2px 5px rgba(0,0,0,0.4);
    transition: transform 0.3s ease, background 0.3s ease;
}
.skill-card:hover {
    transform: scale(1.05);
    background: #3b3b3b;
}

/* Certifications Section */
.cert-list {
    list-style: none;
    margin-top: 1rem;
}
.cert-list li {
    padding: 0.5rem 0;
    border-bottom: 1px solid #333;
}
.cert-list li:last-child {
    border-bottom: none;
}

/* Projects */
.project-grid {
    display: flex;
    gap: 2rem;
    justify-content: center;
    flex-wrap: wrap;
}
.project-card {
    background: #2a2a2a;
    padding: 1rem;
    border-radius: 10px;
    box-shadow: 0 2px 8px rgba(0,0,0,0.5);
    transition: transform 0.3s ease;
    max-width: 300px;
}
.project-card:hover {
    transform: translateY(-5px);
}
.project-card img {
    width: 100%;
    border-radius: 8px;
    border: 2px solid  #0635d0;
}

/* Contact Section */
.contact-section a {
    color: #0635d0;
}
.contact-section a:hover {
    text-decoration: underline;
}

/* Footer */
footer {
    text-align: center;
    padding: 1rem;
    background:#00249c;
    color: #eaeaea;
}

/* Responsive */
@media (max-width: 768px) {
    .home-section {
        flex-direction: column;
        text-align: center;
    }
    .home-section .intro, .intro-img {
        max-width: 100%;
    }
    .skills-grid {
        flex-direction: column;
        align-items: center;
    }
}

```
## OUTPUT
<img width="1919" height="1014" alt="Screenshot 2025-08-11 104552" src="https://github.com/user-attachments/assets/380feb30-7ef0-4905-bf7f-a30232c61dd5" />
<img width="1919" height="1019" alt="Screenshot 2025-08-11 104606" src="https://github.com/user-attachments/assets/88422acc-d457-40b4-a45e-e4321d618120" />
<img width="1919" height="1017" alt="Screenshot 2025-08-11 104613" src="https://github.com/user-attachments/assets/9e29da50-d240-41b6-8f28-3e3bcd0818bc" />


## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.
