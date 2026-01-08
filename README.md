<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AB ARNOB - Social Media Marketing Agency</title>
    <style>
        /* Reset and Base Styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            color: #333;
            background-color: #f4f4f4;
        }
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        /* Header */
        header {
            background-color: #fff;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 100;
        }
        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 1rem 0;
        }
        .logo {
            font-size: 1.5rem;
            font-weight: bold;
            color: #007bff;
        }
        nav ul {
            list-style: none;
            display: flex;
        }
        nav ul li {
            margin-left: 2rem;
        }
        nav ul li a {
            text-decoration: none;
            color: #333;
            transition: color 0.3s;
        }
        nav ul li a:hover {
            color: #007bff;
        }
        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: #fff;
            padding: 150px 0 100px;
            text-align: center;
            animation: fadeIn 1s ease-in;
        }
        .hero h1 {
            font-size: 3rem;
            margin-bottom: 1rem;
        }
        .hero p {
            font-size: 1.2rem;
            margin-bottom: 2rem;
        }
        .cta-btn {
            background-color: #fff;
            color: #007bff;
            padding: 1rem 2rem;
            text-decoration: none;
            border-radius: 5px;
            font-weight: bold;
            transition: background-color 0.3s, color 0.3s;
        }
        .cta-btn:hover {
            background-color: #007bff;
            color: #fff;
        }
        /* Services */
        .services {
            padding: 80px 0;
            background-color: #fff;
        }
        .services h2 {
            text-align: center;
            margin-bottom: 3rem;
            font-size: 2.5rem;
            color: #333;
        }
        .service-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }
        .service-item {
            background-color: #f9f9f9;
            padding: 2rem;
            border-radius: 10px;
            text-align: center;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: transform 0.3s;
        }
        .service-item:hover {
            transform: translateY(-10px);
        }
        .service-item h3 {
            margin-bottom: 1rem;
            color: #007bff;
        }
        /* Pricing */
        .pricing {
            padding: 80px 0;
            background-color: #f4f4f4;
        }
        .pricing h2 {
            text-align: center;
            margin-bottom: 3rem;
            font-size: 2.5rem;
            color: #333;
        }
        .pricing-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
        }
        .pricing-item {
            background-color: #fff;
            padding: 2rem;
            border-radius: 10px;
            text-align: center;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: transform 0.3s;
        }
        .pricing-item:hover {
            transform: translateY(-10px);
        }
        .pricing-item h3 {
            margin-bottom: 1rem;
            color: #007bff;
        }
        .pricing-item ul {
            list-style: none;
            margin-bottom: 2rem;
        }
        .pricing-item ul li {
            margin-bottom: 0.5rem;
        }
        .price {
            font-size: 2rem;
            font-weight: bold;
            color: #333;
            margin-bottom: 1rem;
        }
        /* Testimonials */
        .testimonials {
            padding: 80px 0;
            background-color: #fff;
        }
        .testimonials h2 {
            text-align: center;
            margin-bottom: 3rem;
            font-size: 2.5rem;
            color: #333;
        }
        .testimonial-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
        }
        .testimonial-item {
            background-color: #f9f9f9;
            padding: 2rem;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: transform 0.3s;
        }
        .testimonial-item:hover {
            transform: translateY(-10px);
        }
        .testimonial-item p {
            font-style: italic;
            margin-bottom: 1rem;
        }
        .testimonial-item cite {
            font-weight: bold;
            color: #007bff;
        }
        /* Contact */
        .contact {
            padding: 80px 0;
            background-color: #f4f4f4;
        }
        .contact h2 {
            text-align: center;
            margin-bottom: 3rem;
            font-size: 2.5rem;
            color: #333;
        }
        .contact-form {
            max-width: 600px;
            margin: 0 auto;
            background-color: #fff;
            padding: 2rem;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }
        .contact-form input,
        .contact-form textarea {
            width: 100%;
            padding: 1rem;
            margin-bottom: 1rem;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 1rem;
        }
        .contact-form button {
            width: 100%;
            padding: 1rem;
            background-color: #007bff;
            color: #fff;
            border: none;
            border-radius: 5px;
            font-size: 1rem;
            cursor: pointer;
            transition: background-color 0.3s;
        }
        .contact-form button:hover {
            background-color: #0056b3;
        }
        /* Footer */
        footer {
            background-color: #333;
            color: #fff;
            text-align: center;
            padding: 2rem 0;
        }
        /* Animations */
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        .fade-in {
            animation: fadeIn 1s ease-in;
        }
        /* Responsive Design */
        @media (max-width: 768px) {
            .hero h1 {
                font-size: 2rem;
            }
            .hero p {
                font-size: 1rem;
            }
            nav ul {
                display: none; /* Simple hide for mobile; could add hamburger menu */
            }
            .service-grid, .pricing-grid, .testimonial-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <header>
        <nav class="container">
            <div class="logo">AB ARNOB</div>
            <ul>
                <li><a href="#services">Services</a></li>
                <li><a href="#pricing">Pricing</a></li>
                <li><a href="#testimonials">Testimonials</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section class="hero">
        <div class="container">
            <h1>Boost Your Brand with AB ARNOB</h1>
            <p>Expert social media marketing for Facebook, Instagram, and YouTube to grow your audience and engagement.</p>
            <a href="#contact" class="cta-btn">Get Started Today</a>
        </div>
    </section>

    <section id="services" class="services">
        <div class="container">
            <h2>Our Services</h2>
            <div class="service-grid">
                <div class="service-item fade-in">
                    <h3>Facebook Marketing</h3>
                    <p>Targeted ads, content creation, and community management to increase likes, shares, and conversions on Facebook.</p>
                </div>
                <div class="service-item fade-in">
                    <h3>Instagram Marketing</h3>
                    <p>Stunning visuals, influencer collaborations, and stories to build a loyal following and drive sales on Instagram.</p>
                </div>
                <div class="service-item fade-in">
                    <h3>YouTube Marketing</h3>
                    <p>Video production, SEO optimization, and channel growth strategies to maximize views and subscribers on YouTube.</p>
                </div>
            </div>
        </div>
    </section>

    <section id="pricing" class="pricing">
        <div class="container">
            <h2>Pricing Plans</h2>
            <div class="pricing-grid">
                <div class="pricing-item fade-in">
                    <h3>Basic</h3>
                    <div class="price">$299/month</div>
                    <ul>
                        <li>1 Social Platform</li>
                        <li>5 Posts per Week</li>
                        <li>Basic Analytics</li>
                        <li>Email Support</li>
                    </ul>
                </div>
                <div class="pricing-item fade-in">
                    <h3>Pro</h3>
                    <div class="price">$599/month</div>
                    <ul>
                        <li>2 Social Platforms</li>
                        <li>10 Posts per Week</li>
                        <li>Advanced Analytics</li>
                        <li>Phone Support</li>
                    </ul>
                </div>
                <div class="pricing-item fade-in">
                    <h3>Premium</h3>
                    <div class="price">$999/month</div>
                    <ul>
                        <li>All Platforms</li>
                        <li>Unlimited Posts</li>
                        <li>Custom Strategies</li>
                        <li>24/7 Support</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <section id="testimonials" class="testimonials">
        <div class="container">
            <h2>Client Testimonials</h2>
            <div class="testimonial-grid">
                <div class="testimonial-item fade-in">
                    <p>"AB ARNOB transformed our Instagram presence. Our engagement skyrocketed!"</p>
                    <cite>- Jane Doe, Fashion Brand</cite>
                </div>
                <div class="testimonial-item fade-in">
                    <p>"Their Facebook campaigns brought in 300% more leads. Highly recommend!"</p>
                    <cite>- John Smith, Tech Startup</cite>
                </div>
                <div class="testimonial-item fade-in">
                    <p>"YouTube growth was incredible. We gained 10k subscribers in months."</p>
                    <cite>- Emily Johnson, Content Creator</cite>
                </div>
            </div>
        </div>
    </section>

    <section id="contact" class="contact">
        <div class="container">
            <h2>Contact Us</h2>
            <form class="contact-form">
                <input type="text" placeholder="Your Name" required>
                <input type="email" placeholder="Your Email" required>
                <textarea placeholder="Your Message" rows="5" required></textarea>
                <button type="submit">Send Message</button>
            </form>
        </div>
    </section>

    <footer>
        <div class="container">
            <p>&copy; 2023 AB ARNOB. All rights reserved.</p>
        </div>
    </footer>

    <script>
        // Simple scroll animation trigger
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('fade-in');
                }
            });
        });

        document.querySelectorAll('.service-item, .pricing-item, .testimonial-item').forEach(item => {
            observer.observe(item);
        });
    </script>
</body>
</html># Ab-arnob-websits
