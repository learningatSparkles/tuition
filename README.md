**<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>LearningatSparkles | Bright Futures Begin Here</title>
    <style>
        /* CSS Reset & Variables */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        :root {
            --primary-color: #4A90E2;
            --secondary-color: #FF6B6B;
            --accent-color: #FFD166;
            --dark-color: #2C3E50;
            --light-color: #F8F9FA;
        }

        body {
            line-height: 1.6;
            color: var(--dark-color);
            background-color: var(--light-color);
        }

        /* Navigation */
        header {
            background: #ffffff;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            max-width: 1200px;
            margin: 0 auto;
            padding: 1rem 2rem;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: bold;
            color: var(--primary-color);
        }

        .logo span {
            color: var(--secondary-color);
        }

        .nav-links {
            display: flex;
            list-style: none;
            gap: 1.5rem;
        }

        .nav-links a {
            text-decoration: none;
            color: var(--dark-color);
            font-weight: 600;
            transition: color 0.3s;
        }

        .nav-links a:hover {
            color: var(--primary-color);
        }

        .btn-contact {
            background-color: var(--primary-color);
            color: white;
            padding: 0.5rem 1.2rem;
            border-radius: 20px;
            text-decoration: none;
            font-weight: bold;
            transition: background 0.3s;
        }

        .btn-contact:hover {
            background-color: #357ABD;
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, #e0c3fc 0%, #8ec5fc 100%);
            padding: 4rem 2rem;
            text-align: center;
        }

        .hero-content {
            max-width: 800px;
            margin: 0 auto;
        }

        .hero h1 {
            font-size: 2.5rem;
            margin-bottom: 1rem;
            color: var(--dark-color);
        }

        .hero p {
            font-size: 1.2rem;
            margin-bottom: 2rem;
        }

        /* Features Section */
        .features {
            max-width: 1200px;
            margin: 4rem auto;
            padding: 0 2rem;
        }

        .section-title {
            text-align: center;
            margin-bottom: 3rem;
            font-size: 2rem;
            color: var(--dark-color);
        }

        .feature-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
        }

        .feature-card {
            background: white;
            padding: 2rem;
            border-radius: 10px;
            text-align: center;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
            transition: transform 0.3s;
        }

        .feature-card:hover {
            transform: translateY(-5px);
        }

        .feature-card h3 {
            color: var(--primary-color);
            margin-bottom: 0.5rem;
        }

        /* Courses Section */
        .courses {
            background-color: #ffffff;
            padding: 4rem 2rem;
        }

        .course-container {
            max-width: 1200px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 2rem;
        }

        .course-card {
            border: 1px solid #e1e1e1;
            border-radius: 10px;
            overflow: hidden;
            background: white;
        }

        .course-header {
            background-color: var(--secondary-color);
            color: white;
            padding: 1rem;
            text-align: center;
        }

        .course-body {
            padding: 1.5rem;
        }

        .course-body ul {
            list-style-type: none;
            margin-top: 1rem;
        }

        .course-body li {
            padding: 0.3rem 0;
            border-bottom: 1px solid #f0f0f0;
        }

        /* Contact Section */
        .contact {
            max-width: 800px;
            margin: 4rem auto;
            padding: 0 2rem;
        }

        .form-group {
            margin-bottom: 1.5rem;
        }

        .form-group label {
            display: block;
            margin-bottom: 0.5rem;
            font-weight: 600;
        }

        .form-group input, 
        .form-group textarea, 
        .form-group select {
            width: 100%;
            padding: 0.8rem;
            border: 1px solid #ccc;
            border-radius: 5px;
            font-size: 1rem;
        }

        .btn-submit {
            background-color: var(--primary-color);
            color: white;
            padding: 0.8rem 2rem;
            border: none;
            border-radius: 5px;
            font-size: 1rem;
            cursor: pointer;
            width: 100%;
            font-weight: bold;
        }

        .btn-submit:hover {
            background-color: #357ABD;
        }

        /* Footer */
        footer {
            background-color: var(--dark-color);
            color: white;
            text-align: center;
            padding: 2rem;
            margin-top: 4rem;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .nav-links {
                display: none; /* Can be expanded into a mobile menu */
            }
            
            .hero h1 {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body>

    <!-- Header Navigation -->
    <header>
        <nav>
            <div class="logo">Learningat<span>Sparkles</span></div>
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About Us</a></li>
                <li><a href="#courses">Courses</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
            <a href="#contact" class="btn-contact">Enroll Now</a>
        </nav>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="hero-content">
            <h1>Ignite Your Academic Potential</h1>
            <p>Empowering students through personalized learning, expert tutoring, and interactive educational programs.</p>
            <a href="#contact" class="btn-contact" style="padding: 0.8rem 2rem; font-size: 1.1rem;">Get Started Today</a>
        </div>
    </section>

    <!-- Why Choose Us / Features -->
    <section class="features" id="about">
        <h2 class="section-title">Why LearningatSparkles?</h2>
        <div class="feature-grid">
            <div class="feature-card">
                <h3>Experienced Tutors</h3>
                <p>Dedicated educators committed to building conceptual clarity and student confidence.</p>
            </div>
            <div class="feature-card">
                <h3>Small Batch Sizes</h3>
                <p>Focused attention on every student to address individual learning needs and paces.</p>
            </div>
            <div class="feature-card">
                <h3>Interactive Learning</h3>
                <p>Engaging teaching methodology incorporating modern visual aids and practical examples.</p>
            </div>
            <div class="feature-card">
                <h3>Regular Assessments</h3>
                <p>Track student growth with weekly practice tests and regular parent progress reports.</p>
            </div>
        </div>
    </section>

    <!-- Courses Offered -->
    <section class="courses" id="courses">
        <h2 class="section-title">Our Tuition Programs</h2>
        <div class="course-container">
            <!-- Primary Level -->
            <div class="course-card">
                <div class="course-header">
                    <h3>Primary Foundation</h3>
                    <p>Grade 1 - Grade 5</p>
                </div>
                <div class="course-body">
                    <p>Building strong fundamentals in core subjects through fun, interactive methods.</p>
                    <ul>
                        <li>Mathematics Basics</li>
                        <li>English Reading & Writing</li>
                        <li>General Science</li>
                    </ul>
                </div>
            </div>

            <!-- Middle School -->
            <div class="course-card">
                <div class="course-header" style="background-color: var(--primary-color);">
                    <h3>Middle School Program</h3>
                    <p>Grade 6 - Grade 8</p>
                </div>
                <div class="course-body">
                    <p>Strengthening analytical skills and problem-solving abilities.</p>
                    <ul>
                        <li>Advanced Mathematics</li>
                        <li>Physics, Chemistry & Biology</li>
                        <li>Grammar & Communication</li>
                    </ul>
                </div>
            </div>

            <!-- High School -->
            <div class="course-card">
                <div class="course-header" style="background-color: #2ED573;">
                    <h3>High School Prep</h3>
                    <p>Grade 9 - Grade 12</p>
                </div>
                <div class="course-body">
                    <p>Focused board exam preparation and competitive concept building.</p>
                    <ul>
                        <li>Higher Mathematics</li>
                        <li>Advanced Sciences</li>
                        <li>Exam Strategy & Mock Tests</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Form -->
    <section class="contact" id="contact">
        <h2 class="section-title">Book a Free Trial Class</h2>
        <form onsubmit="alert('Thank you for reaching out! We will contact you soon.'); return false;">
            <div class="form-group">
                <label for="name">Student's Full Name</label>
                <input type="text" id="name" required placeholder="John Doe">
            </div>
            <div class="form-group">
                <label for="grade">Grade / Class</label>
                <select id="grade" required>
                    <option value="">Select Grade</option>
                    <option value="primary">Primary (Grade 1 - 5)</option>
                    <option value="middle">Middle School (Grade 6 - 8)</option>
                    <option value="high">High School (Grade 9 - 12)</option>
                </select>
            </div>
            <div class="form-group">
                <label for="phone">Parent's Phone Number</label>
                <input type="tel" id="phone" required placeholder="+1 234 567 8900">
            </div>
            <div class="form-group">
                <label for="message">Message / Specific Requirements</label>
                <textarea id="message" rows="4" placeholder="Tell us about the subject needs..."></textarea>
            </div>
            <button type="submit" class="btn-submit">Submit Registration</button>
        </form>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2026 LearningatSparkles Tuition Classes. All Rights Reserved.</p>
    </footer>

</body>
</html>**
