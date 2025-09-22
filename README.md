<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Akash Samanta - Full Stack Developer</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap');
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Inter', sans-serif;
            background: linear-gradient(135deg, #0f0f23 0%, #1a1a2e 50%, #16213e 100%);
            color: #ffffff;
            min-height: 100vh;
            overflow-x: hidden;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 2rem;
        }
        
        /* 3D Header Styles */
        .header-3d {
            text-align: center;
            margin-bottom: 3rem;
            perspective: 1000px;
        }
        
        .name-title {
            font-size: 3.5rem;
            font-weight: 700;
            background: linear-gradient(45deg, #00D4FF, #FF6B6B, #FFD93D, #6BCF7F);
            background-size: 400% 400%;
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            animation: gradientShift 8s ease infinite;
            transform-style: preserve-3d;
            transition: transform 0.5s ease;
        }
        
        .name-title:hover {
            transform: rotateX(10deg) rotateY(5deg) scale(1.05);
        }
        
        @keyframes gradientShift {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }
        
        .subtitle {
            font-size: 1.5rem;
            color: #8892b0;
            margin-top: 1rem;
            transform: translateZ(30px);
        }
        
        /* 3D Card Styles */
        .card-3d {
            background: rgba(255, 255, 255, 0.05);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            border-radius: 20px;
            padding: 2rem;
            margin: 2rem 0;
            transform-style: preserve-3d;
            transition: all 0.3s ease;
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.3);
        }
        
        .card-3d:hover {
            transform: translateY(-10px) rotateX(5deg) rotateY(5deg);
            box-shadow: 0 40px 80px rgba(0, 212, 255, 0.2);
            border-color: rgba(0, 212, 255, 0.3);
        }
        
        .section-title {
            font-size: 2rem;
            margin-bottom: 1.5rem;
            color: #00D4FF;
            text-align: center;
        }
        
        /* Skills Grid */
        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 1.5rem;
            margin-top: 2rem;
        }
        
        .skill-item {
            background: rgba(255, 255, 255, 0.1);
            padding: 1.5rem;
            border-radius: 15px;
            text-align: center;
            transition: all 0.3s ease;
            transform-style: preserve-3d;
        }
        
        .skill-item:hover {
            transform: translateY(-5px) rotateX(5deg);
            background: rgba(0, 212, 255, 0.2);
        }
        
        /* Projects Grid */
        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 2rem;
            margin-top: 2rem;
        }
        
        .project-card {
            background: linear-gradient(145deg, #1a1a2e, #16213e);
            border-radius: 20px;
            padding: 2rem;
            transition: all 0.3s ease;
            transform-style: preserve-3d;
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .project-card:hover {
            transform: translateY(-10px) rotateY(5deg) scale(1.02);
            box-shadow: 0 30px 60px rgba(0, 212, 255, 0.3);
        }
        
        /* Stats Section */
        .stats-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
            margin-top: 2rem;
        }
        
        .stat-card {
            background: rgba(255, 255, 255, 0.05);
            padding: 2rem;
            border-radius: 15px;
            text-align: center;
            transition: all 0.3s ease;
        }
        
        .stat-card:hover {
            transform: scale(1.05);
            background: rgba(0, 212, 255, 0.1);
        }
        
        /* Contact Buttons */
        .contact-buttons {
            display: flex;
            justify-content: center;
            gap: 1rem;
            flex-wrap: wrap;
            margin-top: 2rem;
        }
        
        .contact-btn {
            padding: 1rem 2rem;
            border: 2px solid #00D4FF;
            border-radius: 50px;
            color: #00D4FF;
            text-decoration: none;
            transition: all 0.3s ease;
            font-weight: 600;
        }
        
        .contact-btn:hover {
            background: #00D4FF;
            color: #0f0f23;
            transform: translateY(-3px) scale(1.05);
        }
        
        /* Responsive Design */
        @media (max-width: 768px) {
            .name-title {
                font-size: 2.5rem;
            }
            
            .projects-grid {
                grid-template-columns: 1fr;
            }
            
            .skills-grid {
                grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- 3D Header Section -->
        <div class="header-3d">
            <h1 class="name-title">AKASH SAMANTA</h1>
            <p class="subtitle">Java Full Stack Developer | AI Enthusiast | Problem Solver</p>
        </div>

        <!-- About Section -->
        <div class="card-3d">
            <h2 class="section-title">🚀 About Me</h2>
            <p style="font-size: 1.2rem; line-height: 1.6; text-align: center;">
                Passionate Computer Science student with expertise in full-stack development, data analysis, 
                and AI/ML. I love building innovative solutions that solve real-world problems. 
                Currently enhancing my skills in Spring Boot, React.js, and Cloud Technologies.
            </p>
        </div>

        <!-- Skills Section -->
        <div class="card-3d">
            <h2 class="section-title">🛠 Technical Skills</h2>
            <div class="skills-grid">
                <div class="skill-item">
                    <h3>Java</h3>
                    <p>Spring Boot, Hibernate, JDBC</p>
                </div>
                <div class="skill-item">
                    <h3>Frontend</h3>
                    <p>React.js, HTML5, CSS3, JavaScript</p>
                </div>
                <div class="skill-item">
                    <h3>Database</h3>
                    <p>MySQL, PostgreSQL, PL/SQL</p>
                </div>
                <div class="skill-item">
                    <h3>Tools</h3>
                    <p>GitHub, Docker, Postman, VS Code</p>
                </div>
            </div>
        </div>

        <!-- Projects Section -->
        <div class="card-3d">
            <h2 class="section-title">🌟 Featured Projects</h2>
            <div class="projects-grid">
                <!-- Project 1 -->
                <div class="project-card">
                    <h3 style="color: #00D4FF; margin-bottom: 1rem;">🌊 Flood Prediction System</h3>
                    <p>AI-powered system for forecasting flood risks with 85%+ accuracy using meteorological data.</p>
                    <div style="margin-top: 1rem;">
                        <span class="tech-tag">Python</span>
                        <span class="tech-tag">ML</span>
                        <span class="tech-tag">Data Visualization</span>
                    </div>
                </div>

                <!-- Project 2 -->
                <div class="project-card">
                    <h3 style="color: #FF6B6B; margin-bottom: 1rem;">🛒 E-Commerce Platform</h3>
                    <p>Full-stack shopping portal with secure authentication and payment integration.</p>
                    <div style="margin-top: 1rem;">
                        <span class="tech-tag">Spring Boot</span>
                        <span class="tech-tag">React</span>
                        <span class="tech-tag">MySQL</span>
                    </div>
                </div>

                <!-- Project 3 -->
                <div class="project-card">
                    <h3 style="color: #FFD93D; margin-bottom: 1rem;">🔗 QR Code Generator</h3>
                    <p>Dynamic QR code generation tool with instant preview and custom styling options.</p>
                    <div style="margin-top: 1rem;">
                        <span class="tech-tag">JavaScript</span>
                        <span class="tech-tag">HTML5</span>
                        <span class="tech-tag">CSS3</span>
                    </div>
                </div>
            </div>
        </div>

        <!-- GitHub Stats -->
        <div class="card-3d">
            <h2 class="section-title">📊 GitHub Analytics</h2>
            <div class="stats-container">
                <div class="stat-card">
                    <h3>Commits</h3>
                    <p style="font-size: 2rem; color: #00D4FF;">250+</p>
                </div>
                <div class="stat-card">
                    <h3>Repositories</h3>
                    <p style="font-size: 2rem; color: #FF6B6B;">15+</p>
                </div>
                <div class="stat-card">
                    <h3>Contributions</h3>
                    <p style="font-size: 2rem; color: #FFD93D;">500+</p>
                </div>
            </div>
        </div>

        <!-- Contact Section -->
        <div class="card-3d">
            <h2 class="section-title">📞 Let's Connect</h2>
            <div class="contact-buttons">
                <a href="mailto:akashayushsamanta@gmail.com" class="contact-btn">📧 Email</a>
                <a href="https://linkedin.com/in/your-profile" class="contact-btn">💼 LinkedIn</a>
                <a href="https://github.com/yourusername" class="contact-btn">🐙 GitHub</a>
                <a href="https://your-portfolio.com" class="contact-btn">🌐 Portfolio</a>
            </div>
        </div>
    </div>

    <script>
        // 3D Mouse Movement Effect
        document.addEventListener('mousemove', (e) => {
            const cards = document.querySelectorAll('.card-3d');
            const x = (window.innerWidth - e.pageX * 2) / 100;
            const y = (window.innerHeight - e.pageY * 2) / 100;
            
            cards.forEach(card => {
                card.style.transform = `rotateY(${x}deg) rotateX(${y}deg)`;
            });
        });

        // Typing Animation
        const titles = [
            "Java Full Stack Developer",
            "AI Enthusiast", 
            "Problem Solver",
            "Continuous Learner"
        ];
        
        let titleIndex = 0;
        let charIndex = 0;
        const typingElement = document.querySelector('.subtitle');
        
        function typeWriter() {
            if (charIndex < titles[titleIndex].length) {
                typingElement.textContent += titles[titleIndex].charAt(charIndex);
                charIndex++;
                setTimeout(typeWriter, 100);
            } else {
                setTimeout(eraseText, 2000);
            }
        }
        
        function eraseText() {
            if (charIndex > 0) {
                typingElement.textContent = titles[titleIndex].substring(0, charIndex - 1);
                charIndex--;
                setTimeout(eraseText, 50);
            } else {
                titleIndex = (titleIndex + 1) % titles.length;
                setTimeout(typeWriter, 500);
            }
        }
        
        // Start typing animation
        setTimeout(typeWriter, 1000);
    </script>
</body>
</html>
