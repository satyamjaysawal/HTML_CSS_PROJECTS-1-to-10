```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AI & Full Stack Developer LinkedIn Profile Background - Cosmic UI Enhanced</title>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/tailwindcss/2.2.19/tailwind.min.css" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700;900&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
        }
        
        body {
            background: #000;
            color: #fff;
            overflow: hidden;
        }
        
        .linkedin-bg {
            width: 1584px;
            height: 396px;
            position: relative;
            overflow: hidden;
            background: #050520;
        }
        
        .bg-image {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(135deg, #050520, #0a0a3a, #1a1a6c, #2a0a5b);
            animation: gradientShift 25s infinite ease-in-out;
            opacity: 0.9;
            transition: transform 0.5s ease;
        }

        @keyframes gradientShift {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        /* Enhanced Twinkling Stars */
        .stars {
            position: absolute;
            width: 100%;
            height: 100%;
            pointer-events: none;
        }

        .star {
            position: absolute;
            background: #fff;
            border-radius: 50%;
            animation: twinkle 3s infinite ease-in-out, starMove 10s infinite linear;
            box-shadow: 0 0 5px rgba(255, 255, 255, 0.8);
        }

        @keyframes twinkle {
            0%, 100% { opacity: 0.2; transform: scale(0.8); }
            50% { opacity: 1; transform: scale(1.2); }
        }

        @keyframes starMove {
            0% { transform: translateY(0); }
            100% { transform: translateY(-50px); opacity: 0; }
        }

        /* Enhanced Particles with Connections */
        .particles {
            position: absolute;
            width: 100%;
            height: 100%;
        }
        
        .particle {
            position: absolute;
            border-radius: 50%;
            box-shadow: 0 0 20px 5px rgba(100, 180, 255, 0.7);
            animation: float 10s infinite ease-in-out, glow 4s infinite alternate;
            transition: transform 0.3s ease;
        }
        
        .particle:hover {
            transform: scale(1.5);
            box-shadow: 0 0 30px 10px rgba(100, 180, 255, 1);
        }
        
        .particle-connection {
            position: absolute;
            height: 1px;
            background: linear-gradient(90deg, transparent, rgba(100, 180, 255, 0.7), transparent);
            animation: connectPulse 3s infinite ease-in-out;
        }

        @keyframes float {
            0%, 100% { transform: translate(0, 0) scale(1); opacity: 0.8; }
            50% { transform: translate(150px, -80px) scale(1.8); opacity: 0.6; }
        }

        @keyframes connectPulse {
            0%, 100% { opacity: 0.2; transform: scale(0.9); }
            50% { opacity: 0.5; transform: scale(1.1); }
        }

        @keyframes glow {
            0% { box-shadow: 0 0 15px rgba(100, 180, 255, 0.5); }
            100% { box-shadow: 0 0 25px rgba(100, 180, 255, 0.8); }
        }

        .neon-overlay {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: radial-gradient(ellipse at center, rgba(120, 0, 255, 0.2) 0%, rgba(0, 150, 255, 0.1) 50%, rgba(0, 0, 0, 0) 70%);
            animation: neonShift 15s infinite alternate;
        }

        @keyframes neonShift {
            0% { transform: scale(1); opacity: 0.8; }
            100% { transform: scale(1.03); opacity: 1; }
        }

        .grid-lines {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-image: 
                linear-gradient(to right, rgba(100, 180, 255, 0.15) 1px, transparent 1px),
                linear-gradient(to bottom, rgba(100, 180, 255, 0.15) 1px, transparent 1px);
            background-size: 50px 50px;
            opacity: 0.3;
            transform: perspective(800px) rotateX(25deg);
            animation: gridShift 20s infinite linear, gridFade 6s infinite ease-in-out;
            transition: transform 0.5s ease;
        }

        @keyframes gridShift {
            0% { background-position: 0 0; }
            100% { background-position: 50px 50px; }
        }

        @keyframes gridFade {
            0%, 100% { opacity: 0.3; }
            50% { opacity: 0.15; }
        }

        /* Enhanced Cosmic Pattern */
        .cosmic-pattern {
            position: absolute;
            width: 100%;
            height: 100%;
            opacity: 0.7;
        }

        .nebula {
            position: absolute;
            width: 600px;
            height: 600px;
            background: radial-gradient(circle, rgba(100, 180, 255, 0.25) 0%, rgba(0, 0, 0, 0) 70%);
            top: 50%;
            left: 70%;
            transform: translate(-50%, -50%);
            animation: nebulaPulse 20s infinite ease-in-out;
            filter: blur(20px);
        }

        .nebula-2 {
            position: absolute;
            width: 500px;
            height: 500px;
            background: radial-gradient(circle, rgba(200, 0, 255, 0.2) 0%, rgba(0, 0, 0, 0) 70%);
            top: 30%;
            left: 20%;
            transform: translate(-50%, -50%);
            animation: nebulaPulse 18s infinite ease-in-out reverse;
            filter: blur(15px);
        }

        .nebula-3 {
            position: absolute;
            width: 700px;
            height: 700px;
            background: radial-gradient(circle, rgba(0, 255, 200, 0.15) 0%, rgba(0, 0, 0, 0) 80%);
            top: 70%;
            left: 50%;
            transform: translate(-50%, -50%);
            animation: nebulaPulse 25s infinite ease-in-out;
            filter: blur(25px);
        }

        @keyframes nebulaPulse {
            0%, 100% { transform: translate(-50%, -50%) scale(1); opacity: 0.25; }
            50% { transform: translate(-50%, -50%) scale(1.08); opacity: 0.35; }
        }

        .cosmic-pattern-line {
            position: absolute;
            background: linear-gradient(90deg, rgba(0, 150, 255, 0) 0%, rgba(100, 180, 255, 0.7) 50%, rgba(0, 150, 255, 0) 100%);
            height: 2px;
            width: 100%;
            transform-origin: left center;
            box-shadow: 0 0 10px rgba(100, 180, 255, 0.5);
        }

        .cosmic-pattern-shape {
            position: absolute;
            border: 2px solid rgba(100, 180, 255, 0.5);
            border-radius: 50%;
            animation: rotate 15s infinite linear, glow 6s infinite alternate;
            transition: transform 0.3s ease, border-color 0.3s ease;
        }

        .cosmic-pattern-shape:hover {
            transform: translate(-50%, -50%) scale(1.1);
            border-color: rgba(100, 180, 255, 1);
        }

        @keyframes rotate {
            0% { transform: translate(-50%, -50%) rotate(0deg); }
            100% { transform: translate(-50%, -50%) rotate(360deg); }
        }

        /* Profile Section Enhancements */
        .profile-section {
            position: absolute;
            display: flex;
            align-items: center;
            top: 50px; 
            left: 20px; /* Adjusted for better alignment */
            z-index: 10;
            flex-direction: row-reverse;
            filter: drop-shadow(0 0 15px rgba(100, 180, 255, 0.4));
            transition: transform 0.5s ease;
            width: calc(100% - 60px); /* Ensure it fits within container */
        }

        .profile-section::before {
            content: '';
            position: absolute;
            width: 500px;
            height: 500px;
            background: radial-gradient(circle, rgba(100, 180, 255, 0.25) 0%, transparent 70%);
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            z-index: -1;
            animation: glowPulse 8s infinite alternate;
        }

        @keyframes glowPulse {
            0% { opacity: 0.25; transform: translate(-50%, -50%) scale(1); }
            100% { opacity: 0.4; transform: translate(-50%, -50%) scale(1.05); }
        }

        .profile-container {
            position: relative;
            width: 200px; /* Slightly reduced to give more space to content */
            height: 200px;
            margin-left: 20px; /* Reduced margin */
        }

        .profile-pic {
            position: absolute;
            width: 160px; /* Reduced size */
            height: 160px;
            border-radius: 50%;
            overflow: hidden;
            border: 3px solid rgba(100, 180, 255, 0.9);
            box-shadow: 0 0 30px rgba(100, 180, 255, 0.7);
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            z-index: 3;
            transition: transform 0.4s ease, box-shadow 0.4s ease, border-color 0.4s ease;
        }

        .profile-pic:hover {
            transform: translate(-50%, -50%) scale(1.1) rotate(5deg);
            box-shadow: 0 0 50px rgba(100, 180, 255, 1);
            border-color: #ffffff;
        }

        .profile-ring {
            position: absolute;
            width: 180px; /* Adjusted to match profile-pic */
            height: 180px;
            border-radius: 50%;
            border: 3px dashed rgba(100, 180, 255, 0.6);
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            animation: rotate 15s infinite linear, pulseRing 1.5s infinite;
        }

        @keyframes pulseRing {
            0%, 100% { opacity: 0.6; transform: translate(-50%, -50%) scale(1); }
            50% { opacity: 0.9; transform: translate(-50%, -50%) scale(1.05); }
        }

        .content {
            max-width: 1100px; /* Increased slightly to accommodate skills */
            position: relative;
        }

        .name {
            font-size: 2.8rem; /* Slightly reduced to fit better */
            font-weight: 900;
            margin-bottom: 6px;
            background: linear-gradient(90deg, #ffffff, #64b4ff, #ffffff);
            -webkit-background-clip: text;
            background-clip: text;
            -webkit-text-fill-color: transparent;
            text-shadow: 0 0 25px rgba(100, 180, 255, 0.8);
            animation: textGlow 2.5s infinite alternate;
            transition: transform 0.3s ease;
        }

        .name:hover {
            transform: scale(1.05);
        }

        @keyframes textGlow {
            0% { text-shadow: 0 0 15px rgba(100, 180, 255, 0.6); }
            100% { text-shadow: 0 0 35px rgba(100, 180, 255, 0.9); }
        }

        .title {
            font-size: 1.3rem; /* Slightly reduced */
            font-weight: 700;
            background: linear-gradient(90deg, #64b4ff, #ffffff);
            -webkit-background-clip: text;
            background-clip: text;
            -webkit-text-fill-color: transparent;
            margin-bottom: 4px;
            transition: transform 0.3s ease;
        }

        .title:hover {
            transform: translateX(10px);
        }

        .tagline {
            font-size: 1rem; /* Slightly reduced */
            font-weight: 400;
            color: rgba(255, 255, 255, 0.9);
            margin-bottom: 8px;
            animation: fadeIn 2s ease-in-out;
        }

        @keyframes fadeIn {
            0% { opacity: 0; }
            100% { opacity: 0.9; }
        }

        .skills {
            display: flex;
            flex-wrap: wrap; /* Allow wrapping to ensure visibility */
            gap: 8px; /* Reduced gap slightly */
            position: relative;
            z-index: 10;
            max-width: 900px; /* Limit width to fit within container */
            animation: slideIn 1.5s ease-out;
        }

        @keyframes slideIn {
            0% { transform: translateY(20px); opacity: 0; }
            100% { transform: translateY(0); opacity: 1; }
        }

        .skill {
            background: rgba(100, 180, 255, 0.2);
            border: 2px solid rgba(100, 180, 255, 0.7);
            border-radius: 25px;
            padding: 5px 15px; /* Slightly reduced padding */
            font-size: 0.9rem; /* Reduced font size */
            font-weight: 600;
            color: #fff;
            box-shadow: 0 0 10px rgba(100, 180, 255, 0.4);
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
            cursor: pointer;
            white-space: nowrap; /* Keep individual skills from breaking */
        }

        .skill::after {
            content: '';
            position: absolute;
            top: -50%;
            left: -50%;
            width: 200%;
            height: 200%;
            background: radial-gradient(circle, rgba(255, 255, 255, 0.25) 0%, transparent 70%);
            opacity: 0;
            transition: opacity 0.3s ease;
        }

        .skill:hover::after {
            opacity: 1;
        }

        .skill:hover {
            background: rgba(100, 180, 255, 0.4);
            box-shadow: 0 0 20px rgba(100, 180, 255, 0.7);
            transform: scale(1.1) rotate(2deg);
        }

        /* New Floating Orbits */
        .orbit {
            position: absolute;
            border: 1px dashed rgba(100, 180, 255, 0.5);
            border-radius: 50%;
            animation: orbitRotate 20s infinite linear;
        }

        @keyframes orbitRotate {
            0% { transform: translate(-50%, -50%) rotate(0deg); }
            100% { transform: translate(-50%, -50%) rotate(360deg); }
        }
    </style>
</head>
<body>
    <div class="linkedin-bg">
        <div class="bg-image"></div>

        <div class="stars">
            <!-- Stars will be generated via JavaScript -->
        </div>

        <div class="particles">
            <!-- Particles will be generated via JavaScript -->
        </div>

        <div class="neon-overlay"></div>
        <div class="grid-lines"></div>

        <div class="cosmic-pattern">
            <div class="nebula"></div>
            <div class="nebula-2"></div>
            <div class="nebula-3"></div>
            <div class="cosmic-pattern-line" style="top: 20%; transform: rotate(6deg); animation: glow 6s infinite alternate;"></div>
            <div class="cosmic-pattern-line" style="top: 40%; transform: rotate(-4deg); animation: glow 8s infinite alternate-reverse;"></div>
            <div class="cosmic-pattern-line" style="top: 60%; transform: rotate(5deg); animation: glow 10s infinite alternate;"></div>
            <div class="cosmic-pattern-line" style="top: 80%; transform: rotate(-3deg); animation: glow 7s infinite alternate-reverse;"></div>
            <div class="cosmic-pattern-shape" style="width: 400px; height: 400px; top: 50%; left: 70%; transform: translate(-50%, -50%);"></div>
            <div class="cosmic-pattern-shape" style="width: 300px; height: 300px; top: 30%; left: 80%; transform: translate(-50%, -50%); animation-duration: 12s;"></div>
            <div class="cosmic-pattern-shape" style="width: 500px; height: 500px; top: 60%; left: 20%; transform: translate(-50%, -50%); animation-duration: 20s;"></div>
            <div class="orbit" style="width: 300px; height: 300px; top: 50%; left: 50%; transform: translate(-50%, -50%);"></div>
            <div class="orbit" style="width: 400px; height: 400px; top: 50%; left: 50%; transform: translate(-50%, -50%); animation-duration: 25s;"></div>
        </div>

        <div class="profile-section">
            <div class="profile-container">
                <div class="profile-pic">
                    <img src="https://github.com/user-attachments/assets/40e9a6ee-e8ee-4e20-9d19-01273e0f20e9" alt="Profile Picture" class="w-full h-full object-cover">
                </div>
                <div class="profile-ring"></div>
            </div>

            <div class="content">
                <h1 class="name">Satyam Jaysawal</h1>
                <p class="title">AI Developer | Full Stack Developer</p>
                <p class="tagline">Building intelligent systems and scalable apps in a universe of code and creativity.</p>
                
                <div class="skills">
                    <span class="skill">JavaScript</span>
                    <span class="skill">TensorFlow</span>
                    <span class="skill">React.js</span>
                    <span class="skill">Node.js</span>
                    <span class="skill">AWS/AZURE</span>
                    <span class="skill">Python</span>
                    <span class="skill">Machine Learning</span>
                    <span class="skill">Logic APP</span>
                    <span class="skill">Flask</span>
                    <span class="skill">Generative AI</span>
                </div>
            </div>
        </div>
    </div>

    <script>
        // Enhanced Particles
        const particleContainer = document.querySelector('.particles');
        const particleCount = 20;
        for (let i = 0; i < particleCount; i++) {
            const particle = document.createElement('div');
            particle.classList.add('particle');
            particle.style.top = `${Math.random() * 100}%`;
            particle.style.left = `${Math.random() * 100}%`;
            particle.style.width = `${Math.random() * 8 + 3}px`;
            particle.style.height = particle.style.width;
            particle.style.background = `hsl(${Math.random() * 60 + 180}, 80%, 80%)`;
            particle.style.animationDuration = `${Math.random() * 8 + 8}s`;
            particle.style.animationDelay = `${Math.random() * 5}s`;
            particleContainer.appendChild(particle);

            if (i % 2 === 0 && i < particleCount - 1) {
                const connection = document.createElement('div');
                connection.classList.add('particle-connection');
                connection.style.top = particle.style.top;
                connection.style.left = particle.style.left;
                connection.style.width = `${Math.random() * 200 + 50}px`;
                connection.style.transform = `rotate(${Math.random() * 360}deg)`;
                connection.style.animationDelay = `${Math.random() * 2}s`;
                particleContainer.appendChild(connection);
            }
        }

        // Enhanced Twinkling Stars
        const starContainer = document.querySelector('.stars');
        const starCount = 70;
        for (let i = 0; i < starCount; i++) {
            const star = document.createElement('div');
            star.classList.add('star');
            star.style.top = `${Math.random() * 100}%`;
            star.style.left = `${Math.random() * 100}%`;
            star.style.width = `${Math.random() * 3 + 1}px`;
            star.style.height = star.style.width;
            star.style.animationDelay = `${Math.random() * 3}s`;
            star.style.animationDuration = `${Math.random() * 5 + 3}s`;
            starContainer.appendChild(star);
        }

        // Advanced Parallax Effect
        document.addEventListener('mousemove', (e) => {
            const x = (e.clientX / window.innerWidth - 0.5) * 30;
            const y = (e.clientY / window.innerHeight - 0.5) * 30;
            document.querySelector('.bg-image').style.transform = `translate(${x}px, ${y}px) scale(1.02)`;
            document.querySelector('.grid-lines').style.transform = `perspective(800px) rotateX(25deg) translate(${x * 0.5}px, ${y * 0.5}px)`;
            document.querySelector('.profile-section').style.transform = `translate(${x * 0.2}px, ${y * 0.2}px)`;
            document.querySelectorAll('.cosmic-pattern-shape').forEach(shape => {
                shape.style.transform = `translate(-50%, -50%) translate(${x * 0.1}px, ${y * 0.1}px) rotate(${x}deg)`;
            });
        });

        // Skill Tooltip (Optional interactivity)
        document.querySelectorAll('.skill').forEach(skill => {
            skill.addEventListener('mouseover', () => {
                const tooltip = document.createElement('div');
                tooltip.textContent = `Proficient in ${skill.textContent}`;
                tooltip.style.position = 'absolute';
                tooltip.style.background = 'rgba(0, 0, 0, 0.8)';
                tooltip.style.color = '#fff';
                tooltip.style.padding = '5px 10px';
                tooltip.style.borderRadius = '5px';
                tooltip.style.fontSize = '0.9rem';
                tooltip.style.top = `${skill.offsetTop - 30}px`;
                tooltip.style.left = `${skill.offsetLeft + skill.offsetWidth / 2}px`;
                tooltip.style.transform = 'translateX(-50%)';
                tooltip.style.zIndex = '20';
                skill.appendChild(tooltip);
            });
            skill.addEventListener('mouseout', () => {
                const tooltip = skill.querySelector('div');
                if (tooltip) tooltip.remove();
            });
        });
    </script>
</body>
</html>

```
