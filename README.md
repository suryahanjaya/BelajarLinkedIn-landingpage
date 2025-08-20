<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>LinkedIn Learning Landing Page - Documentation</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --primary: #0A66C2;
            --primary-dark: #004182;
            --secondary: #FF9D34;
            --dark: #1D1D1D;
            --light: #FFFFFF;
            --gray: #666666;
            --light-gray: #F5F5F5;
            --transition: all 0.3s ease;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: #f8f9fa;
            color: #333;
            line-height: 1.6;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        
        header {
            background: linear-gradient(135deg, var(--primary) 0%, var(--primary-dark) 100%);
            color: white;
            padding: 60px 20px;
            text-align: center;
            border-radius: 0 0 20px 20px;
            margin-bottom: 40px;
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.1);
        }
        
        header h1 {
            font-size: 2.8rem;
            margin-bottom: 15px;
        }
        
        header p {
            font-size: 1.2rem;
            max-width: 800px;
            margin: 0 auto;
            opacity: 0.9;
        }
        
        .logo {
            font-size: 3rem;
            margin-bottom: 20px;
            color: white;
        }
        
        .section {
            background-color: white;
            border-radius: 15px;
            padding: 30px;
            margin-bottom: 30px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            transition: var(--transition);
        }
        
        .section:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.1);
        }
        
        .section h2 {
            color: var(--primary);
            margin-bottom: 20px;
            padding-bottom: 10px;
            border-bottom: 3px solid var(--secondary);
            display: inline-block;
        }
        
        .tech-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }
        
        .tech-card {
            background: linear-gradient(135deg, #f8faff 0%, #ffffff 100%);
            padding: 20px;
            border-radius: 10px;
            text-align: center;
            transition: var(--transition);
            border: 1px solid #eaeaea;
        }
        
        .tech-card:hover {
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(10, 102, 194, 0.15);
        }
        
        .tech-icon {
            font-size: 2.5rem;
            color: var(--primary);
            margin-bottom: 15px;
        }
        
        .steps {
            margin-left: 20px;
            margin-top: 15px;
        }
        
        .steps li {
            margin-bottom: 10px;
        }
        
        .demo-card {
            text-align: center;
            padding: 40px;
            background: linear-gradient(135deg, #f0f7ff 0%, #e4eeff 100%);
            border-radius: 15px;
            margin-top: 20px;
        }
        
        .demo-btn {
            display: inline-block;
            background: linear-gradient(to right, var(--primary), var(--primary-dark));
            color: white;
            padding: 15px 35px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 600;
            margin-top: 20px;
            transition: var(--transition);
            box-shadow: 0 5px 15px rgba(10, 102, 194, 0.3);
        }
        
        .demo-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 20px rgba(10, 102, 194, 0.4);
        }
        
        .features {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }
        
        .feature {
            background-color: var(--light-gray);
            padding: 20px;
            border-radius: 10px;
            border-left: 4px solid var(--primary);
        }
        
        footer {
            text-align: center;
            margin-top: 50px;
            padding: 20px;
            color: var(--gray);
        }
        
        @media (max-width: 768px) {
            .tech-grid, .features {
                grid-template-columns: 1fr;
            }
            
            header h1 {
                font-size: 2.2rem;
            }
        }
        
        .code-block {
            background-color: #2d2d2d;
            color: #f8f8f2;
            padding: 15px;
            border-radius: 8px;
            margin: 15px 0;
            overflow-x: auto;
            font-family: 'Courier New', monospace;
        }
        
        .tag {
            display: inline-block;
            background-color: var(--primary-light);
            color: var(--primary-dark);
            padding: 5px 10px;
            border-radius: 20px;
            font-size: 0.9rem;
            margin: 5px 5px 5px 0;
        }
    </style>
</head>
<body>
    <header>
        <div class="logo">
            <i class="fab fa-linkedin"></i>
        </div>
        <h1>LinkedIn Learning Landing Page</h1>
        <p>A responsive, interactive landing page designed to promote LinkedIn learning courses with modern UI/UX design principles</p>
    </header>
    
    <div class="container">
        <section class="section">
            <h2>Project Overview</h2>
            <p>This project is a modern, responsive landing page for a LinkedIn learning course titled "Mastering LinkedIn for Career Growth". The page is designed to convert visitors into course participants through compelling design, clear value proposition, and user-friendly interface.</p>
            
            <p>The landing page includes sections for course benefits, testimonials, FAQs, registration form, and feedback collection. It also features dark mode functionality and is fully optimized for all device sizes.</p>
        </section>
        
        <section class="section">
            <h2>Technologies Used</h2>
            <div class="tech-grid">
                <div class="tech-card">
                    <div class="tech-icon">
                        <i class="fab fa-html5"></i>
                    </div>
                    <h3>HTML5</h3>
                    <p>Semantic markup for structure and content</p>
                </div>
                
                <div class="tech-card">
                    <div class="tech-icon">
                        <i class="fab fa-css3-alt"></i>
                    </div>
                    <h3>CSS3</h3>
                    <p>Modern styling with Flexbox, Grid, and animations</p>
                </div>
                
                <div class="tech-card">
                    <div class="tech-icon">
                        <i class="fab fa-js"></i>
                    </div>
                    <h3>JavaScript</h3>
                    <p>Interactive elements and dynamic functionality</p>
                </div>
                
                <div class="tech-card">
                    <div class="tech-icon">
                        <i class="fab fa-font-awesome"></i>
                    </div>
                    <h3>Font Awesome</h3>
                    <p>Icons for improved visual communication</p>
                </div>
                
                <div class="tech-card">
                    <div class="tech-icon">
                        <i class="fas fa-font"></i>
                    </div>
                    <h3>Google Fonts</h3>
                    <p>Typography using Plus Jakarta Sans and Outfit</p>
                </div>
                
                <div class="tech-card">
                    <div class="tech-icon">
                        <i class="fas fa-mobile-alt"></i>
                    </div>
                    <h3>Responsive Design</h3>
                    <p>Fully adaptive layout for all screen sizes</p>
                </div>
            </div>
        </section>
        
        <section class="section">
            <h2>How to Run the Project</h2>
            <p>To run this project locally, follow these steps:</p>
            
            <ol class="steps">
                <li><strong>Download the project files</strong> - Save the HTML file and any associated resources to your local machine</li>
                
                <li><strong>Open the HTML file</strong> - Simply double-click the HTML file to open it in your default web browser</li>
                
                <li><strong>Use a local server (optional)</strong> - For full functionality, you may want to use a local server:
                    <div class="code-block">
                        # Using Python 3<br>
                        python -m http.server 8000
                    </div>
                    
                    <div class="code-block">
                        # Using Node.js and http-server<br>
                        npx http-server
                    </div>
                    
                    <div class="code-block">
                        # Using PHP<br>
                        php -S localhost:8000
                    </div>
                </li>
                
                <li><strong>View in browser</strong> - Navigate to http://localhost:8000 (or the port you specified) to view the project</li>
            </ol>
            
            <p>Alternatively, you can deploy the project to platforms like Vercel, Netlify, or GitHub Pages for live hosting.</p>
        </section>
        
        <section class="section">
            <h2>Live Demo</h2>
            <p>Experience the fully functional landing page with all interactive elements:</p>
            
            <div class="demo-card">
                <h3>LinkedIn Learning Landing Page</h3>
                <p>Explore the responsive design, dark mode functionality, and interactive elements</p>
                <a href="https://belajar-linked-in-landingpage.vercel.app/" class="demo-btn" target="_blank">
                    View Live Demo <i class="fas fa-external-link-alt"></i>
                </a>
            </div>
        </section>
        
        <section class="section">
            <h2>Key Features</h2>
            <div class="features">
                <div class="feature">
                    <h3><i class="fas fa-moon"></i> Dark Mode Toggle</h3>
                    <p>Switch between light and dark themes for better user experience in different lighting conditions</p>
                </div>
                
                <div class="feature">
                    <h3><i class="fas fa-mobile-alt"></i> Fully Responsive</h3>
                    <p>Adapts seamlessly to all screen sizes from mobile to desktop</p>
                </div>
                
                <div class="feature">
                    <h3><i class="fas fa-clipboard-list"></i> Registration Form</h3>
                    <p>Comprehensive form for course registration with validation</p>
                </div>
                
                <div class="feature">
                    <h3><i class="fas fa-comments"></i> Feedback System</h3>
                    <p>Dedicated section for users to provide feedback and suggestions</p>
                </div>
                
                <div class="feature">
                    <h3><i class="fas fa-star"></i> Testimonial Slider</h3>
                    <p>Interactive carousel showcasing user testimonials</p>
                </div>
                
                <div class="feature">
                    <h3><i class="fas fa-question-circle"></i> FAQ Accordion</h3>
                    <p>Expandable sections for common questions and answers</p>
                </div>
            </div>
        </section>
        
        <section class="section">
            <h2>Project Structure</h2>
            <p>The project is organized as a single HTML file with embedded CSS and JavaScript for simplicity:</p>
            
            <div class="code-block">
                linkedin-learning-landingpage.html<br>
                ├── Header with navigation<br>
                ├── Hero section<br>
                ├── About section<br>
                ├── Benefits section<br>
                ├── Testimonials section<br>
                ├── FAQ section<br>
                ├── Feedback section<br>
                ├── Registration section<br>
                ├── Call-to-action section<br>
                └── Footer<br>
                <br>
                CSS is embedded in the &lt;style&gt; tag<br>
                JavaScript is embedded in the &lt;script&gt; tag
            </div>
        </section>
        
        <section class="section">
            <h2>Browser Compatibility</h2>
            <p>This project is compatible with all modern browsers including:</p>
            
            <div class="tags">
                <span class="tag">Chrome 60+</span>
                <span class="tag">Firefox 55+</span>
                <span class="tag">Safari 12+</span>
                <span class="tag">Edge 79+</span>
                <span class="tag">Opera 50+</span>
            </div>
            
            <p style="margin-top: 15px;">For optimal experience, use the latest version of your preferred browser.</p>
        </section>
    </div>
    
    <footer>
        <p>LinkedIn Learning Landing Page Documentation | Created with <i class="fas fa-heart" style="color: #e25555;"></i></p>
        <p>© 2023 | All Rights Reserved</p>
    </footer>
    
    <script>
        // Simple animation for tech cards
        document.addEventListener('DOMContentLoaded', function() {
            const techCards = document.querySelectorAll('.tech-card');
            
            techCards.forEach((card, index) => {
                // Add delay based on index for staggered animation
                card.style.animationDelay = `${index * 0.1}s`;
                card.classList.add('fade-in');
            });
            
            // Add animation for section elements
            const sections = document.querySelectorAll('.section');
            
            const observer = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.classList.add('visible');
                    }
                });
            }, { threshold: 0.1 });
            
            sections.forEach(section => {
                observer.observe(section);
            });
        });
    </script>
</body>
</html>
