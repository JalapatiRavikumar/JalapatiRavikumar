<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Jalapati Ravikumar | Interactive Full Stack & AI/ML Portfolio</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- FontAwesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=JetBrains+Mono:wght@400;700&family=Plus+Jakarta+Sans:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
    
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Plus Jakarta Sans', 'sans-serif'],
                        mono: ['JetBrains Mono', 'monospace'],
                    },
                    colors: {
                        darkBg: '#080b11',
                        darkCard: '#111622',
                        darkBorder: '#1f293d',
                        brandAccent: '#6366f1',
                    }
                }
            }
        }
    </script>
    
    <style>
        body {
            background-color: #080b11;
            font-family: 'Plus Jakarta Sans', sans-serif;
            overflow-x: hidden;
        }
        /* Custom Glowing Scrollbar */
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #080b11;
        }
        ::-webkit-scrollbar-thumb {
            background: #1f293d;
            border-radius: 4px;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: #6366f1;
        }
        /* Custom Neon Glows */
        .neon-glow-indigo {
            box-shadow: 0 0 25px rgba(99, 102, 241, 0.2);
        }
        .neon-glow-emerald {
            box-shadow: 0 0 25px rgba(16, 185, 129, 0.2);
        }
        .neon-glow-rose {
            box-shadow: 0 0 25px rgba(244, 63, 94, 0.2);
        }
        .glassmorphism {
            background: rgba(17, 22, 34, 0.75);
            backdrop-filter: blur(12px);
            border: 1px solid rgba(255, 255, 255, 0.05);
        }
    </style>
</head>
<body class="text-slate-100 antialiased selection:bg-indigo-500 selection:text-white">

    <!-- Top Glow Effects -->
    <div class="absolute top-0 left-1/4 w-[500px] h-[500px] bg-indigo-500/10 rounded-full blur-[120px] pointer-events-none"></div>
    <div class="absolute top-1/3 right-1/4 w-[400px] h-[400px] bg-purple-500/10 rounded-full blur-[100px] pointer-events-none"></div>

    <!-- MAIN HEADER NAVIGATION -->
    <nav class="sticky top-0 z-50 glassmorphism border-b border-darkBorder px-6 py-4">
        <div class="max-w-7xl mx-auto flex flex-col md:flex-row justify-between items-center gap-4">
            <div class="flex items-center gap-3">
                <div class="h-10 w-10 rounded-xl bg-gradient-to-tr from-indigo-500 to-purple-600 flex items-center justify-center font-bold text-white shadow-lg shadow-indigo-500/30">
                    JR
                </div>
                <div>
                    <span class="font-bold text-lg tracking-tight block">Jalapati Ravikumar</span>
                    <span class="text-xs text-indigo-400 font-mono">Full Stack & AI/ML Engineer</span>
                </div>
            </div>
            
            <div class="flex flex-wrap justify-center items-center gap-6 text-sm font-medium text-slate-300">
                <a href="#about" class="hover:text-indigo-400 transition-colors">About</a>
                <a href="#playgrounds" class="hover:text-indigo-400 transition-colors flex items-center gap-1.5"><span class="flex h-2 w-2 rounded-full bg-emerald-500 animate-pulse"></span>Playgrounds</a>
                <a href="#skills" class="hover:text-indigo-400 transition-colors">Skills</a>
                <a href="#projects" class="hover:text-indigo-400 transition-colors">Projects</a>
                <a href="#experience" class="hover:text-indigo-400 transition-colors">Experience</a>
                <a href="#connect" class="px-4 py-2 rounded-lg bg-indigo-600 hover:bg-indigo-500 text-white font-semibold transition-all hover:shadow-lg hover:shadow-indigo-500/20">Let's Chat</a>
            </div>
        </div>
    </nav>

    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-8 space-y-16">

        <!-- HERO BANNER SECTION -->
        <header class="relative rounded-3xl overflow-hidden border border-darkBorder glassmorphism p-8 md:p-12">
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-8 items-center relative z-10">
                <div class="lg:col-span-7 space-y-6">
                    <!-- Open To Work Badge -->
                    <div class="inline-flex items-center gap-2 px-3.5 py-1.5 rounded-full bg-emerald-500/10 text-emerald-400 border border-emerald-500/20 text-xs font-semibold uppercase tracking-wider animate-pulse">
                        <span class="h-2 w-2 rounded-full bg-emerald-400"></span> Actively Open to Work
                    </div>
                    
                    <h1 class="text-4xl sm:text-5xl lg:text-6xl font-extrabold tracking-tight">
                        Hi, I'm <span class="bg-gradient-to-r from-indigo-400 via-purple-400 to-pink-400 bg-clip-text text-transparent">Ravikumar</span>
                    </h1>
                    
                    <!-- Dynamic Typing Emulator -->
                    <div class="min-h-[40px] font-mono text-lg sm:text-xl text-indigo-300 flex items-center">
                        <span id="typing-text"></span><span class="animate-ping text-indigo-500 font-bold ml-1">|</span>
                    </div>

                    <p class="text-slate-400 text-base sm:text-lg max-w-xl">
                        I build high-performance, AI-driven full-stack web applications. Expertly blending pristine <strong class="text-slate-200">React/Next.js</strong> frontends with robust <strong class="text-slate-200">Spring Boot/Node.js</strong> microservices and intelligent ML inference models.
                    </p>

                    <!-- Profile Social Hub -->
                    <div class="flex flex-wrap gap-4 pt-4">
                        <a href="mailto:ravikumarjalapatii@gmail.com" class="flex items-center gap-2 px-4 py-2.5 rounded-xl bg-slate-800 hover:bg-indigo-600 text-slate-200 hover:text-white transition-all font-medium border border-slate-700">
                            <i class="fa-regular fa-envelope text-lg"></i> Email Me
                        </a>
                        <a href="https://www.linkedin.com/in/jalapatiravikumar" target="_blank" class="flex items-center gap-2 px-4 py-2.5 rounded-xl bg-slate-800 hover:bg-indigo-600 text-slate-200 hover:text-white transition-all font-medium border border-slate-700">
                            <i class="fa-brands fa-linkedin text-lg"></i> LinkedIn
                        </a>
                        <a href="https://github.com/JalapatiRavikumar" target="_blank" class="flex items-center gap-2 px-4 py-2.5 rounded-xl bg-slate-800 hover:bg-indigo-600 text-slate-200 hover:text-white transition-all font-medium border border-slate-700">
                            <i class="fa-brands fa-github text-lg"></i> GitHub
                        </a>
                        <a href="https://jalapatiravikumar-portfolio.vercel.app/" target="_blank" class="flex items-center gap-2 px-4 py-2.5 rounded-xl bg-slate-800 hover:bg-indigo-600 text-slate-200 hover:text-white transition-all font-medium border border-slate-700">
                            <i class="fa-solid fa-globe text-lg"></i> Live Portfolio
                        </a>
                    </div>
                </div>

                <!-- Animated Interactive Profile Card -->
                <div class="lg:col-span-5 flex justify-center">
                    <div class="relative w-full max-w-sm rounded-2xl border border-darkBorder bg-slate-950 p-6 shadow-2xl overflow-hidden group">
                        <div class="absolute top-0 right-0 w-32 h-32 bg-indigo-500/20 rounded-full blur-3xl group-hover:bg-indigo-500/35 transition-all"></div>
                        
                        <!-- Header Window Controls -->
                        <div class="flex gap-1.5 mb-6">
                            <span class="w-3 h-3 rounded-full bg-rose-500"></span>
                            <span class="w-3 h-3 rounded-full bg-amber-500"></span>
                            <span class="w-3 h-3 rounded-full bg-emerald-500"></span>
                        </div>

                        <!-- Card Code block Toggles -->
                        <div class="flex justify-between items-center border-b border-darkBorder pb-3 mb-4">
                            <span class="text-xs text-slate-400 font-mono"><i class="fa-solid fa-terminal mr-2"></i>profile.yaml</span>
                            <button onclick="copyToClipboard('ravikumarjalapatii@gmail.com', this)" class="text-xs text-indigo-400 hover:text-indigo-300 font-mono transition-all flex items-center gap-1">
                                <i class="fa-regular fa-copy"></i> Copy Contact
                            </button>
                        </div>

                        <!-- Config Block representation -->
                        <pre class="text-xs sm:text-sm font-mono text-slate-300 leading-relaxed overflow-x-auto select-all">
<span class="text-indigo-400">developer</span>:
  <span class="text-emerald-400">name</span>: Jalapati Ravikumar
  <span class="text-emerald-400">role</span>: Full Stack & AI/ML Dev
  <span class="text-emerald-400">location</span>: Bengaluru, India 🇮🇳
  <span class="text-emerald-400">education</span>: B.Tech CSE (2024)
  <span class="text-emerald-400">experience</span>: Intern @ Kodnest
  <span class="text-emerald-400">focus</span>: MERN · Java · AI · DevOps
<span class="text-indigo-400">motto</span>:
  "I debug with console.log 
   and I'm proud of it! 🚀"
                        </pre>

                        <!-- GitHub Counter badges -->
                        <div class="mt-6 pt-4 border-t border-darkBorder grid grid-cols-2 gap-4 text-center">
                            <div class="p-3 rounded-lg bg-darkCard border border-darkBorder">
                                <div class="text-indigo-400 font-bold text-lg">10+</div>
                                <div class="text-[10px] uppercase text-slate-400">Projects Shipped</div>
                            </div>
                            <div class="p-3 rounded-lg bg-darkCard border border-darkBorder">
                                <div class="text-emerald-400 font-bold text-lg">92%</div>
                                <div class="text-[10px] uppercase text-slate-400">Model Precision</div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </header>

        <!-- IMPACT SCORECARD (Dashboard Cards) -->
        <section id="about" class="space-y-6">
            <h2 class="text-2xl sm:text-3xl font-extrabold tracking-tight flex items-center gap-3">
                <span class="h-8 w-1 bg-indigo-500 rounded-full"></span> Impact Dashboard
            </h2>
            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-6">
                <!-- Stat 1 -->
                <div class="p-6 rounded-2xl bg-darkCard border border-darkBorder hover:border-indigo-500/50 transition-all shadow-xl flex flex-col justify-between">
                    <div class="flex justify-between items-start mb-4">
                        <span class="p-3 rounded-xl bg-indigo-500/10 text-indigo-400"><i class="fa-solid fa-gauge-high text-xl"></i></span>
                        <span class="text-xs text-emerald-400 font-semibold bg-emerald-500/10 px-2 py-1 rounded">Optimized</span>
                    </div>
                    <div>
                        <div class="text-3xl sm:text-4xl font-extrabold font-mono tracking-tight text-white">~40%</div>
                        <div class="text-sm font-semibold text-slate-300 mt-2">Page Load Reduction</div>
                        <p class="text-xs text-slate-400 mt-1">Achieved via lazy loading, code-splitting & progressive image rendering.</p>
                    </div>
                </div>
                <!-- Stat 2 -->
                <div class="p-6 rounded-2xl bg-darkCard border border-darkBorder hover:border-purple-500/50 transition-all shadow-xl flex flex-col justify-between">
                    <div class="flex justify-between items-start mb-4">
                        <span class="p-3 rounded-xl bg-purple-500/10 text-purple-400"><i class="fa-solid fa-shield-halved text-xl"></i></span>
                        <span class="text-xs text-indigo-400 font-semibold bg-indigo-500/10 px-2 py-1 rounded">Highly Precise</span>
                    </div>
                    <div>
                        <div class="text-3xl sm:text-4xl font-extrabold font-mono tracking-tight text-white">92%</div>
                        <div class="text-sm font-semibold text-slate-300 mt-2">Fraud Detection Precision</div>
                        <p class="text-xs text-slate-400 mt-1">TensorFlow model with 89% recall & 90% F1-score across 284k datasets.</p>
                    </div>
                </div>
                <!-- Stat 3 -->
                <div class="p-6 rounded-2xl bg-darkCard border border-darkBorder hover:border-pink-500/50 transition-all shadow-xl flex flex-col justify-between">
                    <div class="flex justify-between items-start mb-4">
                        <span class="p-3 rounded-xl bg-pink-500/10 text-pink-400"><i class="fa-solid fa-cubes text-xl"></i></span>
                        <span class="text-xs text-pink-400 font-semibold bg-pink-500/10 px-2 py-1 rounded">-30% Size</span>
                    </div>
                    <div>
                        <div class="text-3xl sm:text-4xl font-extrabold font-mono tracking-tight text-white">~30%</div>
                        <div class="text-sm font-semibold text-slate-300 mt-2">Bundle Optimization</div>
                        <p class="text-xs text-slate-400 mt-1">Reduced payload via dynamic import rules and strict tree-shaking configs.</p>
                    </div>
                </div>
                <!-- Stat 4 -->
                <div class="p-6 rounded-2xl bg-darkCard border border-darkBorder hover:border-emerald-500/50 transition-all shadow-xl flex flex-col justify-between">
                    <div class="flex justify-between items-start mb-4">
                        <span class="p-3 rounded-xl bg-emerald-500/10 text-emerald-400"><i class="fa-solid fa-circle-check text-xl"></i></span>
                        <span class="text-xs text-emerald-400 font-semibold bg-emerald-500/10 px-2 py-1 rounded">Active</span>
                    </div>
                    <div>
                        <div class="text-3xl sm:text-4xl font-extrabold font-mono tracking-tight text-white">10+</div>
                        <div class="text-sm font-semibold text-slate-300 mt-2">Production Implementations</div>
                        <p class="text-xs text-slate-400 mt-1">Robust platforms built using Django, Spring Boot, React & AI Integrations.</p>
                    </div>
                </div>
            </div>
        </section>

        <!-- THE INTERACTIVE PLAYGROUNDS HUB -->
        <section id="playgrounds" class="space-y-8 relative">
            <div class="absolute -top-12 -left-12 w-64 h-64 bg-emerald-500/5 rounded-full blur-3xl pointer-events-none"></div>
            
            <div class="flex flex-col md:flex-row md:items-end justify-between gap-4 border-b border-darkBorder pb-4">
                <div>
                    <h2 class="text-2xl sm:text-3xl font-extrabold tracking-tight flex items-center gap-3">
                        <span class="h-8 w-1 bg-emerald-500 rounded-full"></span> Tech Playgrounds
                    </h2>
                    <p class="text-slate-400 text-sm mt-1">Experience my projects and code implementation live in these interactive modules.</p>
                </div>
                
                <!-- Playgrounds tabs selection -->
                <div class="flex bg-slate-950 p-1.5 rounded-xl border border-darkBorder text-sm font-semibold">
                    <button onclick="switchPlayground('ai-twin')" id="tab-ai-twin" class="px-4 py-2 rounded-lg bg-indigo-600 text-white transition-all">
                        <i class="fa-solid fa-robot mr-1.5"></i> AI Twin Chat
                    </button>
                    <button onclick="switchPlayground('fraud-model')" id="tab-fraud-model" class="px-4 py-2 rounded-lg text-slate-400 hover:text-white transition-all">
                        <i class="fa-solid fa-chart-line mr-1.5"></i> Fraud ML Model
                    </button>
                    <button onclick="switchPlayground('interview-prep')" id="tab-interview-prep" class="px-4 py-2 rounded-lg text-slate-400 hover:text-white transition-all">
                        <i class="fa-solid fa-graduation-cap mr-1.5"></i> MockMate Sandbox
                    </button>
                </div>
            </div>

            <!-- CONTAINER 1: AI TWIN CHATBOT -->
            <div id="pg-ai-twin" class="grid grid-cols-1 lg:grid-cols-12 gap-8 items-stretch">
                <!-- Quick Bio Details for context -->
                <div class="lg:col-span-4 p-6 rounded-2xl bg-darkCard border border-darkBorder flex flex-col justify-between space-y-6">
                    <div class="space-y-4">
                        <div class="flex items-center gap-3">
                            <span class="p-2 rounded-lg bg-indigo-500/10 text-indigo-400"><i class="fa-solid fa-brain"></i></span>
                            <h3 class="font-extrabold text-lg">Meet my AI Twin</h3>
                        </div>
                        <p class="text-sm text-slate-400 leading-relaxed">
                            This live chatbot represents my professional portfolio. It runs a pre-configured profile system prompt directly against the **Gemini 2.5 Flash** model. 
                        </p>
                        <div class="space-y-2 text-xs font-mono text-indigo-300">
                            <div class="flex items-center gap-2"><i class="fa-solid fa-circle text-[6px] text-emerald-400 animate-pulse"></i> Model: gemini-2.5-flash-preview</div>
                            <div class="flex items-center gap-2"><i class="fa-solid fa-circle text-[6px] text-indigo-400"></i> Context: Full Professional Profile</div>
                        </div>
                    </div>
                    
                    <div class="space-y-2">
                        <span class="text-xs uppercase text-slate-400 font-semibold block">Try asking:</span>
                        <div class="flex flex-col gap-2">
                            <button onclick="sendSuggestedQuestion('What are your top full-stack projects?')" class="text-left text-xs bg-slate-900 hover:bg-indigo-950 hover:text-indigo-300 p-2.5 rounded-lg border border-darkBorder transition-all">
                                💬 "What are your top full-stack projects?"
                            </button>
                            <button onclick="sendSuggestedQuestion('Tell me about your Spring Boot & Microservices experience.')" class="text-left text-xs bg-slate-900 hover:bg-indigo-950 hover:text-indigo-300 p-2.5 rounded-lg border border-darkBorder transition-all">
                                💬 "Tell me about your Spring Boot experience."
                            </button>
                            <button onclick="sendSuggestedQuestion('Can we work together on a freelance project?')" class="text-left text-xs bg-slate-900 hover:bg-indigo-950 hover:text-indigo-300 p-2.5 rounded-lg border border-darkBorder transition-all">
                                💬 "Can we work together?"
                            </button>
                        </div>
                    </div>
                </div>

                <!-- Chat Box panel -->
                <div class="lg:col-span-8 rounded-2xl bg-slate-950 border border-darkBorder overflow-hidden flex flex-col min-h-[450px]">
                    <div class="bg-darkCard px-6 py-4 border-b border-darkBorder flex justify-between items-center">
                        <div class="flex items-center gap-3">
                            <div class="relative">
                                <div class="w-10 h-10 rounded-full bg-gradient-to-r from-indigo-500 to-purple-600 flex items-center justify-center font-bold">JR</div>
                                <span class="absolute bottom-0 right-0 h-3 w-3 rounded-full bg-emerald-500 border-2 border-slate-950"></span>
                            </div>
                            <div>
                                <span class="font-bold text-sm block">Ravikumar's AI Persona</span>
                                <span class="text-[10px] text-emerald-400 flex items-center gap-1"><span class="h-1 w-1 bg-emerald-400 rounded-full animate-pulse"></span> Online & Ready</span>
                            </div>
                        </div>
                        <button onclick="clearChat()" class="text-xs text-slate-400 hover:text-white transition-all"><i class="fa-solid fa-arrow-rotate-right mr-1"></i> Reset</button>
                    </div>

                    <!-- Chat conversation area -->
                    <div id="chat-messages" class="flex-1 p-6 space-y-4 overflow-y-auto max-h-[350px]">
                        <div class="flex gap-3 items-start max-w-[85%]">
                            <div class="h-8 w-8 rounded-full bg-indigo-500/10 border border-indigo-500/30 flex items-center justify-center text-xs text-indigo-400 font-bold shrink-0">AI</div>
                            <div class="p-3.5 rounded-2xl bg-darkCard border border-darkBorder text-sm leading-relaxed text-slate-300">
                                Hello there! I'm Ravikumar's AI Agent. Ask me anything about my tech stack, B.Tech background, interns, projects, or how to contact me. I'm connected directly to Gemini!
                            </div>
                        </div>
                    </div>

                    <!-- Chat input area -->
                    <div class="p-4 bg-darkCard border-t border-darkBorder">
                        <form id="chat-form" onsubmit="handleChatSubmit(event)" class="flex gap-2">
                            <input id="chat-input" type="text" placeholder="Type your inquiry here..." required autocomplete="off" class="flex-1 bg-slate-900 border border-darkBorder rounded-xl px-4 py-3 text-sm text-slate-200 focus:outline-none focus:border-indigo-500 transition-colors" />
                            <button type="submit" id="chat-submit-btn" class="px-5 py-3 rounded-xl bg-indigo-600 hover:bg-indigo-500 text-white text-sm font-semibold transition-all shadow-lg hover:shadow-indigo-500/20">
                                <i class="fa-solid fa-paper-plane"></i>
                            </button>
                        </form>
                    </div>
                </div>
            </div>

            <!-- CONTAINER 2: FRAUD DETECTION AUTOENCODER MODEL SIMULATOR -->
            <div id="pg-fraud-model" class="hidden grid grid-cols-1 lg:grid-cols-12 gap-8 items-stretch">
                <!-- Controls & Info -->
                <div class="lg:col-span-5 p-6 rounded-2xl bg-darkCard border border-darkBorder flex flex-col justify-between space-y-6">
                    <div class="space-y-4">
                        <div class="flex items-center gap-3">
                            <span class="p-2 rounded-lg bg-emerald-500/10 text-emerald-400"><i class="fa-solid fa-chart-line"></i></span>
                            <h3 class="font-extrabold text-lg">Autoencoder Sandbox</h3>
                        </div>
                        <p class="text-sm text-slate-400 leading-relaxed">
                            On my Deep Learning Fraud Detection model, optimizing the reconstruction error threshold was critical to reducing false positives by 25%.
                        </p>
                        <p class="text-xs text-slate-500">
                            Move the slider to adjust the <strong class="text-emerald-400 font-mono">Reconstruction Error Threshold</strong>. Watch how TP (True Positive), FP (False Positive), Precision, Recall, and the overall F1-Score recalculate dynamically!
                        </p>
                    </div>

                    <div class="space-y-4 p-4 rounded-xl bg-slate-950 border border-darkBorder">
                        <div class="flex justify-between items-center text-xs font-semibold">
                            <span class="text-slate-400 uppercase tracking-wider">Error Threshold</span>
                            <span id="threshold-val" class="font-mono text-emerald-400 text-sm bg-emerald-400/10 px-2 py-0.5 rounded">3.20</span>
                        </div>
                        <input id="threshold-slider" type="range" min="1.0" max="7.0" step="0.1" value="3.2" oninput="updateFraudSim(this.value)" class="w-full h-2 bg-slate-900 rounded-lg appearance-none cursor-pointer accent-emerald-400" />
                        <div class="flex justify-between text-[10px] text-slate-500 font-mono">
                            <span>1.0 (Lenient)</span>
                            <span>7.0 (Strict)</span>
                        </div>
                    </div>

                    <div class="space-y-2 text-xs">
                        <span class="text-slate-400 uppercase tracking-widest font-semibold block">Metrics Output:</span>
                        <div class="grid grid-cols-2 gap-2">
                            <div class="p-2 bg-slate-950 rounded border border-darkBorder flex justify-between">
                                <span class="text-slate-400">Precision:</span>
                                <span id="precision-out" class="font-bold text-indigo-400 font-mono">--</span>
                            </div>
                            <div class="p-2 bg-slate-950 rounded border border-darkBorder flex justify-between">
                                <span class="text-slate-400">Recall:</span>
                                <span id="recall-out" class="font-bold text-indigo-400 font-mono">--</span>
                            </div>
                            <div class="p-2 bg-slate-950 rounded border border-darkBorder flex justify-between col-span-2">
                                <span class="text-slate-400">Optimized F1-Score:</span>
                                <span id="f1-out" class="font-bold text-emerald-400 font-mono">--</span>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Live Graph plotting Scatter Matrix / Distribution Curves -->
                <div class="lg:col-span-7 rounded-2xl bg-slate-950 border border-darkBorder p-6 flex flex-col justify-between space-y-6">
                    <div>
                        <div class="flex justify-between items-center border-b border-darkBorder pb-3 mb-4">
                            <span class="text-sm font-semibold tracking-tight"><i class="fa-solid fa-analytics text-slate-400 mr-2"></i>Live Reconstruction Error Scatter Plot</span>
                            <span class="text-xs text-slate-400 font-mono">500 Transactions Matrix</span>
                        </div>
                        <canvas id="fraud-canvas" class="w-full h-[220px] bg-slate-950 rounded-lg"></canvas>
                    </div>

                    <!-- Graph Legend block -->
                    <div class="grid grid-cols-3 gap-2 text-center text-[10px] sm:text-xs">
                        <div class="p-2 rounded bg-emerald-500/10 border border-emerald-500/20 flex items-center justify-center gap-1.5 text-emerald-400">
                            <span class="h-2 w-2 rounded-full bg-emerald-400 inline-block"></span> Normal (TP/TN)
                        </div>
                        <div class="p-2 rounded bg-rose-500/10 border border-rose-500/20 flex items-center justify-center gap-1.5 text-rose-400">
                            <span class="h-2 w-2 rounded-full bg-rose-400 inline-block"></span> Detected Fraud
                        </div>
                        <div class="p-2 rounded bg-amber-500/10 border border-amber-500/20 flex items-center justify-center gap-1.5 text-amber-400">
                            <span class="h-2 w-2 rounded-full bg-amber-400 inline-block"></span> Missed / False Alert
                        </div>
                    </div>
                </div>
            </div>

            <!-- CONTAINER 3: MOCKMATE SANDBOX -->
            <div id="pg-interview-prep" class="hidden grid grid-cols-1 lg:grid-cols-12 gap-8 items-stretch">
                <!-- Sandbox Info Panel -->
                <div class="lg:col-span-5 p-6 rounded-2xl bg-darkCard border border-darkBorder flex flex-col justify-between space-y-6">
                    <div class="space-y-4">
                        <div class="flex items-center gap-3">
                            <span class="p-2 rounded-lg bg-indigo-500/10 text-indigo-400"><i class="fa-solid fa-graduation-cap"></i></span>
                            <h3 class="font-extrabold text-lg">MockMate Interactive AI</h3>
                        </div>
                        <p class="text-sm text-slate-400 leading-relaxed">
                            **MockMate** is an AI Interview Preparation Platform powered by **MERN & Gemini AI**.
                        </p>
                        <p class="text-xs text-slate-400">
                            Select a target engineering domain below, and generate a dynamic interview question complete with dynamic hints powered by real API prompt engineering parameters.
                        </p>
                    </div>

                    <!-- Domain selector selection -->
                    <div class="space-y-3">
                        <label class="text-xs uppercase text-slate-400 tracking-wider font-semibold block">Select Job Domain:</label>
                        <select id="mm-role" class="w-full bg-slate-900 border border-darkBorder rounded-xl p-3 text-sm text-slate-300 focus:outline-none focus:border-indigo-500 transition-colors">
                            <option value="React & Next.js Frontend Engineer">React & Next.js Frontend Engineer</option>
                            <option value="Java Spring Boot Microservices Developer">Java Spring Boot Microservices Developer</option>
                            <option value="AI / ML & Deep Learning Engineer">AI / ML & Deep Learning Engineer</option>
                            <option value="DevOps & Kubernetes Cloud Specialist">DevOps & Kubernetes Cloud Specialist</option>
                        </select>
                    </div>

                    <!-- Action Trigger -->
                    <button onclick="generateMockQuestion()" id="mm-gen-btn" class="w-full py-3 rounded-xl bg-indigo-600 hover:bg-indigo-500 text-white font-semibold text-sm transition-all shadow-lg hover:shadow-indigo-500/20 flex items-center justify-center gap-2">
                        <i class="fa-solid fa-wand-magic-sparkles animate-pulse"></i> Generate Interview Question
                    </button>
                </div>

                <!-- Sandbox Terminal View -->
                <div class="lg:col-span-7 rounded-2xl bg-slate-950 border border-darkBorder overflow-hidden flex flex-col min-h-[350px]">
                    <div class="bg-darkCard px-4 py-3 border-b border-darkBorder flex justify-between items-center text-xs text-slate-400 font-mono">
                        <span><i class="fa-solid fa-code text-indigo-400 mr-2"></i>mockmate-inference-engine.js</span>
                        <span class="flex h-2 w-2 rounded-full bg-indigo-500"></span>
                    </div>
                    
                    <div class="flex-1 p-6 font-mono text-xs sm:text-sm space-y-4 overflow-y-auto max-h-[300px]">
                        <!-- Terminal introductory state -->
                        <div class="space-y-2">
                            <p class="text-slate-500">&gt; System initialized. Awaiting domain prompt generation...</p>
                            <p class="text-slate-500">&gt; Prompt configuration: temperature: 0.7, topK: 40</p>
                        </div>
                        
                        <!-- Output dynamic panel -->
                        <div id="mm-output" class="hidden space-y-4">
                            <div class="p-4 rounded-xl bg-indigo-500/5 border border-indigo-500/10 space-y-2">
                                <span class="text-indigo-400 font-bold block">[QUESTION GENERATED]</span>
                                <p id="mm-question-txt" class="text-slate-200 leading-relaxed text-xs sm:text-sm"></p>
                            </div>
                            <div class="p-4 rounded-xl bg-emerald-500/5 border border-emerald-500/10 space-y-1">
                                <span class="text-emerald-400 font-bold block">[AI EVALUATION HINTS]</span>
                                <p id="mm-hint-txt" class="text-slate-300 leading-relaxed text-xs"></p>
                            </div>
                        </div>

                        <!-- Processing State -->
                        <div id="mm-loader" class="hidden flex flex-col items-center justify-center py-12 space-y-3">
                            <div class="h-8 w-8 border-4 border-indigo-500 border-t-transparent rounded-full animate-spin"></div>
                            <span class="text-slate-400 font-mono text-xs">Querying Gemini API & parsing structured outputs...</span>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- THE TECH STACK & SKILLS MATRIX -->
        <section id="skills" class="space-y-8">
            <div class="flex flex-col md:flex-row md:items-end justify-between gap-4 border-b border-darkBorder pb-4">
                <div>
                    <h2 class="text-2xl sm:text-3xl font-extrabold tracking-tight flex items-center gap-3">
                        <span class="h-8 w-1 bg-indigo-500 rounded-full"></span> Tech Stack Matrix
                    </h2>
                    <p class="text-slate-400 text-sm mt-1">Click on any core skill below to instantly filter my featured projects that use it!</p>
                </div>
                <button onclick="clearSkillFilter()" id="skill-clear-btn" class="hidden text-xs text-rose-400 hover:text-rose-300 transition-all">
                    <i class="fa-solid fa-xmark mr-1"></i> Clear Filter
                </button>
            </div>

            <!-- Skills grid categorization -->
            <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
                <!-- Group 1: Languages & Frontend -->
                <div class="p-6 rounded-2xl bg-darkCard border border-darkBorder space-y-4">
                    <h3 class="font-extrabold text-sm uppercase tracking-widest text-indigo-400 flex items-center gap-2">
                        <i class="fa-solid fa-laptop-code"></i> Frontend & Languages
                    </h3>
                    <div class="flex flex-wrap gap-2">
                        <span onclick="toggleSkillFilter('Java', this)" class="skill-badge cursor-pointer px-3 py-1.5 rounded-lg bg-slate-900 border border-darkBorder hover:border-indigo-500/50 hover:bg-indigo-950/20 text-xs font-semibold text-slate-300 transition-all flex items-center gap-1.5">
                            <i class="fa-brands fa-java text-[#ED8B00]"></i> Java
                        </span>
                        <span onclick="toggleSkillFilter('JavaScript', this)" class="skill-badge cursor-pointer px-3 py-1.5 rounded-lg bg-slate-900 border border-darkBorder hover:border-indigo-500/50 hover:bg-indigo-950/20 text-xs font-semibold text-slate-300 transition-all flex items-center gap-1.5">
                            <i class="fa-brands fa-js text-[#F7DF1E]"></i> JavaScript
                        </span>
                        <span onclick="toggleSkillFilter('TypeScript', this)" class="skill-badge cursor-pointer px-3 py-1.5 rounded-lg bg-slate-900 border border-darkBorder hover:border-indigo-500/50 hover:bg-indigo-950/20 text-xs font-semibold text-slate-300 transition-all flex items-center gap-1.5">
                            <i class="fa-solid fa-code text-[#3178C6]"></i> TypeScript
                        </span>
                        <span onclick="toggleSkillFilter('React', this)" class="skill-badge cursor-pointer px-3 py-1.5 rounded-lg bg-slate-900 border border-darkBorder hover:border-indigo-500/50 hover:bg-indigo-950/20 text-xs font-semibold text-slate-300 transition-all flex items-center gap-1.5">
                            <i class="fa-brands fa-react text-[#61DAFB]"></i> React
                        </span>
                        <span onclick="toggleSkillFilter('Next.js', this)" class="skill-badge cursor-pointer px-3 py-1.5 rounded-lg bg-slate-900 border border-darkBorder hover:border-indigo-500/50 hover:bg-indigo-950/20 text-xs font-semibold text-slate-300 transition-all flex items-center gap-1.5">
                            <i class="fa-solid fa-n text-white"></i> Next.js
                        </span>
                        <span onclick="toggleSkillFilter('Angular', this)" class="skill-badge cursor-pointer px-3 py-1.5 rounded-lg bg-slate-900 border border-darkBorder hover:border-indigo-500/50 hover:bg-indigo-950/20 text-xs font-semibold text-slate-300 transition-all flex items-center gap-1.5">
                            <i class="fa-brands fa-angular text-[#DD0031]"></i> Angular
                        </span>
                        <span onclick="toggleSkillFilter('Tailwind', this)" class="skill-badge cursor-pointer px-3 py-1.5 rounded-lg bg-slate-900 border border-darkBorder hover:border-indigo-500/50 hover:bg-indigo-950/20 text-xs font-semibold text-slate-300 transition-all flex items-center gap-1.5">
                            <i class="fa-solid fa-wind text-[#06B6D4]"></i> Tailwind
                        </span>
                    </div>
                </div>

                <!-- Group 2: Backend & Database -->
                <div class="p-6 rounded-2xl bg-darkCard border border-darkBorder space-y-4">
                    <h3 class="font-extrabold text-sm uppercase tracking-widest text-emerald-400 flex items-center gap-2">
                        <i class="fa-solid fa-server"></i> Backend & Databases
                    </h3>
                    <div class="flex flex-wrap gap-2">
                        <span onclick="toggleSkillFilter('Spring Boot', this)" class="skill-badge cursor-pointer px-3 py-1.5 rounded-lg bg-slate-900 border border-darkBorder hover:border-emerald-500/50 hover:bg-emerald-950/20 text-xs font-semibold text-slate-300 transition-all flex items-center gap-1.5">
                            <i class="fa-solid fa-leaf text-[#6DB33F]"></i> Spring Boot
                        </span>
                        <span onclick="toggleSkillFilter('Node.js', this)" class="skill-badge cursor-pointer px-3 py-1.5 rounded-lg bg-slate-900 border border-darkBorder hover:border-emerald-500/50 hover:bg-emerald-950/20 text-xs font-semibold text-slate-300 transition-all flex items-center gap-1.5">
                            <i class="fa-brands fa-node-js text-[#339933]"></i> Node.js
                        </span>
                        <span onclick="toggleSkillFilter('Django', this)" class="skill-badge cursor-pointer px-3 py-1.5 rounded-lg bg-slate-900 border border-darkBorder hover:border-emerald-500/50 hover:bg-emerald-950/20 text-xs font-semibold text-slate-300 transition-all flex items-center gap-1.5">
                            <i class="fa-brands fa-python text-[#092E20]"></i> Django
                        </span>
                        <span onclick="toggleSkillFilter('MongoDB', this)" class="skill-badge cursor-pointer px-3 py-1.5 rounded-lg bg-slate-900 border border-darkBorder hover:border-emerald-500/50 hover:bg-emerald-950/20 text-xs font-semibold text-slate-300 transition-all flex items-center gap-1.5">
                            <i class="fa-solid fa-database text-[#47A248]"></i> MongoDB
                        </span>
                        <span onclick="toggleSkillFilter('PostgreSQL', this)" class="skill-badge cursor-pointer px-3 py-1.5 rounded-lg bg-slate-900 border border-darkBorder hover:border-emerald-500/50 hover:bg-emerald-950/20 text-xs font-semibold text-slate-300 transition-all flex items-center gap-1.5">
                            <i class="fa-solid fa-database text-[#4169E1]"></i> PostgreSQL
                        </span>
                        <span onclick="toggleSkillFilter('MySQL', this)" class="skill-badge cursor-pointer px-3 py-1.5 rounded-lg bg-slate-900 border border-darkBorder hover:border-emerald-500/50 hover:bg-emerald-950/20 text-xs font-semibold text-slate-300 transition-all flex items-center gap-1.5">
                            <i class="fa-solid fa-database text-[#4479A1]"></i> MySQL
                        </span>
                    </div>
                </div>

                <!-- Group 3: AI/ML & DevOps -->
                <div class="p-6 rounded-2xl bg-darkCard border border-darkBorder space-y-4">
                    <h3 class="font-extrabold text-sm uppercase tracking-widest text-pink-400 flex items-center gap-2">
                        <i class="fa-solid fa-gears"></i> AI/ML & Cloud
                    </h3>
                    <div class="flex flex-wrap gap-2">
                        <span onclick="toggleSkillFilter('Python', this)" class="skill-badge cursor-pointer px-3 py-1.5 rounded-lg bg-slate-900 border border-darkBorder hover:border-pink-500/50 hover:bg-pink-950/20 text-xs font-semibold text-slate-300 transition-all flex items-center gap-1.5">
                            <i class="fa-brands fa-python text-[#3776AB]"></i> Python
                        </span>
                        <span onclick="toggleSkillFilter('TensorFlow', this)" class="skill-badge cursor-pointer px-3 py-1.5 rounded-lg bg-slate-900 border border-darkBorder hover:border-pink-500/50 hover:bg-pink-950/20 text-xs font-semibold text-slate-300 transition-all flex items-center gap-1.5">
                            <i class="fa-solid fa-brain text-[#FF6F00]"></i> TensorFlow
                        </span>
                        <span onclick="toggleSkillFilter('Gemini AI', this)" class="skill-badge cursor-pointer px-3 py-1.5 rounded-lg bg-slate-900 border border-darkBorder hover:border-pink-500/50 hover:bg-pink-950/20 text-xs font-semibold text-slate-300 transition-all flex items-center gap-1.5">
                            <i class="fa-solid fa-robot text-[#4285F4]"></i> Gemini AI
                        </span>
                        <span onclick="toggleSkillFilter('LangChain', this)" class="skill-badge cursor-pointer px-3 py-1.5 rounded-lg bg-slate-900 border border-darkBorder hover:border-pink-500/50 hover:bg-pink-950/20 text-xs font-semibold text-slate-300 transition-all flex items-center gap-1.5">
                            <i class="fa-solid fa-link text-[#1C3C3C]"></i> LangChain
                        </span>
                        <span onclick="toggleSkillFilter('Docker', this)" class="skill-badge cursor-pointer px-3 py-1.5 rounded-lg bg-slate-900 border border-darkBorder hover:border-pink-500/50 hover:bg-pink-950/20 text-xs font-semibold text-slate-300 transition-all flex items-center gap-1.5">
                            <i class="fa-brands fa-docker text-[#2496ED]"></i> Docker
                        </span>
                        <span onclick="toggleSkillFilter('Kubernetes', this)" class="skill-badge cursor-pointer px-3 py-1.5 rounded-lg bg-slate-900 border border-darkBorder hover:border-pink-500/50 hover:bg-pink-950/20 text-xs font-semibold text-slate-300 transition-all flex items-center gap-1.5">
                            <i class="fa-solid fa-dharmachakra text-[#326CE5]"></i> Kubernetes
                        </span>
                    </div>
                </div>
            </div>
        </section>

        <!-- FEATURED PROJECTS SHOWCASE -->
        <section id="projects" class="space-y-8">
            <div class="flex flex-col sm:flex-row sm:items-end justify-between gap-4 border-b border-darkBorder pb-4">
                <div>
                    <h2 class="text-2xl sm:text-3xl font-extrabold tracking-tight flex items-center gap-3">
                        <span class="h-8 w-1 bg-indigo-500 rounded-full"></span> Featured Engineering Projects
                    </h2>
                    <p class="text-slate-400 text-sm mt-1">Explore some of my high-impact production and ML deployments.</p>
                </div>
                
                <!-- Tag Filter Selection -->
                <div class="flex gap-2">
                    <input id="proj-search" type="text" oninput="filterProjects()" placeholder="Search project name..." class="bg-slate-950 border border-darkBorder rounded-xl px-4 py-2 text-xs text-slate-300 focus:outline-none focus:border-indigo-500" />
                </div>
            </div>

            <!-- Grid of Projects -->
            <div id="projects-grid" class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6 transition-all">
                
                <!-- Project 1 -->
                <div class="project-card flex flex-col justify-between p-6 rounded-2xl bg-darkCard border border-darkBorder hover:border-indigo-500/40 hover:-translate-y-1 transition-all shadow-xl group" data-tags="MERN,Gemini AI,React,Node.js,MongoDB,Tailwind">
                    <div class="space-y-4">
                        <div class="flex justify-between items-start">
                            <span class="text-[10px] tracking-wider uppercase font-extrabold text-indigo-400 font-mono">01 · Production App</span>
                            <div class="flex gap-2 text-sm text-slate-400">
                                <a href="https://github.com/JalapatiRavikumar/AI-Projects/tree/main/MockMate" target="_blank" class="hover:text-white transition-colors"><i class="fa-brands fa-github"></i></a>
                                <a href="https://mockmate-react-ai.vercel.app/" target="_blank" class="hover:text-white transition-colors"><i class="fa-solid fa-arrow-up-right-from-square"></i></a>
                            </div>
                        </div>
                        <h4 class="text-lg font-bold group-hover:text-indigo-300 transition-colors">MockMate — AI Interview Platform</h4>
                        <p class="text-xs text-slate-400 leading-relaxed">
                            AI-driven interview prep platform featuring dynamic domain-specific question generation, live context parsing via Gemini API, and low-latency interaction streams.
                        </p>
                    </div>
                    <div class="mt-6 pt-4 border-t border-darkBorder/60 flex flex-wrap gap-1.5">
                        <span class="px-2 py-0.5 rounded text-[10px] font-semibold bg-indigo-500/10 text-indigo-400">MERN</span>
                        <span class="px-2 py-0.5 rounded text-[10px] font-semibold bg-slate-900 text-slate-400">Gemini AI</span>
                        <span class="px-2 py-0.5 rounded text-[10px] font-semibold bg-slate-900 text-slate-400">React</span>
                        <span class="px-2 py-0.5 rounded text-[10px] font-semibold bg-slate-900 text-slate-400">MongoDB</span>
                    </div>
                </div>

                <!-- Project 2 -->
                <div class="project-card flex flex-col justify-between p-6 rounded-2xl bg-darkCard border border-darkBorder hover:border-indigo-500/40 hover:-translate-y-1 transition-all shadow-xl group" data-tags="Next.js,TypeScript,React,Tailwind">
                    <div class="space-y-4">
                        <div class="flex justify-between items-start">
                            <span class="text-[10px] tracking-wider uppercase font-extrabold text-emerald-400 font-mono">02 · Frontend</span>
                            <div class="flex gap-2 text-sm text-slate-400">
                                <a href="https://github.com/JalapatiRavikumar/AI-Projects/tree/main/Resume-Builder" target="_blank" class="hover:text-white transition-colors"><i class="fa-brands fa-github"></i></a>
                                <a href="https://resume-builder-ai-mauve.vercel.app/" target="_blank" class="hover:text-white transition-colors"><i class="fa-solid fa-arrow-up-right-from-square"></i></a>
                            </div>
                        </div>
                        <h4 class="text-lg font-bold group-hover:text-emerald-300 transition-colors">Dynamic Resume Builder</h4>
                        <p class="text-xs text-slate-400 leading-relaxed">
                            Engineered a highly performance-oriented resume editor in Next.js. Integrates seamless print engine parsing and fast, real-time template switching workflows.
                        </p>
                    </div>
                    <div class="mt-6 pt-4 border-t border-darkBorder/60 flex flex-wrap gap-1.5">
                        <span class="px-2 py-0.5 rounded text-[10px] font-semibold bg-emerald-500/10 text-emerald-400">Next.js</span>
                        <span class="px-2 py-0.5 rounded text-[10px] font-semibold bg-slate-900 text-slate-400">TypeScript</span>
                        <span class="px-2 py-0.5 rounded text-[10px] font-semibold bg-slate-900 text-slate-400">React</span>
                        <span class="px-2 py-0.5 rounded text-[10px] font-semibold bg-slate-900 text-slate-400">Tailwind</span>
                    </div>
                </div>

                <!-- Project 3 -->
                <div class="project-card flex flex-col justify-between p-6 rounded-2xl bg-darkCard border border-darkBorder hover:border-indigo-500/40 hover:-translate-y-1 transition-all shadow-xl group" data-tags="React,Django,PostgreSQL,Python">
                    <div class="space-y-4">
                        <div class="flex justify-between items-start">
                            <span class="text-[10px] tracking-wider uppercase font-extrabold text-pink-400 font-mono">03 · Full Stack</span>
                            <div class="flex gap-2 text-sm text-slate-400">
                                <a href="https://github.com/JalapatiRavikumar/AI-Projects/tree/main/FullStack_Ecommerce_App" target="_blank" class="hover:text-white transition-colors"><i class="fa-brands fa-github"></i></a>
                                <a href="https://fullstack-ecommerce-app-pearl.vercel.app/" target="_blank" class="hover:text-white transition-colors"><i class="fa-solid fa-arrow-up-right-from-square"></i></a>
                            </div>
                        </div>
                        <h4 class="text-lg font-bold group-hover:text-pink-300 transition-colors">Full-Stack Django E-Commerce</h4>
                        <p class="text-xs text-slate-400 leading-relaxed">
                            Robust commercial catalog deploying a Django REST structure on PostgreSQL. Secure Stripe integrations handle dynamic purchase routing workflows securely.
                        </p>
                    </div>
                    <div class="mt-6 pt-4 border-t border-darkBorder/60 flex flex-wrap gap-1.5">
                        <span class="px-2 py-0.5 rounded text-[10px] font-semibold bg-pink-500/10 text-pink-400">React</span>
                        <span class="px-2 py-0.5 rounded text-[10px] font-semibold bg-slate-900 text-slate-400">Django</span>
                        <span class="px-2 py-0.5 rounded text-[10px] font-semibold bg-slate-900 text-slate-400">PostgreSQL</span>
                        <span class="px-2 py-0.5 rounded text-[10px] font-semibold bg-slate-900 text-slate-400">Python</span>
                    </div>
                </div>

                <!-- Project 4 -->
                <div class="project-card flex flex-col justify-between p-6 rounded-2xl bg-darkCard border border-darkBorder hover:border-indigo-500/40 hover:-translate-y-1 transition-all shadow-xl group" data-tags="MERN,React,Node.js,MongoDB">
                    <div class="space-y-4">
                        <div class="flex justify-between items-start">
                            <span class="text-[10px] tracking-wider uppercase font-extrabold text-indigo-400 font-mono">04 · Portal Web</span>
                            <div class="flex gap-2 text-sm text-slate-400">
                                <a href="https://github.com/JalapatiRavikumar/AI-Projects/tree/main/Food_Delivery_Application" target="_blank" class="hover:text-white transition-colors"><i class="fa-brands fa-github"></i></a>
                                <a href="https://food-delivery-hub-ashen.vercel.app/" target="_blank" class="hover:text-white transition-colors"><i class="fa-solid fa-arrow-up-right-from-square"></i></a>
                            </div>
                        </div>
                        <h4 class="text-lg font-bold group-hover:text-indigo-300 transition-colors">Hub Food Delivery Platform</h4>
                        <p class="text-xs text-slate-400 leading-relaxed">
                            Complete customer ordering portal featuring interactive state carts, custom checkout APIs, and a comprehensive real-time store manager administration backend.
                        </p>
                    </div>
                    <div class="mt-6 pt-4 border-t border-darkBorder/60 flex flex-wrap gap-1.5">
                        <span class="px-2 py-0.5 rounded text-[10px] font-semibold bg-indigo-500/10 text-indigo-400">MERN</span>
                        <span class="px-2 py-0.5 rounded text-[10px] font-semibold bg-slate-900 text-slate-400">React</span>
                        <span class="px-2 py-0.5 rounded text-[10px] font-semibold bg-slate-900 text-slate-400">Node.js</span>
                        <span class="px-2 py-0.5 rounded text-[10px] font-semibold bg-slate-900 text-slate-400">MongoDB</span>
                    </div>
                </div>

                <!-- Project 5 -->
                <div class="project-card flex flex-col justify-between p-6 rounded-2xl bg-darkCard border border-darkBorder hover:border-indigo-500/40 hover:-translate-y-1 transition-all shadow-xl group" data-tags="React,Spring Boot,Java,MySQL">
                    <div class="space-y-4">
                        <div class="flex justify-between items-start">
                            <span class="text-[10px] tracking-wider uppercase font-extrabold text-emerald-400 font-mono">05 · LMS Enterprise</span>
                            <div class="flex gap-2 text-sm text-slate-400">
                                <a href="https://github.com/PATMESH/Learning-Management-System" target="_blank" class="hover:text-white transition-colors"><i class="fa-brands fa-github"></i></a>
                                <a href="https://farmers-align-wizard-endorsement.trycloudflare.com/" target="_blank" class="hover:text-white transition-colors"><i class="fa-solid fa-arrow-up-right-from-square"></i></a>
                            </div>
                        </div>
                        <h4 class="text-lg font-bold group-hover:text-emerald-300 transition-colors">Spring Boot LMS Portal</h4>
                        <p class="text-xs text-slate-400 leading-relaxed">
                            Robust educational portal backed by a Spring Boot microservices cluster. Features complete course lifecycle tracking and automatic secure PDF certification generation.
                        </p>
                    </div>
                    <div class="mt-6 pt-4 border-t border-darkBorder/60 flex flex-wrap gap-1.5">
                        <span class="px-2 py-0.5 rounded text-[10px] font-semibold bg-emerald-500/10 text-emerald-400">React</span>
                        <span class="px-2 py-0.5 rounded text-[10px] font-semibold bg-slate-900 text-slate-400">Spring Boot</span>
                        <span class="px-2 py-0.5 rounded text-[10px] font-semibold bg-slate-900 text-slate-400">Java</span>
                        <span class="px-2 py-0.5 rounded text-[10px] font-semibold bg-slate-900 text-slate-400">MySQL</span>
                    </div>
                </div>

                <!-- Project 6 -->
                <div class="project-card flex flex-col justify-between p-6 rounded-2xl bg-darkCard border border-darkBorder hover:border-indigo-500/40 hover:-translate-y-1 transition-all shadow-xl group" data-tags="React,Gemini AI,JavaScript">
                    <div class="space-y-4">
                        <div class="flex justify-between items-start">
                            <span class="text-[10px] tracking-wider uppercase font-extrabold text-pink-400 font-mono">06 · Conversational AI</span>
                            <div class="flex gap-2 text-sm text-slate-400">
                                <a href="https://github.com/JalapatiRavikumar/echo-gemini-chat" target="_blank" class="hover:text-white transition-colors"><i class="fa-brands fa-github"></i></a>
                                <a href="https://echo-gemini-chat.vercel.app/" target="_blank" class="hover:text-white transition-colors"><i class="fa-solid fa-arrow-up-right-from-square"></i></a>
                            </div>
                        </div>
                        <h4 class="text-lg font-bold group-hover:text-pink-300 transition-colors">Echo Gemini Chat Portal</h4>
                        <p class="text-xs text-slate-400 leading-relaxed">
                            Highly optimized client-side React chatbot running context-aware Gemini inferences using state-of-the-art optimistic update rendering patterns.
                        </p>
                    </div>
                    <div class="mt-6 pt-4 border-t border-darkBorder/60 flex flex-wrap gap-1.5">
                        <span class="px-2 py-0.5 rounded text-[10px] font-semibold bg-pink-500/10 text-pink-400">React</span>
                        <span class="px-2 py-0.5 rounded text-[10px] font-semibold bg-slate-900 text-slate-400">Gemini AI</span>
                        <span class="px-2 py-0.5 rounded text-[10px] font-semibold bg-slate-900 text-slate-400">JavaScript</span>
                    </div>
                </div>

                <!-- Project 7 -->
                <div class="project-card flex flex-col justify-between p-6 rounded-2xl bg-darkCard border border-darkBorder hover:border-indigo-500/40 hover:-translate-y-1 transition-all shadow-xl group" data-tags="Python,LangChain,Gemini AI">
                    <div class="space-y-4">
                        <div class="flex justify-between items-start">
                            <span class="text-[10px] tracking-wider uppercase font-extrabold text-indigo-400 font-mono">07 · Python AI</span>
                            <div class="flex gap-2 text-sm text-slate-400">
                                <a href="https://github.com/JalapatiRavikumar/AI-Resume-Analyzer" target="_blank" class="hover:text-white transition-colors"><i class="fa-brands fa-github"></i></a>
                            </div>
                        </div>
                        <h4 class="text-lg font-bold group-hover:text-indigo-300 transition-colors">AI Resume Analyzer RAG</h4>
                        <p class="text-xs text-slate-400 leading-relaxed">
                            Engineered a highly advanced career mapping tool. Embeds resume segments into FAISS vector spaces for smart recommendations using OpenAI/LangChain.
                        </p>
                    </div>
                    <div class="mt-6 pt-4 border-t border-darkBorder/60 flex flex-wrap gap-1.5">
                        <span class="px-2 py-0.5 rounded text-[10px] font-semibold bg-indigo-500/10 text-indigo-400">Python</span>
                        <span class="px-2 py-0.5 rounded text-[10px] font-semibold bg-slate-900 text-slate-400">LangChain</span>
                        <span class="px-2 py-0.5 rounded text-[10px] font-semibold bg-slate-900 text-slate-400">Gemini AI</span>
                    </div>
                </div>

                <!-- Project 8 -->
                <div class="project-card flex flex-col justify-between p-6 rounded-2xl bg-darkCard border border-darkBorder hover:border-indigo-500/40 hover:-translate-y-1 transition-all shadow-xl group" data-tags="Python,TensorFlow">
                    <div class="space-y-4">
                        <div class="flex justify-between items-start">
                            <span class="text-[10px] tracking-wider uppercase font-extrabold text-emerald-400 font-mono">08 · Deep Learning</span>
                            <div class="flex gap-2 text-sm text-slate-400">
                                <a href="https://github.com/curiousily/Credit-Card-Fraud-Detection-using-Autoencoders-in-Keras" target="_blank" class="hover:text-white transition-colors"><i class="fa-brands fa-github"></i></a>
                            </div>
                        </div>
                        <h4 class="text-lg font-bold group-hover:text-emerald-300 transition-colors">Fraud Detection Autoencoder</h4>
                        <p class="text-xs text-slate-400 leading-relaxed">
                            Unsupervised Keras neural network trained to detect highly imbalanced (99.8%) anomalies. Reconstruction parameters hit a solid 90% F1 value.
                        </p>
                    </div>
                    <div class="mt-6 pt-4 border-t border-darkBorder/60 flex flex-wrap gap-1.5">
                        <span class="px-2 py-0.5 rounded text-[10px] font-semibold bg-emerald-500/10 text-emerald-400">Python</span>
                        <span class="px-2 py-0.5 rounded text-[10px] font-semibold bg-slate-900 text-slate-400">TensorFlow</span>
                    </div>
                </div>

                <!-- Project 9 -->
                <div class="project-card flex flex-col justify-between p-6 rounded-2xl bg-darkCard border border-darkBorder hover:border-indigo-500/40 hover:-translate-y-1 transition-all shadow-xl group" data-tags="Python,Docker">
                    <div class="space-y-4">
                        <div class="flex justify-between items-start">
                            <span class="text-[10px] tracking-wider uppercase font-extrabold text-pink-400 font-mono">09 · Production MLOps</span>
                            <div class="flex gap-2 text-sm text-slate-400">
                                <a href="https://github.com/entbappy/End-to-end-Machine-Learning-Project-with-MLflow" target="_blank" class="hover:text-white transition-colors"><i class="fa-brands fa-github"></i></a>
                            </div>
                        </div>
                        <h4 class="text-lg font-bold group-hover:text-pink-300 transition-colors">End-to-End ML Pipeline</h4>
                        <p class="text-xs text-slate-400 leading-relaxed">
                            Designed YAML-configured dataset pipeline pipelines leveraging MLflow metric logging alongside modular Flask REST serving wrappers.
                        </p>
                    </div>
                    <div class="mt-6 pt-4 border-t border-darkBorder/60 flex flex-wrap gap-1.5">
                        <span class="px-2 py-0.5 rounded text-[10px] font-semibold bg-pink-500/10 text-pink-400">Python</span>
                        <span class="px-2 py-0.5 rounded text-[10px] font-semibold bg-slate-900 text-slate-400">Docker</span>
                    </div>
                </div>

            </div>
        </section>

        <!-- CAREER TIMELINE & EDUCATION -->
        <section id="experience" class="grid grid-cols-1 lg:grid-cols-12 gap-8 items-start">
            
            <!-- Experience Timeline -->
            <div class="lg:col-span-7 space-y-6">
                <h2 class="text-2xl sm:text-3xl font-extrabold tracking-tight flex items-center gap-3">
                    <span class="h-8 w-1 bg-indigo-500 rounded-full"></span> Professional Journey
                </h2>
                
                <div class="relative border-l-2 border-darkBorder pl-6 ml-4 space-y-10">
                    <!-- Experience Block 1 -->
                    <div class="relative">
                        <!-- Bullet indicator -->
                        <span class="absolute -left-[31px] top-1.5 h-4 w-4 rounded-full bg-slate-950 border-2 border-indigo-500 flex items-center justify-center">
                            <span class="h-1.5 w-1.5 rounded-full bg-indigo-500"></span>
                        </span>
                        
                        <div class="space-y-2">
                            <div class="flex flex-wrap items-center justify-between gap-2">
                                <h3 class="font-extrabold text-lg text-slate-100">Full Stack Developer Intern</h3>
                                <span class="px-2.5 py-1 rounded bg-indigo-500/10 text-indigo-400 text-xs font-semibold">Jul 2024 - Present</span>
                            </div>
                            <span class="text-xs text-slate-400 font-bold block">KODNEST · Bengaluru, India</span>
                            <p class="text-xs sm:text-sm text-slate-400 leading-relaxed">
                                Gained hands-on proficiency across Java full stack microservices and MERN development. Collaborated within Agile workflows to engineer secure REST endpoints, database schemas (MongoDB/MySQL), and ship high-performance user interfaces.
                            </p>
                            <ul class="text-xs text-slate-500 space-y-1 list-disc list-inside">
                                <li>Configured secure token structures utilizing Spring Security APIs.</li>
                                <li>Optimized database response latency using optimized indexing techniques.</li>
                                <li>Assisted in implementing cloud automation frameworks (Docker/Kubernetes).</li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Education Block -->
            <div class="lg:col-span-5 space-y-6">
                <h2 class="text-2xl sm:text-3xl font-extrabold tracking-tight flex items-center gap-3">
                    <span class="h-8 w-1 bg-indigo-500 rounded-full"></span> Education
                </h2>
                
                <div class="p-6 rounded-2xl bg-darkCard border border-darkBorder space-y-4">
                    <div class="flex justify-between items-start gap-4">
                        <span class="p-3 rounded-xl bg-slate-800 text-indigo-400"><i class="fa-solid fa-graduation-cap text-2xl"></i></span>
                        <div class="text-right">
                            <span class="text-xs text-indigo-400 font-bold font-mono">B.Tech CSE</span>
                            <span class="text-[10px] block text-slate-500">Graduated 2024</span>
                        </div>
                    </div>
                    <div>
                        <h3 class="font-extrabold text-slate-200">Santhiram Engineering College</h3>
                        <span class="text-xs text-slate-400">Computer Science Engineering</span>
                        <p class="text-xs text-slate-500 mt-2 leading-relaxed">
                            Core Curriculum: Data Structures & Algorithms, Object-Oriented Analysis, Relational Databases, Computer Network Architectures, and Software Systems Engineering.
                        </p>
                    </div>
                </div>
            </div>
        </section>

        <!-- CONNECT & COLLABORATE PORTAL -->
        <section id="connect" class="relative rounded-3xl overflow-hidden border border-darkBorder glassmorphism p-8 md:p-12">
            <div class="absolute -bottom-16 -right-16 w-80 h-80 bg-indigo-500/5 rounded-full blur-[100px] pointer-events-none"></div>
            
            <div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
                <div class="space-y-6">
                    <span class="px-3 py-1 rounded-full bg-indigo-500/10 text-indigo-400 text-xs font-semibold uppercase tracking-wider border border-indigo-500/20">Let's Connect</span>
                    <h2 class="text-3xl sm:text-4xl font-extrabold tracking-tight">Let's build something extraordinary!</h2>
                    <p class="text-slate-400 text-sm leading-relaxed max-w-md">
                        I am actively open for full-time employment roles, innovative open-source contributions, or consulting projects. Get in touch directly using the contact portal or drop me an email!
                    </p>
                    
                    <div class="space-y-4 text-xs font-mono">
                        <div class="flex items-center gap-3 text-slate-300">
                            <i class="fa-regular fa-envelope text-indigo-400 text-base"></i> ravikumarjalapatii@gmail.com
                        </div>
                        <div class="flex items-center gap-3 text-slate-300">
                            <i class="fa-solid fa-location-dot text-indigo-400 text-base"></i> Bengaluru, Karnataka, India
                        </div>
                    </div>
                </div>

                <!-- Interactive Contact Form -->
                <div class="p-6 rounded-2xl bg-slate-950 border border-darkBorder space-y-4">
                    <form id="contact-form" onsubmit="handleContactSubmit(event)" class="space-y-4">
                        <div class="grid grid-cols-2 gap-4">
                            <div>
                                <label class="text-xs text-slate-400 block mb-1">Your Name</label>
                                <input type="text" required placeholder="John Doe" class="w-full bg-slate-900 border border-darkBorder rounded-xl p-3 text-xs text-slate-200 focus:outline-none focus:border-indigo-500 transition-colors" />
                            </div>
                            <div>
                                <label class="text-xs text-slate-400 block mb-1">Your Email</label>
                                <input type="email" required placeholder="john@example.com" class="w-full bg-slate-900 border border-darkBorder rounded-xl p-3 text-xs text-slate-200 focus:outline-none focus:border-indigo-500 transition-colors" />
                            </div>
                        </div>
                        <div>
                            <label class="text-xs text-slate-400 block mb-1">Subject</label>
                            <input type="text" required placeholder="Inquiry" class="w-full bg-slate-900 border border-darkBorder rounded-xl p-3 text-xs text-slate-200 focus:outline-none focus:border-indigo-500 transition-colors" />
                        </div>
                        <div>
                            <label class="text-xs text-slate-400 block mb-1">Your Message</label>
                            <textarea rows="4" required placeholder="Describe your inquiry..." class="w-full bg-slate-900 border border-darkBorder rounded-xl p-3 text-xs text-slate-200 focus:outline-none focus:border-indigo-500 transition-colors resize-none"></textarea>
                        </div>
                        <button type="submit" class="w-full py-3 rounded-xl bg-indigo-600 hover:bg-indigo-500 text-white font-semibold text-xs transition-all shadow-lg hover:shadow-indigo-500/20">
                            Send Secure Message
                        </button>
                    </form>
                    
                    <!-- Form Success Message Area -->
                    <div id="contact-success" class="hidden p-4 rounded-xl bg-emerald-500/10 border border-emerald-500/20 text-emerald-400 text-center text-xs space-y-1">
                        <span class="font-bold block">✨ Message Logged Successfully!</span>
                        <p class="text-[10px]">Thank you! I will respond to your inquiry shortly.</p>
                    </div>
                </div>
            </div>
        </section>

    </div>

    <!-- Sticky Notification Box -->
    <div id="toast" class="fixed bottom-6 right-6 z-50 transform translate-y-24 opacity-0 transition-all duration-300 max-w-sm p-4 rounded-xl bg-slate-950 border border-darkBorder flex items-center gap-3 shadow-2xl">
        <span class="p-2 rounded bg-emerald-500/10 text-emerald-400 text-sm" id="toast-icon"><i class="fa-solid fa-circle-check"></i></span>
        <span class="text-xs text-slate-300 font-semibold" id="toast-msg">Text copied to clipboard</span>
    </div>

    <!-- Footer block -->
    <footer class="mt-16 border-t border-darkBorder py-12 text-center text-xs text-slate-500 space-y-3">
        <div>&copy; 2026 Jalapati Ravikumar. Custom built and designed from scratch.</div>
        <div class="flex justify-center gap-6 text-base">
            <a href="https://github.com/JalapatiRavikumar" target="_blank" class="hover:text-indigo-400 transition-colors"><i class="fa-brands fa-github"></i></a>
            <a href="https://www.linkedin.com/in/jalapatiravikumar" target="_blank" class="hover:text-indigo-400 transition-colors"><i class="fa-brands fa-linkedin"></i></a>
            <a href="mailto:ravikumarjalapatii@gmail.com" class="hover:text-indigo-400 transition-colors"><i class="fa-regular fa-envelope"></i></a>
        </div>
    </footer>

    <!-- INTERACTIVE JAVASCRIPT LOGIC -->
    <script>
        // 1. TYPING ANIMATION IMPLEMENTATION
        const strings = [
            "🚀 Full Stack Developer | MERN + Java + Python",
            "⚛️ React.js | Next.js | Node.js | Spring Boot",
            "🤖 Gemini AI | LangChain | RAG | Prompt Engineering",
            "🧠 Deep Learning | TensorFlow | Keras | MLOps",
            "☁️ Docker | Kubernetes | Azure AKS | CI/CD DevOps"
        ];
        let currentStringIndex = 0;
        let charIndex = 0;
        let isDeleting = false;
        const typingSpeed = 60;
        const deletingSpeed = 30;
        const pauseTime = 1800;

        function type() {
            const currentString = strings[currentStringIndex];
            const displayEl = document.getElementById('typing-text');
            
            if (isDeleting) {
                displayEl.innerHTML = currentString.substring(0, charIndex - 1);
                charIndex--;
            } else {
                displayEl.innerHTML = currentString.substring(0, charIndex + 1);
                charIndex++;
            }

            if (!isDeleting && charIndex === currentString.length) {
                isDeleting = true;
                setTimeout(type, pauseTime);
            } else if (isDeleting && charIndex === 0) {
                isDeleting = false;
                currentStringIndex = (currentStringIndex + 1) % strings.length;
                setTimeout(type, 300);
            } else {
                setTimeout(type, isDeleting ? deletingSpeed : typingSpeed);
            }
        }

        window.onload = function() {
            // Start Typing animation
            type();
            // Initialize Fraud detection simulation
            initFraudSim();
        }

        // 2. TOAST SYSTEM
        function showToast(message, isSuccess = true) {
            const toast = document.getElementById('toast');
            const toastMsg = document.getElementById('toast-msg');
            const toastIcon = document.getElementById('toast-icon');

            toastMsg.innerText = message;
            if (isSuccess) {
                toastIcon.className = "p-2 rounded bg-emerald-500/10 text-emerald-400 text-sm";
                toastIcon.innerHTML = `<i class="fa-solid fa-circle-check"></i>`;
            } else {
                toastIcon.className = "p-2 rounded bg-rose-500/10 text-rose-400 text-sm";
                toastIcon.innerHTML = `<i class="fa-solid fa-circle-exclamation"></i>`;
            }

            toast.classList.remove('translate-y-24', 'opacity-0');
            setTimeout(() => {
                toast.classList.add('translate-y-24', 'opacity-0');
            }, 3000);
        }

        function copyToClipboard(text, btn) {
            const temp = document.createElement('textarea');
            temp.value = text;
            document.body.appendChild(temp);
            temp.select();
            document.execCommand('copy');
            document.body.removeChild(temp);
            showToast("Copied content directly to clipboard!");
        }

        // 3. PLAYGROUND SWITCHER
        function switchPlayground(target) {
            const pgTwin = document.getElementById('pg-ai-twin');
            const pgFraud = document.getElementById('pg-fraud-model');
            const pgPrep = document.getElementById('pg-interview-prep');

            const tabTwin = document.getElementById('tab-ai-twin');
            const tabFraud = document.getElementById('tab-fraud-model');
            const tabPrep = document.getElementById('tab-interview-prep');

            // Hide all
            pgTwin.classList.add('hidden');
            pgFraud.classList.add('hidden');
            pgPrep.classList.add('hidden');

            // Reset tab styles
            [tabTwin, tabFraud, tabPrep].forEach(t => {
                t.className = "px-4 py-2 rounded-lg text-slate-400 hover:text-white transition-all";
            });

            if (target === 'ai-twin') {
                pgTwin.classList.remove('hidden');
                tabTwin.className = "px-4 py-2 rounded-lg bg-indigo-600 text-white transition-all";
            } else if (target === 'fraud-model') {
                pgFraud.classList.remove('hidden');
                tabFraud.className = "px-4 py-2 rounded-lg bg-indigo-600 text-white transition-all";
                // Trigger canvas redraw
                setTimeout(drawFraudMatrix, 50);
            } else if (target === 'interview-prep') {
                pgPrep.classList.remove('hidden');
                tabPrep.className = "px-4 py-2 rounded-lg bg-indigo-600 text-white transition-all";
            }
        }

        // 4. CHAT COMPONENT (USING GEMINI INFERENCE FLOW)
        const apiKey = ""; // Canvas runtime injection handler
        let conversationContext = [
            {
                role: "user",
                parts: [{ text: `You are the AI Agent of Jalapati Ravikumar. Answer questions confidently and concisely as his professional digital representative.
                Here are your professional attributes and background details:
                - Name: Jalapati Ravikumar
                - Role: Full Stack Developer & AI/ML Engineer
                - Location: Bengaluru, India
                - Education: B.Tech CSE from Santhiram Engineering College (Graduated 2024)
                - Technical Capabilities: Frontend (React, Next.js, Angular, TypeScript, Tailwind), Backend (Spring Boot, Spring Security, Hibernate, Node.js, Express, Django REST, REST APIs, Microservices, JWT Auth, Socket.io), Databases (MongoDB, PostgreSQL, MySQL, Redis), AI/ML (TensorFlow, Keras, Gemini API, LangChain, FAISS VectorDB, Python, Pandas, Streamlit), DevOps (Docker, Kubernetes, Azure AKS, CI/CD, Git).
                - Work Experience: Full Stack Developer Intern at Kodnest, Bengaluru. Gained deep familiarity building robust APIs, securing course portals with JWT, automating workflows, and optimization bundle sizes.
                - Portfolio & Contacts: LinkedIn (linkedin.com/in/jalapatiravikumar), Email (ravikumarjalapatii@gmail.com), Github (github.com/JalapatiRavikumar), Live portfolio (jalapatiravikumar-portfolio.vercel.app).
                - Metrics Accomplished: Optimized bundle payloads by 30%, enhanced frontend performance resulting in 40% speedier renders, and designed unsupervised Autoencoders reducing False Positives by 25% with 92% metric precision.
                Personality details: Energetic, lighthearted, highly programmatic, witty! Feel free to talk about console.log debugging or write custom snippets if relevant. Always keep messages compact, friendly, and structured. Avoid giving standard lengthy disclaimers.` }]
            },
            {
                role: "model",
                parts: [{ text: "Understood! I am now running as Ravikumar's professional digital representitive. Ask me anything and I will provide brief, expert answers." }]
            }
        ];

        async function handleChatSubmit(e) {
            e.preventDefault();
            const inputEl = document.getElementById('chat-input');
            const message = inputEl.value.trim();
            if (!message) return;

            inputEl.value = '';
            appendMessage("User", message);

            const loaderId = appendLoader();

            // Exponential backoff API call
            try {
                const responseText = await queryGeminiAPI(message);
                removeLoader(loaderId);
                appendMessage("AI", responseText);
            } catch (error) {
                removeLoader(loaderId);
                appendMessage("AI", "The AI Twin is currently offline taking a developer break. Please try querying again in a moment, or contact Jalapati directly via email!");
            }
        }

        async function queryGeminiAPI(userText) {
            const payload = {
                contents: [
                    ...conversationContext,
                    { role: "user", parts: [{ text: userText }] }
                ]
            };

            const url = `https://generativelanguage.googleapis.com/v1beta/models/gemini-2.5-flash-preview-09-2025:generateContent?key=${apiKey}`;
            
            // Retry handling with exponential backoff
            let delay = 1000;
            for (let i = 0; i < 5; i++) {
                try {
                    const response = await fetch(url, {
                        method: 'POST',
                        headers: { 'Content-Type': 'application/json' },
                        body: JSON.stringify(payload)
                    });
                    if (response.ok) {
                        const data = await response.json();
                        const parsedText = data.candidates?.[0]?.content?.parts?.[0]?.text;
                        
                        // Push into context history
                        conversationContext.push({ role: "user", parts: [{ text: userText }] });
                        conversationContext.push({ role: "model", parts: [{ text: parsedText }] });
                        return parsedText;
                    }
                } catch (e) {
                    // Suppressing console log as requested by guidelines
                }
                await new Promise(res => setTimeout(res, delay));
                delay *= 2;
            }
            throw new Error("API completely exhausted after retry limits.");
        }

        function appendMessage(sender, text) {
            const chatBox = document.getElementById('chat-messages');
            const msgDiv = document.createElement('div');
            
            if (sender === "User") {
                msgDiv.className = "flex gap-3 items-start justify-end max-w-[85%] ml-auto";
                msgDiv.innerHTML = `
                    <div class="p-3.5 rounded-2xl bg-indigo-600 text-sm leading-relaxed text-white">
                        ${text}
                    </div>
                `;
            } else {
                msgDiv.className = "flex gap-3 items-start max-w-[85%] animate-fadeIn";
                msgDiv.innerHTML = `
                    <div class="h-8 w-8 rounded-full bg-indigo-500/10 border border-indigo-500/30 flex items-center justify-center text-xs text-indigo-400 font-bold shrink-0">AI</div>
                    <div class="p-3.5 rounded-2xl bg-darkCard border border-darkBorder text-sm leading-relaxed text-slate-300">
                        ${text}
                    </div>
                `;
            }
            chatBox.appendChild(msgDiv);
            chatBox.scrollTop = chatBox.scrollHeight;
        }

        function appendLoader() {
            const chatBox = document.getElementById('chat-messages');
            const loaderId = "loader-" + Date.now();
            const loaderDiv = document.createElement('div');
            loaderDiv.id = loaderId;
            loaderDiv.className = "flex gap-3 items-start max-w-[85%] animate-fadeIn";
            loaderDiv.innerHTML = `
                <div class="h-8 w-8 rounded-full bg-indigo-500/10 border border-indigo-500/30 flex items-center justify-center text-xs text-indigo-400 font-bold shrink-0">AI</div>
                <div class="p-3.5 rounded-2xl bg-darkCard border border-darkBorder text-sm leading-relaxed text-slate-400 flex items-center gap-2">
                    <span class="flex h-2 w-2 rounded-full bg-indigo-500 animate-ping"></span> Thinking...
                </div>
            `;
            chatBox.appendChild(loaderDiv);
            chatBox.scrollTop = chatBox.scrollHeight;
            return loaderId;
        }

        function removeLoader(id) {
            const el = document.getElementById(id);
            if (el) el.remove();
        }

        function clearChat() {
            document.getElementById('chat-messages').innerHTML = `
                <div class="flex gap-3 items-start max-w-[85%]">
                    <div class="h-8 w-8 rounded-full bg-indigo-500/10 border border-indigo-500/30 flex items-center justify-center text-xs text-indigo-400 font-bold shrink-0">AI</div>
                    <div class="p-3.5 rounded-2xl bg-darkCard border border-darkBorder text-sm leading-relaxed text-slate-300">
                        Chat reset! Ask me anything about my tech stack, B.Tech background, internships, projects, or how to contact me.
                    </div>
                </div>
            `;
            conversationContext = conversationContext.slice(0, 2);
        }

        function sendSuggestedQuestion(question) {
            document.getElementById('chat-input').value = question;
            document.getElementById('chat-submit-btn').click();
        }

        // 5. INTERACTIVE ML FRAUD SIMULATOR LOGIC
        let transactions = [];
        let curThreshold = 3.2;

        function initFraudSim() {
            // Pre-generate normal & abnormal reconstruction errors to simulate model threshold evaluations
            transactions = [];
            // Generate 400 normal distributions
            for (let i = 0; i < 400; i++) {
                transactions.push({
                    id: i,
                    error: 1.0 + Math.random() * 2.2,
                    isFraud: false
                });
            }
            // Generate 100 abnormal (fraud) distributions
            for (let i = 400; i < 500; i++) {
                transactions.push({
                    id: i,
                    error: 2.8 + Math.random() * 4.2,
                    isFraud: true
                });
            }
            // Sort by index ID to scatter cleanly
            transactions.sort((a, b) => a.id - b.id);
            updateFraudSim(3.2);
        }

        function updateFraudSim(val) {
            curThreshold = parseFloat(val);
            document.getElementById('threshold-val').innerText = curThreshold.toFixed(2);
            
            // Calculate dynamic confusion matrices
            let tp = 0; // Truly classified as Fraud
            let fp = 0; // Normal classified as Fraud
            let tn = 0; // Normal flagged as normal
            let fn = 0; // Fraud missed completely

            transactions.forEach(t => {
                const flagged = t.error >= curThreshold;
                if (flagged && t.isFraud) tp++;
                else if (flagged && !t.isFraud) fp++;
                else if (!flagged && !t.isFraud) tn++;
                else if (!flagged && t.isFraud) fn++;
            });

            const precision = tp / (tp + fp) || 0;
            const recall = tp / (tp + fn) || 0;
            const f1 = (2 * precision * recall) / (precision + recall) || 0;

            document.getElementById('precision-out').innerText = (precision * 100).toFixed(1) + "%";
            document.getElementById('recall-out').innerText = (recall * 100).toFixed(1) + "%";
            document.getElementById('f1-out').innerText = (f1 * 100).toFixed(1) + "%";

            drawFraudMatrix();
        }

        function drawFraudMatrix() {
            const canvas = document.getElementById('fraud-canvas');
            if (!canvas) return;
            const ctx = canvas.getContext('2d');
            
            // Adapt resolutions to container widths dynamically
            const rect = canvas.getBoundingClientRect();
            canvas.width = rect.width;
            canvas.height = rect.height;

            ctx.clearRect(0, 0, canvas.width, canvas.height);

            // Draw clean background grid markings
            ctx.strokeStyle = "#1f293d";
            ctx.lineWidth = 1;
            for (let i = 1; i < 5; i++) {
                const y = (canvas.height / 5) * i;
                ctx.beginPath();
                ctx.moveTo(0, y);
                ctx.lineTo(canvas.width, y);
                ctx.stroke();
            }

            // Draw transaction scatter plots
            transactions.forEach((t) => {
                const x = (t.id / 500) * canvas.width;
                // invert error relative to height representation
                const y = canvas.height - (t.error / 8.0) * canvas.height;

                const flagged = t.error >= curThreshold;
                
                if (t.isFraud) {
                    if (flagged) {
                        ctx.fillStyle = "#f43f5e"; // True positive (Fraud successfully caught)
                    } else {
                        ctx.fillStyle = "#f59e0b"; // False negative (Fraud missed)
                    }
                } else {
                    if (flagged) {
                        ctx.fillStyle = "#fb7185"; // False positive (Safe flagged as alert)
                    } else {
                        ctx.fillStyle = "#10b981"; // True negative (Safe, verified normal)
                    }
                }

                ctx.beginPath();
                ctx.arc(x, y, 3, 0, 2 * Math.PI);
                ctx.fill();
            });

            // Draw dynamic Reconstruction Threshold threshold line
            const lineY = canvas.height - (curThreshold / 8.0) * canvas.height;
            ctx.strokeStyle = "#6366f1";
            ctx.lineWidth = 3.5;
            ctx.setLineDash([6, 4]);
            ctx.beginPath();
            ctx.moveTo(0, lineY);
            ctx.lineTo(canvas.width, lineY);
            ctx.stroke();
            ctx.setLineDash([]);

            // Label line
            ctx.fillStyle = "#6366f1";
            ctx.font = "bold 10px JetBrains Mono";
            ctx.fillText(`Error Cutoff: ${curThreshold.toFixed(2)}`, 12, lineY - 8);
        }

        // Handle dynamically resizing plots
        window.addEventListener('resize', () => {
            if (document.getElementById('pg-fraud-model').classList.contains('hidden')) return;
            drawFraudMatrix();
        });

        // 6. MOCKMATE SANDBOX GENERATOR
        async function generateMockQuestion() {
            const role = document.getElementById('mm-role').value;
            const loader = document.getElementById('mm-loader');
            const output = document.getElementById('mm-output');
            const genBtn = document.getElementById('mm-gen-btn');

            loader.classList.remove('hidden');
            output.classList.add('hidden');
            genBtn.disabled = true;

            const prompt = `Act as an expert technical interviewer. Generate ONE highly challenging, job-specific interview question based on the target position: "${role}".
            Also provide a short section titled [HINT] explaining the architectural concepts expected in an expert solution.
            Output format MUST be EXACTLY:
            Question: {questionText}
            Hint: {hintText}`;

            try {
                const text = await queryGeminiAPI(prompt);
                
                // Parse out question and hint segment structures
                let question = "";
                let hint = "";
                
                if (text.includes("Question:") && text.includes("Hint:")) {
                    const qIdx = text.indexOf("Question:");
                    const hIdx = text.indexOf("Hint:");
                    question = text.substring(qIdx + 9, hIdx).trim();
                    hint = text.substring(hIdx + 5).trim();
                } else {
                    question = text;
                    hint = "Evaluate optimization frameworks, execution timelines, complexity trade-offs, and design system constraints.";
                }

                document.getElementById('mm-question-txt').innerText = question;
                document.getElementById('mm-hint-txt').innerText = hint;

                loader.classList.add('hidden');
                output.classList.remove('hidden');
            } catch (err) {
                loader.classList.add('hidden');
                showToast("Sandbox offline. Please verify API configurations.", false);
            } finally {
                genBtn.disabled = false;
            }
        }

        // 7. TECH STACK SELECTION INTERACTION
        let activeSkillFilter = null;

        function toggleSkillFilter(skillName, badgeEl) {
            const badges = document.querySelectorAll('.skill-badge');
            const clearBtn = document.getElementById('skill-clear-btn');

            // Reset badge styles
            badges.forEach(b => {
                b.className = "skill-badge cursor-pointer px-3 py-1.5 rounded-lg bg-slate-900 border border-darkBorder hover:border-indigo-500/50 hover:bg-indigo-950/20 text-xs font-semibold text-slate-300 transition-all flex items-center gap-1.5";
            });

            if (activeSkillFilter === skillName) {
                // De-activate filter
                activeSkillFilter = null;
                clearBtn.classList.add('hidden');
                filterProjectsByTag(null);
            } else {
                // Activate filter
                activeSkillFilter = skillName;
                badgeEl.className = "skill-badge cursor-pointer px-3 py-1.5 rounded-lg bg-indigo-600 border-indigo-500 text-xs font-semibold text-white transition-all flex items-center gap-1.5 shadow-lg shadow-indigo-600/30";
                clearBtn.classList.remove('hidden');
                filterProjectsByTag(skillName);
            }
        }

        function clearSkillFilter() {
            activeSkillFilter = null;
            document.getElementById('skill-clear-btn').classList.add('hidden');
            const badges = document.querySelectorAll('.skill-badge');
            badges.forEach(b => {
                b.className = "skill-badge cursor-pointer px-3 py-1.5 rounded-lg bg-slate-900 border border-darkBorder hover:border-indigo-500/50 hover:bg-indigo-950/20 text-xs font-semibold text-slate-300 transition-all flex items-center gap-1.5";
            });
            filterProjectsByTag(null);
        }

        function filterProjectsByTag(tag) {
            const projects = document.querySelectorAll('.project-card');
            projects.forEach(p => {
                if (!tag) {
                    p.style.display = "flex";
                    return;
                }
                const pTags = p.getAttribute('data-tags').split(',');
                if (pTags.includes(tag)) {
                    p.style.display = "flex";
                } else {
                    p.style.display = "none";
                }
            });
        }

        function filterProjects() {
            const searchVal = document.getElementById('proj-search').value.toLowerCase().trim();
            const projects = document.querySelectorAll('.project-card');

            projects.forEach(p => {
                const title = p.querySelector('h4').innerText.toLowerCase();
                const desc = p.querySelector('p').innerText.toLowerCase();
                const match = title.includes(searchVal) || desc.includes(searchVal);
                
                // Keep selected tag filters in sync as well
                if (activeSkillFilter) {
                    const pTags = p.getAttribute('data-tags').split(',');
                    const tagMatch = pTags.includes(activeSkillFilter);
                    p.style.display = (match && tagMatch) ? "flex" : "none";
                } else {
                    p.style.display = match ? "flex" : "none";
                }
            });
        }

        // 8. CONTACT FORM SUBMIT
        function handleContactSubmit(e) {
            e.preventDefault();
            const form = document.getElementById('contact-form');
            const successMsg = document.getElementById('contact-success');

            // Perform simple interface animation
            form.classList.add('hidden');
            successMsg.classList.remove('hidden');
            showToast("Successfully sent message!");
        }
    </script>
</body>
</html>
