# Ex01 Portfolio
## Date:30.11.26

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
#style.css
* { margin: 0; padding: 0; box-sizing: border-box; }

body {
    min-height: 100vh;
    background: #dce3eb;
    color: #172b45;
    font-family: Arial, Helvetica, sans-serif;
    padding: 24px;
}

.portfolio {
    width: min(100%, 1220px);
    min-height: 860px;
    margin: 0 auto;
    background: #f8fafc;
    padding: 48px 5.2%;
    display: flex;
    flex-direction: column;
    box-shadow: 0 5px 30px #8794a5;
}

header { display: flex; justify-content: space-between; align-items: center; padding-bottom: 20px; border-bottom: 2px solid #dce5ee; gap: 16px; }
.brand { font-size: 25px; font-weight: 900; color: #142b49; letter-spacing: 1px; }
.brand span { color: #00a6a6; }
.nav { font-size: 11px; letter-spacing: 2px; color: #60758b; text-align: right; }

.hero {
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 28px;
    background: #142b49;
    color: white;
    padding: 34px 5%;
    margin: 26px 0 28px;
    border-radius: 12px;
}
.hero-copy { min-width: 0; }
.tag { color: #47e0d0; font-size: 11px; letter-spacing: 2px; margin-bottom: 8px; }
.hero h1 { font-size: clamp(27px, 3.3vw, 43px); line-height: 1.15; margin-bottom: 7px; }
.hero h1 span { color: #43e0d1; }
.register-number { color: #d3deeb; font-size: 13px; margin: 0 0 12px; letter-spacing: .3px; }
.register-number strong { color: #43e0d1; }
.hero h2 { font-size: 19px; font-weight: 500; margin-bottom: 8px; }
.intro { font-size: 13px; color: #d3deeb; max-width: 430px; line-height: 1.6; }
.contact-btn { display: inline-block; background: #43e0d1; color: #142b49; text-decoration: none; padding: 10px 19px; border-radius: 5px; font-size: 10px; font-weight: bold; margin-top: 14px; }
.contact-btn:hover { background: #70eee2; }
.avatar { width: 132px; height: 132px; border: 4px solid #43e0d1; border-radius: 50%; overflow: hidden; flex: 0 0 auto; background: #203e5f; }
.avatar img { display: block; width: 100%; height: 100%; object-fit: cover; object-position: 48% 35%; }

.content { display: grid; grid-template-columns: 1fr 1fr; gap: 3%; flex: 1; }
.left-column, .right-column { display: flex; flex-direction: column; gap: 16px; min-width: 0; }
.card { background: white; border: 1px solid #e0e8ef; border-radius: 8px; padding: 20px; }
.card h3 { color: #009e9e; font-size: 13px; letter-spacing: 1px; margin-bottom: 10px; }
.card p { color: #526477; font-size: 12px; line-height: 1.65; }
.about { flex: 1.05; }
.left-column > .card:nth-child(2) { flex: 1.5; }
.skill { margin: 8px 0; }
.skill span { font-size: 11px; font-weight: bold; }
.track { background: #e5edf3; height: 5px; margin-top: 4px; border-radius: 10px; }
.fill { height: 100%; background: #00b8ad; border-radius: 10px; }
.f1 { width: 90%; } .f2 { width: 85%; } .f3 { width: 65%; } .f4 { width: 60%; } .f5 { width: 80%; }
.education { flex: .85; }
.card h4 { font-size: 13px; margin-bottom: 5px; color: #183653; }
.projects { flex: 1.5; }
.project { padding: 7px 0; border-bottom: 1px solid #e4ebf1; }
.project:last-child { border-bottom: none; }
.project h4 { color: #183653; }
.strengths { display: grid; grid-template-columns: 1fr 1fr; gap: 12px; }
.strengths span { color: #526477; font-size: 11px; }
.contact { flex: 1; }
.contact p { margin: 5px 0; overflow-wrap: anywhere; }
.contact b { color: #183653; display: inline-block; width: 55px; }
footer { border-top: 2px solid #dce5ee; margin-top: 22px; padding-top: 16px; display: flex; justify-content: space-between; gap: 12px; color: #718196; font-size: 10px; letter-spacing: 1px; }

@media (max-width: 700px) {
    body { padding: 0; background: #f8fafc; }
    .portfolio { min-height: 100vh; padding: 24px 18px; box-shadow: none; }
    header { align-items: flex-start; }
    .brand { font-size: 20px; }
    .nav { max-width: 125px; line-height: 1.5; font-size: 9px; }
    .hero { padding: 25px 22px; margin: 20px 0; align-items: flex-start; }
    .hero h1 { font-size: clamp(25px, 7vw, 36px); }
    .hero h1 span { display: block; }
    .hero h2 { font-size: 16px; }
    .avatar { width: 94px; height: 94px; }
    .content { grid-template-columns: 1fr; gap: 16px; }
    .left-column, .right-column { gap: 16px; }
    .card { padding: 18px; }
    footer { flex-direction: column; font-size: 9px; }
}

@media (max-width: 430px) {
    .hero { flex-direction: column-reverse; }
    .avatar { width: 112px; height: 112px; align-self: flex-start; }
}

@page { size: A4 landscape; margin: 0; }
@media print {
    html, body { width: 297mm; min-height: 210mm; padding: 0; background: white; }
    .portfolio { width: 297mm; min-height: 210mm; margin: 0; padding: 10mm 13mm; box-shadow: none; print-color-adjust: exact; -webkit-print-color-adjust: exact; }
}



#index.html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Student portfolio of Sribalakumaran R.">
    <title>Sribalakumaran R | Portfolio</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
<div class="portfolio">
    <header>
        <div class="brand">MY<span>PORTFOLIO.</span></div>
        <div class="nav">STUDENT PORTFOLIO | 2026</div>
    </header>

    <main>
        <section class="hero">
            <div class="hero-copy">
                <p class="tag">HELLO, WELCOME TO MY PORTFOLIO</p>
                <h1>I'm <span>Sribalakumaran R</span></h1>
                <p class="register-number">Register Number: <strong>212225220104</strong></p>
                <h2>Web Developer &amp; Student</h2>
                <p class="intro">
                    Passionate about technology, creative design
                    and building modern web applications.
                </p>
                <a href="mailto:yourname@gmail.com" class="contact-btn">CONTACT ME</a>
            </div>
            <div class="avatar">
                <img src="assets/profile.jpg" alt="Portrait of Sribalakumaran R">
            </div>
        </section>

        <div class="content">
            <div class="left-column">
                <section class="card about">
                    <h3>01 / ABOUT ME</h3>
                    <p>
                        I am a college student interested in web development and technology.
                        I enjoy creating attractive, user-friendly websites. I am passionate
                        about learning new skills and improving my programming knowledge.
                    </p>
                </section>

                <section class="card">
                    <h3>02 / TECHNICAL SKILLS</h3>
                    <div class="skill"><span>HTML5</span><div class="track"><div class="fill f1"></div></div></div>
                    <div class="skill"><span>CSS3</span><div class="track"><div class="fill f2"></div></div></div>
                    <div class="skill"><span>JavaScript</span><div class="track"><div class="fill f3"></div></div></div>
                    <div class="skill"><span>Python</span><div class="track"><div class="fill f4"></div></div></div>
                    <div class="skill"><span>Problem Solving</span><div class="track"><div class="fill f5"></div></div></div>
                </section>

                <section class="card education">
                    <h3>03 / EDUCATION</h3>
                    <h4>Undergraduate Degree</h4>
                    <p>Your College Name</p>
                    <p>Department: Your Department</p>
                    <p>Currently Pursuing | 2026</p>
                </section>
            </div>

            <div class="right-column">
                <section class="card projects">
                    <h3>04 / MY PROJECTS</h3>
                    <div class="project"><h4>01. Personal Portfolio</h4><p>A responsive portfolio website using HTML and CSS.</p></div>
                    <div class="project"><h4>02. Login Page</h4><p>A simple and attractive user login interface.</p></div>
                    <div class="project"><h4>03. Landing Page</h4><p>A modern landing page with a clean user interface.</p></div>
                </section>

                <section class="card">
                    <h3>05 / PERSONAL STRENGTHS</h3>
                    <div class="strengths">
                        <span>✓ Quick Learner</span><span>✓ Teamwork</span>
                        <span>✓ Creativity</span><span>✓ Time Management</span>
                    </div>
                </section>

                <section class="card contact">
                    <h3>06 / GET IN TOUCH</h3>
                    <p><b>Email</b> yourname@gmail.com</p>
                    <p><b>Phone</b> +91 9876543210</p>
                    <p><b>Location</b> Tamil Nadu, India</p>
                    <p><b>GitHub</b> github.com/yourusername</p>
                </section>
            </div>
        </div>
    </main>

    <footer>
        <span>DESIGNED WITH PASSION</span>
        <span>© 2026 SRIBALAKUMARAN R | ALL RIGHTS RESERVED</span>
    </footer>
</div>
</body>
</html>






## OUTPUT

<img width="1280" height="832" alt="image" src="https://github.com/user-attachments/assets/fafaa482-4247-480f-b3ef-e3805cd32c30" />



## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.
