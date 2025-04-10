<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rx Marketing Solution | Specialized Marketing for Pharmacies</title>
    <style>
        :root {
            --primary-color: #000000;
            --secondary-color: #ffffff;
            --accent-color: #f0f0f0;
            --text-color: #333333;
            --section-padding: 80px 0;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            line-height: 1.6;
            color: var(--text-color);
            overflow-x: hidden;
        }
        
        a {
            text-decoration: none;
            color: inherit;
        }
        
        ul {
            list-style: none;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* Header Styles */
        header {
            background-color: var(--primary-color);
            color: var(--secondary-color);
            position: fixed;
            width: 100%;
            z-index: 1000;
            padding: 15px 0;
            transition: 0.3s ease;
        }
        
        .header-container {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            display: flex;
            align-items: center;
            font-weight: 700;
        }
        
        .logo img {
            height: 40px;
            margin-right: 10px;
        }
        
        .nav-links {
            display: flex;
        }
        
        .nav-links li {
            margin-left: 30px;
        }
        
        .nav-links a {
            font-weight: 500;
            transition: 0.3s ease;
        }
        
        .nav-links a:hover {
            opacity: 0.8;
        }
        
        .hamburger {
            display: none;
            cursor: pointer;
        }
        
        .hamburger div {
            width: 25px;
            height: 3px;
            background-color: var(--secondary-color);
            margin: 5px;
            transition: 0.3s ease;
        }
        
        /* Hero Section */
        .hero {
            background-color: var(--primary-color);
            color: var(--secondary-color);
            height: 100vh;
            display: flex;
            align-items: center;
            position: relative;
            overflow: hidden;
        }
        
        .hero-content {
            position: relative;
            z-index: 1;
            max-width: 600px;
        }
        
        .hero h1 {
            font-size: 48px;
            margin-bottom: 20px;
            line-height: 1.2;
        }
        
        .hero p {
            font-size: 18px;
            margin-bottom: 30px;
            opacity: 0.9;
        }
        
        .cta-button {
            display: inline-block;
            background-color: var(--secondary-color);
            color: var(--primary-color);
            padding: 12px 30px;
            border-radius: 30px;
            font-weight: 600;
            text-transform: uppercase;
            letter-spacing: 1px;
            transition: 0.3s ease;
        }
        
        .cta-button:hover {
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }
        
        .hero-shape {
            position: absolute;
            right: 0;
            top: 0;
            width: 40%;
            height: 100%;
            background-color: var(--accent-color);
            border-radius: 0 0 0 300px;
        }
        
        /* About Section */
        .about {
            padding: var(--section-padding);
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 60px;
        }
        
        .section-title h2 {
            font-size: 36px;
            margin-bottom: 15px;
            position: relative;
            display: inline-block;
        }
        
        .section-title h2:after {
            content: '';
            position: absolute;
            left: 50%;
            bottom: -10px;
            transform: translateX(-50%);
            width: 60px;
            height: 3px;
            background-color: var(--primary-color);
        }
        
        .about-content {
            display: flex;
            align-items: center;
            gap: 50px;
        }
        
        .about-image {
            flex: 1;
        }
        
        .about-image img {
            width: 100%;
            border-radius: 10px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.1);
        }
        
        .about-text {
            flex: 1;
        }
        
        .about-text h3 {
            font-size: 28px;
            margin-bottom: 20px;
        }
        
        .about-text p {
            margin-bottom: 15px;
            color: #666;
        }
        
        /* Services Section */
        .services {
            padding: var(--section-padding);
            background-color: var(--accent-color);
        }
        
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .service-card {
            background-color: var(--secondary-color);
            border-radius: 10px;
            padding: 30px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            transition: 0.3s ease;
        }
        
        .service-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.1);
        }
        
        .service-icon {
            font-size: 40px;
            margin-bottom: 20px;
            color: var(--primary-color);
        }
        
        .service-card h3 {
            font-size: 22px;
            margin-bottom: 15px;
        }
        
        .service-card p {
            color: #666;
        }
        
        /* Clients Section */
        .clients {
            padding: var(--section-padding);
        }
        
        .client-logos {
            display: flex;
            justify-content: space-around;
            align-items: center;
            flex-wrap: wrap;
            gap: 40px;
        }
        
        .client-logo {
            max-width: 150px;
            filter: grayscale(100%);
            opacity: 0.7;
            transition: 0.3s ease;
        }
        
        .client-logo:hover {
            filter: grayscale(0);
            opacity: 1;
        }
        
        /* Testimonials Section */
        .testimonials {
            padding: var(--section-padding);
            background-color: var(--accent-color);
        }
        
        .testimonial-slider {
            max-width: 700px;
            margin: 0 auto;
            text-align: center;
        }
        
        .testimonial {
            padding: 30px;
        }
        
        .testimonial-text {
            font-size: 18px;
            font-style: italic;
            margin-bottom: 20px;
        }
        
        .testimonial-author {
            font-weight: 600;
            color: var(--primary-color);
        }
        
        .testimonial-position {
            font-size: 14px;
            color: #666;
        }
        
        /* Contact Section */
        .contact {
            padding: var(--section-padding);
        }
        
        .contact-content {
            display: flex;
            gap: 50px;
        }
        
        .contact-info {
            flex: 1;
        }
        
        .contact-info h3 {
            font-size: 24px;
            margin-bottom: 20px;
        }
        
        .contact-detail {
            display: flex;
            align-items: center;
            margin-bottom: 15px;
        }
        
        .contact-icon {
            margin-right: 15px;
            font-size: 20px;
            color: var(--primary-color);
        }
        
        .contact-form {
            flex: 1;
        }
        
        .form-group {
            margin-bottom: 20px;
        }
        
        .form-control {
            width: 100%;
            padding: 12px 15px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 16px;
            transition: 0.3s ease;
        }
        
        .form-control:focus {
            border-color: var(--primary-color);
            outline: none;
        }
        
        textarea.form-control {
            min-height: 150px;
        }
        
        .submit-button {
            background-color: var(--primary-color);
            color: var(--secondary-color);
            border: none;
            padding: 12px 30px;
            border-radius: 30px;
            font-size: 16px;
            font-weight: 600;
            cursor: pointer;
            transition: 0.3s ease;
        }
        
        .submit-button:hover {
            opacity: 0.9;
        }
        
        /* Footer */
        footer {
            background-color: var(--primary-color);
            color: var(--secondary-color);
            padding: 50px 0 20px;
        }
        
        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 40px;
            margin-bottom: 30px;
        }
        
        .footer-logo {
            font-size: 24px;
            font-weight: 700;
            margin-bottom: 15px;
        }
        
        .footer-description {
            margin-bottom: 20px;
            opacity: 0.8;
        }
        
        .social-links {
            display: flex;
            gap: 15px;
        }
        
        .social-icon {
            width: 36px;
            height: 36px;
            background-color: rgba(255, 255, 255, 0.1);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: 0.3s ease;
        }
        
        .social-icon:hover {
            background-color: rgba(255, 255, 255, 0.2);
        }
        
        .footer-title {
            font-size: 18px;
            margin-bottom: 20px;
            position: relative;
        }
        
        .footer-title:after {
            content: '';
            position: absolute;
            left: 0;
            bottom: -8px;
            width: 40px;
            height: 2px;
            background-color: var(--secondary-color);
        }
        
        .footer-links li {
            margin-bottom: 10px;
            opacity: 0.8;
            transition: 0.3s ease;
        }
        
        .footer-links li:hover {
            opacity: 1;
            padding-left: 5px;
        }
        
        .copyright {
            text-align: center;
            padding-top: 20px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            font-size: 14px;
            opacity: 0.8;
        }
        
        /* Responsive Design */
        @media screen and (max-width: 992px) {
            .about-content {
                flex-direction: column;
            }
            
            .contact-content {
                flex-direction: column;
            }
        }
        
        @media screen and (max-width: 768px) {
            .nav-links {
                position: absolute;
                right: 0;
                top: 70px;
                background-color: var(--primary-color);
                flex-direction: column;
                width: 100%;
                text-align: center;
                transform: translateX(100%);
                transition: 0.3s ease;
                padding: 20px 0;
                box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
            }
            
            .nav-links.active {
                transform: translateX(0);
            }
            
            .nav-links li {
                margin: 15px 0;
            }
            
            .hamburger {
                display: block;
            }
            
            .hero h1 {
                font-size: 36px;
            }
            
            .hero-shape {
                display: none;
            }
        }
    </style>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container header-container">
            <div class="logo">
                <img src="/api/placeholder/80/40" alt="Rx Marketing Solution Logo">
                <span>Rx Marketing Solution</span>
            </div>
            <ul class="nav-links">
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About Us</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#clients">Clients</a></li>
                <li><a href="#testimonials">Testimonials</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
            <div class="hamburger">
                <div class="line1"></div>
                <div class="line2"></div>
                <div class="line3"></div>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero" id="home">
        <div class="container">
            <div class="hero-content">
                <h1>Specialized Marketing Solutions for Pharmacies</h1>
                <p>We help pharmaceutical businesses grow their customer base, increase sales, and build a strong digital presence through strategic marketing campaigns.</p>
                <a href="#contact" class="cta-button">Get Started</a>
            </div>
        </div>
        <div class="hero-shape"></div>
    </section>

    <!-- About Section -->
    <section class="about" id="about">
        <div class="container">
            <div class="section-title">
                <h2>About Us</h2>
                <p>Learn more about our agency and mission</p>
            </div>
            <div class="about-content">
                <div class="about-image">
                    <img src="/api/placeholder/600/400" alt="About Rx Marketing Solution">
                </div>
                <div class="about-text">
                    <h3>Your Pharmacy Marketing Partner</h3>
                    <p>Rx Marketing Solution was founded with a clear mission: to provide specialized marketing services exclusively for pharmaceutical businesses. With our deep understanding of the healthcare industry and marketing expertise, we help pharmacies thrive in a competitive market.</p>
                    <p>Our team consists of healthcare marketing specialists who understand the unique challenges and regulations in the pharmaceutical industry. We develop customized strategies that drive tangible results while maintaining compliance with industry standards.</p>
                    <p>From digital presence to customer loyalty programs, we offer end-to-end marketing solutions that help pharmacies connect with their communities and build lasting relationships with patients.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section class="services" id="services">
        <div class="container">
            <div class="section-title">
                <h2>Our Services</h2>
                <p>Comprehensive marketing solutions for your pharmacy</p>
            </div>
            <div class="services-grid">
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-globe"></i>
                    </div>
                    <h3>Digital Presence Management</h3>
                    <p>We develop and optimize your pharmacy's website, social media profiles, and online listings to ensure patients can find you when they need you most.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-bullhorn"></i>
                    </div>
                    <h3>Pharmacy Advertising</h3>
                    <p>Our targeted advertising campaigns help you reach potential patients in your community through digital channels, print media, and local outreach.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-chart-line"></i>
                    </div>
                    <h3>Marketing Analytics</h3>
                    <p>We provide detailed insights into your marketing performance, customer behavior, and ROI to continuously improve your marketing strategy.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-envelope"></i>
                    </div>
                    <h3>Patient Communication</h3>
                    <p>Develop effective email marketing, SMS reminders, and loyalty programs to keep your patients engaged and coming back to your pharmacy.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-search"></i>
                    </div>
                    <h3>SEO for Pharmacies</h3>
                    <p>Improve your pharmacy's visibility in local searches with our specialized SEO strategies designed for the healthcare industry.</p>
                </div>
                <div class="service-card">
                    <div class="service-icon">
                        <i class="fas fa-handshake"></i>
                    </div>
                    <h3>Community Outreach</h3>
                    <p>We help you build strong relationships within your community through health awareness programs, events, and partnerships.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Clients Section -->
    <section class="clients" id="clients">
        <div class="container">
            <div class="section-title">
                <h2>Our Clients</h2>
                <p>Trusted by pharmacies across the region</p>
            </div>
            <div class="client-logos">
                <img src="/api/placeholder/150/80" alt="Client Logo" class="client-logo">
                <img src="/api/placeholder/150/80" alt="Client Logo" class="client-logo">
                <img src="/api/placeholder/150/80" alt="Client Logo" class="client-logo">
                <img src="/api/placeholder/150/80" alt="Client Logo" class="client-logo">
                <img src="/api/placeholder/150/80" alt="Client Logo" class="client-logo">
            </div>
        </div>
    </section>

    <!-- Testimonials Section -->
    <section class="testimonials" id="testimonials">
        <div class="container">
            <div class="section-title">
                <h2>Testimonials</h2>
                <p>What our clients say about our services</p>
            </div>
            <div class="testimonial-slider">
                <div class="testimonial">
                    <p class="testimonial-text">"Rx Marketing Solution transformed our pharmacy's digital presence. Our website traffic has increased by 150% and we've seen a significant boost in new customers since working with them."</p>
                    <p class="testimonial-author">Dr. Sarah Johnson</p>
                    <p class="testimonial-position">Owner, Community Care Pharmacy</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section class="contact" id="contact">
        <div class="container">
            <div class="section-title">
                <h2>Contact Us</h2>
                <p>Get in touch for a free consultation</p>
            </div>
            <div class="contact-content">
                <div class="contact-info">
                    <h3>Let's Discuss Your Pharmacy's Marketing Needs</h3>
                    <div class="contact-detail">
                        <div class="contact-icon">
                            <i class="fas fa-map-marker-alt"></i>
                        </div>
                        <p>123 Marketing Ave, Suite 101<br>Business District, NY 10001</p>
                    </div>
                    <div class="contact-detail">
                        <div class="contact-icon">
                            <i class="fas fa-phone"></i>
                        </div>
                        <p>+1 (555) 123-4567</p>
                    </div>
                    <div class="contact-detail">
                        <div class="contact-icon">
                            <i class="fas fa-envelope"></i>
                        </div>
                        <p>info@rxmarketingsolution.com</p>
                    </div>
                    <div class="contact-detail">
                        <div class="contact-icon">
                            <i class="fas fa-clock"></i>
                        </div>
                        <p>Monday - Friday: 9:00 AM - 6:00 PM</p>
                    </div>
                </div>
                <div class="contact-form">
                    <form>
                        <div class="form-group">
                            <input type="text" class="form-control" placeholder="Your Name">
                        </div>
                        <div class="form-group">
                            <input type="email" class="form-control" placeholder="Your Email">
                        </div>
                        <div class="form-group">
                            <input type="text" class="form-control" placeholder="Subject">
                        </div>
                        <div class="form-group">
                            <textarea class="form-control" placeholder="Your Message"></textarea>
                        </div>
                        <button type="submit" class="submit-button">Send Message</button>
                    </form>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div>
                    <div class="footer-logo">Rx Marketing Solution</div>
                    <p class="footer-description">Specialized marketing services for pharmaceutical businesses.</p>
                    <div class="social-links">
                        <a href="https://www.facebook.com/rxmarketingsolution" class="social-icon"><i class="fab fa-facebook-f"></i></a>
                        <a href="#" class="social-icon"><i class="fab fa-twitter"></i></a>
                        <a href="#" class="social-icon"><i class="fab fa-linkedin-in"></i></a>
                        <a href="#" class="social-icon"><i class="fab fa-instagram"></i></a>
                    </div>
                </div>
                <div>
                    <h3 class="footer-title">Quick Links</h3>
                    <ul class="footer-links">
                        <li><a href="#home">Home</a></li>
                        <li><a href="#about">About Us</a></li>
                        <li><a href="#services">Services</a></li>
                        <li><a href="#clients">Clients</a></li>
                        <li><a href="#testimonials">Testimonials</a></li>
                    </ul>
                </div>
                <div>
                    <h3 class="footer-title">Services</h3>
                    <ul class="footer-links">
                        <li><a href="#services">Digital Presence</a></li>
                        <li><a href="#services">Pharmacy Advertising</a></li>
                        <li><a href="#services">Marketing Analytics</a></li>
                        <li><a href="#services">Patient Communication</a></li>
                        <li><a href="#services">SEO for Pharmacies</a></li>
                    </ul>
                </div>
                <div>
                    <h3 class="footer-title">Newsletter</h3>
                    <p>Subscribe to our newsletter for the latest updates.</p>
                    <form class="footer-form">
                        <input type="email" class="form-control" placeholder="Your Email" style="margin-bottom: 10px;">
                        <button type="submit" class="submit-button">Subscribe</button>
                    </form>
                </div>
            </div>
            <div class="copyright">
                <p>&copy; 2025 Rx Marketing Solution. All Rights Reserved.</p>
            </div>
        </div>
    </footer>

    <script>
        // JavaScript for Toggle Menu
        const hamburger = document.querySelector('.hamburger');
        const navLinks = document.querySelector('.nav-links');
        
        hamburger.addEventListener('click', () => {
            navLinks.classList.toggle('active');
        });
        
        // JavaScript for Smooth Scrolling
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
                
                if (navLinks.classList.contains('active')) {
                    navLinks.classList.remove('active');
                }
            });
        });
        
        // JavaScript for Sticky Header
        window.addEventListener('scroll', function() {
            const header = document.querySelector('header');
            header.classList.toggle('sticky', window.scrollY > 0);
        });
    </script>
</body>
</html>
