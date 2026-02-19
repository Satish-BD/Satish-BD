<svg width="900" height="620" viewBox="0 0 900 620" xmlns="http://www.w3.org/2000/svg" font-family="'Courier New', monospace">
  <defs>
    <!-- Background gradient -->
    <linearGradient id="bgGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#0D1117"/>
      <stop offset="45%" style="stop-color:#0a1929"/>
      <stop offset="100%" style="stop-color:#0d2137"/>
    </linearGradient>

    <!-- Card gradients -->
    <linearGradient id="card1" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#0f2744;stop-opacity:1"/>
      <stop offset="100%" style="stop-color:#0a1929;stop-opacity:1"/>
    </linearGradient>
    <linearGradient id="card2" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#0d2137;stop-opacity:1"/>
      <stop offset="100%" style="stop-color:#0f2744;stop-opacity:1"/>
    </linearGradient>
    <linearGradient id="card3" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#0a1929;stop-opacity:1"/>
      <stop offset="100%" style="stop-color:#0f2744;stop-opacity:1"/>
    </linearGradient>
    <linearGradient id="card4" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#0f2744;stop-opacity:1"/>
      <stop offset="100%" style="stop-color:#0a1929;stop-opacity:1"/>
    </linearGradient>

    <!-- Glow filters -->
    <filter id="glow-blue">
      <feGaussianBlur stdDeviation="3.5" result="coloredBlur"/>
      <feMerge><feMergeNode in="coloredBlur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <filter id="glow-soft">
      <feGaussianBlur stdDeviation="2" result="coloredBlur"/>
      <feMerge><feMergeNode in="coloredBlur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <filter id="glow-strong">
      <feGaussianBlur stdDeviation="6" result="coloredBlur"/>
      <feMerge><feMergeNode in="coloredBlur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <filter id="shadow">
      <feDropShadow dx="0" dy="4" stdDeviation="8" flood-color="#58A6FF" flood-opacity="0.15"/>
    </filter>

    <!-- Title gradient -->
    <linearGradient id="titleGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#58A6FF"/>
      <stop offset="100%" style="stop-color:#A0C4FF"/>
    </linearGradient>

    <!-- Bubble gradient -->
    <radialGradient id="bubble1" cx="35%" cy="35%">
      <stop offset="0%" style="stop-color:#58A6FF;stop-opacity:0.25"/>
      <stop offset="100%" style="stop-color:#58A6FF;stop-opacity:0.04"/>
    </radialGradient>
    <radialGradient id="bubble2" cx="35%" cy="35%">
      <stop offset="0%" style="stop-color:#A0C4FF;stop-opacity:0.18"/>
      <stop offset="100%" style="stop-color:#A0C4FF;stop-opacity:0.03"/>
    </radialGradient>
    <radialGradient id="bubble3" cx="35%" cy="35%">
      <stop offset="0%" style="stop-color:#7dd3fc;stop-opacity:0.2"/>
      <stop offset="100%" style="stop-color:#7dd3fc;stop-opacity:0.03"/>
    </radialGradient>

    <!-- Clip paths for cards -->
    <clipPath id="clip1"><rect x="22" y="80" width="415" height="230" rx="14"/></clipPath>
    <clipPath id="clip2"><rect x="463" y="80" width="415" height="230" rx="14"/></clipPath>
    <clipPath id="clip3"><rect x="22" y="330" width="415" height="220" rx="14"/></clipPath>
    <clipPath id="clip4"><rect x="463" y="330" width="415" height="220" rx="14"/></clipPath>

    <!-- Animations -->
    <style>
      .star { animation: twinkle 3s infinite alternate; }
      .star2 { animation: twinkle 4.5s infinite alternate-reverse; }
      .star3 { animation: twinkle 2.5s infinite alternate; }
      .bubble { animation: floatUp 8s infinite ease-in-out; }
      .bubble2 { animation: floatUp 11s infinite ease-in-out reverse; }
      .atom-orbit { animation: spin 12s linear infinite; transform-origin: center; }
      .atom-orbit2 { animation: spin 18s linear infinite reverse; transform-origin: center; }
      .atom-orbit3 { animation: spin 22s linear infinite; transform-origin: center; }
      .dot-pulse { animation: pulse 2s infinite; }

      @keyframes twinkle {
        0% { opacity: 0.2; r: 1; }
        50% { opacity: 0.9; }
        100% { opacity: 0.4; r: 1.5; }
      }
      @keyframes floatUp {
        0% { transform: translateY(0px) scale(1); opacity: 0.5; }
        50% { transform: translateY(-18px) scale(1.05); opacity: 0.8; }
        100% { transform: translateY(0px) scale(1); opacity: 0.5; }
      }
      @keyframes spin {
        from { transform: rotate(0deg); }
        to { transform: rotate(360deg); }
      }
      @keyframes pulse {
        0%, 100% { opacity: 0.4; }
        50% { opacity: 1; }
      }
    </style>
  </defs>

  <!-- ═══ BACKGROUND ═══ -->
  <rect width="900" height="620" fill="url(#bgGrad)" rx="18"/>

  <!-- ═══ STARS ═══ -->
  <!-- Tiny random stars scattered across bg -->
  <circle class="star" cx="45" cy="25" r="1" fill="#ffffff" opacity="0.6"/>
  <circle class="star2" cx="130" cy="12" r="1.2" fill="#A0C4FF" opacity="0.7"/>
  <circle class="star3" cx="210" cy="35" r="0.8" fill="#ffffff" opacity="0.5"/>
  <circle class="star" cx="320" cy="18" r="1.1" fill="#58A6FF" opacity="0.8"/>
  <circle class="star2" cx="420" cy="8" r="0.9" fill="#ffffff" opacity="0.6"/>
  <circle class="star3" cx="510" cy="28" r="1.3" fill="#A0C4FF" opacity="0.7"/>
  <circle class="star" cx="600" cy="15" r="1" fill="#ffffff" opacity="0.5"/>
  <circle class="star2" cx="690" cy="30" r="1.2" fill="#58A6FF" opacity="0.8"/>
  <circle class="star3" cx="780" cy="10" r="0.8" fill="#ffffff" opacity="0.6"/>
  <circle class="star" cx="855" cy="22" r="1" fill="#A0C4FF" opacity="0.7"/>
  <circle class="star2" cx="70" cy="290" r="1" fill="#58A6FF" opacity="0.5"/>
  <circle class="star3" cx="175" cy="420" r="1.2" fill="#ffffff" opacity="0.6"/>
  <circle class="star" cx="440" cy="280" r="0.9" fill="#A0C4FF" opacity="0.7"/>
  <circle class="star2" cx="840" cy="200" r="1.1" fill="#58A6FF" opacity="0.6"/>
  <circle class="star3" cx="880" cy="390" r="1" fill="#ffffff" opacity="0.5"/>
  <circle class="star" cx="860" cy="530" r="1.2" fill="#A0C4FF" opacity="0.7"/>
  <circle class="star2" cx="30" cy="560" r="0.9" fill="#58A6FF" opacity="0.6"/>
  <circle class="star3" cx="450" cy="590" r="1.1" fill="#ffffff" opacity="0.5"/>
  <circle class="star" cx="750" cy="580" r="1" fill="#A0C4FF" opacity="0.8"/>

  <!-- 4-pointed sparkle stars -->
  <g filter="url(#glow-soft)">
    <path d="M 80 60 L 82 55 L 84 60 L 82 65 Z" fill="#58A6FF" opacity="0.7"/>
    <path d="M 77 60 L 82 58 L 87 60 L 82 62 Z" fill="#58A6FF" opacity="0.7"/>
  </g>
  <g filter="url(#glow-soft)">
    <path d="M 820 55 L 822 49 L 824 55 L 822 61 Z" fill="#A0C4FF" opacity="0.6"/>
    <path d="M 816 55 L 822 53 L 828 55 L 822 57 Z" fill="#A0C4FF" opacity="0.6"/>
  </g>
  <g filter="url(#glow-soft)">
    <path d="M 450 570 L 452 564 L 454 570 L 452 576 Z" fill="#7dd3fc" opacity="0.5"/>
    <path d="M 446 570 L 452 568 L 458 570 L 452 572 Z" fill="#7dd3fc" opacity="0.5"/>
  </g>

  <!-- ═══ FLOATING BUBBLES ═══ -->
  <circle class="bubble" cx="860" cy="150" r="45" fill="url(#bubble1)" stroke="#58A6FF" stroke-width="0.5" opacity="0.6"/>
  <circle class="bubble2" cx="42" cy="480" r="32" fill="url(#bubble2)" stroke="#A0C4FF" stroke-width="0.5" opacity="0.5"/>
  <circle class="bubble" cx="448" cy="305" r="20" fill="url(#bubble3)" stroke="#7dd3fc" stroke-width="0.4" opacity="0.4"/>
  <circle class="bubble2" cx="880" cy="450" r="22" fill="url(#bubble1)" stroke="#58A6FF" stroke-width="0.4" opacity="0.4"/>
  <circle class="bubble" cx="15" cy="150" r="18" fill="url(#bubble2)" stroke="#A0C4FF" stroke-width="0.3" opacity="0.35"/>

  <!-- ═══ ATOM STRUCTURES ═══ -->
  <!-- Atom 1 — top right area -->
  <g transform="translate(840, 85)">
    <!-- nucleus -->
    <circle cx="0" cy="0" r="5" fill="#58A6FF" opacity="0.9" filter="url(#glow-blue)"/>
    <circle cx="0" cy="0" r="2" fill="#ffffff" opacity="0.8"/>
    <!-- orbit 1 -->
    <g class="atom-orbit">
      <ellipse cx="0" cy="0" rx="22" ry="9" fill="none" stroke="#58A6FF" stroke-width="0.9" opacity="0.5"/>
      <circle cx="22" cy="0" r="2.5" fill="#58A6FF" opacity="0.9" filter="url(#glow-soft)"/>
    </g>
    <!-- orbit 2 -->
    <g class="atom-orbit2" style="transform:rotate(60deg)">
      <ellipse cx="0" cy="0" rx="22" ry="9" fill="none" stroke="#A0C4FF" stroke-width="0.9" opacity="0.45"/>
      <circle cx="-22" cy="0" r="2" fill="#A0C4FF" opacity="0.85"/>
    </g>
    <!-- orbit 3 -->
    <g class="atom-orbit3" style="transform:rotate(120deg)">
      <ellipse cx="0" cy="0" rx="22" ry="9" fill="none" stroke="#7dd3fc" stroke-width="0.9" opacity="0.4"/>
      <circle cx="0" cy="9" r="2" fill="#7dd3fc" opacity="0.85"/>
    </g>
  </g>

  <!-- Atom 2 — bottom left -->
  <g transform="translate(60, 540)">
    <circle cx="0" cy="0" r="4" fill="#58A6FF" opacity="0.85" filter="url(#glow-soft)"/>
    <circle cx="0" cy="0" r="1.5" fill="#ffffff" opacity="0.8"/>
    <g class="atom-orbit2">
      <ellipse cx="0" cy="0" rx="18" ry="7" fill="none" stroke="#58A6FF" stroke-width="0.8" opacity="0.45"/>
      <circle cx="18" cy="0" r="2" fill="#58A6FF" opacity="0.9"/>
    </g>
    <g class="atom-orbit3" style="transform:rotate(60deg)">
      <ellipse cx="0" cy="0" rx="18" ry="7" fill="none" stroke="#A0C4FF" stroke-width="0.8" opacity="0.4"/>
      <circle cx="-18" cy="0" r="1.8" fill="#A0C4FF" opacity="0.85"/>
    </g>
  </g>

  <!-- Atom 3 — center divider area (small) -->
  <g transform="translate(450, 308)">
    <circle cx="0" cy="0" r="3.5" fill="#7dd3fc" opacity="0.8" filter="url(#glow-soft)"/>
    <g class="atom-orbit">
      <ellipse cx="0" cy="0" rx="14" ry="6" fill="none" stroke="#7dd3fc" stroke-width="0.7" opacity="0.4"/>
      <circle cx="14" cy="0" r="1.8" fill="#7dd3fc" opacity="0.9"/>
    </g>
    <g class="atom-orbit3" style="transform:rotate(90deg)">
      <ellipse cx="0" cy="0" rx="14" ry="6" fill="none" stroke="#58A6FF" stroke-width="0.7" opacity="0.35"/>
      <circle cx="0" cy="6" r="1.5" fill="#58A6FF" opacity="0.85"/>
    </g>
  </g>

  <!-- ═══ CONNECTING DOTS LINE (decorative) ═══ -->
  <g opacity="0.25">
    <circle class="dot-pulse" cx="200" cy="58" r="1.5" fill="#58A6FF"/>
    <circle class="dot-pulse" cx="230" cy="58" r="1.5" fill="#58A6FF" style="animation-delay:0.3s"/>
    <circle class="dot-pulse" cx="260" cy="58" r="1.5" fill="#58A6FF" style="animation-delay:0.6s"/>
    <circle class="dot-pulse" cx="650" cy="58" r="1.5" fill="#58A6FF" style="animation-delay:0.9s"/>
    <circle class="dot-pulse" cx="680" cy="58" r="1.5" fill="#58A6FF" style="animation-delay:1.2s"/>
    <circle class="dot-pulse" cx="710" cy="58" r="1.5" fill="#58A6FF" style="animation-delay:1.5s"/>
  </g>

  <!-- ═══ SECTION TITLE ═══ -->
  <text x="450" y="50" text-anchor="middle" font-family="'Courier New', monospace" font-size="22" font-weight="bold" fill="url(#titleGrad)" filter="url(#glow-blue)">
    &gt; highlights
  </text>
  <line x1="160" y1="58" x2="330" y2="58" stroke="#58A6FF" stroke-width="0.8" opacity="0.35"/>
  <line x1="570" y1="58" x2="740" y2="58" stroke="#58A6FF" stroke-width="0.8" opacity="0.35"/>

  <!-- ════════════════ CARD 1 — API & Backend ════════════════ -->
  <rect x="22" y="80" width="415" height="230" rx="14" fill="url(#card1)" filter="url(#shadow)"/>
  <rect x="22" y="80" width="415" height="230" rx="14" fill="none" stroke="#58A6FF" stroke-width="0.8" opacity="0.35"/>
  <!-- top accent line -->
  <rect x="22" y="80" width="415" height="3" rx="2" fill="#58A6FF" opacity="0.8"/>
  <!-- icon + title -->
  <text x="50" y="113" font-family="'Courier New', monospace" font-size="15" fill="#58A6FF" font-weight="bold" filter="url(#glow-soft)">⚙️  API &amp; Backend</text>
  <line x1="45" y1="122" x2="420" y2="122" stroke="#58A6FF" stroke-width="0.5" opacity="0.25"/>
  <!-- items -->
  <text x="50" y="147" font-size="12.5" fill="#8B949E" font-family="'Courier New', monospace"><tspan fill="#58A6FF" opacity="0.8">✦</tspan>  REST API design &amp; development</text>
  <text x="50" y="167" font-size="12.5" fill="#8B949E" font-family="'Courier New', monospace"><tspan fill="#58A6FF" opacity="0.8">✦</tspan>  FastAPI · Flask · Python</text>
  <text x="50" y="187" font-size="12.5" fill="#8B949E" font-family="'Courier New', monospace"><tspan fill="#58A6FF" opacity="0.8">✦</tspan>  Auth systems &amp; Role-Based Access</text>
  <text x="50" y="207" font-size="12.5" fill="#8B949E" font-family="'Courier New', monospace"><tspan fill="#58A6FF" opacity="0.8">✦</tspan>  Third-party API integrations</text>
  <text x="50" y="227" font-size="12.5" fill="#8B949E" font-family="'Courier New', monospace"><tspan fill="#58A6FF" opacity="0.8">✦</tspan>  File upload &amp; processing systems</text>
  <text x="50" y="247" font-size="12.5" fill="#8B949E" font-family="'Courier New', monospace"><tspan fill="#58A6FF" opacity="0.8">✦</tspan>  Resume generation systems</text>
  <!-- corner glow dot -->
  <circle cx="418" cy="93" r="4" fill="#58A6FF" opacity="0.5" filter="url(#glow-soft)"/>

  <!-- ════════════════ CARD 2 — Data & Automation ════════════════ -->
  <rect x="463" y="80" width="415" height="230" rx="14" fill="url(#card2)" filter="url(#shadow)"/>
  <rect x="463" y="80" width="415" height="230" rx="14" fill="none" stroke="#58A6FF" stroke-width="0.8" opacity="0.35"/>
  <rect x="463" y="80" width="415" height="3" rx="2" fill="#A0C4FF" opacity="0.8"/>
  <text x="490" y="113" font-family="'Courier New', monospace" font-size="15" fill="#A0C4FF" font-weight="bold" filter="url(#glow-soft)">📊  Data &amp; Automation</text>
  <line x1="485" y1="122" x2="860" y2="122" stroke="#A0C4FF" stroke-width="0.5" opacity="0.25"/>
  <text x="490" y="147" font-size="12.5" fill="#8B949E" font-family="'Courier New', monospace"><tspan fill="#A0C4FF" opacity="0.8">✦</tspan>  Pandas · data cleaning &amp; pipelines</text>
  <text x="490" y="167" font-size="12.5" fill="#8B949E" font-family="'Courier New', monospace"><tspan fill="#A0C4FF" opacity="0.8">✦</tspan>  OCR-based structured extraction</text>
  <text x="490" y="187" font-size="12.5" fill="#8B949E" font-family="'Courier New', monospace"><tspan fill="#A0C4FF" opacity="0.8">✦</tspan>  Excel &amp; PDF data processing</text>
  <text x="490" y="207" font-size="12.5" fill="#8B949E" font-family="'Courier New', monospace"><tspan fill="#A0C4FF" opacity="0.8">✦</tspan>  UiPath automation workflows</text>
  <text x="490" y="227" font-size="12.5" fill="#8B949E" font-family="'Courier New', monospace"><tspan fill="#A0C4FF" opacity="0.8">✦</tspan>  Email automation on conditions</text>
  <text x="490" y="247" font-size="12.5" fill="#8B949E" font-family="'Courier New', monospace"><tspan fill="#A0C4FF" opacity="0.8">✦</tspan>  Power BI business dashboards</text>
  <circle cx="858" cy="93" r="4" fill="#A0C4FF" opacity="0.5" filter="url(#glow-soft)"/>

  <!-- ════════════════ CARD 3 — Database ════════════════ -->
  <rect x="22" y="330" width="415" height="220" rx="14" fill="url(#card3)" filter="url(#shadow)"/>
  <rect x="22" y="330" width="415" height="220" rx="14" fill="none" stroke="#7dd3fc" stroke-width="0.8" opacity="0.3"/>
  <rect x="22" y="330" width="415" height="3" rx="2" fill="#7dd3fc" opacity="0.8"/>
  <text x="50" y="363" font-family="'Courier New', monospace" font-size="15" fill="#7dd3fc" font-weight="bold" filter="url(#glow-soft)">🗄️  Database</text>
  <line x1="45" y1="372" x2="420" y2="372" stroke="#7dd3fc" stroke-width="0.5" opacity="0.25"/>
  <text x="50" y="397" font-size="12.5" fill="#8B949E" font-family="'Courier New', monospace"><tspan fill="#7dd3fc" opacity="0.8">✦</tspan>  MySQL &amp; relational design</text>
  <text x="50" y="417" font-size="12.5" fill="#8B949E" font-family="'Courier New', monospace"><tspan fill="#7dd3fc" opacity="0.8">✦</tspan>  Schema design &amp; normalization</text>
  <text x="50" y="437" font-size="12.5" fill="#8B949E" font-family="'Courier New', monospace"><tspan fill="#7dd3fc" opacity="0.8">✦</tspan>  Query optimization</text>
  <text x="50" y="457" font-size="12.5" fill="#8B949E" font-family="'Courier New', monospace"><tspan fill="#7dd3fc" opacity="0.8">✦</tspan>  Relational data modeling</text>
  <text x="50" y="477" font-size="12.5" fill="#8B949E" font-family="'Courier New', monospace"><tspan fill="#7dd3fc" opacity="0.8">✦</tspan>  Clean folder architecture</text>
  <circle cx="418" cy="343" r="4" fill="#7dd3fc" opacity="0.5" filter="url(#glow-soft)"/>

  <!-- ════════════════ CARD 4 — Currently Exploring ════════════════ -->
  <rect x="463" y="330" width="415" height="220" rx="14" fill="url(#card4)" filter="url(#shadow)"/>
  <rect x="463" y="330" width="415" height="220" rx="14" fill="none" stroke="#58A6FF" stroke-width="0.8" opacity="0.35"/>
  <rect x="463" y="330" width="415" height="3" rx="2" fill="#58A6FF" opacity="0.9"/>
  <!-- animated blinking dot -->
  <circle class="dot-pulse" cx="478" cy="348" r="4" fill="#58A6FF" filter="url(#glow-blue)"/>
  <text x="490" y="363" font-family="'Courier New', monospace" font-size="15" fill="#58A6FF" font-weight="bold" filter="url(#glow-soft)">🚀  Currently Exploring</text>
  <line x1="485" y1="372" x2="860" y2="372" stroke="#58A6FF" stroke-width="0.5" opacity="0.25"/>
  <text x="490" y="397" font-size="12.5" fill="#8B949E" font-family="'Courier New', monospace"><tspan fill="#58A6FF" opacity="0.8">✦</tspan>  System Design principles</text>
  <text x="490" y="417" font-size="12.5" fill="#8B949E" font-family="'Courier New', monospace"><tspan fill="#58A6FF" opacity="0.8">✦</tspan>  Scalable distributed architectures</text>
  <text x="490" y="437" font-size="12.5" fill="#8B949E" font-family="'Courier New', monospace"><tspan fill="#58A6FF" opacity="0.8">✦</tspan>  Cloud deployment strategies</text>
  <text x="490" y="457" font-size="12.5" fill="#8B949E" font-family="'Courier New', monospace"><tspan fill="#58A6FF" opacity="0.8">✦</tspan>  Microservices patterns</text>
  <text x="490" y="477" font-size="12.5" fill="#8B949E" font-family="'Courier New', monospace"><tspan fill="#58A6FF" opacity="0.8">✦</tspan>  Docker &amp; containerization</text>
  <circle cx="858" cy="343" r="4" fill="#58A6FF" opacity="0.5" filter="url(#glow-soft)"/>

  <!-- ═══ BOTTOM TAGLINE ═══ -->
  <text x="450" y="597" text-anchor="middle" font-family="'Courier New', monospace" font-size="11" fill="#58A6FF" opacity="0.45">
    ── clean code · scalable systems · continuous improvement ──
  </text>

</svg>
