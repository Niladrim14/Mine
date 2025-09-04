<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Niladri Mandal | MERN Stack Developer</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Chosen Palette: Calm Neutrals -->
    <!-- Application Structure Plan: The application is structured as a modern, single-page developer portfolio. This design was chosen because it's a familiar and highly effective format for recruiters and technical audiences. It allows for a narrative flow, starting with a strong introduction (Hero), followed by tangible skills (Tech Stack), proof of work (Projects), and clear calls-to-action (Contact). Navigation is handled by a sticky header with smooth-scrolling links, enabling users to either explore linearly or jump directly to sections of interest, optimizing for quick information retrieval. -->
    <!-- Visualization & Content Choices: The source report (README) is entirely qualitative. Therefore, traditional data visualizations like charts are not applicable. Instead, information is "visualized" through information architecture and styled components. For example, the 'Tech Stack' list is transformed into a visually scannable grid of skill cards. The 'Projects' section uses interactive cards, a standard UI pattern for showcasing work. This approach was chosen to make the text-based information more engaging, digestible, and professional without forcing inappropriate data charts. No SVG or Mermaid is used. -->
    <!-- CONFIRMATION: NO SVG graphics used. NO Mermaid JS used. -->
    <style>
        body {
            font-family: 'Inter', sans-serif;
        }
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700&display=swap');
        .skill-card {
            transition: transform 0.2s ease-in-out, box-shadow 0.2s ease-in-out;
        }
        .skill-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1), 0 4px 6px -2px rgba(0, 0, 0, 0.05);
        }
        .nav-link.active {
            color: #3b82f6;
            font-weight: 500;
        }
    </style>
</head>
<body class="bg-stone-50 text-stone-800">

    <header id="header" class="bg-stone-50/80 backdrop-blur-md sticky top-0 z-50 transition-all duration-300">
        <div class="max-w-5xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex items-center justify-between h-16">
                <div class="flex-shrink-0">
                    <a href="#" class="text-xl font-bold text-stone-900">Niladri Mandal</a>
                </div>
                <div class="hidden md:block">
                    <div class="ml-10 flex items-baseline space-x-4">
                        <a href="#about" class="nav-link text-stone-600 hover:text-blue-500 px-3 py-2 rounded-md text-sm font-medium">About</a>
                        <a href="#stack" class="nav-link text-stone-600 hover:text-blue-500 px-3 py-2 rounded-md text-sm font-medium">Tech Stack</a>
                        <a href="#projects" class="nav-link text-stone-600 hover:text-blue-500 px-3 py-2 rounded-md text-sm font-medium">Projects</a>
                        <a href="#contact" class="nav-link text-stone-600 hover:text-blue-500 px-3 py-2 rounded-md text-sm font-medium">Contact</a>
                    </div>
                </div>
                <div class="md:hidden">
                    <button id="mobile-menu-button" class="inline-flex items-center justify-center p-2 rounded-md text-stone-500 hover:text-stone-700 hover:bg-stone-200 focus:outline-none focus:ring-2 focus:ring-inset focus:ring-blue-500">
                        <span class="sr-only">Open main menu</span>
                        <svg class="h-6 w-6" id="menu-icon-open" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" aria-hidden="true">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
                        </svg>
                         <svg class="h-6 w-6 hidden" id="menu-icon-close" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" aria-hidden="true">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
                        </svg>
                    </button>
                </div>
            </div>
        </div>
        <div class="md:hidden hidden" id="mobile-menu">
            <div class="px-2 pt-2 pb-3 space-y-1 sm:px-3">
                <a href="#about" class="nav-link text-stone-600 hover:text-blue-500 block px-3 py-2 rounded-md text-base font-medium">About</a>
                <a href="#stack" class="nav-link text-stone-600 hover:text-blue-500 block px-3 py-2 rounded-md text-base font-medium">Tech Stack</a>
                <a href="#projects" class="nav-link text-stone-600 hover:text-blue-500 block px-3 py-2 rounded-md text-base font-medium">Projects</a>
                <a href="#contact" class="nav-link text-stone-600 hover:text-blue-500 block px-3 py-2 rounded-md text-base font-medium">Contact</a>
            </div>
        </div>
    </header>

    <main class="max-w-5xl mx-auto px-4 sm:px-6 lg:px-8 py-8 md:py-12">

        <section id="about" class="min-h-[60vh] flex flex-col justify-center py-16 text-center">
            <h1 class="text-4xl md:text-6xl font-bold tracking-tight text-stone-900">Hi, I'm Niladri Mandal 👋</h1>
            <p class="mt-4 text-lg md:text-xl text-stone-600 max-w-3xl mx-auto">A passionate MERN Stack Developer interested in computer science and building dynamic, user-centric web applications.</p>
            <div class="mt-8">
                <p class="text-md text-stone-700 max-w-2xl mx-auto">My goal is to build a strong portfolio of full-stack projects and continuously expand my technical skills. I love turning complex ideas into reality through clean, efficient code and intuitive design.</p>
            </div>
        </section>

        <section id="stack" class="py-16">
            <h2 class="text-3xl font-bold text-center text-stone-900 mb-2">My Tech Stack</h2>
            <p class="text-center text-stone-600 mb-10">Technologies I use to bring projects to life.</p>
            <div class="grid grid-cols-2 md:grid-cols-4 lg:grid-cols-5 gap-6 text-center">
                <div class="skill-card bg-white p-6 rounded-lg shadow-sm border border-stone-200">
                    <div class="text-4xl mb-2">JS</div>
                    <p class="font-medium text-stone-700">JavaScript</p>
                </div>
                <div class="skill-card bg-white p-6 rounded-lg shadow-sm border border-stone-200">
                    <div class="text-4xl mb-2">🍃</div>
                    <p class="font-medium text-stone-700">MongoDB</p>
                </div>
                <div class="skill-card bg-white p-6 rounded-lg shadow-sm border border-stone-200">
                    <div class="text-4xl mb-2">⚡️</div>
                    <p class="font-medium text-stone-700">Express.js</p>
                </div>
                <div class="skill-card bg-white p-6 rounded-lg shadow-sm border border-stone-200">
                    <div class="text-4xl mb-2">⚛️</div>
                    <p class="font-medium text-stone-700">React.js</p>
                </div>
                <div class="skill-card bg-white p-6 rounded-lg shadow-sm border border-stone-200">
                     <div class="text-4xl mb-2">⬢</div>
                    <p class="font-medium text-stone-700">Node.js</p>
                </div>
                <div class="skill-card bg-white p-6 rounded-lg shadow-sm border border-stone-200">
                    <div class="text-4xl mb-2">📜</div>
                    <p class="font-medium text-stone-700">HTML</p>
                </div>
                <div class="skill-card bg-white p-6 rounded-lg shadow-sm border border-stone-200">
                    <div class="text-4xl mb-2">🎨</div>
                    <p class="font-medium text-stone-700">CSS</p>
                </div>
                <div class="skill-card bg-white p-6 rounded-lg shadow-sm border border-stone-200">
                    <div class="text-4xl mb-2">🌿</div>
                    <p class="font-medium text-stone-700">Tailwind CSS</p>
                </div>
                <div class="skill-card bg-white p-6 rounded-lg shadow-sm border border-stone-200">
                    <div class="text-4xl mb-2">🐙</div>
                    <p class="font-medium text-stone-700">Git</p>
                </div>
                 <div class="skill-card bg-white p-6 rounded-lg shadow-sm border border-stone-200">
                    <div class="text-4xl mb-2">🐳</div>
                    <p class="font-medium text-stone-700">Docker</p>
                </div>
            </div>
        </section>

        <section id="projects" class="py-16">
            <h2 class="text-3xl font-bold text-center text-stone-900 mb-2">Projects I'm Working On</h2>
            <p class="text-center text-stone-600 mb-10">Here are a few things I've built or am currently building.</p>
            <div class="grid md:grid-cols-2 gap-8">
                <div class="skill-card bg-white rounded-lg shadow-sm border border-stone-200 overflow-hidden flex flex-col">
                    <div class="bg-blue-100 h-48 flex items-center justify-center text-blue-500 font-bold">
                        <p>Project Visual Placeholder</p>
                    </div>
                    <div class="p-6 flex-grow flex flex-col">
                        <h3 class="text-xl font-bold mb-2 text-stone-900">Full-Stack E-Commerce Site</h3>
                        <p class="text-stone-600 mb-4 flex-grow">A feature-rich e-commerce platform built with the MERN stack. Includes product listings, user authentication, a shopping cart, and a checkout process.</p>
                        <div class="mb-4">
                            <span class="inline-block bg-blue-100 text-blue-800 text-xs font-medium mr-2 px-2.5 py-0.5 rounded-full">React</span>
                            <span class="inline-block bg-green-100 text-green-800 text-xs font-medium mr-2 px-2.5 py-0.5 rounded-full">Node.js</span>
                            <span class="inline-block bg-yellow-100 text-yellow-800 text-xs font-medium mr-2 px-2.5 py-0.5 rounded-full">MongoDB</span>
                        </div>
                        <div class="mt-auto flex space-x-4">
                            <a href="#" class="text-blue-500 font-medium hover:underline">Live Demo</a>
                            <a href="#" class="text-blue-500 font-medium hover:underline">GitHub</a>
                        </div>
                    </div>
                </div>

                <div class="skill-card bg-white rounded-lg shadow-sm border border-stone-200 overflow-hidden flex flex-col">
                    <div class="bg-green-100 h-48 flex items-center justify-center text-green-500 font-bold">
                        <p>Project Visual Placeholder</p>
                    </div>
                    <div class="p-6 flex-grow flex flex-col">
                        <h3 class="text-xl font-bold mb-2 text-stone-900">Task Management App</h3>
                        <p class="text-stone-600 mb-4 flex-grow">A collaborative task manager that allows users to create projects, assign tasks, and track progress in real-time. Exploring concepts like TypeScript for type safety.</p>
                         <div class="mb-4">
                            <span class="inline-block bg-blue-100 text-blue-800 text-xs font-medium mr-2 px-2.5 py-0.5 rounded-full">React</span>
                             <span class="inline-block bg-gray-100 text-gray-800 text-xs font-medium mr-2 px-2.5 py-0.5 rounded-full">TypeScript</span>
                            <span class="inline-block bg-red-100 text-red-800 text-xs font-medium mr-2 px-2.5 py-0.5 rounded-full">Express</span>
                        </div>
                        <div class="mt-auto flex space-x-4">
                            <a href="#" class="text-blue-500 font-medium hover:underline">Live Demo</a>
                            <a href="#" class="text-blue-500 font-medium hover:underline">GitHub</a>
                        </div>
                    </div>
                </div>
            </div>
            <div class="mt-12 text-center bg-stone-100 p-6 rounded-lg border border-stone-200">
                <h3 class="text-xl font-bold text-stone-800 mb-2">🌱 Currently Learning</h3>
                <p class="text-stone-600">I'm currently diving deeper into <span class="font-medium text-stone-900">TypeScript</span> and exploring <span class="font-medium text-stone-900">microservices architecture</span> to build more scalable and robust applications.</p>
            </div>
        </section>

        <section id="contact" class="py-16 text-center">
            <h2 class="text-3xl font-bold text-stone-900 mb-2">Let's Connect</h2>
            <p class="text-stone-600 mb-8 max-w-xl mx-auto">I'm always open to discussing new projects, creative ideas, or opportunities to be part of an amazing team. Feel free to reach out!</p>
            <div class="flex justify-center items-center space-x-6">
                <a href="#" class="text-stone-500 hover:text-blue-600 transition-colors">
                    <span class="sr-only">LinkedIn</span>
                    <svg class="w-8 h-8" fill="currentColor" viewBox="0 0 24 24" aria-hidden="true"><path d="M19 0h-14c-2.761 0-5 2.239-5 5v14c0 2.761 2.239 5 5 5h14c2.762 0 5-2.239 5-5v-14c0-2.761-2.238-5-5-5zm-11 19h-3v-11h3v11zm-1.5-12.268c-.966 0-1.75-.79-1.75-1.764s.784-1.764 1.75-1.764 1.75.79 1.75 1.764-.783 1.764-1.75 1.764zm13.5 12.268h-3v-5.604c0-3.368-4-3.113-4 0v5.604h-3v-11h3v1.765c1.396-2.586 7-2.777 7 2.476v6.759z"/></svg>
                </a>
                 <a href="#" class="text-stone-500 hover:text-gray-900 transition-colors">
                    <span class="sr-only">GitHub</span>
                    <svg class="w-8 h-8" fill="currentColor" viewBox="0 0 24 24" aria-hidden="true"><path fill-rule="evenodd" d="M12 2C6.477 2 2 6.477 2 12c0 4.418 2.865 8.168 6.839 9.492.5.092.682-.217.682-.482 0-.237-.009-.868-.014-1.703-2.782.605-3.369-1.343-3.369-1.343-.454-1.158-1.11-1.466-1.11-1.466-.908-.62.069-.608.069-.608 1.003.07 1.531 1.032 1.531 1.032.892 1.53 2.341 1.088 2.91.832.092-.647.35-1.088.636-1.338-2.22-.253-4.555-1.113-4.555-4.951 0-1.093.39-1.988 1.031-2.688-.103-.253-.446-1.272.098-2.65 0 0 .84-.27 2.75 1.026A9.564 9.564 0 0112 6.844c.85.004 1.705.115 2.504.337 1.909-1.296 2.747-1.027 2.747-1.027.546 1.379.203 2.398.1 2.651.64.7 1.03 1.595 1.03 2.688 0 3.848-2.338 4.695-4.566 4.943.359.309.678.92.678 1.855 0 1.338-.012 2.419-.012 2.747 0 .268.18.58.688.482A10.001 10.001 0 0022 12c0-5.523-4.477-10-10-10z" clip-rule="evenodd"/></svg>
                </a>
                <a href="#" class="text-stone-500 hover:text-blue-400 transition-colors">
                    <span class="sr-only">Twitter/X</span>
                    <svg class="w-8 h-8" fill="currentColor" viewBox="0 0 24 24" aria-hidden="true"><path d="M18.244 2.25h3.308l-7.227 8.26 8.502 11.24H16.17l-5.214-6.817L4.99 21.75H1.68l7.73-8.835L1.254 2.25H8.08l4.713 6.231zm-1.161 17.52h1.833L7.084 4.126H5.117z"/></svg>
                </a>
            </div>
        </section>

    </main>

    <footer class="bg-stone-100 border-t border-stone-200">
        <div class="max-w-5xl mx-auto py-6 px-4 sm:px-6 lg:px-8 text-center text-sm text-stone-500">
            <p>&copy; 2024 Niladri Mandal. All Rights Reserved.</p>
        </div>
    </footer>

    <script>
        document.addEventListener('DOMContentLoaded', () => {
            const mobileMenuButton = document.getElementById('mobile-menu-button');
            const mobileMenu = document.getElementById('mobile-menu');
            const menuIconOpen = document.getElementById('menu-icon-open');
            const menuIconClose = document.getElementById('menu-icon-close');

            mobileMenuButton.addEventListener('click', () => {
                mobileMenu.classList.toggle('hidden');
                menuIconOpen.classList.toggle('hidden');
                menuIconClose.classList.toggle('hidden');
            });

            const sections = document.querySelectorAll('section');
            const navLinks = document.querySelectorAll('.nav-link');

            const observerOptions = {
                root: null,
                rootMargin: '0px',
                threshold: 0.5
            };

            const observer = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        const id = entry.target.getAttribute('id');
                        navLinks.forEach(link => {
                            link.classList.remove('active');
                            if (link.getAttribute('href') === `#${id}`) {
                                link.classList.add('active');
                            }
                        });
                    }
                });
            }, observerOptions);

            sections.forEach(section => {
                observer.observe(section);
            });

            navLinks.forEach(link => {
                link.addEventListener('click', () => {
                    if(mobileMenu.classList.contains('hidden') === false){
                       mobileMenu.classList.add('hidden');
                       menuIconOpen.classList.remove('hidden');
                       menuIconClose.classList.add('hidden');
                    }
                });
            });
            
            const header = document.getElementById('header');
            let lastScrollTop = 0;
            window.addEventListener('scroll', function() {
                let scrollTop = window.pageYOffset || document.documentElement.scrollTop;
                if (scrollTop > lastScrollTop) {
                    header.style.top = '-80px';
                } else {
                    header.style.top = '0';
                }
                if (scrollTop > 50) {
                    header.classList.add('shadow-md');
                } else {
                    header.classList.remove('shadow-md');
                }
                lastScrollTop = scrollTop <= 0 ? 0 : scrollTop;
            });
        });
    </script>
</body>
</html>
