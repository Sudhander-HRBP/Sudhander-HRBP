<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sudhander Rajendran | HR Business Partner</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&family=Montserrat:wght@400;500;600&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary-color: #667eea;
            --secondary-color: #764ba2;
            --accent-color: #f093fb;
            --dark-color: #2d3748;
            --light-color: #f7fafc;
            --text-color: #4a5568;
            --success-color: #48bb78;
            --warning-color: #ed8936;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        html {
            scroll-behavior: smooth;
        }
        
        body {
            font-family: 'Poppins', sans-serif;
            color: var(--text-color);
            line-height: 1.6;
            background-color: var(--light-color);
        }
        
        h1, h2, h3, h4 {
            font-family: 'Montserrat', sans-serif;
            color: var(--dark-color);
            font-weight: 600;
        }
        
        .container {
            width: 90%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* Header & Navigation */
        header {
            background-color: white;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
        }
        
        .nav-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 0;
        }
        
        .logo {
            font-size: 1.8rem;
            font-weight: 700;
            color: var(--primary-color);
            text-decoration: none;
        }
        
        .logo span {
            color: var(--secondary-color);
        }
        
        .nav-links {
            display: flex;
            list-style: none;
        }
        
        .nav-links li {
            margin-left: 30px;
        }
        
        .nav-links a {
            text-decoration: none;
            color: var(--dark-color);
            font-weight: 500;
            transition: color 0.3s;
        }
        
        .nav-links a:hover {
            color: var(--primary-color);
        }
        
        .mobile-menu-btn {
            display: none;
            background: none;
            border: none;
            font-size: 1.5rem;
            color: var(--dark-color);
            cursor: pointer;
        }
        
        /* Hero Section */
        .hero {
            padding: 150px 0 100px;
            background: linear-gradient(135deg, var(--primary-color) 0%, var(--secondary-color) 100%);
            color: white;
            text-align: center;
        }
        
        .hero h1 {
            font-size: 3.5rem;
            color: white;
            margin-bottom: 20px;
        }
        
        .hero p {
            font-size: 1.2rem;
            max-width: 700px;
            margin: 0 auto 30px;
            opacity: 0.9;
        }
        
        .hero-badges {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 10px;
            margin-bottom: 40px;
        }
        
        .badge {
            background-color: rgba(255,255,255,0.2);
            padding: 8px 16px;
            border-radius: 50px;
            font-size: 0.9rem;
        }
        
        .btn {
            display: inline-block;
            background-color: white;
            color: var(--primary-color);
            padding: 12px 30px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 600;
            transition: all 0.3s;
            border: 2px solid white;
        }
        
        .btn:hover {
            background-color: transparent;
            color: white;
        }
        
        .btn-outline {
            background-color: transparent;
            color: white;
            border: 2px solid white;
        }
        
        .btn-outline:hover {
            background-color: white;
            color: var(--primary-color);
        }
        
        /* Section Styles */
        section {
            padding: 100px 0;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 60px;
        }
        
        .section-title h2 {
            font-size: 2.5rem;
            margin-bottom: 15px;
            position: relative;
            display: inline-block;
        }
        
        .section-title h2:after {
            content: '';
            position: absolute;
            width: 70px;
            height: 4px;
            background: linear-gradient(to right, var(--primary-color), var(--secondary-color));
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            border-radius: 2px;
        }
        
        /* About Section */
        .about-content {
            display: flex;
            align-items: center;
            gap: 50px;
        }
        
        .about-text {
            flex: 1;
        }
        
        .about-text h3 {
            font-size: 1.8rem;
            margin-bottom: 20px;
            color: var(--primary-color);
        }
        
        .about-stats {
            display: flex;
            margin-top: 30px;
            gap: 30px;
        }
        
        .stat {
            text-align: center;
        }
        
        .stat-number {
            font-size: 2.5rem;
            font-weight: 700;
            color: var(--primary-color);
            display: block;
        }
        
        .stat-label {
            font-size: 0.9rem;
            color: var(--text-color);
        }
        
        /* Experience Section */
        .timeline {
            position: relative;
            max-width: 800px;
            margin: 0 auto;
        }
        
        .timeline:before {
            content: '';
            position: absolute;
            left: 50%;
            transform: translateX(-50%);
            width: 2px;
            height: 100%;
            background-color: var(--primary-color);
            opacity: 0.3;
        }
        
        .timeline-item {
            display: flex;
            margin-bottom: 50px;
        }
        
        .timeline-item:nth-child(odd) {
            flex-direction: row-reverse;
        }
        
        .timeline-content {
            background-color: white;
            padding: 25px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            width: 45%;
            position: relative;
        }
        
        .timeline-content:after {
            content: '';
            position: absolute;
            top: 20px;
            width: 20px;
            height: 20px;
            background-color: white;
            transform: rotate(45deg);
        }
        
        .timeline-item:nth-child(even) .timeline-content:after {
            right: -10px;
        }
        
        .timeline-item:nth-child(odd) .timeline-content:after {
            left: -10px;
        }
        
        .timeline-dot {
            position: absolute;
            left: 50%;
            transform: translateX(-50%);
            width: 20px;
            height: 20px;
            border-radius: 50%;
            background-color: var(--primary-color);
            border: 4px solid white;
            box-shadow: 0 0 0 4px rgba(102, 126, 234, 0.2);
        }
        
        .timeline-date {
            position: absolute;
            top: -30px;
            left: 50%;
            transform: translateX(-50%);
            background-color: var(--primary-color);
            color: white;
            padding: 5px 15px;
            border-radius: 20px;
            font-size: 0.9rem;
            font-weight: 500;
        }
        
        /* Skills Section */
        .skills-container {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .skill-category {
            background-color: white;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
        }
        
        .skill-category h3 {
            margin-bottom: 20px;
            color: var(--primary-color);
        }
        
        .skill-item {
            margin-bottom: 20px;
        }
        
        .skill-name {
            display: flex;
            justify-content: space-between;
            margin-bottom: 5px;
        }
        
        .skill-bar {
            height: 10px;
            background-color: #e2e8f0;
            border-radius: 5px;
            overflow: hidden;
        }
        
        .skill-progress {
            height: 100%;
            background: linear-gradient(to right, var(--primary-color), var(--secondary-color));
            border-radius: 5px;
        }
        
        /* Education & Achievements */
        .cards-container {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .card {
            background-color: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
            transition: transform 0.3s;
        }
        
        .card:hover {
            transform: translateY(-10px);
        }
        
        .card-header {
            padding: 20px;
            background: linear-gradient(135deg, var(--primary-color) 0%, var(--secondary-color) 100%);
            color: white;
        }
        
        .card-body {
            padding: 25px;
        }
        
        /* Contact Section */
        .contact-container {
            display: flex;
            gap: 50px;
        }
        
        .contact-info {
            flex: 1;
        }
        
        .contact-item {
            display: flex;
            align-items: center;
            margin-bottom: 25px;
        }
        
        .contact-icon {
            width: 50px;
            height: 50px;
            background: linear-gradient(135deg, var(--primary-color) 0%, var(--secondary-color) 100%);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin-right: 15px;
            color: white;
            font-size: 1.2rem;
        }
        
        /* Footer */
        footer {
            background-color: var(--dark-color);
            color: white;
            padding: 60px 0 30px;
        }
        
        .footer-content {
            display: flex;
            justify-content: space-between;
            flex-wrap: wrap;
            gap: 40px;
            margin-bottom: 40px;
        }
        
        .footer-links {
            display: flex;
            flex-direction: column;
        }
        
        .footer-links a {
            color: #cbd5e0;
            text-decoration: none;
            margin-bottom: 10px;
            transition: color 0.3s;
        }
        
        .footer-links a:hover {
            color: white;
        }
        
        .social-links {
            display: flex;
            gap: 15px;
            margin-top: 20px;
        }
        
        .social-link {
            width: 40px;
            height: 40px;
            background-color: rgba(255,255,255,0.1);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            text-decoration: none;
            transition: all 0.3s;
        }
        
        .social-link:hover {
            background-color: var(--primary-color);
            transform: translateY(-5px);
        }
        
        .copyright {
            text-align: center;
            padding-top: 30px;
            border-top: 1px solid rgba(255,255,255,0.1);
            color: #a0aec0;
            font-size: 0.9rem;
        }
        
        /* Responsive Styles */
        @media (max-width: 992px) {
            .about-content {
                flex-direction: column;
            }
            
            .contact-container {
                flex-direction: column;
            }
            
            .timeline:before {
                left: 30px;
            }
            
            .timeline-item {
                flex-direction: row !important;
            }
            
            .timeline-content {
                width: calc(100% - 80px);
                margin-left: 80px;
            }
            
            .timeline-content:after {
                left: -10px !important;
                right: auto !important;
            }
            
            .timeline-dot, .timeline-date {
                left: 30px;
            }
        }
        
        @media (max-width: 768px) {
            .nav-links {
                display: none;
                position: absolute;
                top: 100%;
                left: 0;
                width: 100%;
                background-color: white;
                flex-direction: column;
                padding: 20px;
                box-shadow: 0 10px 15px rgba(0,0,0,0.1);
            }
            
            .nav-links.active {
                display: flex;
            }
            
            .nav-links li {
                margin: 10px 0;
            }
            
            .mobile-menu-btn {
                display: block;
            }
            
            .hero h1 {
                font-size: 2.5rem;
            }
            
            .section-title h2 {
                font-size: 2rem;
            }
            
            .about-stats {
                flex-direction: column;
                gap: 20px;
            }
        }
    </style>
</head>
<body>
    <!-- Header & Navigation -->
    <header>
        <div class="container nav-container">
            <a href="#home" class="logo">Sudhander<span>Rajendran</span></a>
            
            <button class="mobile-menu-btn" id="mobileMenuBtn">
                <i class="fas fa-bars"></i>
            </button>
            
            <ul class="nav-links" id="navLinks">
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#experience">Experience</a></li>
                <li><a href="#skills">Skills</a></li>
                <li><a href="#education">Education</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="container">
            <h1>Sudhander Rajendran</h1>
            <p>Strategic HR Business Partner with 9+ years of experience partnering with leadership teams to drive people strategy, organizational development, and performance outcomes.</p>
            
            <div class="hero-badges">
                <div class="badge">HR Business Partner</div>
                <div class="badge">Strategic People Operations</div>
                <div class="badge">Talent Management</div>
                <div class="badge">Remote & Global Teams</div>
            </div>
            
            <div>
                <a href="#contact" class="btn">Get In Touch</a>
                <a href="#experience" class="btn btn-outline">View Experience</a>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="about">
        <div class="container">
            <div class="section-title">
                <h2>About Me</h2>
                <p>Strategic HR professional with expertise in driving organizational success</p>
            </div>
            
            <div class="about-content">
                <div class="about-text">
                    <h3>Strategic HR Business Partner</h3>
                    <p>I am a results-driven HR professional with extensive experience in partnering with leadership teams to align HR strategy with business objectives. My expertise spans organizational development, workforce planning, employee engagement, and translating business goals into effective HR initiatives across remote and global teams.</p>
                    
                    <p>I have a proven track record of implementing HR systems, improving retention rates, and leading successful change management initiatives. My approach combines strategic thinking with practical implementation to create sustainable people solutions.</p>
                    
                    <div class="about-stats">
                        <div class="stat">
                            <span class="stat-number">9+</span>
                            <span class="stat-label">Years Experience</span>
                        </div>
                        <div class="stat">
                            <span class="stat-number">15%</span>
                            <span class="stat-label">Retention Increase</span>
                        </div>
                        <div class="stat">
                            <span class="stat-number">100+</span>
                            <span class="stat-label">HR Projects</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Experience Section -->
    <section id="experience" style="background-color: #f8f9fa;">
        <div class="container">
            <div class="section-title">
                <h2>Work Experience</h2>
                <p>My professional journey in Human Resources</p>
            </div>
            
            <div class="timeline">
                <!-- Experience 1 -->
                <div class="timeline-item">
                    <div class="timeline-dot"></div>
                    <div class="timeline-date">2023 - Present</div>
                    <div class="timeline-content">
                        <h3>HR Manager / Talent Acquisition</h3>
                        <h4>Alp Consulting Pvt Ltd</h4>
                        <ul>
                            <li>Partner with senior leaders to align HR strategy with business objectives</li>
                            <li>Advise management on organizational development, workforce planning, and employee engagement</li>
                            <li>Lead performance management cycles and development planning</li>
                            <li>Analyze HR metrics (turnover, retention, performance) to support decision-making</li>
                        </ul>
                    </div>
                </div>
                
                <!-- Experience 2 -->
                <div class="timeline-item">
                    <div class="timeline-dot"></div>
                    <div class="timeline-date">2020 - 2023</div>
                    <div class="timeline-content">
                        <h3>Assistant Manager Human Resources</h3>
                        <h4>Nithyo Infotech</h4>
                        <ul>
                            <li>Supported managers on employee relations, performance improvement plans, and policy interpretation</li>
                            <li>Assisted in talent reviews and succession planning initiatives</li>
                            <li>Acted as HR advisor for operational leaders across multiple locations</li>
                            <li>Supported change initiatives and HR system implementation projects</li>
                        </ul>
                    </div>
                </div>
                
                <!-- Experience 3 -->
                <div class="timeline-item">
                    <div class="timeline-dot"></div>
                    <div class="timeline-date">2017 - 2020</div>
                    <div class="timeline-content">
                        <h3>Executive HR & Operation</h3>
                        <h4>DMS Software Engineering</h4>
                        <ul>
                            <li>Responsible for processing and proofing of monthly payroll of clients</li>
                            <li>Calculated statutory payments and terminal benefits (Gratuity, Bonus, VRS, Leave payments)</li>
                            <li>Prepared Cristal Reports, Reconciliations, Journal Entries and all payroll-related reports</li>
                            <li>Managed bank file uploads, EPF, ETF, APIT schedules, and stamp duty processing</li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Skills Section -->
    <section id="skills">
        <div class="container">
            <div class="section-title">
                <h2>Skills & Expertise</h2>
                <p>Core competencies and professional skills</p>
            </div>
            
            <div class="skills-container">
                <div class="skill-category">
                    <h3>Strategic HR</h3>
                    <div class="skill-item">
                        <div class="skill-name">
                            <span>HR Business Partnering</span>
                            <span>95%</span>
                        </div>
                        <div class="skill-bar">
                            <div class="skill-progress" style="width: 95%"></div>
                        </div>
                    </div>
                    <div class="skill-item">
                        <div class="skill-name">
                            <span>Organizational Development</span>
                            <span>90%</span>
                        </div>
                        <div class="skill-bar">
                            <div class="skill-progress" style="width: 90%"></div>
                        </div>
                    </div>
                    <div class="skill-item">
                        <div class="skill-name">
                            <span>Stakeholder Management</span>
                            <span>92%</span>
                        </div>
                        <div class="skill-bar">
                            <div class="skill-progress" style="width: 92%"></div>
                        </div>
                    </div>
                    <div class="skill-item">
                        <div class="skill-name">
                            <span>Workforce Planning</span>
                            <span>88%</span>
                        </div>
                        <div class="skill-bar">
                            <div class="skill-progress" style="width: 88%"></div>
                        </div>
                    </div>
                </div>
                
                <div class="skill-category">
                    <h3>Talent Management</h3>
                    <div class="skill-item">
                        <div class="skill-name">
                            <span>Performance Management</span>
                            <span>93%</span>
                        </div>
                        <div class="skill-bar">
                            <div class="skill-progress" style="width: 93%"></div>
                        </div>
                    </div>
                    <div class="skill-item">
                        <div class="skill-name">
                            <span>Employee Engagement</span>
                            <span>90%</span>
                        </div>
                        <div class="skill-bar">
                            <div class="skill-progress" style="width: 90%"></div>
                        </div>
                    </div>
                    <div class="skill-item">
                        <div class="skill-name">
                            <span>Succession Planning</span>
                            <span>85%</span>
                        </div>
                        <div class="skill-bar">
                            <div class="skill-progress" style="width: 85%"></div>
                        </div>
                    </div>
                    <div class="skill-item">
                        <div class="skill-name">
                            <span>Talent Acquisition</span>
                            <span>87%</span>
                        </div>
                        <div class="skill-bar">
                            <div class="skill-progress" style="width: 87%"></div>
                        </div>
                    </div>
                </div>
                
                <div class="skill-category">
                    <h3>HR Operations</h3>
                    <div class="skill-item">
                        <div class="skill-name">
                            <span>Policy & Compliance</span>
                            <span>94%</span>
                        </div>
                        <div class="skill-bar">
                            <div class="skill-progress" style="width: 94%"></div>
                        </div>
                    </div>
                    <div class="skill-item">
                        <div class="skill-name">
                            <span>HR Analytics</span>
                            <span>82%</span>
                        </div>
                        <div class="skill-bar">
                            <div class="skill-progress" style="width: 82%"></div>
                        </div>
                    </div>
                    <div class="skill-item">
                        <div class="skill-name">
                            <span>Change Management</span>
                            <span>88%</span>
                        </div>
                        <div class="skill-bar">
                            <div class="skill-progress" style="width: 88%"></div>
                        </div>
                    </div>
                    <div class="skill-item">
                        <div class="skill-name">
                            <span>Payroll Management</span>
                            <span>90%</span>
                        </div>
                        <div class="skill-bar">
                            <div class="skill-progress" style="width: 90%"></div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Education & Achievements -->
    <section id="education" style="background-color: #f8f9fa;">
        <div class="container">
            <div class="section-title">
                <h2>Education & Achievements</h2>
                <p>Academic background and professional accomplishments</p>
            </div>
            
            <div class="cards-container">
                <!-- Education 1 -->
                <div class="card">
                    <div class="card-header">
                        <h3>Master of Human Resource Management</h3>
                        <p>Human Resource Management Institute</p>
                    </div>
                    <div class="card-body">
                        <p><strong>2024 - Present | Currently Reading</strong></p>
                        <p>Advanced studies in strategic human resource management, organizational behavior, and talent development strategies.</p>
                    </div>
                </div>
                
                <!-- Education 2 -->
                <div class="card">
                    <div class="card-header">
                        <h3>Diploma in Human Resource Management</h3>
                        <p>Thondaman Vocational Training Centre</p>
                    </div>
                    <div class="card-body">
                        <p><strong>2012</strong></p>
                        <p>Comprehensive foundation in HR principles, labor laws, recruitment, and employee relations.</p>
                    </div>
                </div>
                
                <!-- Achievement 1 -->
                <div class="card">
                    <div class="card-header">
                        <h3>Employee Retention Award</h3>
                        <p>Professional Achievement</p>
                    </div>
                    <div class="card-body">
                        <p>Developed a candidate evaluation process that led to a <strong>15% increase</strong> in employee retention rates over a two-year period.</p>
                        <p>Implemented targeted engagement strategies and improved onboarding processes.</p>
                    </div>
                </div>
                
                <!-- Achievement 2 -->
                <div class="card">
                    <div class="card-header">
                        <h3>HR System Implementation</h3>
                        <p>Project Leadership</p>
                    </div>
                    <div class="card-body">
                        <p>Played a key role in the successful transition to an online performance management system, improving tracking and feedback processes.</p>
                        <p>Led training sessions and change management initiatives for smooth adoption.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact">
        <div class="container">
            <div class="section-title">
                <h2>Get In Touch</h2>
                <p>Let's discuss how I can contribute to your organization</p>
            </div>
            
            <div class="contact-container">
                <div class="contact-info">
                    <h3>Contact Information</h3>
                    <p>I'm available for HR consulting, strategic partnerships, and leadership opportunities. Feel free to reach out!</p>
                    
                    <div class="contact-item">
                        <div class="contact-icon">
                            <i class="fas fa-envelope"></i>
                        </div>
                        <div>
                            <h4>Email</h4>
                            <p>asudhander@gmail.com</p>
                        </div>
                    </div>
                    
                    <div class="contact-item">
                        <div class="contact-icon">
                            <i class="fas fa-phone"></i>
                        </div>
                        <div>
                            <h4>Phone</h4>
                            <p>+94 777 547 922</p>
                        </div>
                    </div>
                    
                    <div class="contact-item">
                        <div class="contact-icon">
                            <i class="fas fa-map-marker-alt"></i>
                        </div>
                        <div>
                            <h4>Location</h4>
                            <p>Negombo, Sri Lanka</p>
                            <p>Open to Remote & Global Opportunities</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div>
                    <h3>Sudhander Rajendran</h3>
                    <p>Strategic HR Business Partner</p>
                    <p>Specializing in people strategy, organizational development, and talent management</p>
                    
                    <div class="social-links">
                        <a href="mailto:asudhander@gmail.com" class="social-link">
                            <i class="fas fa-envelope"></i>
                        </a>
                        <a href="tel:+94777547922" class="social-link">
                            <i class="fas fa-phone"></i>
                        </a>
                        <a href="#" class="social-link">
                            <i class="fab fa-linkedin-in"></i>
                        </a>
                    </div>
                </div>
                
                <div class="footer-links">
                    <h4>Quick Links</h4>
                    <a href="#home">Home</a>
                    <a href="#about">About</a>
                    <a href="#experience">Experience</a>
                    <a href="#skills">Skills</a>
                    <a href="#education">Education</a>
                    <a href="#contact">Contact</a>
                </div>
                
                <div class="footer-links">
                    <h4>Expertise</h4>
                    <a href="#skills">HR Business Partnering</a>
                    <a href="#skills">Organizational Development</a>
                    <a href="#skills">Talent Management</a>
                    <a href="#skills">Employee Engagement</a>
                    <a href="#skills">Workforce Planning</a>
                </div>
            </div>
            
            <div class="copyright">
                <p>&copy; 2024 Sudhander Rajendran. All rights reserved.</p>
                <p>Designed as a professional portfolio for HR career showcase</p>
            </div>
        </div>
    </footer>

    <!-- JavaScript -->
    <script>
        // Mobile menu toggle
        const mobileMenuBtn = document.getElementById('mobileMenuBtn');
        const navLinks = document.getElementById('navLinks');
        
        mobileMenuBtn.addEventListener('click', () => {
            navLinks.classList.toggle('active');
            mobileMenuBtn.innerHTML = navLinks.classList.contains('active') 
                ? '<i class="fas fa-times"></i>' 
                : '<i class="fas fa-bars"></i>';
        });
        
        // Close mobile menu when clicking a link
        document.querySelectorAll('.nav-links a').forEach(link => {
            link.addEventListener('click', () => {
                navLinks.classList.remove('active');
                mobileMenuBtn.innerHTML = '<i class="fas fa-bars"></i>';
            });
        });
        
        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                
                const targetId = this.getAttribute('href');
                if(targetId === '#') return;
                
                const targetElement = document.querySelector(targetId);
                if(targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop - 80,
                        behavior: 'smooth'
                    });
                }
            });
        });
        
        // Add scroll effect to header
        window.addEventListener('scroll', () => {
            const header = document.querySelector('header');
            if(window.scrollY > 50) {
                header.style.boxShadow = '0 5px 15px rgba(0,0,0,0.1)';
            } else {
                header.style.boxShadow = '0 2px 10px rgba(0,0,0,0.1)';
            }
        });
    </script>
</body>
</html>
