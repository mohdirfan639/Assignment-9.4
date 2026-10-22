ssignment 9.4 — Responsive Landing Page: Build
This assignment focuses on building the initial desktop version of a landing page using HTML and CSS, with semantic sections, buttons, feature cards, Flexbox, and CSS Grid.

We'll create a travel landing page called Wanderlust with a modern design, green color palette, large hero image, call-to-action buttons, and three feature cards.

1. Project folder structure
Create a folder named Assignment-9.4 with this structure:


text
Assignment-9.4/
├── index.html
├── style.css
└── images/
    ├── hero.jpg
    ├── destination-1.jpg
    ├── destination-2.jpg
    └── destination-3.jpg
Download suitable landscape photographs from Unsplash  and save them using the filenames above. You can also use the image URLs in the code below to preview the design before downloading local copies.

2. HTML file — index.html
This file defines the navigation bar, hero section, features, and footer using semantic HTML.


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Discover beautiful destinations and plan your next adventure with Wanderlust.">
    <title>Wanderlust — Discover Your Next Adventure</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <!-- Navigation -->
    <header class="site-header">
        <div class="container navbar">
            <a href="#home" class="logo">wanderlust<span>.</span></a>

            <nav aria-label="Main navigation">
                <a href="#home">Home</a>
                <a href="#destinations">Destinations</a>
                <a href="#features">Features</a>
                <a href="#about">About Us</a>
            </nav>

            <a href="#destinations" class="nav-cta">Explore Now ↗</a>
        </div>
    </header>

    <main>
        <!-- Hero Section -->
        <section class="hero container" id="home">
            <div class="hero-content">
                <span class="eyebrow">
                    <span class="status-dot"></span>
                    YOUR NEXT ADVENTURE STARTS HERE
                </span>

                <h1>Discover the world, <span>one journey</span> at a time.</h1>

                <p class="hero-description">
                    Escape the ordinary and explore extraordinary places.
                    Find inspiration, discover hidden gems, and create
                    memories that last a lifetime.
                </p>

                <div class="hero-buttons">
                    <a href="#destinations" class="button button-primary">
                        Explore Destinations <span>→</span>
                    </a>
                    <a href="#about" class="button button-outline">
                        Learn More
                    </a>
                </div>

                <div class="travel-stats">
                    <div>
                        <strong>120+</strong>
                        <span>Destinations</span>
                    </div>
                    <div>
                        <strong>15k+</strong>
                        <span>Happy Travelers</span>
                    </div>
                    <div>
                        <strong>4.9/5</strong>
                        <span>Traveler Rating</span>
                    </div>
                </div>
            </div>

            <div class="hero-visual">
                <img
                    src="https://images.unsplash.com/photo-1470770841072-f978cf4d019e?auto=format&fit=crop&w=1400&q=85"
                    alt="A beautiful alpine lake surrounded by green mountains">

                <div class="image-badge">
                    <span class="badge-icon">✦</span>
                    <div>
                        <strong>Find your happy place</strong>
                        <span>Adventure is calling</span>
                    </div>
                </div>
            </div>
        </section>

        <!-- Destinations Section -->
        <section class="destinations section" id="destinations">
            <div class="container">
                <div class="section-header">
                    <div>
                        <p class="section-label">EXPLORE THE WORLD</p>
                        <h2>Popular destinations</h2>
                    </div>
                    <a href="#features" class="text-link">
                        Discover more →
                    </a>
                </div>

                <div class="destination-grid">
                    <article class="destination-card">
                        <img
                            src="https://images.unsplash.com/photo-1516483638261-f4dbaf036963?auto=format&fit=crop&w=900&q=85"
                            alt="Colorful coastal villages in Italy">
                        <div class="destination-info">
                            <div>
                                <h3>Italian Coast</h3>
                                <p>Italy, Europe</p>
                            </div>
                            <span class="destination-arrow">↗</span>
                        </div>
                    </article>

                    <article class="destination-card">
                        <img
                            src="https://images.unsplash.com/photo-1500530855697-b586d89ba3ee?auto=format&fit=crop&w=900&q=85"
                            alt="Mountain landscape surrounded by nature">
                        <div class="destination-info">
                            <div>
                                <h3>Mountain Escape</h3>
                                <p>Swiss Alps, Europe</p>
                            </div>
                            <span class="destination-arrow">↗</span>
                        </div>
                    </article>

                    <article class="destination-card">
                        <img
                            src="https://images.unsplash.com/photo-1507525428034-b723cf961d3e?auto=format&fit=crop&w=900&q=85"
                            alt="Tropical beach with turquoise water">
                        <div class="destination-info">
                            <div>
                                <h3>Tropical Paradise</h3>
                                <p>Bali, Indonesia</p>
                            </div>
                            <span class="destination-arrow">↗</span>
                        </div>
                    </article>
                </div>
            </div>
        </section>

        <!-- Features Section -->
        <section class="features section" id="features">
            <div class="container">
                <div class="section-header">
                    <div>
                        <p class="section-label">THE WANDERLUST EXPERIENCE</p>
                        <h2>Travel made simple</h2>
                    </div>
                </div>

                <div class="feature-grid">
                    <article class="feature-card">
                        <span class="feature-icon">◎</span>
                        <h3>Handpicked Places</h3>
                        <p>
                            Discover carefully selected destinations
                            for unforgettable experiences.
                        </p>
                    </article>

                    <article class="feature-card">
                        <span class="feature-icon">✈</span>
                        <h3>Easy Planning</h3>
                        <p>
                            Find inspiration and organize your next
                            adventure with less effort.
                        </p>
                    </article>

                    <article class="feature-card">
                        <span class="feature-icon">♡</span>
                        <h3>Memorable Moments</h3>
                        <p>
                            Explore new cultures and create memories
                            worth sharing with the world.
                        </p>
                    </article>
                </div>
            </div>
        </section>

        <!-- About Section -->
        <section class="about section" id="about">
            <div class="container about-content">
                <p class="section-label">ABOUT WANDERLUST</p>
                <h2>The world is too beautiful to stay in one place.</h2>
                <p>
                    Wanderlust is designed to inspire your next adventure.
                    Explore remarkable destinations, embrace new experiences,
                    and make every journey count.
                </p>
                <a href="#home" class="button button-primary">
                    Start Exploring →
                </a>
            </div>
        </section>
    </main>

    <!-- Footer -->
    <footer class="site-footer">
        <div class="container footer-content">
            <a href="#home" class="logo">wanderlust<span>.</span></a>
            <p>Discover more. Travel further. Live fully.</p>
            <p>© 2026 Wanderlust. All rights reserved.</p>
        </div>
    </footer>

</body>
</html>
3. CSS file — style.css
The CSS implements the initial desktop design using a centered container, Flexbox for the navbar and hero, and Grid for destination and feature cards.


css

/* Assignment 9.4 - Wanderlust Landing Page */

/* 1. Reset and global styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: Arial, Helvetica, sans-serif;
    color: #20332b;
    background-color: #ffffff;
    line-height: 1.6;
}

img {
    display: block;
    max-width: 100%;
}

a {
    text-decoration: none;
    color: inherit;
}

.container {
    width: min(1200px, calc(100% - 64px));
    margin-inline: auto;
}

.section {
    padding: 80px 0;
}

/* 2. Header and navigation */
.site-header {
    background: #ffffff;
    border-bottom: 1px solid #edf0ed;
}

.navbar {
    min-height: 84px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 28px;
}

.logo {
    font-size: 27px;
    font-weight: 800;
    letter-spacing: -1.2px;
    color: #203f31;
    white-space: nowrap;
}

.logo span {
    color: #e6a756;
}

.navbar nav {
    display: flex;
    align-items: center;
    gap: 30px;
}

.navbar nav a {
    font-size: 14px;
    color: #59675f;
    transition: color 0.2s ease;
}

.navbar nav a:hover {
    color: #26734f;
}

.nav-cta {
    padding: 12px 19px;
    border-radius: 7px;
    background: #26734f;
    color: #ffffff;
    font-size: 14px;
    font-weight: 700;
    white-space: nowrap;
}

.nav-cta:hover,
.button-primary:hover {
    background: #1c5b3e;
}

/* 3. Hero section */
.hero {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 64px;
    padding-top: 76px;
    padding-bottom: 85px;
}

.hero-content {
    flex: 1;
    min-width: 0;
}

.eyebrow {
    display: inline-flex;
    align-items: center;
    gap: 9px;
    margin-bottom: 24px;
    color: #26734f;
    font-size: 11px;
    font-weight: 800;
    letter-spacing: 1.3px;
}

.status-dot {
    width: 8px;
    height: 8px;
    border-radius: 50%;
    background: #e6a756;
}

.hero h1 {
    max-width: 580px;
    margin-bottom: 22px;
    color: #203f31;
    font-size: 58px;
    line-height: 1.12;
    letter-spacing: -2.2px;
}

.hero h1 span {
    color: #2d8058;
}

.hero-description {
    max-width: 490px;
    margin-bottom: 28px;
    color: #69776e;
    font-size: 16px;
    line-height: 1.9;
}

.hero-buttons {
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    gap: 14px;
}

.button {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    gap: 14px;
    padding: 14px 20px;
    border-radius: 7px;
    font-size: 14px;
    font-weight: 700;
    transition: background 0.2s ease;
}

.button-primary {
    background: #26734f;
    color: #ffffff;
}

.button-outline {
    border: 1px solid #dce4de;
    color: #344b3e;
    background: #ffffff;
}

.button-outline:hover {
    background: #f2f6f2;
}

.travel-stats {
    display: flex;
    flex-wrap: wrap;
    gap: 30px;
    margin-top: 42px;
    padding-top: 24px;
    border-top: 1px solid #e8ede9;
}

.travel-stats div {
    display: flex;
    flex-direction: column;
    gap: 3px;
}

.travel-stats strong {
    color: #203f31;
    font-size: 21px;
}

.travel-stats span {
    color: #778178;
    font-size: 12px;
}

.hero-visual {
    position: relative;
    flex: 1;
    min-width: 0;
}

.hero-visual > img {
    width: 100%;
    height: 480px;
    object-fit: cover;
    border-radius: 16px;
}

.image-badge {
    position: absolute;
    right: -18px;
    bottom: 25px;
    display: flex;
    align-items: center;
    gap: 13px;
    max-width: calc(100% - 20px);
    padding: 16px 19px;
    background: #ffffff;
    border-radius: 10px;
    box-shadow: 0 8px 30px rgba(28, 55, 39, 0.14);
}

.badge-icon {
    display: grid;
    place-items: center;
    flex-shrink: 0;
    width: 38px;
    height: 38px;
    border-radius: 9px;
    background: #edf5ed;
    color: #26734f;
    font-size: 21px;
}

.image-badge div {
    display: flex;
    flex-direction: column;
}

.image-badge strong {
    color: #203f31;
    font-size: 13px;
}

.image-badge div span {
    color: #778178;
    font-size: 12px;
}

/* 4. Section headings */
.section-label {
    margin-bottom: 10px;
    color: #26734f;
    font-size: 11px;
    font-weight: 800;
    letter-spacing: 1.5px;
}

.section-header {
    display: flex;
    align-items: flex-end;
    justify-content: space-between;
    gap: 20px;
    margin-bottom: 30px;
}

.section-header h2,
.about-content h2 {
    color: #203f31;
    font-size: 36px;
    line-height: 1.25;
    letter-spacing: -1px;
}

.text-link {
    color: #26734f;
    font-size: 14px;
    font-weight: 700;
}

/* 5. Destination cards - CSS Grid */
.destinations {
    background: #f6f8f4;
}

.destination-grid {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 25px;
}

.destination-card {
    min-width: 0;
    overflow: hidden;
    background: #ffffff;
    border: 1px solid #e9eee8;
    border-radius: 12px;
}

.destination-card > img {
    width: 100%;
    height: 245px;
    object-fit: cover;
}

.destination-info {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 12px;
    padding: 20px;
}

.destination-info h3 {
    margin-bottom: 4px;
    color: #203f31;
    font-size: 18px;
}

.destination-info p {
    color: #778178;
    font-size: 13px;
}

.destination-arrow {
    display: grid;
    place-items: center;
    flex-shrink: 0;
    width: 36px;
    height: 36px;
    border-radius: 50%;
    background: #edf5ed;
    color: #26734f;
    font-size: 18px;
}

/* 6. Features section - CSS Grid */
.feature-grid {
    display: grid;
    grid-template-columns: repeat(3, minmax(0, 1fr));
    gap: 25px;
}

.feature-card {
    padding: 28px;
    border: 1px solid #e8ede9;
    border-radius: 12px;
    background: #ffffff;
}

.feature-icon {
    display: grid;
    place-items: center;
    width: 48px;
    height: 48px;
    margin-bottom: 20px;
    border-radius: 10px;
    background: #edf5ed;
    color: #26734f;
    font-size: 25px;
}

.feature-card h3 {
    margin-bottom: 10px;
    color: #203f31;
    font-size: 18px;
}

.feature-card p {
    color: #69776e;
    font-size: 14px;
    line-height: 1.8;
}

/* 7. About section */
.about {
    padding: 85px 0;
    background: #edf5ed;
}

.about-content {
    max-width: 800px;
    text-align: center;
}

.about-content h2 {
    margin-bottom: 18px;
}

.about-content > p:not(.section-label) {
    margin-bottom: 25px;
    color: #69776e;
    font-size: 16px;
}

/* 8. Footer */
.site-footer {
    padding: 30px 0;
    background: #203f31;
    color: #ffffff;
}

.footer-content {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 20px;
}

.footer-content .logo {
    color: #ffffff;
}

.footer-content p {
    color: #d1ddd4;
    font-size: 12px;
}

/* 9. Tablet layout */
@media screen and (max-width: 1000px) {
    .container {
        width: calc(100% - 48px);
    }

    .navbar {
        gap: 18px;
    }

    .navbar nav {
        gap: 16px;
    }

    .hero {
        gap: 35px;
    }

    .hero h1 {
        font-size: 45px;
    }

    .hero-visual > img {
        height: 400px;
    }

    .travel-stats {
        gap: 18px;
    }

    .destination-card > img {
        height: 200px;
    }
}

/* 10. Mobile layout */
@media screen and (max-width: 700px) {
    .container {
        width: calc(100% - 36px);
    }

    .section {
        padding: 55px 0;
    }

    .navbar {
        flex-wrap: wrap;
        justify-content: space-between;
        padding: 18px 0;
    }

    .logo {
        font-size: 24px;
    }

    .navbar nav {
        order: 3;
        width: 100%;
        justify-content: center;
        flex-wrap: wrap;
        gap: 12px 22px;
    }

    .navbar nav a {
        font-size: 13px;
    }

    .nav-cta {
        padding: 10px 12px;
        font-size: 12px;
    }

    .hero {
        flex-direction: column;
        align-items: stretch;
        gap: 35px;
        padding-top: 48px;
        padding-bottom: 55px;
    }

    .hero h1 {
        font-size: clamp(36px, 9vw, 48px);
        letter-spacing: -1.5px;
    }

    .hero-description {
        font-size: 15px;
    }

    .travel-stats {
        gap: 18px;
    }

    .travel-stats strong {
        font-size: 18px;
    }

    .travel-stats span {
        font-size: 11px;
    }

    .hero-visual > img {
        height: 330px;
    }

    .image-badge {
        right: 10px;
        bottom: 15px;
        padding: 12px;
    }

    .section-header {
        align-items: flex-start;
        flex-direction: column;
    }

    .section-header h2,
    .about-content h2 {
        font-size: 30px;
    }

    .destination-grid,
    .feature-grid {
        grid-template-columns: minmax(0, 1fr);
        gap: 20px;
    }

    .destination-card > img {
        height: 240px;
    }

    .feature-card {
        padding: 24px;
    }

    .about {
        padding: 60px 0;
    }

    .footer-content {
        flex-direction: column;
        text-align: center;
    }
}
4. Design elements used
Element

Design choice

Primary color

Forest green #26734f

Background

White #ffffff and light green #f6f8f4

Typography

Arial, sans-serif

Hero layout

Two columns on desktop

Destination cards

Three-column CSS Grid

Feature cards

Three-column CSS Grid

Navbar

Flexbox

Images

Rounded corners with object-fit: cover

5. How to run the project
Open the Assignment-9.4 folder in VS Code.

Create index.html and style.css.

Paste the corresponding code into each file.

Open index.html using the Live Server extension, or open it directly in Chrome.

Verify the desktop layout at 1440px wide.

The provided code currently loads images from Unsplash, so an internet connection is needed for those images. To use local files as required by your folder structure, download your chosen photographs into the images folder and replace the corresponding image URLs with paths such as images/hero.jpg.

6. Screenshots for submission
Capture screenshots of your actual webpage after running it.

TrailNest — Adventure Travel Website by Sienna Rose on Dribbble
desktop.png

Capture the navbar, hero section, buttons, statistics, and main image at 1440px width.

Accent Creative Digital Solutions
mobile.png

Capture the page at 375px width to show the responsive layout.

The images above are design references, not screenshots of your actual code.

7. Push the project to GitHub
First, create a new empty repository named Assignment-9.4 on GitHub. Then open the VS Code terminal in your project folder and run these commands:


bash
git init
git add index.html style.css images/
git commit -m "Complete Assignment 9.4 landing page"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/Assignment-9.4.git
git push -u origin main
Replace YOUR-USERNAME with your actual GitHub username. If Git reports that the remote already exists, update it with git remote set-url origin followed by your repository URL.

Once the push succeeds, your repository link will be:

https://github.com/YOUR-USERNAME/Assignment-9.4

Do not submit the example URL as your real repository link; use your actual GitHub username and verify that the repository is accessible.

8. Assignment report
Writing


Assignment 9.4 — Responsive Landing Page: Build
Objective: To build the initial version of a landing page based on a modern travel website design.

Technologies Used: HTML5, CSS3, Flexbox, CSS Grid, VS Code, Git, and GitHub.

Implementation:

Created the project structure with index.html, style.css, and an images folder.
Built a semantic navigation bar, hero section, buttons, destination cards, feature cards, and footer.
Applied a consistent color palette and typography.
Used Flexbox for navigation, hero alignment, and footer layout.
Used CSS Grid for destination and feature card layouts.
Added desktop styling and media queries for smaller screens.
Added images, spacing, borders, and rounded corners to improve the visual appearance.
Prepared the project for version control and GitHub submission.
Result: A travel-themed landing page with a desktop-first design and responsive styling for smaller screens.

Conclusion: The assignment demonstrates how HTML, CSS Flexbox, and CSS Grid can be combined to build a structured and visually appealing landing page. Git and GitHub are used to manage and publish the source code.

