<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GitHub Profile README</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        @keyframes float {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-10px); }
        }
        .float-animation {
            animation: float 3s ease-in-out infinite;
        }
        .gradient-text {
            background-clip: text;
            -webkit-background-clip: text;
            color: transparent;
            background-image: linear-gradient(90deg, #3b82f6, #8b5cf6);
        }
        .card-hover {
            transition: all 0.3s ease;
        }
        .card-hover:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.1);
        }
        .typewriter {
            overflow: hidden;
            border-right: .15em solid #3b82f6;
            white-space: nowrap;
            letter-spacing: .15em;
            animation: typing 3.5s steps(40, end), blink-caret .75s step-end infinite;
        }
        @keyframes typing {
            from { width: 0 }
            to { width: 100% }
        }
        @keyframes blink-caret {
            from, to { border-color: transparent }
            50% { border-color: #3b82f6; }
        }
    </style>
</head>
<body class="bg-gray-50 min-h-screen font-sans">
    <div class="container mx-auto px-4 py-12 max-w-4xl">
        <!-- Header Section -->
        <header class="flex flex-col md:flex-row items-center justify-between mb-16">
            <div class="flex items-center mb-6 md:mb-0">
                <img src="https://avatars.githubusercontent.com/u/583231?v=4" alt="Profile" class="w-24 h-24 rounded-full border-4 border-white shadow-lg float-animation">
                <div class="ml-6">
                    <h1 class="text-3xl font-bold text-gray-800">Hi there, I'm <span class="gradient-text">Your Name</span> 👋</h1>
                    <p class="text-gray-600 mt-1">Full Stack Developer | Open Source Enthusiast</p>
                </div>
            </div>
            <div class="flex space-x-4">
                <a href="#" class="bg-gray-800 hover:bg-gray-700 text-white px-4 py-2 rounded-lg flex items-center transition">
                    <i class="fab fa-github mr-2"></i> GitHub
                </a>
                <a href="#" class="bg-blue-600 hover:bg-blue-500 text-white px-4 py-2 rounded-lg flex items-center transition">
                    <i class="fab fa-linkedin mr-2"></i> LinkedIn
                </a>
            </div>
        </header>

        <!-- About Section -->
        <section class="mb-16 bg-white rounded-xl p-8 shadow-md card-hover">
            <h2 class="text-2xl font-bold text-gray-800 mb-4 flex items-center">
                <i class="fas fa-user mr-3 text-blue-500"></i> About Me
            </h2>
            <p class="text-gray-700 mb-4">
                I'm a passionate developer with expertise in JavaScript, React, Node.js, and cloud technologies. 
                I love building scalable applications and contributing to open-source projects.
            </p>
            <div class="flex flex-wrap gap-2 mt-4">
                <span class="bg-blue-100 text-blue-800 px-3 py-1 rounded-full text-sm">Full Stack</span>
                <span class="bg-purple-100 text-purple-800 px-3 py-1 rounded-full text-sm">DevOps</span>
                <span class="bg-green-100 text-green-800 px-3 py-1 rounded-full text-sm">Open Source</span>
                <span class="bg-yellow-100 text-yellow-800 px-3 py-1 rounded-full text-sm">Cloud</span>
            </div>
        </section>

        <!-- Stats Section -->
        <section class="mb-16 grid grid-cols-1 md:grid-cols-3 gap-4">
            <div class="bg-white p-6 rounded-xl shadow-md flex items-center card-hover">
                <div class="bg-blue-100 p-3 rounded-full mr-4">
                    <i class="fas fa-code text-blue-600 text-xl"></i>
                </div>
                <div>
                    <p class="text-gray-500 text-sm">Repositories</p>
                    <h3 class="text-2xl font-bold text-gray-800">42</h3>
                </div>
            </div>
            <div class="bg-white p-6 rounded-xl shadow-md flex items-center card-hover">
                <div class="bg-purple-100 p-3 rounded-full mr-4">
                    <i class="fas fa-star text-purple-600 text-xl"></i>
                </div>
                <div>
                    <p class="text-gray-500 text-sm">Stars</p>
                    <h3 class="text-2xl font-bold text-gray-800">128</h3>
                </div>
            </div>
            <div class="bg-white p-6 rounded-xl shadow-md flex items-center card-hover">
                <div class="bg-green-100 p-3 rounded-full mr-4">
                    <i class="fas fa-code-branch text-green-600 text-xl"></i>
                </div>
                <div>
                    <p class="text-gray-500 text-sm">Contributions</p>
                    <h3 class="text-2xl font-bold text-gray-800">56</h3>
                </div>
            </div>
        </section>

        <!-- Projects Section -->
        <section class="mb-16">
            <h2 class="text-2xl font-bold text-gray-800 mb-6 flex items-center">
                <i class="fas fa-project-diagram mr-3 text-blue-500"></i> Featured Projects
            </h2>
            <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                <div class="bg-white rounded-xl p-6 shadow-md card-hover">
                    <div class="flex justify-between items-start mb-3">
                        <h3 class="text-xl font-bold text-gray-800">Awesome Project</h3>
                        <span class="bg-blue-100 text-blue-800 px-2 py-1 rounded text-xs">JavaScript</span>
                    </div>
                    <p class="text-gray-600 mb-4">A modern web application built with React and Node.js that solves real-world problems.</p>
                    <div class="flex justify-between items-center">
                        <div class="flex space-x-2">
                            <span class="text-gray-500 text-sm"><i class="fas fa-star mr-1"></i> 42</span>
                            <span class="text-gray-500 text-sm"><i class="fas fa-code-branch mr-1"></i> 5</span>
                        </div>
                        <a href="#" class="text-blue-500 hover:text-blue-600 text-sm font-medium">View Project →</a>
                    </div>
                </div>
                <div class="bg-white rounded-xl p-6 shadow-md card-hover">
                    <div class="flex justify-between items-start mb-3">
                        <h3 class="text-xl font-bold text-gray-800">Dev Tools</h3>
                        <span class="bg-purple-100 text-purple-800 px-2 py-1 rounded text-xs">TypeScript</span>
                    </div>
                    <p class="text-gray-600 mb-4">A collection of developer tools to boost productivity and streamline workflows.</p>
                    <div class="flex justify-between items-center">
                        <div class="flex space-x-2">
                            <span class="text-gray-500 text-sm"><i class="fas fa-star mr-1"></i> 86</span>
                            <span class="text-gray-500 text-sm"><i class="fas fa-code-branch mr-1"></i> 12</span>
                        </div>
                        <a href="#" class="text-blue-500 hover:text-blue-600 text-sm font-medium">View Project →</a>
                    </div>
                </div>
            </div>
        </section>

        <!-- Skills Section -->
        <section class="mb-16">
            <h2 class="text-2xl font-bold text-gray-800 mb-6 flex items-center">
                <i class="fas fa-laptop-code mr-3 text-blue-500"></i> Skills & Technologies
            </h2>
            <div class="bg-white rounded-xl p-6 shadow-md">
                <div class="grid grid-cols-2 md:grid-cols-4 gap-4">
                    <div class="flex items-center p-3 rounded-lg bg-gray-50">
                        <i class="fab fa-js text-yellow-400 text-2xl mr-3"></i>
                        <span class="font-medium">JavaScript</span>
                    </div>
                    <div class="flex items-center p-3 rounded-lg bg-gray-50">
                        <i class="fab fa-react text-blue-400 text-2xl mr-3"></i>
                        <span class="font-medium">React</span>
                    </div>
                    <div class="flex items-center p-3 rounded-lg bg-gray-50">
                        <i class="fab fa-node-js text-green-500 text-2xl mr-3"></i>
                        <span class="font-medium">Node.js</span>
                    </div>
                    <div class="flex items-center p-3 rounded-lg bg-gray-50">
                        <i class="fab fa-python text-blue-600 text-2xl mr-3"></i>
                        <span class="font-medium">Python</span>
                    </div>
                    <div class="flex items-center p-3 rounded-lg bg-gray-50">
                        <i class="fas fa-database text-blue-700 text-2xl mr-3"></i>
                        <span class="font-medium">SQL</span>
                    </div>
                    <div class="flex items-center p-3 rounded-lg bg-gray-50">
                        <i class="fab fa-aws text-orange-500 text-2xl mr-3"></i>
                        <span class="font-medium">AWS</span>
                    </div>
                    <div class="flex items-center p-3 rounded-lg bg-gray-50">
                        <i class="fas fa-server text-green-600 text-2xl mr-3"></i>
                        <span class="font-medium">Docker</span>
                    </div>
                    <div class="flex items-center p-3 rounded-lg bg-gray-50">
                        <i class="fab fa-git-alt text-orange-600 text-2xl mr-3"></i>
                        <span class="font-medium">Git</span>
                    </div>
                </div>
            </div>
        </section>

        <!-- Contact Section -->
        <section class="bg-gradient-to-r from-blue-500 to-purple-600 rounded-xl p-8 text-white">
            <h2 class="text-2xl font-bold mb-4">Let's Connect!</h2>
            <p class="mb-6">I'm always open to collaborating on interesting projects or just chatting about tech.</p>
            <div class="flex flex-wrap gap-4">
                <a href="#" class="bg-white text-blue-600 hover:bg-gray-100 px-5 py-2 rounded-lg font-medium flex items-center transition">
                    <i class="fas fa-envelope mr-2"></i> Email Me
                </a>
                <a href="#" class="bg-transparent border border-white hover:bg-white hover:bg-opacity-10 px-5 py-2 rounded-lg font-medium flex items-center transition">
                    <i class="fab fa-twitter mr-2"></i> Twitter
                </a>
                <a href="#" class="bg-transparent border border-white hover:bg-white hover:bg-opacity-10 px-5 py-2 rounded-lg font-medium flex items-center transition">
                    <i class="fab fa-linkedin-in mr-2"></i> LinkedIn
                </a>
            </div>
        </section>

        <!-- Footer -->
        <footer class="mt-12 text-center text-gray-500">
            <p>Made with <i class="fas fa-heart text-red-500"></i> and JavaScript</p>
            <p class="mt-2 text-sm">© 2023 Your Name. All rights reserved.</p>
        </footer>
    </div>

    <script>
        // Typewriter effect for the header
        document.addEventListener('DOMContentLoaded', function() {
            const phrases = [
                "Full Stack Developer",
                "Open Source Enthusiast",
                "Tech Blogger",
                "Cloud Architect",
                "Problem Solver"
            ];
            let currentPhrase = 0;
            const subtitle = document.querySelector('.typewriter');
            
            function typeWriter() {
                if (subtitle) {
                    subtitle.textContent = phrases[currentPhrase];
                    subtitle.style.animation = 'none';
                    void subtitle.offsetWidth; // Trigger reflow
                    subtitle.style.animation = 'typing 3.5s steps(40, end), blink-caret .75s step-end infinite';
                    
                    currentPhrase = (currentPhrase + 1) % phrases.length;
                    setTimeout(typeWriter, 4000);
                }
            }
            
            // Start the typewriter effect
            setTimeout(typeWriter, 1000);
            
            // Add hover effects to cards
            const cards = document.querySelectorAll('.card-hover');
            cards.forEach(card => {
                card.addEventListener('mouseenter', () => {
                    card.style.transform = 'translateY(-5px)';
                    card.style.boxShadow = '0 10px 25px -5px rgba(0, 0, 0, 0.1)';
                });
                card.addEventListener('mouseleave', () => {
                    card.style.transform = '';
                    card.style.boxShadow = '';
                });
            });
        });
    </script>
</body>
</html>
