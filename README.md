<div align="center">

<!-- ═══════════════════════════════════════════════════════════════ -->
<!-- ███████████████ ANIMATED HUD HEADER — SVG ███████████████████ -->
<!-- ═══════════════════════════════════════════════════════════════ -->

<svg xmlns="http://www.w3.org/2000/svg" width="100%" height="340" viewBox="0 0 1000 340" style="background:#060a10;border-radius:8px;display:block;">

  <defs>
    <linearGradient id="bgGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#060a10"/>
      <stop offset="50%" stop-color="#0b1929"/>
      <stop offset="100%" stop-color="#060a10"/>
    </linearGradient>
    <linearGradient id="glowLine" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#38bdf8" stop-opacity="0"/>
      <stop offset="50%" stop-color="#38bdf8" stop-opacity="0.6"/>
      <stop offset="100%" stop-color="#38bdf8" stop-opacity="0"/>
    </linearGradient>
  </defs>

  <!-- BG -->
  <rect width="1000" height="340" fill="url(#bgGrad)"/>

  <!-- GRID LINES -->
  <line x1="0" y1="0" x2="0" y2="340" stroke="#38bdf8" stroke-width="0.3" opacity="0.04">
    <animate attributeName="opacity" values="0.04;0.08;0.04" dur="6s" repeatCount="indefinite"/>
  </line>
  <line x1="200" y1="0" x2="200" y2="340" stroke="#38bdf8" stroke-width="0.3" opacity="0.04"/>
  <line x1="400" y1="0" x2="400" y2="340" stroke="#38bdf8" stroke-width="0.3" opacity="0.04"/>
  <line x1="600" y1="0" x2="600" y2="340" stroke="#38bdf8" stroke-width="0.3" opacity="0.04"/>
  <line x1="800" y1="0" x2="800" y2="340" stroke="#38bdf8" stroke-width="0.3" opacity="0.04"/>
  <line x1="1000" y1="0" x2="1000" y2="340" stroke="#38bdf8" stroke-width="0.3" opacity="0.04"/>
  <line x1="0" y1="80" x2="1000" y2="80" stroke="#38bdf8" stroke-width="0.3" opacity="0.04"/>
  <line x1="0" y1="160" x2="1000" y2="160" stroke="#38bdf8" stroke-width="0.3" opacity="0.04"/>
  <line x1="0" y1="240" x2="1000" y2="240" stroke="#38bdf8" stroke-width="0.3" opacity="0.04"/>
  <line x1="0" y1="320" x2="1000" y2="320" stroke="#38bdf8" stroke-width="0.3" opacity="0.04"/>

  <!-- SCANLINE SWEEP -->
  <g>
    <rect x="0" y="0" width="1000" height="2" fill="#38bdf8" opacity="0.08">
      <animate attributeName="y" values="-2;340" dur="2.5s" repeatCount="indefinite"/>
    </rect>
    <rect x="0" y="0" width="1000" height="1" fill="#7dd3fc" opacity="0.12">
      <animate attributeName="y" values="-1;340" dur="2.3s" repeatCount="indefinite"/>
    </rect>
  </g>

  <!-- PULSING RADAR RINGS -->
  <circle cx="500" cy="150" r="0" fill="none" stroke="#38bdf8" stroke-width="0.5" opacity="0">
    <animate attributeName="r" values="0;180" dur="4s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.6;0" dur="4s" repeatCount="indefinite"/>
  </circle>
  <circle cx="500" cy="150" r="0" fill="none" stroke="#38bdf8" stroke-width="0.5" opacity="0">
    <animate attributeName="r" values="0;180" dur="4s" begin="1.5s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.6;0" dur="4s" begin="1.5s" repeatCount="indefinite"/>
  </circle>
  <circle cx="500" cy="150" r="0" fill="none" stroke="#38bdf8" stroke-width="0.5" opacity="0">
    <animate attributeName="r" values="0;180" dur="4s" begin="3s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.6;0" dur="4s" begin="3s" repeatCount="indefinite"/>
  </circle>

  <!-- HUD CORNER BRACKETS -->
  <g opacity="0.8">
    <!-- TL -->
    <path d="M 25,25 L 90,25" stroke="#38bdf8" stroke-width="2" fill="none"/>
    <path d="M 25,25 L 25,90" stroke="#38bdf8" stroke-width="2" fill="none"/>
    <circle cx="25" cy="25" r="3" fill="#38bdf8"/>
    <!-- TR -->
    <path d="M 975,25 L 910,25" stroke="#38bdf8" stroke-width="2" fill="none"/>
    <path d="M 975,25 L 975,90" stroke="#38bdf8" stroke-width="2" fill="none"/>
    <circle cx="975" cy="25" r="3" fill="#38bdf8"/>
    <!-- BL -->
    <path d="M 25,315 L 90,315" stroke="#38bdf8" stroke-width="2" fill="none"/>
    <path d="M 25,315 L 25,250" stroke="#38bdf8" stroke-width="2" fill="none"/>
    <circle cx="25" cy="315" r="3" fill="#38bdf8"/>
    <!-- BR -->
    <path d="M 975,315 L 910,315" stroke="#38bdf8" stroke-width="2" fill="none"/>
    <path d="M 975,315 L 975,250" stroke="#38bdf8" stroke-width="2" fill="none"/>
    <circle cx="975" cy="315" r="3" fill="#38bdf8"/>
  </g>

  <!-- TOP STATUS BAR -->
  <rect x="30" y="35" width="940" height="1" fill="url(#glowLine)"/>
  <text x="45" y="25" font-family="monospace" font-size="10" fill="#38bdf8" opacity="0.5">LOBOS-3 :: SECURE TERMINAL v2.4</text>
  <text x="790" y="25" font-family="monospace" font-size="10" fill="#38bdf8" opacity="0.5">CONNECTION: </text>
  <text x="875" y="25" font-family="monospace" font-size="10" fill="#00ff80" opacity="0.8">SECURE</text>
  <circle cx="865" cy="22" r="3" fill="#00ff80">
    <animate attributeName="opacity" values="1;0.1;1" dur="1.5s" repeatCount="indefinite"/>
  </circle>

  <!-- GLITCH TEXT : NAME -->
  <!-- Layer 0 — base white -->
  <text x="500" y="148" text-anchor="middle" font-family="Consolas, monospace" font-size="52" font-weight="bold" fill="#e0f4ff" letter-spacing="3">LOGESHWARAN S</text>

  <!-- Layer 1 — cyan offset -->
  <text x="500" y="148" text-anchor="middle" font-family="Consolas, monospace" font-size="52" font-weight="bold" fill="#38bdf8" letter-spacing="3" opacity="0">
    <animate attributeName="x" values="500;504;498;500;506;500;495;500" dur="0.35s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0;0.7;0;0.5;0;0.8;0;0.4;0" dur="0.45s" repeatCount="indefinite"/>
    LOGESHWARAN S
  </text>

  <!-- Layer 2 — red offset -->
  <text x="500" y="148" text-anchor="middle" font-family="Consolas, monospace" font-size="52" font-weight="bold" fill="#ff0040" letter-spacing="3" opacity="0">
    <animate attributeName="x" values="500;497;503;500;494;502;500" dur="0.3s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0;0.5;0;0.3;0;0.6;0" dur="0.5s" repeatCount="indefinite"/>
    LOGESHWARAN S
  </text>

  <!-- Layer 3 — green glitch pixel -->
  <text x="500" y="148" text-anchor="middle" font-family="Consolas, monospace" font-size="52" font-weight="bold" fill="#00ff80" letter-spacing="3" opacity="0">
    <animate attributeName="y" values="148;146;150;148" dur="0.2s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0;0.4;0;0.2;0" dur="0.6s" repeatCount="indefinite"/>
    LOGESHWARAN S
  </text>

  <!-- ALIAS BADGE -->
  <g transform="translate(500, 178)">
    <rect x="-60" y="-10" width="120" height="20" rx="10" fill="none" stroke="#38bdf8" stroke-width="0.8" opacity="0.5">
      <animate attributeName="opacity" values="0.5;0.8;0.5" dur="3s" repeatCount="indefinite"/>
    </rect>
    <text x="0" y="5" text-anchor="middle" font-family="monospace" font-size="10" fill="#7dd3fc" letter-spacing="4">SECURITY ANALYST</text>
  </g>

  <!-- GLITCH SCREEN FLASH -->
  <rect x="0" y="0" width="1000" height="340" fill="#38bdf8" opacity="0">
    <animate attributeName="opacity" values="0;0;0;0;0.03;0;0;0;0;0;0;0;0;0.02;0;0;0;0;0;0" dur="8s" repeatCount="indefinite"/>
  </rect>
  <rect x="0" y="0" width="1000" height="340" fill="#ffffff" opacity="0">
    <animate attributeName="opacity" values="0;0;0;0;0;0;0;0;0;0;0;0;0.04;0;0;0;0;0;0;0" dur="8s" repeatCount="indefinite"/>
  </rect>

  <!-- ANIMATED GLITCH HORIZONTAL BANDS -->
  <rect x="0" y="110" width="1000" height="3" fill="#38bdf8" opacity="0">
    <animate attributeName="y" values="110;200;300;50;180;110" dur="4s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0;0;0.08;0;0;0;0.05;0;0;0;0.1;0;0" dur="6s" repeatCount="indefinite"/>
  </rect>

  <!-- TERMINAL PROMPT -->
  <text x="40" y="258" font-family="monospace" font-size="12" fill="#38bdf8" opacity="0.7">┌──(</text>
  <text x="80" y="258" font-family="monospace" font-size="12" fill="#00ff80" opacity="0.9">logesh</text>
  <text x="132" y="258" font-family="monospace" font-size="12" fill="#38bdf8" opacity="0.7">㉿</text>
  <text x="146" y="258" font-family="monospace" font-size="12" fill="#00ff80" opacity="0.9">sec-ops</text>
  <text x="195" y="258" font-family="monospace" font-size="12" fill="#38bdf8" opacity="0.7">)</text>
  <text x="204" y="258" font-family="monospace" font-size="12" fill="#7dd3fc" opacity="0.7">─[</text>
  <text x="220" y="258" font-family="monospace" font-size="12" fill="#e0f4ff" opacity="0.8">~/readme</text>
  <text x="278" y="258" font-family="monospace" font-size="12" fill="#7dd3fc" opacity="0.7">]</text>
  <text x="40" y="278" font-family="monospace" font-size="12" fill="#38bdf8" opacity="0.7">└─$ cat &gt;&gt; /dev/brain &lt;&lt; whoami</text>

  <!-- BLINKING CURSOR -->
  <rect x="222" y="270" width="6" height="11" fill="#38bdf8" opacity="0">
    <animate attributeName="opacity" values="0;1;0" dur="1s" repeatCount="indefinite"/>
  </rect>

  <!-- BOTTOM STATUS LINE -->
  <rect x="30" y="305" width="940" height="1" fill="url(#glowLine)"/>
  <text x="40" y="320" font-family="monospace" font-size="9" fill="#38bdf8" opacity="0.3">[SYS: NOMINAL] [UPTIME: 1337d] [NET: WAF ENABLED]</text>
  <text x="760" y="320" font-family="monospace" font-size="9" fill="#38bdf8" opacity="0.3">[NODE: README.md] [AUTH: loki]</text>
</svg>

<br/><br/>

<!-- TYPING SVG -->
<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=15&pause=2000&color=38BDF8&center=true&vCenter=true&multiline=true&repeat=true&width=900&height=80&lines=%24+cat+%2Fetc%2Fmotd;%E2%94%8C%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%90;%E2%94%82+WARNING+%3A+Unauthorized+access+prohibited+%E2%94%82;%E2%94%82+This+system+is+monitored+24%2F7+%F0%9F%94%8D+%E2%94%82;%E2%94%94%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%80%E2%94%98" alt="typing-intro" />

</div>

<br/>

---

<br/>

<!-- ═══════════════════════════════════════════════════════════════ -->
<!-- █████████████████ SYSTEM BOOT SEQUENCE █████████████████████ -->
<!-- ═══════════════════════════════════════════════════════════════ -->

<div align="center">

<svg xmlns="http://www.w3.org/2000/svg" width="100%" height="180" viewBox="0 0 900 180" style="background:#060a10;border-radius:6px;">

  <defs>
    <linearGradient id="bootGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#38bdf8"/>
      <stop offset="100%" stop-color="#00ff80"/>
    </linearGradient>
  </defs>

  <rect width="900" height="180" fill="#060a10" rx="6"/>

  <!-- TOP LINE -->
  <text x="30" y="30" font-family="monospace" font-size="10" fill="#38bdf8" opacity="0.4">[BOOT SEQUENCE]</text>

  <!-- STEP 1: Initializing -->
  <text x="40" y="65" font-family="monospace" font-size="12" fill="#38bdf8" opacity="0">
    <animate attributeName="opacity" from="0" to="0.8" begin="0s" dur="0.5s" fill="freeze"/>
    [  OK  ] Initializing kernel modules...
  </text>

  <!-- STEP 2: Loading -->
  <text x="40" y="85" font-family="monospace" font-size="12" fill="#38bdf8" opacity="0">
    <animate attributeName="opacity" from="0" to="0.8" begin="0.8s" dur="0.5s" fill="freeze"/>
    [  OK  ] Loading security profiles...
  </text>

  <!-- STEP 3: Network -->
  <text x="40" y="105" font-family="monospace" font-size="12" fill="#38bdf8" opacity="0">
    <animate attributeName="opacity" from="0" to="0.8" begin="1.6s" dur="0.5s" fill="freeze"/>
    [  OK  ] Establishing secure channel...
  </text>

  <!-- STEP 4: Ready -->
  <text x="40" y="125" font-family="monospace" font-size="12" fill="#38bdf8" opacity="0">
    <animate attributeName="opacity" from="0" to="0.8" begin="2.4s" dur="0.5s" fill="freeze"/>
    [  OK  ] Syncing threat intelligence feeds...
  </text>

  <!-- PROGRESS BAR BG -->
  <rect x="40" y="145" width="820" height="16" rx="8" fill="#0b1929" stroke="#1a3a5c" stroke-width="1" opacity="0.7"/>

  <!-- PROGRESS BAR FILL -->
  <rect x="40" y="145" width="0" height="16" rx="8" fill="url(#bootGrad)" opacity="0.9">
    <animate attributeName="width" from="0" to="820" dur="3s" begin="0.5s" fill="freeze"/>
  </rect>

  <!-- PROGRESS TEXT -->
  <text x="450" y="157" text-anchor="middle" font-family="monospace" font-size="10" fill="#060a10" font-weight="bold" opacity="0">
    <animate attributeName="opacity" from="0" to="1" begin="1s" dur="0.01s" fill="freeze"/>
    INITIALIZING... 100%
  </text>

  <!-- SYSTEM READY FLASH -->
  <text x="450" y="157" text-anchor="middle" font-family="monospace" font-size="10" fill="#060a10" font-weight="bold" opacity="0">
    <animate attributeName="opacity" from="0" to="1" begin="3.5s" dur="0.01s" fill="freeze"/>
    SYSTEM READY
  </text>

  <!-- BLINKING DONE -->
  <text x="820" y="125" font-family="monospace" font-size="12" fill="#00ff80" opacity="0">
    <animate attributeName="opacity" from="0" to="1" begin="3s" dur="0.5s" fill="freeze"/>
    [DONE]
  </text>
  <circle cx="808" cy="121" r="3" fill="#00ff80" opacity="0">
    <animate attributeName="opacity" from="0" to="1" begin="3.5s" dur="0.01s" fill="freeze"/>
    <animate attributeName="opacity" values="1;0.2;1" dur="1.5s" repeatCount="indefinite"/>
  </circle>

</svg>

</div>

<br/>

---

<br/>

<!-- ═══════════════════════════════════════════════════════════════ -->
<!-- █████████████████ ANIMATED WHOAMI TERMINAL █████████████████ -->
<!-- ═══════════════════════════════════════════════════════════════ -->

<div align="center">

<svg xmlns="http://www.w3.org/2000/svg" width="100%" height="400" viewBox="0 0 960 400" style="border-radius:8px;">

  <defs>
    <linearGradient id="termGrad" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" stop-color="#0d1b2a"/>
      <stop offset="100%" stop-color="#060a10"/>
    </linearGradient>
    <filter id="glow">
      <feGaussianBlur stdDeviation="2" result="blur"/>
      <feMerge><feMergeNode in="blur"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
  </defs>

  <!-- Window shadow bg -->
  <rect x="2" y="2" width="956" height="396" rx="8" fill="#000" opacity="0.5"/>

  <!-- Window bg -->
  <rect x="0" y="0" width="956" height="396" rx="8" fill="url(#termGrad)" stroke="#1a3a5c" stroke-width="1.5"/>

  <!-- Title bar -->
  <rect x="0" y="0" width="956" height="36" rx="8" fill="#0b1929" stroke="#1a3a5c" stroke-width="1"/>
  <rect x="0" y="28" width="956" height="8" fill="#0b1929"/>

  <!-- Window buttons -->
  <circle cx="25" cy="18" r="6" fill="#ff5f56">
    <animate attributeName="opacity" values="1;0.5;1" dur="3s" repeatCount="indefinite"/>
  </circle>
  <circle cx="45" cy="18" r="6" fill="#ffbd2e"/>
  <circle cx="65" cy="18" r="6" fill="#27c93f"/>

  <!-- Title -->
  <text x="478" y="23" text-anchor="middle" font-family="monospace" font-size="11" fill="#7dd3fc" opacity="0.7">logesh@sec-ops: ~/whoami.sh</text>

  <!-- Terminal content — line by line appearance -->
  <text x="30" y="70" font-family="monospace" font-size="12" fill="#38bdf8" opacity="0">
    <animate attributeName="opacity" from="0" to="1" begin="0.3s" dur="0.3s" fill="freeze"/>
    $ ./whoami.sh --verbose
  </text>

  <text x="30" y="92" font-family="monospace" font-size="12" fill="#7dd3fc" opacity="0">
    <animate attributeName="opacity" from="0" to="1" begin="0.8s" dur="0.3s" fill="freeze"/>
    ─────────────────────────────────────────────────────────
  </text>

  <text x="30" y="116" font-family="monospace" font-size="12" fill="#38bdf8" opacity="0">
    <animate attributeName="opacity" from="0" to="1" begin="1.2s" dur="0.3s" fill="freeze"/>
    USER
    <text x="120" y="116" font-family="monospace" font-size="12" fill="#e0f4ff" opacity="0">
      <animate attributeName="opacity" from="0" to="1" begin="1.3s" dur="0.3s" fill="freeze"/>
      : Logeshwaran S
    </text>
  </text>

  <text x="30" y="138" font-family="monospace" font-size="12" fill="#38bdf8" opacity="0">
    <animate attributeName="opacity" from="0" to="1" begin="1.6s" dur="0.3s" fill="freeze"/>
    ALIAS
    <text x="120" y="138" font-family="monospace" font-size="12" fill="#e0f4ff" opacity="0">
      <animate attributeName="opacity" from="0" to="1" begin="1.7s" dur="0.3s" fill="freeze"/>
      : Loki
    </text>
    <text x="170" y="138" font-family="monospace" font-size="12" fill="#38bdf8" opacity="0">
      <animate attributeName="opacity" from="0" to="1" begin="1.75s" dur="0.3s" fill="freeze"/>
      // "God of Mischief" — Norse mythology
    </text>
  </text>

  <text x="30" y="160" font-family="monospace" font-size="12" fill="#38bdf8" opacity="0">
    <animate attributeName="opacity" from="0" to="1" begin="2s" dur="0.3s" fill="freeze"/>
    LOCATION
    <text x="120" y="160" font-family="monospace" font-size="12" fill="#e0f4ff" opacity="0">
      <animate attributeName="opacity" from="0" to="1" begin="2.1s" dur="0.3s" fill="freeze"/>
      : Tamil Nadu, India 🇮🇳
    </text>
  </text>

  <text x="30" y="182" font-family="monospace" font-size="12" fill="#38bdf8" opacity="0">
    <animate attributeName="opacity" from="0" to="1" begin="2.4s" dur="0.3s" fill="freeze"/>
    TITLE
    <text x="120" y="182" font-family="monospace" font-size="12" fill="#e0f4ff" opacity="0">
      <animate attributeName="opacity" from="0" to="1" begin="2.5s" dur="0.3s" fill="freeze"/>
      : Security Analyst
    </text>
  </text>

  <text x="30" y="204" font-family="monospace" font-size="12" fill="#38bdf8" opacity="0">
    <animate attributeName="opacity" from="0" to="1" begin="2.8s" dur="0.3s" fill="freeze"/>
    DOMAIN
    <text x="120" y="204" font-family="monospace" font-size="12" fill="#e0f4ff" opacity="0">
      <animate attributeName="opacity" from="0" to="1" begin="2.9s" dur="0.3s" fill="freeze"/>
      : SOC / VAPT / Security Engineering
    </text>
  </text>

  <text x="30" y="226" font-family="monospace" font-size="12" fill="#38bdf8" opacity="0">
    <animate attributeName="opacity" from="0" to="1" begin="3.2s" dur="0.3s" fill="freeze"/>
    BOUNTIES
    <text x="120" y="226" font-family="monospace" font-size="12" fill="#e0f4ff" opacity="0">
      <animate attributeName="opacity" from="0" to="1" begin="3.3s" dur="0.3s" fill="freeze"/>
      : Google Android VRP
    </text>
  </text>

  <text x="120" y="248" font-family="monospace" font-size="12" fill="#e0f4ff" opacity="0">
    <animate attributeName="opacity" from="0" to="1" begin="3.6s" dur="0.3s" fill="freeze"/>
    : NVIDIA PSIRT
  </text>

  <text x="120" y="270" font-family="monospace" font-size="12" fill="#e0f4ff" opacity="0">
    <animate attributeName="opacity" from="0" to="1" begin="3.9s" dur="0.3s" fill="freeze"/>
    : CERT-In (Government of India)
  </text>

  <text x="30" y="292" font-family="monospace" font-size="12" fill="#38bdf8" opacity="0">
    <animate attributeName="opacity" from="0" to="1" begin="4.2s" dur="0.3s" fill="freeze"/>
    STATUS
    <text x="120" y="292" font-family="monospace" font-size="12" fill="#00ff80" opacity="0">
      <animate attributeName="opacity" from="0" to="1" begin="4.3s" dur="0.3s" fill="freeze"/>
      : Active — Open to opportunities
    </text>
  </text>

  <text x="30" y="314" font-family="monospace" font-size="12" fill="#38bdf8" opacity="0">
    <animate attributeName="opacity" from="0" to="1" begin="4.6s" dur="0.3s" fill="freeze"/>
    CONTACT
    <text x="120" y="314" font-family="monospace" font-size="12" fill="#e0f4ff" opacity="0">
      <animate attributeName="opacity" from="0" to="1" begin="4.7s" dur="0.3s" fill="freeze"/>
      : logesh.spy@gmail.com
    </text>
  </text>

  <text x="30" y="342" font-family="monospace" font-size="12" fill="#7dd3fc" opacity="0">
    <animate attributeName="opacity" from="0" to="1" begin="5s" dur="0.3s" fill="freeze"/>
    ─────────────────────────────────────────────────────────
  </text>

  <text x="30" y="366" font-family="monospace" font-size="12" fill="#38bdf8" opacity="0">
    <animate attributeName="opacity" from="0" to="1" begin="5.3s" dur="0.3s" fill="freeze"/>
    $ <tspan fill="#00ff80">Scan complete. 0 threats detected.</tspan>
  </text>

  <!-- BLINKING CURSOR at the end -->
  <rect x="42" y="362" width="6" height="11" fill="#38bdf8" opacity="0">
    <animate attributeName="opacity" from="0" to="1" begin="5.8s" dur="0.01s" fill="freeze"/>
    <animate attributeName="opacity" values="1;0;1" dur="1s" repeatCount="indefinite"/>
  </rect>

</svg>

</div>

<br/>

---

<br/>

<!-- ═══════════════════════════════════════════════════════════════ -->
<!-- █████████████████ SKILLS — ANIMATED DASHBOARD ███████████████ -->
<!-- ═══════════════════════════════════════════════════════════════ -->

### `❯ ./skills --animate --dashboard`

<div align="center">

<br/>

<svg xmlns="http://www.w3.org/2000/svg" width="100%" height="380" viewBox="0 0 900 380" style="border-radius:6px;">

  <defs>
    <linearGradient id="bar1" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#38bdf8"/>
      <stop offset="100%" stop-color="#0ea5e9"/>
    </linearGradient>
    <linearGradient id="bar2" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#00ff80"/>
      <stop offset="100%" stop-color="#059669"/>
    </linearGradient>
    <linearGradient id="bar3" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#f59e0b"/>
      <stop offset="100%" stop-color="#d97706"/>
    </linearGradient>
    <linearGradient id="bar4" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#a855f7"/>
      <stop offset="100%" stop-color="#7c3aed"/>
    </linearGradient>
  </defs>

  <rect width="900" height="380" fill="#060a10" rx="6"/>

  <!-- HEADER -->
  <text x="450" y="30" text-anchor="middle" font-family="monospace" font-size="13" fill="#38bdf8" letter-spacing="2">SKILL PROFICIENCY METRICS</text>
  <line x1="200" y1="40" x2="700" y2="40" stroke="#38bdf8" stroke-width="0.5" opacity="0.3"/>

  <!-- BAR 1: SOC & BLUE TEAM -->
  <text x="30" y="72" font-family="monospace" font-size="12" fill="#e0f4ff">SOC &amp; BLUE TEAM</text>
  <text x="830" y="72" font-family="monospace" font-size="12" fill="#38bdf8" text-anchor="end">92%</text>
  <!-- Bar bg -->
  <rect x="30" y="80" width="840" height="18" rx="4" fill="#0b1929" stroke="#1a3a5c" stroke-width="0.5"/>
  <!-- Bar fill -->
  <rect x="30" y="80" width="0" height="18" rx="4" fill="url(#bar1)" opacity="0.85">
    <animate attributeName="width" from="0" to="772" dur="2s" begin="0.2s" fill="freeze"/>
  </rect>
  <text x="60" y="94" font-family="monospace" font-size="9" fill="#060a10" font-weight="bold" opacity="0">
    <animate attributeName="opacity" from="0" to="1" begin="1.2s" dur="0.01s" fill="freeze"/>
    SOC Analysis · Incident Response · SIEM · Threat Hunting
  </text>

  <!-- BAR 2: VAPT & RED TEAM -->
  <text x="30" y="132" font-family="monospace" font-size="12" fill="#e0f4ff">VAPT &amp; RED TEAM</text>
  <text x="830" y="132" font-family="monospace" font-size="12" fill="#00ff80" text-anchor="end">86%</text>
  <rect x="30" y="140" width="840" height="18" rx="4" fill="#0b1929" stroke="#1a3a5c" stroke-width="0.5"/>
  <rect x="30" y="140" width="0" height="18" rx="4" fill="url(#bar2)" opacity="0.85">
    <animate attributeName="width" from="0" to="722" dur="2s" begin="0.6s" fill="freeze"/>
  </rect>
  <text x="60" y="154" font-family="monospace" font-size="9" fill="#060a10" font-weight="bold" opacity="0">
    <animate attributeName="opacity" from="0" to="1" begin="1.6s" dur="0.01s" fill="freeze"/>
    Web Pentest · Network Pentest · Bug Bounty · Exploit Dev
  </text>

  <!-- BAR 3: SECURITY ENGINEERING -->
  <text x="30" y="192" font-family="monospace" font-size="12" fill="#e0f4ff">SECURITY ENGINEERING</text>
  <text x="830" y="192" font-family="monospace" font-size="12" fill="#f59e0b" text-anchor="end">78%</text>
  <rect x="30" y="200" width="840" height="18" rx="4" fill="#0b1929" stroke="#1a3a5c" stroke-width="0.5"/>
  <rect x="30" y="200" width="0" height="18" rx="4" fill="url(#bar3)" opacity="0.85">
    <animate attributeName="width" from="0" to="655" dur="2s" begin="1s" fill="freeze"/>
  </rect>
  <text x="60" y="214" font-family="monospace" font-size="9" fill="#060a10" font-weight="bold" opacity="0">
    <animate attributeName="opacity" from="0" to="1" begin="2s" dur="0.01s" fill="freeze"/>
    Python · Bash · SIEM Engineering · Docker · Automation
  </text>

  <!-- BAR 4: THREAT INTELLIGENCE -->
  <text x="30" y="252" font-family="monospace" font-size="12" fill="#e0f4ff">THREAT INTELLIGENCE</text>
  <text x="830" y="252" font-family="monospace" font-size="12" fill="#a855f7" text-anchor="end">90%</text>
  <rect x="30" y="260" width="840" height="18" rx="4" fill="#0b1929" stroke="#1a3a5c" stroke-width="0.5"/>
  <rect x="30" y="260" width="0" height="18" rx="4" fill="url(#bar4)" opacity="0.85">
    <animate attributeName="width" from="0" to="756" dur="2s" begin="1.4s" fill="freeze"/>
  </rect>
  <text x="60" y="274" font-family="monospace" font-size="9" fill="#060a10" font-weight="bold" opacity="0">
    <animate attributeName="opacity" from="0" to="1" begin="2.4s" dur="0.01s" fill="freeze"/>
    MITRE ATT&amp;CK · CTI Analysis · CVE Research · OSINT
  </text>

  <!-- BOTTOM STATUS -->
  <line x1="30" y="300" x2="870" y2="300" stroke="#1a3a5c" stroke-width="0.5"/>
  <text x="450" y="325" text-anchor="middle" font-family="monospace" font-size="10" fill="#38bdf8" opacity="0.5">███▒▒▒▒▒▒▒▒▒ LOADING NEXT MODULE ▒▒▒▒▒▒▒▒▒███</text>

  <!-- Pulse dots -->
  <circle cx="350" cy="352" r="3" fill="#38bdf8" opacity="0">
    <animate attributeName="opacity" values="0;0.8;0" dur="2s" repeatCount="indefinite"/>
  </circle>
  <circle cx="370" cy="352" r="3" fill="#38bdf8" opacity="0">
    <animate attributeName="opacity" values="0;0.8;0" dur="2s" begin="0.3s" repeatCount="indefinite"/>
  </circle>
  <circle cx="390" cy="352" r="3" fill="#38bdf8" opacity="0">
    <animate attributeName="opacity" values="0;0.8;0" dur="2s" begin="0.6s" repeatCount="indefinite"/>
  </circle>
  <circle cx="410" cy="352" r="3" fill="#38bdf8" opacity="0">
    <animate attributeName="opacity" values="0;0.8;0" dur="2s" begin="0.9s" repeatCount="indefinite"/>
  </circle>
  <circle cx="430" cy="352" r="3" fill="#38bdf8" opacity="0">
    <animate attributeName="opacity" values="0;0.8;0" dur="2s" begin="1.2s" repeatCount="indefinite"/>
  </circle>
  <circle cx="450" cy="352" r="3" fill="#38bdf8" opacity="0">
    <animate attributeName="opacity" values="0;0.8;0" dur="2s" begin="1.5s" repeatCount="indefinite"/>
  </circle>
  <circle cx="470" cy="352" r="3" fill="#38bdf8" opacity="0">
    <animate attributeName="opacity" values="0;0.8;0" dur="2s" begin="1.8s" repeatCount="indefinite"/>
  </circle>
  <circle cx="490" cy="352" r="3" fill="#38bdf8" opacity="0">
    <animate attributeName="opacity" values="0;0.8;0" dur="2s" begin="2.1s" repeatCount="indefinite"/>
  </circle>
  <circle cx="510" cy="352" r="3" fill="#38bdf8" opacity="0">
    <animate attributeName="opacity" values="0;0.8;0" dur="2s" begin="2.4s" repeatCount="indefinite"/>
  </circle>
  <circle cx="530" cy="352" r="3" fill="#38bdf8" opacity="0">
    <animate attributeName="opacity" values="0;0.8;0" dur="2s" begin="2.7s" repeatCount="indefinite"/>
  </circle>
  <circle cx="550" cy="352" r="3" fill="#38bdf8" opacity="0">
    <animate attributeName="opacity" values="0;0.8;0" dur="2s" begin="3s" repeatCount="indefinite"/>
  </circle>

</svg>

</div>

<div align="center">

<table>
<tr>
<td width="25%" align="center" valign="top">

#### 🛡️ SOC / BLUE
![Splunk](https://img.shields.io/badge/Splunk-0b1929?style=flat-square&logo=splunk&logoColor=38BDF8)
![Microsoft Sentinel](https://img.shields.io/badge/Sentinel-0b1929?style=flat-square&logo=microsoftazure&logoColor=38BDF8)
![Wireshark](https://img.shields.io/badge/Wireshark-0b1929?style=flat-square&logo=wireshark&logoColor=38BDF8)
![LetsDefend](https://img.shields.io/badge/LetsDefend-0b1929?style=flat-square&logo=protonmail&logoColor=38BDF8)
![TryHackMe](https://img.shields.io/badge/TryHackMe-0b1929?style=flat-square&logo=tryhackme&logoColor=38BDF8)

</td>
<td width="25%" align="center" valign="top">

#### ⚔️ VAPT / RED
![Burp Suite](https://img.shields.io/badge/Burp_Suite-0b1929?style=flat-square&logo=burp-suite&logoColor=38BDF8)
![Kali Linux](https://img.shields.io/badge/Kali_Linux-0b1929?style=flat-square&logo=kali-linux&logoColor=38BDF8)
![Metasploit](https://img.shields.io/badge/Metasploit-0b1929?style=flat-square&logo=metasploit&logoColor=38BDF8)
![OWASP](https://img.shields.io/badge/OWASP_Top_10-0b1929?style=flat-square&logo=owasp&logoColor=38BDF8)
![Nmap](https://img.shields.io/badge/Nmap-0b1929?style=flat-square&logo=nmap&logoColor=38BDF8)

</td>
<td width="25%" align="center" valign="top">

#### ⚙️ SEC ENG
![Python](https://img.shields.io/badge/Python-0b1929?style=flat-square&logo=python&logoColor=38BDF8)
![Bash](https://img.shields.io/badge/Bash-0b1929?style=flat-square&logo=gnu-bash&logoColor=38BDF8)
![Linux](https://img.shields.io/badge/Linux-0b1929?style=flat-square&logo=linux&logoColor=38BDF8)
![Docker](https://img.shields.io/badge/Docker-0b1929?style=flat-square&logo=docker&logoColor=38BDF8)
![Git](https://img.shields.io/badge/Git-0b1929?style=flat-square&logo=git&logoColor=38BDF8)

</td>
<td width="25%" align="center" valign="top">

#### 🌐 THREAT INTEL
![MITRE ATT&CK](https://img.shields.io/badge/MITRE_ATT%26CK-0b1929?style=flat-square&logo=target&logoColor=38BDF8)
![IOC Analysis](https://img.shields.io/badge/IOC-0b1929?style=flat-square&logo=hackthebox&logoColor=38BDF8)
![CVE Research](https://img.shields.io/badge/CVE-0b1929?style=flat-square&logo=googlecloud&logoColor=38BDF8)
![Threat Hunting](https://img.shields.io/badge/Threat_Hunting-0b1929?style=flat-square&logo=moleculer&logoColor=38BDF8)
![OSINT](https://img.shields.io/badge/OSINT-0b1929?style=flat-square&logo=signal&logoColor=38BDF8)

</td>
</tr>
</table>

</div>

<br/>

---

<br/>

<!-- ═══════════════════════════════════════════════════════════════ -->
<!-- █████████████████ GITHUB STATS & TROPHY CASE ████████████████ -->
<!-- ═══════════════════════════════════════════════════════════════ -->

### `❯ ./github --stats --achievements`

<div align="center">

<br/>

<svg xmlns="http://www.w3.org/2000/svg" width="100%" height="50" viewBox="0 0 900 50" style="border-radius:4px;">
  <rect width="900" height="50" fill="#060a10" rx="4"/>
  <text x="360" y="30" font-family="monospace" font-size="12" fill="#38bdf8" opacity="0.6">LIVE GITHUB ANALYTICS</text>
  <circle cx="830" cy="26" r="4" fill="#00ff80">
    <animate attributeName="opacity" values="1;0.2;1" dur="2s" repeatCount="indefinite"/>
  </circle>
  <text x="842" y="30" font-family="monospace" font-size="10" fill="#00ff80" opacity="0.8">LIVE</text>
  <line x1="30" y1="40" x2="870" y2="40" stroke="#1a3a5c" stroke-width="0.5"/>
</svg>

<br/>

<img width="48%" src="https://github-readme-stats.vercel.app/api?username=logesh-GIT001&show_icons=true&hide_border=false&bg_color=0b1929&title_color=38bdf8&icon_color=38bdf8&text_color=bae6fd&border_color=1a3a5c&count_private=true&theme=github_dark&ring_color=38bdf8" />
&nbsp;
<img width="48%" src="https://streak-stats.demolab.com?user=logesh-GIT001&hide_border=false&background=0b1929&ring=38bdf8&fire=38bdf8&currStreakLabel=38bdf8&border=1a3a5c&sideLabels=bae6fd&dates=7dd3fc" />

<br/><br/>

<img width="48%" src="https://github-readme-stats.vercel.app/api/top-langs/?username=logesh-GIT001&layout=compact&hide_border=false&bg_color=0b1929&title_color=38bdf8&text_color=bae6fd&border_color=1a3a5c&langs_count=8&theme=github_dark" />
&nbsp;
<img width="48%" src="https://github-profile-trophy.vercel.app/?username=logesh-GIT001&theme=onestar&no-frame=true&column=4&margin-w=15&margin-h=15&row=2&no-bg=true" />

<br/><br/>

<img width="96%" src="https://github-readme-activity-graph.vercel.app/graph?username=logesh-GIT001&bg_color=0b1929&color=38bdf8&line=38bdf8&point=00d4ff&area=true&area_color=38bdf8&border_color=1a3a5c&hide_border=false&theme=react-dark&custom_title=Contribution+Activity+%26+Patterns" />

<br/><br/>

<img width="96%" src="https://github-readme-stats.vercel.app/api?username=logesh-GIT001&show=reviews,discussions_started,discussions_answered,prs_merged,prs_merged_percentage&hide_border=false&bg_color=0b1929&title_color=38bdf8&icon_color=38bdf8&text_color=bae6fd&border_color=1a3a5c&count_private=true&theme=github_dark&include_all_commits=true&custom_title=Contribution+Breakdown" />

</div>

<br/>

---

<br/>

<!-- ═══════════════════════════════════════════════════════════════ -->
<!-- ███████████████ SNAKE CONTRIBUTIONS — UNTOUCHED █████████████ -->
<!-- ═══════════════════════════════════════════════════════════════ -->

### `❯ watch --contributions`

<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/logesh-GIT001/logesh-GIT001/output/github-snake-dark.svg"/>
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/logesh-GIT001/logesh-GIT001/output/github-snake.svg"/>
  <img alt="github-snake" src="https://raw.githubusercontent.com/logesh-GIT001/logesh-GIT001/output/github-snake.svg"/>
</picture>

</div>

<br/>

---

<br/>

<!-- ═══════════════════════════════════════════════════════════════ -->
<!-- █████████████████ CONNECT — BADGES + LINKS ██████████████████ -->
<!-- ═══════════════════════════════════════════════════════════════ -->

### `❯ connect --channels --encrypt`

<div align="center">

<a href="https://x.com/Loki_1718">
  <img src="https://img.shields.io/badge/X_%2F_Twitter-0b1929?style=for-the-badge&logo=x&logoColor=38BDF8&labelColor=060a10"/>
</a>&nbsp;&nbsp;
<a href="https://linkedin.com/in/logeshwaran-s-b5aa5b27b">
  <img src="https://img.shields.io/badge/LinkedIn-0b1929?style=for-the-badge&logo=linkedin&logoColor=38BDF8&labelColor=060a10"/>
</a>&nbsp;&nbsp;
<a href="https://github.com/logesh-GIT001">
  <img src="https://img.shields.io/badge/GitHub-0b1929?style=for-the-badge&logo=github&logoColor=38BDF8&labelColor=060a10"/>
</a>&nbsp;&nbsp;
<a href="https://logesh-git001.github.io/loki/index.html">
  <img src="https://img.shields.io/badge/Portfolio-0b1929?style=for-the-badge&logo=githubpages&logoColor=38BDF8&labelColor=060a10"/>
</a>&nbsp;&nbsp;
<a href="mailto:logesh.spy@gmail.com">
  <img src="https://img.shields.io/badge/Email-0b1929?style=for-the-badge&logo=gmail&logoColor=38BDF8&labelColor=060a10"/>
</a>

<br/><br/>

<a href="https://tryhackme.com/p/your-profile">
  <img src="https://img.shields.io/badge/TryHackMe-0b1929?style=for-the-badge&logo=tryhackme&logoColor=38BDF8&labelColor=060a10"/>
</a>&nbsp;&nbsp;
<a href="#">
  <img src="https://img.shields.io/badge/Bugcrowd-0b1929?style=for-the-badge&logo=bugcrowd&logoColor=38BDF8&labelColor=060a10"/>
</a>&nbsp;&nbsp;
<a href="#">
  <img src="https://img.shields.io/badge/HackerOne-0b1929?style=for-the-badge&logo=hackerone&logoColor=38BDF8&labelColor=060a10"/>
</a>&nbsp;&nbsp;
<a href="https://logesh-git001.github.io/loki/index.html">
  <img src="https://img.shields.io/badge/PGP_Key-0b1929?style=for-the-badge&logo=lock&logoColor=38BDF8&labelColor=060a10"/>
</a>

</div>

<br/>

---

<br/>

<!-- ═══════════════════════════════════════════════════════════════ -->
<!-- █████████████████ ANIMATED SECURITY FOOTER █████████████████ -->
<!-- ═══════════════════════════════════════════════════════════════ -->

<div align="center">

<svg xmlns="http://www.w3.org/2000/svg" width="100%" height="320" viewBox="0 0 1000 320" style="border-radius:6px;">

  <defs>
    <linearGradient id="footerGrad" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" stop-color="#060a10"/>
      <stop offset="100%" stop-color="#020408"/>
    </linearGradient>
  </defs>

  <rect width="1000" height="320" fill="url(#footerGrad)" rx="6"/>

  <!-- Scanline -->
  <rect x="0" y="0" width="1000" height="2" fill="#38bdf8" opacity="0.05">
    <animate attributeName="y" values="0;320" dur="4s" repeatCount="indefinite"/>
  </rect>

  <!-- HUD corners (smaller) -->
  <path d="M 40,40 L 80,40" stroke="#38bdf8" stroke-width="1.5" fill="none" opacity="0.5"/>
  <path d="M 40,40 L 40,80" stroke="#38bdf8" stroke-width="1.5" fill="none" opacity="0.5"/>
  <path d="M 960,40 L 920,40" stroke="#38bdf8" stroke-width="1.5" fill="none" opacity="0.5"/>
  <path d="M 960,40 L 960,80" stroke="#38bdf8" stroke-width="1.5" fill="none" opacity="0.5"/>
  <path d="M 40,280 L 80,280" stroke="#38bdf8" stroke-width="1.5" fill="none" opacity="0.5"/>
  <path d="M 40,280 L 40,240" stroke="#38bdf8" stroke-width="1.5" fill="none" opacity="0.5"/>
  <path d="M 960,280 L 920,280" stroke="#38bdf8" stroke-width="1.5" fill="none" opacity="0.5"/>
  <path d="M 960,280 L 960,240" stroke="#38bdf8" stroke-width="1.5" fill="none" opacity="0.5"/>

  <!-- QUOTE FRAME -->
  <rect x="150" y="55" width="700" height="80" rx="4" fill="#0b1929" stroke="#1a3a5c" stroke-width="1" opacity="0.8"/>
  <rect x="150" y="55" width="700" height="1" fill="#38bdf8" opacity="0.3">
    <animate attributeName="opacity" values="0.3;0.6;0.3" dur="3s" repeatCount="indefinite"/>
  </rect>
  <text x="500" y="88" text-anchor="middle" font-family="monospace" font-size="13" fill="#7dd3fc" opacity="0.9">"The quieter you become, the more you can hear."</text>
  <text x="500" y="110" text-anchor="middle" font-family="monospace" font-size="11" fill="#38bdf8" opacity="0.5">— Kali Linux Motto</text>

  <!-- STATUS BADGES ROW -->
  <g transform="translate(500, 175)">
    <rect x="-160" y="-10" width="320" height="20" rx="10" fill="none" stroke="#1a3a5c" stroke-width="0.5"/>
    <circle cx="-130" cy="0" r="4" fill="#00ff80">
      <animate attributeName="opacity" values="1;0.2;1" dur="1.5s" repeatCount="indefinite"/>
    </circle>
    <text x="-118" y="5" font-family="monospace" font-size="10" fill="#00ff80" opacity="0.8">STATUS: ACTIVE</text>
    <circle cx="20" cy="0" r="4" fill="#38bdf8">
      <animate attributeName="opacity" values="1;0.2;1" dur="2s" begin="0.5s" repeatCount="indefinite"/>
    </circle>
    <text x="32" y="5" font-family="monospace" font-size="10" fill="#38bdf8" opacity="0.8">NODE: README.md</text>
  </g>

  <!-- THREAT LEVEL METER -->
  <g transform="translate(500, 215)">
    <text x="0" y="0" text-anchor="middle" font-family="monospace" font-size="9" fill="#38bdf8" opacity="0.4">THREAT LEVEL</text>
    <rect x="-100" y="8" width="200" height="12" rx="6" fill="#0b1929" stroke="#1a3a5c" stroke-width="0.5"/>
    <rect x="-100" y="8" width="40" height="12" rx="6" fill="#00ff80">
      <animate attributeName="opacity" values="1;0.6;1" dur="2s" repeatCount="indefinite"/>
    </rect>
    <text x="-15" y="18" font-family="monospace" font-size="8" fill="#060a10" font-weight="bold">LOW</text>
  </g>

  <!-- Animated loading dots -->
  <g transform="translate(500, 260)">
    <circle cx="-30" cy="0" r="3" fill="#38bdf8" opacity="0">
      <animate attributeName="opacity" values="0;0.8;0" dur="1.5s" repeatCount="indefinite"/>
    </circle>
    <circle cx="-10" cy="0" r="3" fill="#38bdf8" opacity="0">
      <animate attributeName="opacity" values="0;0.8;0" dur="1.5s" begin="0.3s" repeatCount="indefinite"/>
    </circle>
    <circle cx="10" cy="0" r="3" fill="#38bdf8" opacity="0">
      <animate attributeName="opacity" values="0;0.8;0" dur="1.5s" begin="0.6s" repeatCount="indefinite"/>
    </circle>
    <circle cx="30" cy="0" r="3" fill="#38bdf8" opacity="0">
      <animate attributeName="opacity" values="0;0.8;0" dur="1.5s" begin="0.9s" repeatCount="indefinite"/>
    </circle>
  </g>

  <!-- Matrix-style footer characters -->
  <g font-family="monospace" font-size="8" fill="#38bdf8" opacity="0.08">
    <text x="20" y="300">01001000 01100001 01100011 01101011 00100000 01110100 01101000 01100101 00100000 01110000 01101100 01100001 01101110 01100101 01110100</text>
  </g>
  <g font-family="monospace" font-size="8" fill="#38bdf8" opacity="0.05">
    <text x="320" y="310">01000100 01100101 01100110 01100101 01101110 01110011 01100101 00100000 01110100 01101000 01100101 00100000 01100011 01100001 01110011 01110100 01101100 01100101</text>
  </g>

  <!-- Bottom status -->
  <text x="40" y="305" font-family="monospace" font-size="9" fill="#38bdf8" opacity="0.25">[SECURE CHANNEL ESTABLISHED]</text>
  <text x="810" y="305" font-family="monospace" font-size="9" fill="#38bdf8" opacity="0.25">[ENCRYPTION: AES-256]</text>

</svg>

<br/><br/>

<img src="https://img.shields.io/badge/status-online-38bdf8?style=flat-square&labelColor=060a10&logo=vercel&logoColor=38bdf8" />&nbsp;&nbsp;
<img src="https://komarev.com/ghpvc/?username=logesh-GIT001&color=38bdf8&style=flat-square&label=profile+views&labelColor=060a10" />&nbsp;&nbsp;
<img src="https://img.shields.io/badge/availability-open_to_work-00ff80?style=flat-square&labelColor=060a10&logo=telegram&logoColor=38bdf8" />&nbsp;&nbsp;
<img src="https://img.shields.io/github/followers/logesh-GIT001?style=flat-square&labelColor=060a10&color=38bdf8&logo=github&logoColor=38bdf8" />&nbsp;&nbsp;
<img src="https://img.shields.io/badge/loki_online-true-00ff80?style=flat-square&labelColor=060a10&logo=matrix&logoColor=38bdf8" />

</div>

<br/>

<img src="https://capsule-render.vercel.app/api?type=venom&color=0:060a10,50:0b1929,100:060a10&height=120&section=footer" width="100%"/>
