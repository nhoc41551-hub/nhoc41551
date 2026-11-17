<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nguyen Thai Hoc | IT Student & Aspiring Software Engineer</title>
    <meta name="description" content="Personal Portfolio & CV of Nguyen Thai Hoc - Information Technology student at Hanoi Polytechnic College. Aspiring Software Developer specializing in Web & Java development.">
    <meta name="keywords" content="Nguyen Thai Hoc, Portfolio, Hanoi Polytechnic College, IT Student, Software Developer, Java, MySQL, Web Developer">
    <meta name="author" content="Nguyen Thai Hoc">

    <!-- Google Fonts: Plus Jakarta Sans & JetBrains Mono -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=JetBrains+Mono:wght@400;500;600&family=Plus+Jakarta+Sans:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">

    <!-- Font Awesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">

    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <script>
        tailwind.config = {
            darkMode: 'class',
            theme: {
                extend: {
                    colors: {
                        primary: {
                            50: '#eef2ff',
                            100: '#e0e7ff',
                            500: '#6366f1',
                            600: '#4f46e5',
                            700: '#4338ca',
                            900: '#1e1b4b',
                        },
                        accent: {
                            cyan: '#06b6d4',
                            blue: '#0284c7',
                        },
                        dark: {
                            bg: '#0b0f19',
                            card: '#111827',
                            border: '#1f2937',
                            hover: '#1e293b'
                        }
                    },
                    fontFamily: {
                        sans: ['"Plus Jakarta Sans"', 'sans-serif'],
                        mono: ['"JetBrains Mono"', 'monospace'],
                    }
                }
            }
        }
    </script>

    <style>
        * {
            transition: background-color 0.25s ease, border-color 0.25s ease;
        }
        .glow-effect {
            box-shadow: 0 0 45px -10px rgba(99, 102, 241, 0.4);
        }
        .card-blur {
            backdrop-filter: blur(14px);
            -webkit-backdrop-filter: blur(14px);
        }
    </style>
</head>
<body class="bg-slate-50 dark:bg-dark-bg text-slate-800 dark:text-slate-200 font-sans antialiased selection:bg-indigo-500 selection:text-white">

    <!-- ================= NAVBAR ================= -->
    <header class="fixed top-0 left-0 w-full z-50 bg-white/85 dark:bg-dark-bg/85 card-blur border-b border-slate-200 dark:border-dark-border">
        <div class="max-w-7xl mx-auto px-6 h-20 flex items-center justify-between">
            <!-- Brand Logo -->
            <a href="#home" class="flex items-center gap-3 group">
                <span class="w-10 h-10 rounded-xl bg-gradient-to-tr from-indigo-600 via-primary-500 to-accent-cyan flex items-center justify-center text-white font-bold text-lg shadow-md shadow-indigo-500/20 group-hover:scale-105 transition-transform">
                    TH
                </span>
                <div class="flex flex-col">
                    <span class="font-bold text-lg tracking-tight text-slate-900 dark:text-white group-hover:text-indigo-600 dark:group-hover:text-indigo-400 transition-colors">
                        Nguyen Thai Hoc
                    </span>
                    <span class="text-xs text-slate-500 dark:text-slate-400 font-mono">HPC • IT Student</span>
                </div>
            </a>

            <!-- Desktop Nav Links -->
            <nav class="hidden md:flex items-center gap-7 text-sm font-medium">
                <a href="#home" class="text-slate-600 dark:text-slate-300 hover:text-indigo-600 dark:hover:text-indigo-400 transition-colors">Home</a>
                <a href="#about" class="text-slate-600 dark:text-slate-300 hover:text-indigo-600 dark:hover:text-indigo-400 transition-colors">About</a>
                <a href="#education" class="text-slate-600 dark:text-slate-300 hover:text-indigo-600 dark:hover:text-indigo-400 transition-colors">Education</a>
                <a href="#skills" class="text-slate-600 dark:text-slate-300 hover:text-indigo-600 dark:hover:text-indigo-400 transition-colors">Skills</a>
                <a href="#projects" class="text-slate-600 dark:text-slate-300 hover:text-indigo-600 dark:hover:text-indigo-400 transition-colors">Projects</a>
                <a href="#experience" class="text-slate-600 dark:text-slate-300 hover:text-indigo-600 dark:hover:text-indigo-400 transition-colors">Experience</a>
                <a href="#contact" class="text-slate-600 dark:text-slate-300 hover:text-indigo-600 dark:hover:text-indigo-400 transition-colors">Contact</a>
            </nav>

            <!-- Actions: Dark Mode Toggle & Quick Phone CTA -->
            <div class="flex items-center gap-3">
                <!-- Phone Quick Action -->
                <a href="tel:0367730151" class="hidden xl:inline-flex items-center gap-2 px-3.5 py-2 rounded-xl bg-slate-100 dark:bg-slate-800 text-xs font-semibold text-slate-700 dark:text-slate-200 hover:text-indigo-600 transition">
                    <i class="fa-solid fa-phone text-emerald-500"></i>
                    <span>0367 730 151</span>
                </a>

                <!-- Theme Toggle Button -->
                <button id="themeToggle" aria-label="Toggle Dark Mode" class="w-10 h-10 rounded-xl border border-slate-200 dark:border-dark-border bg-slate-100 dark:bg-slate-800/80 flex items-center justify-center text-slate-600 dark:text-amber-400 hover:bg-slate-200 dark:hover:bg-slate-700 transition">
                    <i id="themeIcon" class="fa-solid fa-moon"></i>
                </button>

                <!-- Primary CTA Button -->
                <a href="#contact" class="hidden sm:inline-flex items-center gap-2 px-5 py-2.5 rounded-xl bg-gradient-to-r from-indigo-600 to-accent-cyan text-white text-sm font-semibold hover:shadow-lg hover:shadow-indigo-500/25 hover:-translate-y-0.5 active:translate-y-0 transition-all">
                    <span>Contact Me</span>
                    <i class="fa-solid fa-arrow-right text-xs"></i>
                </a>

                <!-- Mobile Menu Button -->
                <button id="mobileMenuBtn" aria-label="Toggle navigation" class="md:hidden w-10 h-10 rounded-xl border border-slate-200 dark:border-dark-border bg-slate-100 dark:bg-slate-800 flex items-center justify-center text-slate-700 dark:text-slate-200">
                    <i class="fa-solid fa-bars"></i>
                </button>
            </div>
        </div>

        <!-- Mobile Drawer Menu -->
        <div id="mobileMenu" class="hidden md:hidden border-t border-slate-200 dark:border-dark-border bg-white dark:bg-dark-bg px-6 py-6 space-y-4">
            <a href="#home" class="mobile-nav-link block text-base font-medium text-slate-700 dark:text-slate-200">Home</a>
            <a href="#about" class="mobile-nav-link block text-base font-medium text-slate-700 dark:text-slate-200">About Me</a>
            <a href="#education" class="mobile-nav-link block text-base font-medium text-slate-700 dark:text-slate-200">Education & Campus</a>
            <a href="#skills" class="mobile-nav-link block text-base font-medium text-slate-700 dark:text-slate-200">Skills</a>
            <a href="#projects" class="mobile-nav-link block text-base font-medium text-slate-700 dark:text-slate-200">Projects</a>
            <a href="#experience" class="mobile-nav-link block text-base font-medium text-slate-700 dark:text-slate-200">Experience</a>
            <a href="#contact" class="mobile-nav-link block text-base font-medium text-slate-700 dark:text-slate-200">Contact</a>
            <div class="pt-2 flex flex-col gap-2">
                <a href="tel:0367730151" class="w-full py-3 rounded-xl border border-slate-300 dark:border-dark-border text-slate-800 dark:text-slate-200 font-semibold flex items-center justify-center gap-2">
                    <i class="fa-solid fa-phone text-emerald-500"></i>
                    <span>Call: 0367 730 151</span>
                </a>
                <a href="#contact" class="w-full py-3 rounded-xl bg-indigo-600 text-white font-semibold flex items-center justify-center gap-2">
                    <i class="fa-regular fa-envelope"></i>
                    <span>Get in Touch</span>
                </a>
            </div>
        </div>
    </header>

    <!-- ================= HERO SECTION ================= -->
    <section id="home" class="pt-32 pb-20 md:pt-40 md:pb-32 overflow-hidden relative">
        <div class="absolute -top-32 -left-32 w-96 h-96 bg-indigo-500/15 dark:bg-indigo-600/15 rounded-full blur-3xl pointer-events-none"></div>
        <div class="absolute top-1/2 -right-32 w-96 h-96 bg-cyan-500/15 dark:bg-cyan-600/15 rounded-full blur-3xl pointer-events-none"></div>

        <div class="max-w-7xl mx-auto px-6 grid grid-cols-1 lg:grid-cols-12 gap-12 lg:gap-8 items-center">
            
            <!-- Left Column: Introduction -->
            <div class="lg:col-span-7 space-y-6 text-center lg:text-left">
                <!-- Status Badge -->
                <div class="inline-flex items-center gap-2.5 px-4 py-2 rounded-full border border-emerald-500/30 bg-emerald-50 dark:bg-emerald-950/40 text-emerald-700 dark:text-emerald-400 text-xs font-semibold uppercase tracking-wider">
                    <span class="w-2.5 h-2.5 rounded-full bg-emerald-500 animate-pulse"></span>
                    Available for IT Internships & Web Projects
                </div>

                <!-- Main Greeting -->
                <div>
                    <p class="text-slate-500 dark:text-slate-400 font-medium text-lg mb-2">Hello, I am</p>
                    <h1 class="text-4xl sm:text-5xl lg:text-6xl font-extrabold text-slate-900 dark:text-white tracking-tight leading-tight">
                        Nguyen Thai Hoc
                    </h1>
                    <div class="mt-3 flex items-center justify-center lg:justify-start gap-3">
                        <span class="h-1 w-10 bg-indigo-600 rounded-full hidden sm:block"></span>
                        <h2 class="text-xl sm:text-2xl font-bold bg-gradient-to-r from-indigo-600 to-accent-cyan bg-clip-text text-transparent">
                            Information Technology Student
                        </h2>
                    </div>
                </div>

                <!-- Bio Summary -->
                <p class="text-base sm:text-lg text-slate-600 dark:text-slate-300 max-w-2xl mx-auto lg:mx-0 leading-relaxed font-normal">
                    Currently pursuing an Information Technology degree at <strong class="text-slate-900 dark:text-white font-semibold">Hanoi Polytechnic College</strong> (322 My Dinh Street, Hanoi). Focused on software engineering, website development, and database architecture with a drive to create impactful technology solutions.
                </p>

                <!-- CTA Actions -->
                <div class="pt-2 flex flex-wrap items-center justify-center lg:justify-start gap-4">
                    <a href="#projects" class="px-7 py-3.5 rounded-xl bg-indigo-600 hover:bg-indigo-700 text-white font-semibold shadow-lg shadow-indigo-600/25 hover:-translate-y-0.5 transition-all flex items-center gap-2">
                        <i class="fa-solid fa-laptop-code"></i>
                        <span>View Projects</span>
                    </a>
                    <a href="tel:0367730151" class="px-6 py-3.5 rounded-xl border border-slate-300 dark:border-dark-border bg-white/80 dark:bg-dark-card hover:bg-slate-100 dark:hover:bg-dark-hover text-slate-800 dark:text-slate-200 font-semibold hover:-translate-y-0.5 transition-all flex items-center gap-2">
                        <i class="fa-solid fa-phone text-emerald-500"></i>
                        <span>Call 0367 730 151</span>
                    </a>
                </div>

                <!-- Quick Contacts & Social Bar -->
                <div class="pt-4 flex flex-wrap items-center justify-center lg:justify-start gap-3 text-slate-500 dark:text-slate-400">
                    <a href="mailto:nhoc41551@gmail.com" title="Email" class="w-10 h-10 rounded-xl border border-slate-200 dark:border-dark-border flex items-center justify-center hover:text-indigo-600 dark:hover:text-indigo-400 hover:border-indigo-500 transition-colors">
                        <i class="fa-solid fa-envelope"></i>
                    </a>
                    <a href="tel:0367730151" title="Direct Phone" class="w-10 h-10 rounded-xl border border-slate-200 dark:border-dark-border flex items-center justify-center hover:text-emerald-500 hover:border-emerald-500 transition-colors">
                        <i class="fa-solid fa-phone"></i>
                    </a>
                    <a href="https://www.facebook.com/share/1BXNfsAmka/?mibextid=wwXIfr" target="_blank" rel="noopener noreferrer" title="Facebook Profile" class="w-10 h-10 rounded-xl border border-slate-200 dark:border-dark-border flex items-center justify-center hover:text-blue-500 hover:border-blue-500 transition-colors">
                        <i class="fa-brands fa-facebook-f"></i>
                    </a>
                    <span class="inline-flex items-center gap-1.5 text-xs text-slate-500 dark:text-slate-400 ml-2">
                        <i class="fa-solid fa-location-dot text-indigo-500"></i> Nam Tu Liem, Hanoi
                    </span>
                </div>
            </div>

            <!-- Right Column: Avatar Photo & Floating Badges -->
            <div class="lg:col-span-5 flex justify-center relative">
                <div class="relative w-72 sm:w-80 md:w-96">
                    <!-- Glowing Background Gradient -->
                    <div class="absolute inset-0 bg-gradient-to-tr from-indigo-500 via-primary-500 to-accent-cyan rounded-3xl blur-2xl opacity-40 -rotate-2 scale-95"></div>

                    <!-- Main Avatar Frame -->
                    <div class="relative rounded-3xl overflow-hidden p-2.5 bg-white dark:bg-dark-card border-2 border-slate-200/80 dark:border-dark-border shadow-2xl">
                        <img 
                            src="images/avatar.jpg" 
                            alt="Nguyen Thai Hoc - Portrait" 
                            class="w-full h-[400px] sm:h-[450px] object-cover object-[center_15%] rounded-2xl hover:scale-105 transition-transform duration-500"
                            onerror="this.onerror=null; this.src='https://nhoc41551-hub.github.io/images/avatar.jpg.jpg';"
                        >
                    </div>

                    <!-- Floating Badge: Campus Location -->
                    <div class="absolute -bottom-5 -left-4 sm:-left-6 px-4 py-3 rounded-2xl bg-white/95 dark:bg-dark-card/95 card-blur border border-slate-200 dark:border-dark-border shadow-xl flex items-center gap-3">
                        <div class="w-10 h-10 rounded-xl bg-indigo-50 dark:bg-indigo-950/60 text-indigo-600 dark:text-indigo-400 flex items-center justify-center text-lg">
                            <i class="fa-solid fa-graduation-cap"></i>
                        </div>
                        <div>
                            <p class="text-[11px] text-slate-400 font-mono">Hanoi Polytechnic</p>
                            <p class="text-xs sm:text-sm font-bold text-slate-800 dark:text-white">322 My Dinh, Hanoi</p>
                        </div>
                    </div>

                    <!-- Floating Badge: Major & Phone -->
                    <div class="absolute -top-4 -right-4 sm:-right-6 px-4 py-3 rounded-2xl bg-white/95 dark:bg-dark-card/95 card-blur border border-slate-200 dark:border-dark-border shadow-xl flex items-center gap-3">
                        <div class="w-10 h-10 rounded-xl bg-cyan-50 dark:bg-cyan-950/60 text-cyan-600 dark:text-cyan-400 flex items-center justify-center text-lg">
                            <i class="fa-solid fa-code"></i>
                        </div>
                        <div>
                            <p class="text-[11px] text-slate-400 font-mono">Direct Contact</p>
                            <p class="text-xs sm:text-sm font-bold text-slate-800 dark:text-white">0367 730 151</p>
                        </div>
                    </div>
                </div>
            </div>

        </div>
    </section>

    <!-- ================= ABOUT SECTION ================= -->
    <section id="about" class="py-20 border-t border-slate-200 dark:border-dark-border bg-white dark:bg-dark-card/40">
        <div class="max-w-7xl mx-auto px-6">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <span class="text-xs font-mono font-semibold uppercase tracking-widest text-indigo-600 dark:text-indigo-400 bg-indigo-50 dark:bg-indigo-950/60 px-3 py-1 rounded-md">
                    About Me
                </span>
                <h2 class="text-3xl sm:text-4xl font-extrabold text-slate-900 dark:text-white mt-3">
                    Driven by Curiosity & Passion for Code
                </h2>
                <p class="text-slate-600 dark:text-slate-400 mt-4 leading-relaxed">
                    Get to know more about my background, career vision, and passion for software engineering.
                </p>
            </div>

            <div class="grid grid-cols-1 lg:grid-cols-12 gap-10 items-center">
                <div class="lg:col-span-7 space-y-6">
                    <h3 class="text-2xl font-bold text-slate-900 dark:text-white">
                        Who is Nguyen Thai Hoc?
                    </h3>
                    <p class="text-slate-600 dark:text-slate-300 leading-relaxed text-base sm:text-lg">
                        I am an energetic and determined Information Technology student at <strong class="text-indigo-600 dark:text-indigo-400">Hanoi Polytechnic College</strong> (Trường Cao đẳng Công nghệ Bách Khoa Hà Nội). I possess a deep fascination with software engineering, modern web applications, and database management.
                    </p>
                    <p class="text-slate-600 dark:text-slate-300 leading-relaxed text-base sm:text-lg">
                        With an autodidactic mindset and a commitment to continuous growth, I actively practice building web applications with HTML, CSS, JavaScript, Java, and MySQL. My career objective is to become a high-impact, professional Software Developer capable of delivering robust and user-centric digital products.
                    </p>

                    <!-- Key Traits -->
                    <div class="grid grid-cols-1 sm:grid-cols-2 gap-4 pt-2">
                        <div class="p-4 rounded-xl border border-slate-200 dark:border-dark-border bg-slate-50 dark:bg-dark-card flex items-start gap-3">
                            <i class="fa-solid fa-lightbulb text-indigo-500 text-lg mt-1"></i>
                            <div>
                                <h4 class="font-bold text-slate-900 dark:text-white text-sm">Passionate Learner</h4>
                                <p class="text-xs text-slate-500 dark:text-slate-400 mt-0.5">Constantly exploring new tools, clean coding standards, and algorithmic thinking.</p>
                            </div>
                        </div>
                        <div class="p-4 rounded-xl border border-slate-200 dark:border-dark-border bg-slate-50 dark:bg-dark-card flex items-start gap-3">
                            <i class="fa-solid fa-users text-cyan-500 text-lg mt-1"></i>
                            <div>
                                <h4 class="font-bold text-slate-900 dark:text-white text-sm">Team Collaboration</h4>
                                <p class="text-xs text-slate-500 dark:text-slate-400 mt-0.5">Reliable team player with strong interpersonal and presentation skills.</p>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Fast Facts Snapshot Card -->
                <div class="lg:col-span-5 p-8 rounded-3xl border border-slate-200 dark:border-dark-border bg-gradient-to-b from-slate-50 to-white dark:from-dark-card dark:to-dark-bg shadow-xl space-y-6">
                    <h3 class="text-xl font-bold text-slate-900 dark:text-white flex items-center gap-2">
                        <i class="fa-solid fa-id-card text-indigo-500"></i>
                        <span>Profile Snapshot</span>
                    </h3>

                    <div class="space-y-4 text-sm">
                        <div class="flex justify-between border-b border-slate-200 dark:border-dark-border pb-3">
                            <span class="text-slate-500 dark:text-slate-400">Full Name</span>
                            <span class="font-semibold text-slate-900 dark:text-white">Nguyen Thai Hoc</span>
                        </div>
                        <div class="flex justify-between border-b border-slate-200 dark:border-dark-border pb-3">
                            <span class="text-slate-500 dark:text-slate-400">Phone Number</span>
                            <a href="tel:0367730151" class="font-semibold text-indigo-600 dark:text-indigo-400 hover:underline">0367 730 151</a>
                        </div>
                        <div class="flex justify-between border-b border-slate-200 dark:border-dark-border pb-3">
                            <span class="text-slate-500 dark:text-slate-400">Email</span>
                            <a href="mailto:nhoc41551@gmail.com" class="font-semibold text-indigo-600 dark:text-indigo-400 hover:underline">nhoc41551@gmail.com</a>
                        </div>
                        <div class="flex justify-between border-b border-slate-200 dark:border-dark-border pb-3">
                            <span class="text-slate-500 dark:text-slate-400">College</span>
                            <span class="font-semibold text-slate-900 dark:text-white text-right">Hanoi Polytechnic College</span>
                        </div>
                        <div class="flex justify-between border-b border-slate-200 dark:border-dark-border pb-3">
                            <span class="text-slate-500 dark:text-slate-400">Campus Address</span>
                            <span class="font-semibold text-slate-900 dark:text-white text-right text-xs">322 My Dinh, Nam Tu Liem, Hanoi</span>
                        </div>
                        <div class="flex justify-between pb-1">
                            <span class="text-slate-500 dark:text-slate-400">Major</span>
                            <span class="font-semibold text-emerald-600 dark:text-emerald-400">Information Technology</span>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- ================= EDUCATION & CAMPUS ================= -->
    <section id="education" class="py-20 border-t border-slate-200 dark:border-dark-border bg-slate-50/50 dark:bg-dark-bg">
        <div class="max-w-7xl mx-auto px-6">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <span class="text-xs font-mono font-semibold uppercase tracking-widest text-indigo-600 dark:text-indigo-400 bg-indigo-50 dark:bg-indigo-950/60 px-3 py-1 rounded-md">
                    Academic Background
                </span>
                <h2 class="text-3xl sm:text-4xl font-extrabold text-slate-900 dark:text-white mt-3">
                    Education & Campus Details
                </h2>
                <p class="text-slate-600 dark:text-slate-400 mt-4 leading-relaxed">
                    Formal training, location details, and core computer science coursework.
                </p>
            </div>

            <div class="max-w-4xl mx-auto">
                <div class="relative pl-8 sm:pl-10 border-l-2 border-indigo-500/40 space-y-12">
                    
                    <div class="relative group">
                        <!-- Dot Marker -->
                        <span class="absolute -left-[41px] sm:-left-[49px] top-1 w-6 h-6 rounded-full bg-white dark:bg-dark-bg border-4 border-indigo-600 group-hover:scale-125 transition-transform"></span>

                        <div class="p-6 sm:p-8 rounded-2xl border border-slate-200 dark:border-dark-border bg-white dark:bg-dark-card shadow-sm hover:shadow-xl transition-all">
                            <div class="flex flex-wrap items-center justify-between gap-2 mb-3">
                                <span class="px-3 py-1 rounded-full bg-indigo-50 dark:bg-indigo-950/60 text-indigo-600 dark:text-indigo-400 text-xs font-mono font-semibold">
                                    2024 - Present • College Degree
                                </span>
                                <a href="https://maps.google.com/?q=322+Đường+Mỹ+Đình+Phường+Nhân+Mỹ+Từ+Liêm+Hà+Nội" target="_blank" rel="noopener noreferrer" class="text-xs text-indigo-600 dark:text-indigo-400 hover:underline flex items-center gap-1 font-medium">
                                    <i class="fa-solid fa-map-location-dot"></i> View on Google Maps
                                </a>
                            </div>

                            <h3 class="text-2xl font-bold text-slate-900 dark:text-white">
                                Hanoi Polytechnic College (HPC)
                            </h3>
                            <p class="text-xs sm:text-sm font-medium text-slate-500 dark:text-slate-400 mt-1 flex items-center gap-2">
                                <i class="fa-solid fa-building-columns text-indigo-500"></i>
                                <span><strong>Campus Address:</strong> 322 My Dinh Street, Nhan My, Nam Tu Liem District, Hanoi, Vietnam</span>
                            </p>

                            <h4 class="text-base font-semibold text-indigo-600 dark:text-indigo-400 mt-3">
                                Major: Information Technology (Công nghệ thông tin)
                            </h4>

                            <p class="text-slate-600 dark:text-slate-300 mt-3 leading-relaxed text-sm sm:text-base">
                                Enrolled in a comprehensive IT training curriculum emphasizing practical software engineering, web application structure, object-oriented concepts, and relational databases.
                            </p>

                            <!-- Academic Modules -->
                            <div class="mt-6">
                                <p class="text-xs font-mono uppercase text-slate-500 dark:text-slate-400 mb-3 font-semibold">
                                    Core Academic Modules Studied:
                                </p>
                                <div class="flex flex-wrap gap-2">
                                    <span class="px-3 py-1.5 rounded-lg border border-slate-200 dark:border-dark-border bg-slate-50 dark:bg-dark-bg text-xs font-medium text-slate-700 dark:text-slate-300">
                                        <i class="fa-brands fa-html5 text-orange-500 mr-1.5"></i>Web Development (HTML5 & CSS3)
                                    </span>
                                    <span class="px-3 py-1.5 rounded-lg border border-slate-200 dark:border-dark-border bg-slate-50 dark:bg-dark-bg text-xs font-medium text-slate-700 dark:text-slate-300">
                                        <i class="fa-brands fa-java text-red-500 mr-1.5"></i>OOP with Java
                                    </span>
                                    <span class="px-3 py-1.5 rounded-lg border border-slate-200 dark:border-dark-border bg-slate-50 dark:bg-dark-bg text-xs font-medium text-slate-700 dark:text-slate-300">
                                        <i class="fa-solid fa-database text-blue-500 mr-1.5"></i>MySQL Relational Database
                                    </span>
                                    <span class="px-3 py-1.5 rounded-lg border border-slate-200 dark:border-dark-border bg-slate-50 dark:bg-dark-bg text-xs font-medium text-slate-700 dark:text-slate-300">
                                        <i class="fa-solid fa-cubes text-emerald-500 mr-1.5"></i>Software Development Fundamentals
                                    </span>
                                </div>
                            </div>
                        </div>
                    </div>

                </div>
            </div>
        </div>
    </section>

    <!-- ================= SKILLS SECTION ================= -->
    <section id="skills" class="py-20 border-t border-slate-200 dark:border-dark-border bg-white dark:bg-dark-card/40">
        <div class="max-w-7xl mx-auto px-6">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <span class="text-xs font-mono font-semibold uppercase tracking-widest text-indigo-600 dark:text-indigo-400 bg-indigo-50 dark:bg-indigo-950/60 px-3 py-1 rounded-md">
                    Capabilities
                </span>
                <h2 class="text-3xl sm:text-4xl font-extrabold text-slate-900 dark:text-white mt-3">
                    Technical & Professional Skills
                </h2>
                <p class="text-slate-600 dark:text-slate-400 mt-4 leading-relaxed">
                    Overview of core programming languages, tools, databases
