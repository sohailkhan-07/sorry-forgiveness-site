<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Heartfelt Apology</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@100..900&display=swap" rel="stylesheet">
    
    <style>
        /* Custom CSS for Animations and Particles */
        :root {
            --primary-color: #ff69b4; /* Hot Pink for love/apology */
            --secondary-color: #f7a8b8; /* Lighter Pink */
        }
        
        body {
            font-family: 'Inter', sans-serif;
            background: linear-gradient(135deg, #fce3e7 0%, #fff0f5 100%);
            overflow: hidden; /* Hide scrollbars, manage content visibility with JS */
        }

        /* 1. Pulse Animation for the initial button/card */
        @keyframes pulse-once {
            0% { transform: scale(0.95); opacity: 0.7; }
            50% { transform: scale(1.05); opacity: 1; }
            100% { transform: scale(1); opacity: 1; }
        }

        .pulse-effect {
            animation: pulse-once 1.5s cubic-bezier(0.25, 0.46, 0.45, 0.94) forwards;
        }

        /* 2. Confetti/Heart Particle Effect */
        .heart-particle {
            position: absolute;
            width: 15px;
            height: 15px;
            background-color: var(--primary-color);
            transform: rotate(45deg);
            z-index: 50;
            pointer-events: none;
            opacity: 0;
            will-change: transform, opacity;
        }

        .heart-particle::before,
        .heart-particle::after {
            content: "";
            position: absolute;
            width: 15px;
            height: 15px;
            border-radius: 50%;
            background-color: var(--primary-color);
        }

        .heart-particle::before {
            top: -50%;
            left: 0;
        }

        .heart-particle::after {
            top: 0;
            left: 50%;
        }

        /* Keyframes for falling/exploding hearts */
        @keyframes fall {
            0% { opacity: 1; transform: translate(0, 0) rotate(0deg); }
            100% { opacity: 0; transform: translate(var(--x), var(--y)) rotate(var(--r)); }
        }

        /* 3. Main SORRY reveal animation */
        @keyframes pop-in {
            0% { opacity: 0; transform: scale(0.5) translateY(50px); }
            80% { opacity: 1; transform: scale(1.05) translateY(0); }
            100% { transform: scale(1); }
        }
        
        #apology-content {
            display: none;
            animation: pop-in 1s cubic-bezier(0.68, -0.55, 0.27, 1.55) forwards;
        }
    </style>
</head>
<body class="flex items-center justify-center min-h-screen p-4">

    <!-- 1. Initial Greeting Card -->
    <div id="initial-card" class="w-full max-w-md bg-white p-8 rounded-2xl shadow-2xl text-center transition-all duration-700 pulse-effect">
        <p class="text-3xl mb-4 text-pink-600 font-extrabold">A Special Message</p>
        <p class="text-gray-700 mb-6 text-lg">
            I have a small, heartfelt message just for you.
            <br>
            Would you like to open it?
        </p>
        <button id="reveal-button" 
                class="px-8 py-3 bg-pink-500 text-white font-bold text-xl rounded-full shadow-lg 
                       hover:bg-pink-600 transition-all duration-300 transform hover:scale-105 
                       focus:outline-none focus:ring-4 focus:ring-pink-300">
            Yes, I would!
        </button>
    </div>

    <!-- 2. Apology Content (Initially Hidden) -->
    <div id="apology-content" class="w-full max-w-2xl p-6 md:p-12 text-center transition-all duration-1000 bg-white/90 backdrop-blur-md rounded-3xl shadow-3xl absolute inset-0 flex flex-col justify-center items-center">
        
        <!-- Main SORRY Header -->
        <h1 class="text-7xl md:text-9xl font-black mb-6 text-transparent bg-clip-text 
                   bg-gradient-to-r from-red-500 to-pink-600 drop-shadow-lg">
            SORRY!
        </h1>
        
        <!-- Animated Message -->
        <p class="text-3xl md:text-5xl font-extrabold text-pink-700 mb-8 animate-bounce-slow">
            <span id="animated-text"></span>
        </p>

        <!-- Detailed Apology Text -->
        <div class="bg-pink-50 p-6 rounded-xl shadow-inner max-w-xl mx-auto">
            <p class="text-gray-800 text-lg md:text-xl leading-relaxed">
                I know I was wrong. My words or actions have hurt you, and I am truly sorry. You are the most special person in the world to me, and I can't stand seeing you upset.
                <br><br>
                Please, just give me one last chance. I promise this will never happen again.
            </p>
        </div>
        
        <p class="mt-8 text-2xl font-semibold text-red-500">
            Please forgive me!
        </p>

    </div>

    <!-- Particle Container for Hearts -->
    <div id="particle-container" class="absolute inset-0 z-40 pointer-events-none"></div>

    <script>
        const revealButton = document.getElementById('reveal-button');
        const initialCard = document.getElementById('initial-card');
        const apologyContent = document.getElementById('apology-content');
        const animatedText = document.getElementById('animated-text');
        const particleContainer = document.getElementById('particle-container');

        // State machine for the apology text animation
        const messages = [
            "I sincerely apologize from the bottom of my heart.",
            "I'm truly sorry...",
            "Your anger deeply hurts me.",
            "Please, forgive me! 🙏",
            "Sorry!"
        ];
        let messageIndex = 0;
        let charIndex = 0;
        let isDeleting = false;
        let typingSpeed = 100;

        function typeApology() {
            const currentMessage = messages[messageIndex];
            
            if (isDeleting) {
                // Delete mode
                animatedText.textContent = currentMessage.substring(0, charIndex - 1);
                charIndex--;
                typingSpeed = 50; // Faster deletion
            } else {
                // Type mode
                animatedText.textContent = currentMessage.substring(0, charIndex + 1);
                charIndex++;
                typingSpeed = 100; // Normal typing speed
            }

            if (!isDeleting && charIndex === currentMessage.length) {
                // Done typing current message, start deleting after a pause
                isDeleting = true;
                typingSpeed = 1000; // Pause
            } else if (isDeleting && charIndex === 0) {
                // Done deleting, move to next message and start typing
                isDeleting = false;
                messageIndex = (messageIndex + 1) % messages.length;
                typingSpeed = 150; // Slight pause before next word
            }

            // Loop the typing/deleting process
            setTimeout(typeApology, typingSpeed);
        }

        // --- Confetti/Heart Particle Generator ---
        function createHeartParticle() {
            const heart = document.createElement('div');
            heart.classList.add('heart-particle');
            
            // Random initial position (start from the top center)
            const startX = window.innerWidth / 2;
            const startY = -20; 
            
            heart.style.left = `${startX + (Math.random() - 0.5) * 400}px`;
            heart.style.top = `${startY}px`;

            // Set variables for fall animation
            const xFinal = (Math.random() - 0.5) * 800; // +/- 400px movement
            const yFinal = window.innerHeight + 100; // Fall past the screen
            const rotation = Math.random() * 720 - 360; // Random rotation

            heart.style.setProperty('--x', `${xFinal}px`);
            heart.style.setProperty('--y', `${yFinal}px`);
            heart.style.setProperty('--r', `${rotation}deg`);

            // Random duration and delay for the fall
            const duration = 5 + Math.random() * 5; // 5 to 10 seconds
            const delay = Math.random() * 2; // 0 to 2 seconds

            heart.style.animation = `fall ${duration}s linear ${delay}s forwards`;
            
            particleContainer.appendChild(heart);

            // Clean up the element after it finishes falling
            setTimeout(() => {
                heart.remove();
            }, (duration + delay) * 1000);
        }

        // --- Main Reveal Logic ---
        revealButton.addEventListener('click', () => {
            // 1. Hide the initial card
            initialCard.classList.remove('pulse-effect');
            initialCard.classList.add('opacity-0', 'scale-75');
            
            // Wait for the transition to finish before swapping content
            setTimeout(() => {
                initialCard.style.display = 'none';
                
                // 2. Show the apology content
                apologyContent.style.display = 'flex';
                
                // 3. Start the typing animation
                typeApology();

                // 4. Start the continuous particle effect (confetti/hearts)
                const particleInterval = setInterval(createHeartParticle, 100);
                
                // Optional: Stop the particle effect after a minute (60 seconds)
                // If you want it to run indefinitely, comment out the line below.
                // setTimeout(() => clearInterval(particleInterval), 60000);

            }, 700); // Wait 700ms for the scale/opacity transition on the initial card
        });
    </script>

</body>
</html>
