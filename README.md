<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Imran Masood - Media & Hosting Professional</title>
    <!-- FontAwesome for Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary-color: #0b1f3a;
            --accent-color: #d4af37;
            --text-light: #f4f6f8;
            --text-dark: #333333;
            --bg-light: #f9fbfd;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: var(--bg-light);
            color: var(--text-dark);
            line-height: 1.6;
        }

        header {
            background: linear-gradient(135deg, var(--primary-color), #1b365d);
            color: var(--text-light);
            padding: 2rem 1rem;
            text-align: center;
            position: relative;
        }

        .header-container {
            max-width: 1000px;
            margin: 0 auto;
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 1.5rem;
        }

        @media (min-width: 768px) {
            .header-container {
                flex-direction: row;
                text-align: left;
            }
        }

        .profile-img {
            width: 180px;
            height: 180px;
            border-radius: 50%;
            border: 4px solid var(--accent-color);
            object-fit: cover;
            box-shadow: 0 4px 15px rgba(0,0,0,0.3);
        }

        .header-content h1 {
            font-size: 2.5rem;
            color: var(--text-light);
            margin-bottom: 0.5rem;
        }

        .header-content h1 span {
            color: var(--accent-color);
        }

        .header-content p.subtitle {
            font-size: 1.2rem;
            color: var(--accent-color);
            letter-spacing: 1px;
            margin-bottom: 1rem;
            text-transform: uppercase;
            font-weight: 600;
        }

        .contact-quick-info {
            display: flex;
            flex-wrap: wrap;
            gap: 1rem;
            font-size: 0.95krem;
            justify-content: center;
        }

        @media (min-width: 768px) {
            .contact-quick-info {
                justify-content: flex-start;
            }
        }

        .contact-quick-info div {
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }

        .contact-quick-info i {
            color: var(--accent-color);
        }

        /* Navigation Bar */
        nav {
            background-color: #061426;
            padding: 0.8rem;
            text-align: center;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 5px rgba(0,0,0,0.2);
        }

        nav a {
            color: var(--text-light);
            text-decoration: none;
            margin: 0 1rem;
            font-weight: 600;
            transition: color 0.3s;
        }

        nav a:hover {
            color: var(--accent-color);
        }

        /* Main Container */
        .container {
            max-width: 1000px;
            margin: 2rem auto;
            padding: 0 1rem;
            display: grid;
            gap: 2rem;
        }

        section {
            background: #ffffff;
            padding: 2rem;
            border-radius: 8px;
            box-shadow: 0 4px 10px rgba(0,0,0,0.05);
        }

        h2.section-title {
            font-size: 1.8rem;
            color: var(--primary-color);
            margin-bottom: 1.5rem;
            border-bottom: 3px solid var(--accent-color);
            padding-bottom: 0.5rem;
            display: inline-block;
        }

        /* Grid Layout for Skills and Info */
        .grid-2 {
            display: grid;
            grid-template-columns: 1fr;
            gap: 2rem;
        }

        @media (min-width: 768px) {
            .grid-2 {
                grid-template-columns: 1fr 1fr;
            }
        }

        /* Lists and Badges */
        ul {
            list-style-type: none;
        }

        ul.styled-list li {
            position: relative;
            padding-left: 1.5rem;
            margin-bottom: 0.8rem;
        }

        ul.styled-list li::before {
            content: "▪";
            color: var(--accent-color);
            position: absolute;
            left: 0;
            font-size: 1.2rem;
        }

        .skills-chips {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
        }

        .skill-chip {
            background-color: #f0f4f8;
            color: var(--primary-color);
            padding: 0.5rem 1rem;
            border-radius: 20px;
            font-size: 0.9rem;
            font-weight: 600;
            border: 1px solid #d1d9e0;
        }

        /* CV Download Section */
        .cv-box {
            text-align: center;
            background: linear-gradient(135deg, #f4f6f8, #e9edf2);
            padding: 2.5rem;
            border-radius: 8px;
            border: 2px dashed var(--accent-color);
        }

        .btn {
            display: inline-block;
            background-color: var(--primary-color);
            color: var(--text-light);
            padding: 0.8rem 2rem;
            border-radius: 4px;
            text-decoration: none;
            font-weight: bold;
            transition: background 0.3s, transform 0.2s;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
            margin-top: 1rem;
        }

        .btn:hover {
            background-color: var(--accent-color);
            color: var(--primary-color);
            transform: translateY(-2px);
        }

        .btn i {
            margin-right: 0.5rem;
        }

        /* Footer */
        footer {
            background-color: var(--primary-color);
            color: var(--text-light);
            text-align: center;
            padding: 1.5rem;
            margin-top: 3rem;
            font-size: 0.9rem;
        }

        table.info-table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 1rem;
        }

        table.info-table td {
            padding: 0.6rem 0;
            border-bottom: 1px solid #eee;
        }

        table.info-table td:first-child {
            font-weight: bold;
            color: var(--primary-color);
            width: 35%;
        }
    </style>
</head>
<body>

    <!-- Header / Hero Section -->
    <header>
        <div class="header-container">
            <!-- آپ اپنی پروفائل تصویر کا لنک یہاں لگا سکتے ہیں -->
            <img src="profile.jpg" alt="Imran Masood" class="profile-img" onerror="this.src='https://via.placeholder.com/180?text=Imran+Masood'">
            <div class="header-content">
                <h1>Imran <span>Masood</span></h1>
                <p class="subtitle">Media • Hosting • Digital Content</p>
                <div class="contact-quick-info">
                    <div><i class="fas fa-phone"></i> 0305-505-4165</div>
                    <div><i class="fas fa-envelope"></i> imran223344@gmail.com</div>
                    <div><i class="fas fa-map-marker-alt"></i> Bhara Khu, Islamabad</div>
                </div>
            </div>
        </div>
    </header>

    <!-- Navigation -->
    <nav>
        <a href="#about">About</a>
        <a href="#experience">Experience</a>
        <a href="#skills">Skills</a>
        <a href="#education">Education</a>
        <a href="#cv-download">Download CV</a>
    </nav>

    <!-- Main Content Container -->
    <div class="container">

        <!-- Media Profile Section -->
        <section id="about">
            <h2 class="section-title">Media Profile</h2>
            <p>Media and digital-content professional with practical experience in hosting, public communication, event coverage, digital channel work, and audience engagement. Experienced in appearing as a host for Imran Production TV and working across multiple digital media platforms and cultural events.</p>
        </section>

        <!-- Experience & Skills Grid -->
        <div class="grid-2">
            <!-- Media Experience -->
            <section id="experience">
                <h2 class="section-title">Media Experience</h2>
                <div style="margin-bottom: 1.5rem;">
                    <h3 style="color: var(--primary-color);">Imran Production TV — Host / Media Person</h3>
                    <ul class="styled-list" style="margin-top: 0.5rem;">
                        <li>Worked as a host/presenter for Imran Production TV YouTube channel.</li>
                        <li>Presented and covered media content with a focus on clear public communication.</li>
                        <li>Engaged with guests, audiences, and event participants in a professional manner.</li>
                        <li>Participated in and covered multiple events for digital-media content.</li>
                    </ul>
                </div>
                <div>
                    <h3 style="color: var(--primary-color);">Digital Media & Channel Work</h3>
                    <ul class="styled-list" style="margin-top: 0.5rem;">
                        <li>Worked with / contributed to multiple digital channels, including 9T News and other digital-media platforms.</li>
                        <li>Participated in media activities, event coverage, interviews, and digital content creation.</li>
                    </ul>
                </div>
            </section>

            <!-- Skills & Platforms -->
            <section id="skills">
                <h2 class="section-title">Hosting & Skills</h2>
                <div class="skills-chips" style="margin-bottom: 1.5rem;">
                    <span class="skill-chip">Hosting & On-Camera Presentation</span>
                    <span class="skill-chip">Public Speaking & Communication</span>
                    <span class="skill-chip">Digital Content Creation</span>
                    <span class="skill-chip">Audience Engagement</span>
                    <span class="skill-chip">Script / Caption Preparation</span>
                    <span class="skill-chip">Interviewing & Guest Interaction</span>
                    <span class="skill-chip">Event Coverage & Field Reporting</span>
                    <span class="skill-chip">Social Media / YouTube Content</span>
                    <span class="skill-chip">Event & Media Coordination</span>
                    <span class="skill-chip">Professional Public Dealing</span>
                </div>

                <h3 style="color: var(--primary-color); font-size: 1.2rem; margin-bottom: 0.5rem;">Languages</h3>
                <p><strong>Urdu:</strong> Native &nbsp;|&nbsp; <strong>English:</strong> Good</p>
            </section>
        </div>

        <!-- Events & Education Grid -->
        <div class="grid-2">
            <!-- Events & Cultural Media Exposure -->
            <section>
                <h2 class="section-title">Cultural Exposure</h2>
                <ul class="styled-list">
                    <li>Attended and participated in a wide range of public, cultural, social, and media events.</li>
                    <li>Media exposure and event participation connected with Lok Virsa and Pakistan National Council of the Arts (PNCA).</li>
                    <li>Experienced in interacting with guests, artists, organizers, and event participants.</li>
                </ul>
            </section>

            <!-- Education & Personal Info -->
            <section id="education">
                <h2 class="section-title">Education</h2>
                <ul class="styled-list" style="margin-bottom: 1.5rem;">
                    <li>3 Year DAE in Electrical Engineering — Bhara Khu Poly Technical College, Islamabad (2012–2015).</li>
                    <li>Islamabad Model School for Boys (2001–2012).</li>
                </ul>

                <h3 style="color: var(--primary-color); font-size: 1.2rem; margin-bottom: 0.5rem;">Personal Information</h3>
                <table class="info-table">
                    <tr><td>Date of Birth:</td><td>20 October 1995</td></tr>
                    <tr><td>Nationality:</td><td>Pakistani</td></tr>
                    <tr><td>Marital Status:</td><td>Single</td></tr>
                    <tr><td>Religion:</td><td>Islam</td></tr>
                </table>
            </section>
        </div>

        <!-- CV Download / View Section -->
        <section id="cv-download" class="cv-box">
            <h2 class="section-title" style="border-bottom: none; margin-bottom: 0.5rem;">Download / View CV</h2>
            <p style="margin-bottom: 1rem; color: #555;">آپ میری مکمل پروفیشنل سی وی یہاں سے براہ راست ڈاؤن لوڈ کر سکتے ہیں:</p>
            <!-- یہاں اپنی سی وی کی PDF فائل کا لنک (جیسے cv.pdf) دے سکتے ہیں -->
            <a href="cv.pdf" class="btn" download><i class="fas fa-download"></i> Download CV (PDF)</a>
        </section>

    </div>

    <!-- Footer -->
    <footer>
        <p>&copy; 2026 Imran Masood. All Rights Reserved. | Designed for Imran Production TV</p>
    </footer>

</body>
</html>
