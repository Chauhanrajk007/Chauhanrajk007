<svg viewBox="0 0 880 490" width="880" height="490" fill="none" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <!-- Deep Canvas Gradient -->
    <linearGradient id="bg" x1="0" y1="0" x2="880" y2="490" gradientUnits="userSpaceOnUse">
      <stop offset="0%" stop-color="#07090e" />
      <stop offset="50%" stop-color="#0b0f19" />
      <stop offset="100%" stop-color="#07080d" />
    </linearGradient>

    <!-- Top Shimmer Prism Line -->
    <linearGradient id="topHighlight" x1="0" y1="0" x2="880" y2="0" gradientUnits="userSpaceOnUse">
      <stop offset="0%" stop-color="#38bdf8" stop-opacity="0" />
      <stop offset="30%" stop-color="#818cf8" stop-opacity="0.8" />
      <stop offset="70%" stop-color="#c084fc" stop-opacity="0.8" />
      <stop offset="100%" stop-color="#f472b6" stop-opacity="0" />
    </linearGradient>

    <!-- Name Shimmer Gradient -->
    <linearGradient id="nameGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#67e8f9">
        <animate attributeName="stop-color" values="#67e8f9;#c084fc;#f472b6;#67e8f9" dur="9s" repeatCount="indefinite"/>
      </stop>
      <stop offset="50%" stop-color="#a78bfa">
        <animate attributeName="stop-color" values="#a78bfa;#38bdf8;#f43f5e;#a78bfa" dur="9s" repeatCount="indefinite"/>
      </stop>
      <stop offset="100%" stop-color="#f472b6">
        <animate attributeName="stop-color" values="#f472b6;#67e8f9;#a78bfa;#f472b6" dur="9s" repeatCount="indefinite"/>
      </stop>
    </linearGradient>

    <!-- Glass Cards Gradients -->
    <linearGradient id="cardGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#ffffff" stop-opacity="0.05" />
      <stop offset="100%" stop-color="#ffffff" stop-opacity="0.015" />
    </linearGradient>

    <linearGradient id="cardBorder" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#ffffff" stop-opacity="0.14" />
      <stop offset="100%" stop-color="#ffffff" stop-opacity="0.04" />
    </linearGradient>

    <!-- Ambient Glow Lights -->
    <radialGradient id="neonGlowLeft" cx="150" cy="110" r="280" gradientUnits="userSpaceOnUse">
      <stop offset="0%" stop-color="#6366f1" stop-opacity="0.18" />
      <stop offset="100%" stop-color="#6366f1" stop-opacity="0" />
    </radialGradient>

    <radialGradient id="neonGlowRight" cx="740" cy="190" r="260" gradientUnits="userSpaceOnUse">
      <stop offset="0%" stop-color="#06b6d4" stop-opacity="0.15" />
      <stop offset="100%" stop-color="#06b6d4" stop-opacity="0" />
    </radialGradient>

    <!-- Micro Dot Grid -->
    <pattern id="dotPattern" width="24" height="24" patternUnits="userSpaceOnUse">
      <circle cx="2" cy="2" r="1" fill="#ffffff" fill-opacity="0.035" />
    </pattern>
  </defs>

  <style>
    .font-sans { font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Inter, Helvetica, Arial, sans-serif; }
    .font-mono { font-family: 'JetBrains Mono', 'SF Mono', Consolas, 'Fira Code', monospace; }

    @keyframes blink { 0%, 100% { opacity: 1; } 50% { opacity: 0; } }
    @keyframes pulseGlow { 0%, 100% { transform: scale(1); opacity: 0.95; } 50% { transform: scale(1.25); opacity: 0.35; } }

    .cursor-blink { animation: blink 1.1s infinite steps(1); }
    .status-pulse { animation: pulseGlow 2.2s infinite ease-in-out; transform-origin: center; }
    
    .social-card { transition: all 0.2s ease; cursor: pointer; }
    .social-card:hover rect { fill-opacity: 0.08; stroke-opacity: 0.35; }
  </style>

  <!-- ================= CANVAS BACKGROUND ================= -->
  <rect width="880" height="490" rx="18" fill="url(#bg)" />
  <rect width="880" height="490" rx="18" fill="url(#dotPattern)" />
  <rect width="880" height="490" rx="18" fill="url(#neonGlowLeft)" />
  <rect width="880" height="490" rx="18" fill="url(#neonGlowRight)" />

  <!-- Outer Border & Prism Line -->
  <rect x="0.5" y="0.5" width="879" height="489" rx="17.5" stroke="#ffffff" stroke-opacity="0.08" />
  <line x1="120" y1="1" x2="760" y2="1" stroke="url(#topHighlight)" stroke-width="2" />

  <!-- ================= TOP NAVIGATION HUD ================= -->
  <!-- GitHub ID Badge -->
  <g transform="translate(32, 24)">
    <rect width="250" height="28" rx="7" fill="#ffffff" fill-opacity="0.03" stroke="#ffffff" stroke-opacity="0.06" />
    <circle cx="14" cy="14" r="3.5" fill="#f43f5e" />
    <circle cx="26" cy="14" r="3.5" fill="#f59e0b" />
    <circle cx="38" cy="14" r="3.5" fill="#10b981" />
    <text x="52" y="18" class="font-mono" font-size="11.5" fill="#94a3b8" letter-spacing="0.5">github/Chauhanrajk007</text>
  </g>

  <!-- Live Status Badge -->
  <g transform="translate(620, 24)">
    <rect width="228" height="28" rx="14" fill="#022c22" fill-opacity="0.6" stroke="#059669" stroke-opacity="0.4" />
    <circle cx="16" cy="14" r="7" fill="#34d399" fill-opacity="0.25" class="status-pulse" />
    <circle cx="16" cy="14" r="4" fill="#10b981" />
    <text x="29" y="18" class="font-mono" font-size="11" fill="#a7f3d0" font-weight="600">Available for Opportunities</text>
  </g>

  <!-- ================= HERO IDENTITY ================= -->
  <g transform="translate(32, 74)">
    <!-- Eyebrow Tag -->
    <rect x="0" y="0" width="180" height="22" rx="11" fill="#4f46e5" fill-opacity="0.15" stroke="#6366f1" stroke-opacity="0.3" />
    <text x="90" y="15" text-anchor="middle" class="font-mono" font-size="10.5" fill="#a5b4fc" font-weight="600" letter-spacing="1">FULL-STACK · ML &amp; DL</text>

    <!-- Name Headline -->
    <text x="0" y="56" class="font-sans" font-size="44" font-weight="800" fill="url(#nameGrad)" letter-spacing="-1.2">
      Chauhan Raj K
    </text>

    <!-- Subtitle -->
    <g transform="translate(0, 84)">
      <text x="0" y="0" class="font-mono" font-size="14.5" fill="#e2e8f0" font-weight="500">
        <tspan fill="#a855f7">❯</tspan> Full-Stack Developer &amp; ML/DL Engineer
      </text>
      <rect x="355" y="-12" width="7" height="15" fill="#38bdf8" class="cursor-blink" rx="1"/>
    </g>

    <!-- Meta Info -->
    <g transform="translate(0, 108)">
      <text class="font-mono" font-size="11.5" fill="#94a3b8">
        🎓 <tspan fill="#cbd5e1">CSE (IoT) · Presidency University</tspan>
        <tspan fill="#475569" dx="8">|</tspan>
        <tspan dx="8">📍</tspan> <tspan fill="#cbd5e1">Bengaluru, IN</tspan>
      </text>
    </g>
  </g>

  <!-- ================= BENTO STATS (RIGHT) ================= -->
  <!-- Card 1: LeetCode (Java) -->
  <g transform="translate(528, 72)">
    <rect width="320" height="62" rx="12" fill="url(#cardGrad)" stroke="url(#cardBorder)" />
    <circle cx="32" cy="31" r="15" fill="#f59e0b" fill-opacity="0.12" stroke="#f59e0b" stroke-opacity="0.3" />
    <text x="32" y="36" text-anchor="middle" font-size="13">⚡</text>

    <text x="58" y="25" class="font-sans" font-size="10" font-weight="600" fill="#f59e0b" letter-spacing="1">LEETCODE &amp; DSA</text>
    <text x="58" y="46" class="font-sans" font-size="14.5" font-weight="700" fill="#f8fafc">
      90+ Problems <tspan font-weight="600" fill="#fbbf24">in Java</tspan>
    </text>
  </g>

  <!-- Card 2: AI & ML/DL -->
  <g transform="translate(528, 142)">
    <rect width="320" height="62" rx="12" fill="url(#cardGrad)" stroke="url(#cardBorder)" />
    <circle cx="32" cy="31" r="15" fill="#c084fc" fill-opacity="0.12" stroke="#c084fc" stroke-opacity="0.3" />
    <text x="32" y="36" text-anchor="middle" font-size="13">🧠</text>

    <text x="58" y="25" class="font-sans" font-size="10" font-weight="600" fill="#c084fc" letter-spacing="1">INTELLIGENT SYSTEMS &amp; AWARDS</text>
    <text x="58" y="46" class="font-sans" font-size="14" font-weight="700" fill="#f8fafc">
      ML / DL · RAG <tspan font-weight="400" fill="#64748b">|</tspan> <tspan fill="#d8b4fe" font-size="12">2x Hackathon Finalist</tspan>
    </text>
  </g>

  <!-- ================= SECTION DIVIDER ================= -->
  <line x1="32" y1="218" x2="848" y2="218" stroke="#ffffff" stroke-opacity="0.06" />

  <!-- ================= ALL 11 TECH STACK PILLS ================= -->
  <text x="32" y="240" class="font-mono" font-size="10.5" font-weight="600" fill="#64748b" letter-spacing="1.5">TECH ARSENAL</text>

  <!-- Row 1: Frontend & Backend Core (7 Items) -->
  <g transform="translate(32, 252)">
    <!-- React -->
    <g transform="translate(0, 0)">
      <rect width="78" height="28" rx="7" fill="#0f172a" stroke="#0284c7" stroke-opacity="0.35"/>
      <circle cx="14" cy="14" r="4" fill="none" stroke="#38bdf8" stroke-width="1.2"/>
      <text x="25" y="18" class="font-mono" font-size="11.5" fill="#7dd3fc">React</text>
    </g>
    <!-- Node.js -->
    <g transform="translate(86, 0)">
      <rect width="90" height="28" rx="7" fill="#0f172a" stroke="#16a34a" stroke-opacity="0.35"/>
      <polygon points="14,10 18,12 18,16 14,18 10,16 10,12" fill="none" stroke="#4ade80" stroke-width="1.2"/>
      <text x="25" y="18" class="font-mono" font-size="11.5" fill="#86efac">Node.js</text>
    </g>
    <!-- Express -->
    <g transform="translate(184, 0)">
      <rect width="86" height="28" rx="7" fill="#0f172a" stroke="#ffffff" stroke-opacity="0.12"/>
      <text x="14" y="18" class="font-mono" font-size="11.5" fill="#e2e8f0">Express</text>
    </g>
    <!-- Tailwind CSS -->
    <g transform="translate(278, 0)">
      <rect width="114" height="28" rx="7" fill="#0f172a" stroke="#0891b2" stroke-opacity="0.35"/>
      <text x="14" y="18" class="font-mono" font-size="11.5" fill="#67e8f9">Tailwind CSS</text>
    </g>
    <!-- MongoDB -->
    <g transform="translate(400, 0)">
      <rect width="96" height="28" rx="7" fill="#0f172a" stroke="#059669" stroke-opacity="0.35"/>
      <path d="M14 9 C12 12, 12 15, 14 17 C16 15, 16 12, 14 9 Z" fill="#34d399"/>
      <text x="24" y="18" class="font-mono" font-size="11.5" fill="#6ee7b7">MongoDB</text>
    </g>
    <!-- Firebase -->
    <g transform="translate(504, 0)">
      <rect width="92" height="28" rx="7" fill="#0f172a" stroke="#f59e0b" stroke-opacity="0.35"/>
      <text x="14" y="18" class="font-mono" font-size="11.5" fill="#fcd34d">Firebase</text>
    </g>
    <!-- Supabase -->
    <g transform="translate(604, 0)">
      <rect width="98" height="28" rx="7" fill="#0f172a" stroke="#059669" stroke-opacity="0.35"/>
      <path d="M13 14 L16 10 L15 13 L18 13 L14 18 L15 14 Z" fill="#10b981"/>
      <text x="25" y="18" class="font-mono" font-size="11.5" fill="#a7f3d0">Supabase</text>
    </g>
  </g>

  <!-- Row 2: Languages & AI / Search (4 Items + Highlights) -->
  <g transform="translate(32, 288)">
    <!-- Java -->
    <g transform="translate(0, 0)">
      <rect width="112" height="28" rx="7" fill="#1e130c" stroke="#ea580c" stroke-opacity="0.45"/>
      <circle cx="15" cy="14" r="4" fill="#f97316"/>
      <text x="26" y="18" class="font-mono" font-size="11.5" fill="#fed7aa" font-weight="600">Java (DSA)</text>
    </g>
    <!-- Python -->
    <g transform="translate(120, 0)">
      <rect width="92" height="28" rx="7" fill="#0f172a" stroke="#38bdf8" stroke-opacity="0.35"/>
      <circle cx="14" cy="12" r="1.5" fill="#38bdf8"/>
      <circle cx="18" cy="16" r="1.5" fill="#facc15"/>
      <text x="26" y="18" class="font-mono" font-size="11.5" fill="#bae6fd">Python</text>
    </g>
    <!-- C++ -->
    <g transform="translate(220, 0)">
      <rect width="70" height="28" rx="7" fill="#0f172a" stroke="#6366f1" stroke-opacity="0.35"/>
      <text x="14" y="18" class="font-mono" font-size="11.5" fill="#a5b4fc">C++</text>
    </g>
    <!-- RAG Search -->
    <g transform="translate(298, 0)">
      <rect width="124" height="28" rx="7" fill="#24123b" stroke="#c084fc" stroke-opacity="0.5"/>
      <path d="M14 10 L15 13 L18 14 L15 15 L14 18 L13 15 L10 14 L13 13 Z" fill="#c084fc"/>
      <text x="25" y="18" class="font-mono" font-size="11.5" fill="#f3e8ff" font-weight="600">RAG Search</text>
    </g>
    <!-- Machine Learning & Deep Learning Badge -->
    <g transform="translate(430, 0)">
      <rect width="180" height="28" rx="7" fill="#1e1b4b" stroke="#818cf8" stroke-opacity="0.45"/>
      <circle cx="15" cy="14" r="3.5" fill="#818cf8"/>
      <text x="26" y="18" class="font-mono" font-size="11.5" fill="#c7d2fe" font-weight="500">ML / Deep Learning</text>
    </g>
  </g>

  <!-- ================= SECTION DIVIDER ================= -->
  <line x1="32" y1="334" x2="848" y2="334" stroke="#ffffff" stroke-opacity="0.06" />

  <!-- ================= CONNECT HUD: 4 BALANCED CARDS ================= -->
  <text x="32" y="358" class="font-mono" font-size="10.5" font-weight="600" fill="#64748b" letter-spacing="1.5">CONNECT &amp; REACH OUT</text>

  <g transform="translate(32, 372)">
    <!-- GitHub Link Card -->
    <a href="https://github.com/Chauhanrajk007" target="_blank" class="social-card">
      <g transform="translate(0, 0)">
        <rect width="194" height="46" rx="9" fill="#ffffff" fill-opacity="0.03" stroke="#ffffff" stroke-opacity="0.09" />
        <!-- GitHub Mark -->
        <circle cx="24" cy="23" r="11" fill="#ffffff" fill-opacity="0.08" />
        <path d="M24 15 C19.6 15 16 18.6 16 23 C16 26.6 18.3 29.5 21.5 30.6 C21.9 30.7 22.1 30.4 22.1 30.2 V28.8 C19.9 29.3 19.4 27.7 19.4 27.7 C19 26.8 18.5 26.5 18.5 26.5 C17.8 26 18.6 26 18.6 26 C19.4 26.1 19.8 26.9 19.8 26.9 C20.5 28.1 21.7 27.8 22.1 27.5 C22.2 27 22.4 26.6 22.7 26.4 C20.9 26.2 19.1 25.5 19.1 22.3 C19.1 21.4 19.4 20.7 20 20.1 C19.9 19.9 19.6 19 20.1 17.8 C20.1 17.8 20.8 17.6 22.3 18.7 C23 18.5 23.7 18.4 24.5 18.4 C25.3 18.4 26 18.5 26.7 18.7 C28.2 17.6 28.9 17.8 28.9 17.8 C29.4 19 29.1 19.9 29 20.1 C29.6 20.7 29.9 21.4 29.9 22.3 C29.9 25.5 28.1 26.2 26.3 26.4 C26.6 26.7 26.9 27.2 26.9 28 V30.2 C26.9 30.4 27.1 30.7 27.5 30.6 C30.7 29.5 33 26.5 33 23 C33 18.6 29.4 15 24 15 Z" fill="#e2e8f0"/>
        <text x="44" y="20" class="font-sans" font-size="11" font-weight="600" fill="#f1f5f9">GitHub</text>
        <text x="44" y="34" class="font-mono" font-size="10" fill="#94a3b8">@Chauhanrajk007</text>
      </g>
    </a>

    <!-- LinkedIn Link Card -->
    <a href="https://linkedin.com/in/chauhan-raj-k" target="_blank" class="social-card">
      <g transform="translate(206, 0)">
        <rect width="194" height="46" rx="9" fill="#ffffff" fill-opacity="0.03" stroke="#ffffff" stroke-opacity="0.09" />
        <circle cx="24" cy="23" r="11" fill="#0077b5" fill-opacity="0.15" />
        <text x="24" y="28" text-anchor="middle" class="font-sans" font-size="12" font-weight="bold" fill="#38bdf8">in</text>
        <text x="44" y="20" class="font-sans" font-size="11" font-weight="600" fill="#f1f5f9">LinkedIn</text>
        <text x="44" y="34" class="font-mono" font-size="10" fill="#94a3b8">/in/chauhan-raj-k</text>
      </g>
    </a>

    <!-- LeetCode Link Card -->
    <a href="https://leetcode.com/Chauhanrajk007" target="_blank" class="social-card">
      <g transform="translate(412, 0)">
        <rect width="194" height="46" rx="9" fill="#ffffff" fill-opacity="0.03" stroke="#ffffff" stroke-opacity="0.09" />
        <circle cx="24" cy="23" r="11" fill="#f59e0b" fill-opacity="0.15" />
        <text x="24" y="28" text-anchor="middle" font-size="12">⚡</text>
        <text x="44" y="20" class="font-sans" font-size="11" font-weight="600" fill="#f1f5f9">LeetCode</text>
        <text x="44" y="34" class="font-mono" font-size="10" fill="#fbbf24">@Chauhanrajk007</text>
      </g>
    </a>

    <!-- Email Link Card -->
    <a href="mailto:chauhanrajk007@gmail.com" target="_blank" class="social-card">
      <g transform="translate(618, 0)">
        <rect width="198" height="46" rx="9" fill="#ffffff" fill-opacity="0.03" stroke="#ffffff" stroke-opacity="0.09" />
        <circle cx="24" cy="23" r="11" fill="#ef4444" fill-opacity="0.15" />
        <text x="24" y="28" text-anchor="middle" font-size="12">✉️</text>
        <text x="44" y="20" class="font-sans" font-size="11" font-weight="600" fill="#f1f5f9">Email</text>
        <text x="44" y="34" class="font-mono" font-size="9" fill="#94a3b8">chauhanrajk007@...</text>
      </g>
    </a>
  </g>

  <!-- ================= MINI FOOTER BAR ================= -->
  <g transform="translate(32, 442)">
    <text class="font-mono" font-size="11" fill="#64748b">
      🌐 Portfolio: <tspan fill="#38bdf8">chauhanrajk007.github.io/raj-portfolio</tspan>
    </text>
    <text x="635" class="font-mono" font-size="11" fill="#64748b">
      Designed for GitHub Profile README
    </text>
  </g>
</svg>
