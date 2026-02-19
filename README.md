<svg xmlns="http://www.w3.org/2000/svg" width="900" height="120" viewBox="0 0 900 120">
  <defs>
    <radialGradient id="nebulaGlow" cx="50%" cy="50%" r="50%">
      <stop offset="0%" stop-color="#0d1b4b" stop-opacity="1"/>
      <stop offset="100%" stop-color="#020210" stop-opacity="1"/>
    </radialGradient>
    <radialGradient id="glow1" cx="50%" cy="50%" r="50%">
      <stop offset="0%" stop-color="#58A6FF" stop-opacity="0.6"/>
      <stop offset="100%" stop-color="#58A6FF" stop-opacity="0"/>
    </radialGradient>
    <radialGradient id="glow2" cx="50%" cy="50%" r="50%">
      <stop offset="0%" stop-color="#a78bfa" stop-opacity="0.5"/>
      <stop offset="100%" stop-color="#a78bfa" stop-opacity="0"/>
    </radialGradient>
    <filter id="blur1">
      <feGaussianBlur stdDeviation="2"/>
    </filter>
    <filter id="blur2">
      <feGaussianBlur stdDeviation="4"/>
    </filter>
  </defs>

  <!-- Background -->
  <rect width="900" height="120" fill="url(#nebulaGlow)"/>

  <!-- Nebula blobs -->
  <ellipse cx="150" cy="60" rx="120" ry="50" fill="#0d1b4b" opacity="0.5" filter="url(#blur2)"/>
  <ellipse cx="450" cy="40" rx="180" ry="60" fill="#0a0a40" opacity="0.4" filter="url(#blur2)"/>
  <ellipse cx="780" cy="70" rx="140" ry="55" fill="#0d1040" opacity="0.5" filter="url(#blur2)"/>

  <!-- Glow orbs -->
  <circle cx="200" cy="55" r="30" fill="url(#glow1)" filter="url(#blur1)"/>
  <circle cx="650" cy="45" r="25" fill="url(#glow2)" filter="url(#blur1)"/>
  <circle cx="850" cy="80" r="20" fill="url(#glow1)" filter="url(#blur1)"/>

  <!-- STARS — small white dots with individual twinkle animations -->
  <!-- Bright stars -->
  <circle cx="45" cy="15" r="1.5" fill="#ffffff"><animate attributeName="opacity" values="1;0.1;1" dur="2.1s" repeatCount="indefinite"/></circle>
  <circle cx="130" cy="35" r="2" fill="#ffffff"><animate attributeName="opacity" values="0.3;1;0.3" dur="1.7s" repeatCount="indefinite"/></circle>
  <circle cx="220" cy="10" r="1.5" fill="#58A6FF"><animate attributeName="opacity" values="1;0.2;1" dur="3.2s" repeatCount="indefinite"/></circle>
  <circle cx="310" cy="50" r="1" fill="#ffffff"><animate attributeName="opacity" values="0.5;1;0.5" dur="2.4s" repeatCount="indefinite"/></circle>
  <circle cx="380" cy="20" r="2" fill="#a78bfa"><animate attributeName="opacity" values="1;0.1;1" dur="1.9s" repeatCount="indefinite"/></circle>
  <circle cx="460" cy="70" r="1.5" fill="#ffffff"><animate attributeName="opacity" values="0.2;1;0.2" dur="2.8s" repeatCount="indefinite"/></circle>
  <circle cx="540" cy="30" r="1" fill="#58A6FF"><animate attributeName="opacity" values="1;0.3;1" dur="1.5s" repeatCount="indefinite"/></circle>
  <circle cx="620" cy="55" r="2" fill="#ffffff"><animate attributeName="opacity" values="0.4;1;0.4" dur="3.5s" repeatCount="indefinite"/></circle>
  <circle cx="700" cy="15" r="1.5" fill="#a78bfa"><animate attributeName="opacity" values="1;0.2;1" dur="2.2s" repeatCount="indefinite"/></circle>
  <circle cx="780" cy="40" r="1" fill="#ffffff"><animate attributeName="opacity" values="0.6;1;0.6" dur="1.8s" repeatCount="indefinite"/></circle>
  <circle cx="855" cy="20" r="2" fill="#58A6FF"><animate attributeName="opacity" values="1;0.1;1" dur="2.9s" repeatCount="indefinite"/></circle>
  <circle cx="890" cy="65" r="1.5" fill="#ffffff"><animate attributeName="opacity" values="0.3;1;0.3" dur="2.3s" repeatCount="indefinite"/></circle>

  <!-- Medium stars -->
  <circle cx="80" cy="60" r="1" fill="#ccddff"><animate attributeName="opacity" values="0.8;0.1;0.8" dur="2.6s" repeatCount="indefinite"/></circle>
  <circle cx="165" cy="80" r="1.2" fill="#ffffff"><animate attributeName="opacity" values="1;0.4;1" dur="1.6s" repeatCount="indefinite"/></circle>
  <circle cx="260" cy="90" r="1" fill="#58A6FF"><animate attributeName="opacity" values="0.5;1;0.5" dur="3.1s" repeatCount="indefinite"/></circle>
  <circle cx="340" cy="75" r="1.5" fill="#ffffff"><animate attributeName="opacity" values="1;0.2;1" dur="2.0s" repeatCount="indefinite"/></circle>
  <circle cx="420" cy="100" r="1" fill="#a78bfa"><animate attributeName="opacity" values="0.3;1;0.3" dur="2.7s" repeatCount="indefinite"/></circle>
  <circle cx="500" cy="85" r="1.2" fill="#ffffff"><animate attributeName="opacity" values="1;0.1;1" dur="1.4s" repeatCount="indefinite"/></circle>
  <circle cx="575" cy="95" r="1" fill="#58A6FF"><animate attributeName="opacity" values="0.7;1;0.7" dur="3.3s" repeatCount="indefinite"/></circle>
  <circle cx="660" cy="80" r="1.5" fill="#ffffff"><animate attributeName="opacity" values="1;0.3;1" dur="2.1s" repeatCount="indefinite"/></circle>
  <circle cx="730" cy="100" r="1" fill="#a78bfa"><animate attributeName="opacity" values="0.4;1;0.4" dur="1.9s" repeatCount="indefinite"/></circle>
  <circle cx="810" cy="90" r="1.2" fill="#ffffff"><animate attributeName="opacity" values="1;0.2;1" dur="2.5s" repeatCount="indefinite"/></circle>

  <!-- Tiny dim stars -->
  <circle cx="20" cy="90" r="0.8" fill="#aaaacc"><animate attributeName="opacity" values="0.6;0.1;0.6" dur="3.8s" repeatCount="indefinite"/></circle>
  <circle cx="100" cy="105" r="0.8" fill="#aaaacc"><animate attributeName="opacity" values="0.2;0.8;0.2" dur="2.2s" repeatCount="indefinite"/></circle>
  <circle cx="190" cy="110" r="0.8" fill="#aaaacc"><animate attributeName="opacity" values="0.7;0.1;0.7" dur="3.0s" repeatCount="indefinite"/></circle>
  <circle cx="290" cy="25" r="0.8" fill="#aaaacc"><animate attributeName="opacity" values="0.3;0.9;0.3" dur="1.8s" repeatCount="indefinite"/></circle>
  <circle cx="360" cy="110" r="0.8" fill="#aaaacc"><animate attributeName="opacity" values="0.8;0.1;0.8" dur="2.4s" repeatCount="indefinite"/></circle>
  <circle cx="480" cy="10" r="0.8" fill="#aaaacc"><animate attributeName="opacity" values="0.1;0.9;0.1" dur="3.5s" repeatCount="indefinite"/></circle>
  <circle cx="555" cy="108" r="0.8" fill="#aaaacc"><animate attributeName="opacity" values="0.6;0.1;0.6" dur="1.7s" repeatCount="indefinite"/></circle>
  <circle cx="635" cy="10" r="0.8" fill="#aaaacc"><animate attributeName="opacity" values="0.2;0.7;0.2" dur="2.9s" repeatCount="indefinite"/></circle>
  <circle cx="715" cy="112" r="0.8" fill="#aaaacc"><animate attributeName="opacity" values="0.9;0.1;0.9" dur="2.3s" repeatCount="indefinite"/></circle>
  <circle cx="795" cy="8" r="0.8" fill="#aaaacc"><animate attributeName="opacity" values="0.3;0.8;0.3" dur="3.4s" repeatCount="indefinite"/></circle>
  <circle cx="870" cy="110" r="0.8" fill="#aaaacc"><animate attributeName="opacity" values="0.7;0.1;0.7" dur="2.0s" repeatCount="indefinite"/></circle>

  <!-- SHOOTING STAR 1 -->
  <g>
    <line x1="0" y1="30" x2="60" y2="38" stroke="white" stroke-width="1" stroke-linecap="round" opacity="0">
      <animate attributeName="opacity" values="0;0;0;0;1;0" dur="6s" repeatCount="indefinite"/>
      <animateTransform attributeName="transform" type="translate" values="0,0;0,0;0,0;0,0;300,20;600,40" dur="6s" repeatCount="indefinite"/>
    </line>
  </g>
  <!-- SHOOTING STAR 2 -->
  <g>
    <line x1="0" y1="70" x2="55" y2="75" stroke="#a78bfa" stroke-width="0.8" stroke-linecap="round" opacity="0">
      <animate attributeName="opacity" values="0;0;0;1;0;0" dur="9s" repeatCount="indefinite"/>
      <animateTransform attributeName="transform" type="translate" values="0,0;0,0;0,0;200,0;500,-10;900,0" dur="9s" repeatCount="indefinite"/>
    </line>
  </g>

  <!-- 4-pointed star sparkles -->
  <g transform="translate(70,25)" opacity="0">
    <path d="M0,-4 L0.5,-0.5 L4,0 L0.5,0.5 L0,4 L-0.5,0.5 L-4,0 L-0.5,-0.5 Z" fill="#58A6FF"/>
    <animate attributeName="opacity" values="0;1;0" dur="3s" repeatCount="indefinite" begin="0.5s"/>
  </g>
  <g transform="translate(500,50)" opacity="0">
    <path d="M0,-5 L0.6,-0.6 L5,0 L0.6,0.6 L0,5 L-0.6,0.6 L-5,0 L-0.6,-0.6 Z" fill="#ffffff"/>
    <animate attributeName="opacity" values="0;1;0" dur="4s" repeatCount="indefinite" begin="1.5s"/>
  </g>
  <g transform="translate(820,30)" opacity="0">
    <path d="M0,-4 L0.5,-0.5 L4,0 L0.5,0.5 L0,4 L-0.5,0.5 L-4,0 L-0.5,-0.5 Z" fill="#a78bfa"/>
    <animate attributeName="opacity" values="0;1;0" dur="3.5s" repeatCount="indefinite" begin="2s"/>
  </g>
</svg>
