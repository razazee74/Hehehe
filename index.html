<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Premium Social Media Services - SMFixer Clone</title>
    
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">

    <style>
        /* --- CSS STYLES --- */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: #0f172a; /* Fallback Dark Background */
            color: #e2e8f0; /* Light Text */
            line-height: 1.6;
            overflow-x: hidden;
            position: relative; /* Required for canvas positioning */
        }

        /* --- MOTION BACKGROUND CANVAS STYLE --- */
        #particle-canvas {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -1; /* Content ke peeche rahega */
            pointer-events: none; /* Is par click nahi hoga */
        }

        .container {
            max-width: 1100px;
            margin: 0 auto;
            padding: 20px;
            position: relative; /* Canvas ke upar dikhne ke liye */
            z-index: 1;
        }

        /* --- Scroll Animations --- */
        .reveal {
            opacity: 0;
            transform: translateY(50px);
            transition: all 0.8s ease-out;
        }
        .reveal.active {
            opacity: 1;
            transform: translateY(0);
        }

        .slide-left {
            opacity: 0;
            transform: translateX(-50px);
            transition: all 1s ease-out;
        }
        .slide-left.active {
            opacity: 1;
            transform: translateX(0);
        }

        /* Header */
        header {
            text-align: center;
            padding: 80px 20px;
            /* Background ko thoda transparent banaya taaki motion dikhe */
            background: linear-gradient(to bottom, rgba(30, 41, 59, 0.9), rgba(15, 23, 42, 0.9));
            border-bottom: 1px solid #334155;
            position: relative;
            z-index: 1;
        }

        header h1 {
            font-size: 2.8rem;
            color: #38bdf8;
            margin-bottom: 15px;
            text-transform: uppercase;
            letter-spacing: 2px;
        }

        header p {
            font-size: 1.2rem;
            color: #94a3b8;
            max-width: 650px;
            margin: 0 auto 30px auto;
        }

        /* Header Buttons */
        .cta-buttons {
            display: flex;
            justify-content: center;
            gap: 20px;
            flex-wrap: wrap;
        }

        .btn {
            padding: 14px 35px;
            font-size: 1.1rem;
            font-weight: bold;
            text-decoration: none;
            border-radius: 50px;
            transition: transform 0.3s, box-shadow 0.3s;
            display: inline-flex;
            align-items: center;
            gap: 10px;
        }
        
        .btn i { font-size: 1.4rem; }
        
        /* Button Colors */
        .btn-telegram { background-color: #229ED9; color: white; }
        .btn-whatsapp { background-color: #25D366; color: white; }
        
        .btn:hover { transform: translateY(-5px); box-shadow: 0 10px 20px rgba(0,0,0,0.4); }

        /* Services Grid */
        .section-title {
            text-align: center;
            font-size: 2.2rem;
            margin: 80px 0 50px;
            color: #f8fafc;
            position: relative;
        }
        .section-title::after {
            content: '';
            display: block;
            width: 80px;
            height: 4px;
            background: #38bdf8;
            margin: 15px auto;
            border-radius: 2px;
        }

        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 30px;
        }

        /* Cards ko thoda transparent banaya */
        .service-card {
            background-color: rgba(30, 41, 59, 0.85); /* Slight transparency */
            padding: 30px;
            border-radius: 16px;
            border: 1px solid #334155;
            transition: transform 0.3s, border-color 0.3s;
            box-shadow: 0 4px 6px rgba(0,0,0,0.2);
            backdrop-filter: blur(5px); /* Mast effect ke liye */
        }
        .service-card:hover {
            border-color: #38bdf8;
            transform: translateY(-5px);
        }
        .service-card h3 {
            font-size: 1.6rem;
            margin-bottom: 20px;
            color: #fff;
            border-bottom: 1px solid #334155;
            padding-bottom: 15px;
            display: flex;
            align-items: center;
            gap: 12px;
        }

        /* Icons Colors */
        .fa-instagram { color: #E1306C; }
        .fa-twitter, .fa-x-twitter { color: #1DA1F2; }
        .fa-whatsapp { color: #25D366; }
        .fa-tiktok { color: #ff0050; }
        .fa-facebook { color: #1877F2; }
        .fa-youtube { color: #FF0000; }

        .service-item { margin-bottom: 18px; }
        .service-name { font-weight: 600; color: #cbd5e1; font-size: 1.05rem; display: block; }
        .service-price { color: #4ade80; font-weight: bold; font-size: 1rem; }
        .service-time { color: #64748b; font-size: 0.9rem; font-style: italic; }

        /* Info Boxes transparent */
        .info-box {
            background-color: rgba(30, 41, 59, 0.85);
            padding: 35px;
            border-radius: 12px;
            margin-bottom: 30px;
            text-align: center;
            border-left: 5px solid #38bdf8;
            font-size: 1.1rem;
            backdrop-filter: blur(5px);
        }

        /* Footer (Fixed position and spacing, transparent bg) */
        footer {
            text-align: center;
            padding: 40px 20px;
            padding-bottom: 130px; 
            margin-top: 80px;
            background-color: rgba(30, 41, 59, 0.9); /* Transparent */
            border-top: 1px solid #334155;
            color: #94a3b8;
            font-size: 0.95rem;
            position: relative;
            z-index: 1;
        }

        /* --- FLOATING SHIELD & POPUP STYLES --- */

        /* The Round Shield Button (Blue Theme) */
        .shield-btn {
            position: fixed;
            bottom: 25px;
            right: 25px;
            width: 65px;
            height: 65px;
            background-color: #38bdf8; /* Blue Theme Color */
            border-radius: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
            cursor: pointer;
            box-shadow: 0 5px 15px rgba(56, 189, 248, 0.4);
            z-index: 999;
            transition: transform 0.3s ease;
        }

        .shield-btn:hover {
            transform: scale(1.1);
        }

        .shield-btn i {
            color: #0f172a;
            font-size: 30px;
        }

        /* The Modal Background Overlay */
        .modal-overlay {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.85);
            display: flex;
            justify-content: center;
            align-items: center;
            z-index: 1000;
            opacity: 0;
            pointer-events: none;
            transition: opacity 0.3s ease;
        }

        .modal-overlay.active {
            opacity: 1;
            pointer-events: auto;
        }

        /* The Popup Box (MOBILE FIXED) */
        .modal-content {
            background: #1e293b; /* Solid background for popup to stay readable */
            width: 90%; /* Mobile width */
            max-width: 500px; /* Desktop max width */
            max-height: 85vh; /* 85% of screen height */
            display: flex;
            flex-direction: column; /* Stack items */
            padding: 25px;
            border-radius: 15px;
            text-align: center;
            border: 2px solid #38bdf8; /* Blue Border */
            transform: scale(0.8);
            transition: transform 0.3s ease;
            box-shadow: 0 0 25px rgba(56, 189, 248, 0.2);
        }

        .modal-overlay.active .modal-content {
            transform: scale(1);
        }

        .modal-content h2 {
            color: #38bdf8;
            margin-bottom: 15px;
            font-size: 1.5rem;
            text-transform: uppercase;
            flex-shrink: 0;
        }

        /* Internal Scrollable Area */
        .tos-text {
            color: #cbd5e1;
            font-size: 1rem;
            text-align: left;
            margin-bottom: 15px;
            background: #0f172a;
            padding: 15px;
            border-radius: 8px;
            overflow-y: auto;
            flex-grow: 1;
            border: 1px solid #334155;
        }

        .tos-text ul {
            list-style-type: none;
        }

        .tos-text li {
            margin-bottom: 10px;
            padding-left: 10px;
            border-left: 3px solid #38bdf8;
        }

        /* Okay Button */
        .btn-okay {
            background-color: #38bdf8;
            color: #0f172a;
            border: none;
            padding: 12px 0;
            width: 100%;
            font-size: 1.1rem;
            font-weight: bold;
            border-radius: 50px;
            cursor: pointer;
            transition: background 0.3s;
            flex-shrink: 0;
        }

        .btn-okay:hover {
            background-color: #0ea5e9;
        }

        @media (max-width: 600px) {
            header h1 { font-size: 2rem; }
            .btn { width: 100%; justify-content: center; }
            .shield-btn { width: 55px; height: 55px; bottom: 20px; right: 20px; }
        }
    </style>
</head>
<body>
    <canvas id="particle-canvas"></canvas>

    <header>
        <div class="container slide-left reveal">
            <h1>Premium Social Media Services</h1>
            <p>Trusted • Private • Efficient — Services across Instagram, Twitter, WhatsApp, TikTok, Facebook, YouTube and more.</p>
            
            <div class="cta-buttons">
                <a href="https://t.me/resays" class="btn btn-telegram" target="_blank">
                    <i class="fa-brands fa-telegram"></i> Telegram
                </a>
                
                <a href="#" class="btn btn-whatsapp">
                    <i class="fa-brands fa-whatsapp" style="color: white;"></i> WhatsApp
                </a>
            </div>
        </div>
    </header>

    <div class="container">

        <h2 class="section-title reveal">Our Services</h2>
        <div class="services-grid">
            
            <div class="service-card reveal">
                <h3><i class="fa-brands fa-instagram"></i> Instagram</h3>
                <div class="service-item">
                    <span class="service-name">Removal</span>
                    <span class="service-price">Starting Price - $250</span><br>
                    <span class="service-time">Turnaround: 0-72 hours</span>
                </div>
                <div class="service-item">
                    <span class="service-name">Recovery</span>
                    <span class="service-price">Normal - $2500 | Copyright - $3500</span><br>
                    <span class="service-time">Turnaround: 0-24 hours</span>
                </div>
                <div class="service-item">
                    <span class="service-name">Verification</span>
                    <span class="service-price">Price - $7000+</span><br>
                    <span class="service-time">Turnaround: 0-1 week</span>
                </div>
            </div>

            <div class="service-card reveal">
                <h3><i class="fa-brands fa-twitter"></i> Twitter / X</h3>
                <div class="service-item">
                    <span class="service-name">Removal</span>
                    <span class="service-price">Starting Price - $5000</span><br>
                    <span class="service-time">Turnaround: 0-1 week</span>
                </div>
                <div class="service-item">
                    <span class="service-name">Recovery</span>
                    <span class="service-price">Starting Price - $10000</span><br>
                    <span class="service-time">Turnaround: 0-1 week</span>
                </div>
            </div>

            <div class="service-card reveal">
                <h3><i class="fa-brands fa-whatsapp"></i> WhatsApp</h3>
                <div class="service-item">
                    <span class="service-name">Removal (Ban)</span>
                    <span class="service-price">Price - $300</span><br>
                    <span class="service-time">Turnaround: 0-72 hours</span>
                </div>
                <div class="service-item">
                    <span class="service-name">Recovery (Unban)</span>
                    <span class="service-price">Price - $999</span><br>
                    <span class="service-time">Turnaround: 0-1 week</span>
                </div>
            </div>

            <div class="service-card reveal">
                <h3><i class="fa-brands fa-tiktok"></i> TikTok</h3>
                <div class="service-item">
                    <span class="service-name">Removal</span>
                    <span class="service-price">Starting Price - $299</span><br>
                    <span class="service-time">Turnaround: 0-48 hours</span>
                </div>
                <div class="service-item">
                    <span class="service-name">Verification</span>
                    <span class="service-price">Price - $5000</span><br>
                    <span class="service-time">Turnaround: 0-2 weeks</span>
                </div>
            </div>

            <div class="service-card reveal">
                <h3><i class="fa-brands fa-facebook"></i> Facebook</h3>
                <div class="service-item">
                    <span class="service-name">Removal</span>
                    <span class="service-price">Starting Price - $500</span><br>
                    <span class="service-time">Turnaround: 0-1 week</span>
                </div>
                <div class="service-item">
                    <span class="service-name">Recovery</span>
                    <span class="service-price">Starting Price - $3000</span><br>
                    <span class="service-time">Turnaround: 0-48 hours</span>
                </div>
            </div>

             <div class="service-card reveal">
                <h3><i class="fa-brands fa-youtube"></i> YouTube</h3>
                <div class="service-item">
                    <span class="service-name">Channel Removal</span>
                    <span class="service-price">Price - $3000</span><br>
                    <span class="service-time">Turnaround: 0-1 week</span>
                </div>
                <div class="service-item">
                    <span class="service-name">Video Removal</span>
                    <span class="service-price">Price - $500 per video</span><br>
                    <span class="service-time">Turnaround: 0-72 hours</span>
                </div>
            </div>

        </div>

        <h2 class="section-title reveal">Other Services</h2>
        <div class="info-box reveal">
            <p>We also provide services for other platforms like Reddit, OnlyFans, Airbnb, and more. Contact us via Telegram or WhatsApp.</p>
        </div>

        <h2 class="section-title reveal">Important Notice</h2>
        <div class="info-box reveal" style="border-left-color: #ef4444;">
            <p>We only perform account removals or takedowns for platforms if the account is violating the platform's community guidelines or copying your legally owned content.</p>
        </div>

        <h2 class="section-title reveal">FAQs</h2>
        <div class="info-box reveal">
            <p style="text-align: left; margin-bottom: 10px;"><strong>Q: How do I request a service?</strong><br>A: Click the Telegram or WhatsApp button above.</p>
            <p style="text-align: left; margin-bottom: 10px;"><strong>Q: How do I pay?</strong><br>A: Payment details are shared after inquiry. Secure methods only.</p>
            <p style="text-align: left;"><strong>Q: Do I get a refund if it fails?</strong><br>A: Yes, 100% refund if we fail to deliver.</p>
        </div>

    </div>

    <footer>
        <p>&copy; 2025 SMFixer.site — All Rights Reserved.</p>
    </footer>

    <div class="shield-btn" onclick="openPopup()">
        <i class="fas fa-shield-alt"></i>
    </div>

    <div id="tosPopup" class="modal-overlay">
        <div class="modal-content">
            <h2>Terms of Service</h2>
            
            <div class="tos-text">
                <p>Welcome to SMFixer. By using our services, you agree to the following terms:</p>
                <br>
                <ul>
                    <li>1. <strong>Confidentiality:</strong> All services are strictly confidential and private. We never share client data.</li>
                    <li>2. <strong>Payments:</strong> Payments must be made in advance or via escrow as agreed.</li>
                    <li>3. <strong>Refund Policy:</strong> We guarantee a full refund if the service is not delivered within the agreed timeframe.</li>
                    <li>4. <strong>Legal Use:</strong> We do not support illegal activities or hacking. Services are for recovery and policy-based takedowns only.</li>
                    <li>5. <strong>Turnaround Time:</strong> Turnaround times are estimates and may vary based on platform updates.</li>
                    <li>6. <strong>Verification:</strong> Verification services require legitimate press and notability.</li>
                    <li>7. <strong>Liability:</strong> We are not liable for platform policy changes that occur after service delivery.</li>
                </ul>
                <p>Please contact support for more details.</p>
            </div>
            
            <button class="btn-okay" onclick="closePopup()">Okay</button>
        </div>
    </div>

    <script>
        // --- MOTION BACKGROUND SCRIPT ---
        const canvas = document.getElementById('particle-canvas');
        const ctx = canvas.getContext('2d');
        canvas.width = window.innerWidth;
        canvas.height = window.innerHeight;

        let particlesArray;
        const numberOfParticles = (canvas.height * canvas.width) / 9000; // Adjust density here

        // Particle Class
        class Particle {
            constructor() {
                this.x = Math.random() * canvas.width;
                this.y = Math.random() * canvas.height;
                this.size = Math.random() * 2 + 1;
                this.speedX = Math.random() * 1 - 0.5;
                this.speedY = Math.random() * 1 - 0.5;
                this.color = 'rgba(56, 189, 248, 0.5)'; // Light Blue color for particles
            }
            update() {
                this.x += this.speedX;
                this.y += this.speedY;
                if (this.size > 0.2) this.size -= 0.1;
                if (this.x > canvas.width || this.x < 0) this.speedX = -this.speedX;
                if (this.y > canvas.height || this.y < 0) this.speedY = -this.speedY;
            }
            draw() {
                ctx.fillStyle = this.color;
                ctx.beginPath();
                ctx.arc(this.x, this.y, this.size, 0, Math.PI * 2);
                ctx.fill();
            }
        }

        function init() {
            particlesArray = [];
            for (let i = 0; i < numberOfParticles; i++) {
                particlesArray.push(new Particle());
            }
        }

        function animate() {
            ctx.clearRect(0, 0, canvas.width, canvas.height);
            for (let i = 0; i < particlesArray.length; i++) {
                particlesArray[i].update();
                particlesArray[i].draw();
                for (let j = i; j < particlesArray.length; j++) {
                    const dx = particlesArray[i].x - particlesArray[j].x;
                    const dy = particlesArray[i].y - particlesArray[j].y;
                    const distance = Math.sqrt(dx * dx + dy * dy);
                    if (distance < 100) {
                        ctx.beginPath();
                        ctx.strokeStyle = `rgba(56, 189, 248, ${1 - distance / 100})`; // Blue lines fading out
                        ctx.lineWidth = 0.5;
                        ctx.moveTo(particlesArray[i].x, particlesArray[i].y);
                        ctx.lineTo(particlesArray[j].x, particlesArray[j].y);
                        ctx.stroke();
                    }
                }
            }
            requestAnimationFrame(animate);
        }

        window.addEventListener('resize', function() {
            canvas.width = window.innerWidth;
            canvas.height = window.innerHeight;
            init();
        });

        init();
        animate();

        // --- EXISTING SCROLL REVEAL SCRIPT ---
        function reveal() {
            var reveals = document.querySelectorAll(".reveal");
            for (var i = 0; i < reveals.length; i++) {
                var windowHeight = window.innerHeight;
                var elementTop = reveals[i].getBoundingClientRect().top;
                var elementVisible = 100;
                if (elementTop < windowHeight - elementVisible) {
                    reveals[i].classList.add("active");
                }
            }
        }
        window.addEventListener("scroll", reveal);
        reveal();

        // --- EXISTING POPUP LOGIC ---
        function openPopup() {
            document.getElementById('tosPopup').classList.add('active');
            document.body.style.overflow = 'hidden'; 
        }

        function closePopup() {
            document.getElementById('tosPopup').classList.remove('active');
            document.body.style.overflow = 'auto'; 
        }
    </script>

</body>
</html>
