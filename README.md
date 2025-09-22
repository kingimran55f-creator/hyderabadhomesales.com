# hyderabadhomesales.com
The official website for Hyderabad Home Sales, a modern real estate business helping clients buy, sell, and rent properties in Hyderabad.
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Hyderabad Home Sales - Your Trusted Real Estate Partner</title>
    <style>
        /* General Styles */
        :root {
            --primary-color: #0d1b2a; /* Dark Blue */
            --secondary-color: #fca311; /* Gold/Yellow */
            --light-color: #e5e5e5;
            --white-color: #ffffff;
        }

        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            color: var(--primary-color);
            background-color: var(--white-color);
            line-height: 1.6;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        a {
            text-decoration: none;
            color: var(--primary-color);
            font-weight: bold;
        }

        /* Header & Navigation */
        header {
            background-color: var(--white-color);
            padding: 20px 0;
            border-bottom: 2px solid var(--light-color);
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.8em;
            font-weight: bold;
            color: var(--primary-color);
        }

        .logo span {
            color: var(--secondary-color);
        }

        .nav-links a {
            margin-left: 25px;
            transition: color 0.3s;
        }

        .nav-links a:hover {
            color: var(--secondary-color);
        }

        /* Hero Section */
        .hero {
            background-color: var(--primary-color);
            color: var(--white-color);
            text-align: center;
            padding: 100px 20px;
        }

        .hero h1 {
            font-size: 3em;
            margin-bottom: 10px;
        }

        .hero p {
            font-size: 1.2em;
            max-width: 600px;
            margin: 0 auto 30px;
        }

        .cta-buttons a {
            background-color: var(--secondary-color);
            color: var(--primary-color);
            padding: 12px 25px;
            border-radius: 5px;
            margin: 0 10px;
            transition: background-color 0.3s;
            display: inline-block;
        }

        .cta-buttons a:hover {
            background-color: #ffb703;
        }

        /* Section Styles */
        .section {
            padding: 80px 0;
            text-align: center;
        }
        
        .section-light {
            background-color: var(--light-color);
        }

        .section-title {
            font-size: 2.5em;
            margin-bottom: 20px;
            color: var(--primary-color);
        }
        
        .section-subtitle {
            font-size: 1.2em;
            max-width: 700px;
            margin: 0 auto 40px;
        }

        /* About Us */
        .about-content {
            max-width: 800px;
            margin: 0 auto;
            font-size: 1.1em;
            text-align: left;
        }
        
        /* Services */
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-top: 40px;
        }

        .service-card {
            background-color: var(--white-color);
            padding: 30px;
            border-radius: 8px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
        }

        .service-card h3 {
            color: var(--secondary-color);
            margin-top: 0;
        }

        /* Featured Properties */
        .property-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 20px;
            margin-top: 40px;
        }

        .property-card {
            background-color: var(--white-color);
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
            text-align: left;
        }

        .property-card img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }

        .property-card-content {
            padding: 20px;
        }

        .property-card h4 {
            margin: 0 0 10px;
            color: var(--primary-color);
        }

        /* Contact Section */
        .contact-content {
            max-width: 800px;
            margin: 0 auto;
            text-align: center;
        }

        .contact-info {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 30px;
            margin-bottom: 40px;
        }

        .contact-item {
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        
        .contact-item .icon {
            font-size: 2em;
            color: var(--secondary-color);
            margin-bottom: 10px;
        }
        
        .contact-form {
            display: flex;
            flex-direction: column;
            gap: 20px;
            text-align: left;
        }
        
        .contact-form input, .contact-form textarea {
            width: 100%;
            padding: 12px;
            border: 1px solid var(--primary-color);
            border-radius: 5px;
            font-size: 1em;
        }
        
        .contact-form button {
            background-color: var(--secondary-color);
            color: var(--primary-color);
            border: none;
            padding: 15px;
            border-radius: 5px;
            font-size: 1.1em;
            cursor: pointer;
            transition: background-color 0.3s;
        }
        
        .contact-form button:hover {
            background-color: #ffb703;
        }

        /* Footer */
        footer {
            background-color: var(--primary-color);
            color: var(--light-color);
            padding: 40px 0;
            text-align: center;
        }

        .footer-content {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 20px;
        }

        .footer-logo {
            font-size: 1.5em;
            font-weight: bold;
            color: var(--white-color);
        }

        .footer-links a, .social-links a {
            color: var(--light-color);
            margin: 0 10px;
            transition: color 0.3s;
        }

        .footer-links a:hover, .social-links a:hover {
            color: var(--secondary-color);
        }
        
        /* Mobile adjustments */
        @media (max-width: 768px) {
            .nav-links {
                display: none;
            }
            .hero h1 {
                font-size: 2em;
            }
            .cta-buttons a {
                display: block;
                margin: 10px 0;
            }
        }
    </style>
</head>
<body>

    <header>
        <div class="container">
            <nav>
                <div class="logo">Hyderabad <span>Home Sales</span></div>
                <div class="nav-links">
                    <a href="#about">About</a>
                    <a href="#services">Services</a>
                    <a href="#properties">Properties</a>
                    <a href="#contact">Contact</a>
                </div>
            </nav>
        </div>
    </header>

    <main>
        <section class="hero">
            <div class="container">
                <h1>Helping you find the perfect home in Hyderabad!</h1>
                <p>Your trusted partner for property buying, selling, and rentals.</p>
                <div class="cta-buttons">
                    <a href="#contact">Buy a Home</a>
                    <a href="#contact">Sell a Home</a>
                    <a href="#contact">Rent a Home</a>
                </div>
            </div>
        </section>

        <section id="about" class="section">
            <div class="container">
                <h2 class="section-title">About Us</h2>
                <div class="about-content">
                    <p>At Hyderabad Home Sales, we believe finding a home should be simple and stress-free.</p>
                    <p>Whether you’re buying your first home, selling your property, or looking for a rental, our team ensures a smooth and transparent process.</p>
                    <p>With our local expertise in Hyderabad’s real estate market, we help you make the best property decisions with confidence.</p>
                </div>
            </div>
        </section>

        <section id="services" class="section section-light">
            <div class="container">
                <h2 class="section-title">Our Services</h2>
                <p class="section-subtitle">We offer comprehensive real estate solutions tailored to your needs.</p>
                <div class="services-grid">
                    <div class="service-card">
                        <h3>🏡 Property Buying</h3>
                        <p>Find your dream home in Hyderabad with verified listings and expert support.</p>
                    </div>
                    <div class="service-card">
                        <h3>🏠 Property Selling</h3>
                        <p>Get the right buyers quickly and sell your property at the best value.</p>
                    </div>
                    <div class="service-card">
                        <h3>🏢 Rental Services</h3>
                        <p>From apartments to independent houses, we make renting hassle-free.</p>
                    </div>
                </div>
            </div>
        </section>

        <section id="properties" class="section">
            <div class="container">
                <h2 class="section-title">Featured Properties</h2>
                <p class="section-subtitle">A glimpse of the homes we have for sale or rent in Hyderabad.</p>
                <div class="property-grid">
                    <div class="property-card">
                        <img src="https://via.placeholder.com/400x250" alt="Luxury 3BHK Apartment">
                        <div class="property-card-content">
                            <h4>Luxury 3BHK Apartment – Gachibowli</h4>
                        </div>
                    </div>
                    <div class="property-card">
                        <img src="https://via.placeholder.com/400x250" alt="Affordable 2BHK Flat">
                        <div class="property-card-content">
                            <h4>Affordable 2BHK Flat – Kukatpally</h4>
                        </div>
                    </div>
                    <div class="property-card">
                        <img src="https://via.placeholder.com/400x250" alt="Spacious Villa">
                        <div class="property-card-content">
                            <h4>Spacious Villa – Shamshabad</h4>
                        </div>
                    </div>
                    <div class="property-card">
                        <img src="https://via.placeholder.com/400x250" alt="Commercial Office Space">
                        <div class="property-card-content">
                            <h4>Commercial Office Space – Hitech City</h4>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <section id="contact" class="section section-light">
            <div class="container">
                <h2 class="section-title">Contact Us</h2>
                <div class="contact-content">
                    <p>We're here to help you with all your real estate needs. Get in touch today!</p>
                    <div class="contact-info">
                        <div class="contact-item">
                            <span class="icon">📞</span>
                            <p><strong>Call/WhatsApp:</strong> +91 7013873980</p>
                        </div>
                        <div class="contact-item">
                            <span class="icon">📧</span>
                            <p><strong>Email:</strong> imransiddiqi511@gmail.com</p>
                        </div>
                    </div>
                    
                    <form class="contact-form">
                        <input type="text" name="name" placeholder="Full Name" required>
                        <input type="email" name="email" placeholder="Email Address" required>
                        <input type="tel" name="phone" placeholder="Phone Number" required>
                        <textarea name="message" rows="5" placeholder="Your Message" required></textarea>
                        <button type="submit">Send Message</button>
                    </form>
                </div>
            </div>
        </section>

    </main>

    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-logo">Hyderabad Home Sales</div>
                <p>Trusted Real Estate Solutions in Hyderabad</p>
                <div class="footer-links">
                    <a href="#about">About</a> | 
                    <a href="#services">Services</a> | 
                    <a href="#properties">Properties</a> | 
                    <a href="#contact">Contact</a>
                </div>
                <div class="social-links">
                    <a href="https://www.facebook.com/profile.php?id=61564985129950" target="_blank">🌐 Facebook</a> | 
                    <a href="https://www.instagram.com/hyderabadhomes_sales/" target="_blank">📷 Instagram</a>
                </div>
                <p>&copy; 2024 Hyderabad Home Sales. All rights reserved.</p>
            </div>
        </div>
    </footer>

</body>
</html>
