<!-- assets/header.svg -->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 300" width="1200" height="300" preserveAspectRatio="xMidYMid meet">
  <defs>
    <linearGradient id="g" x1="0" x2="1" y1="0" y2="0">
      <stop offset="0%" stop-color="#00C9FF"/>
      <stop offset="50%" stop-color="#92FE9D"/>
      <stop offset="100%" stop-color="#FF9A9E"/>
      <!-- hareket için offset değiştiriyoruz -->
      <animate xlink:href="#g stop[offset='50%']" attributeName="x" values="0;1;0" dur="6s" repeatCount="indefinite"/>
    </linearGradient>

    <filter id="soft" x="-20%" y="-20%" width="140%" height="140%">
      <feGaussianBlur stdDeviation="6" result="b"/>
      <feBlend in="SourceGraphic" in2="b"/>
    </filter>
  </defs>

  <rect width="100%" height="100%" fill="#0f1724"/>

  <!-- hafif hareket eden kabarcıklar -->
  <g opacity="0.12" filter="url(#soft)">
    <circle cx="1100" cy="40" r="60" fill="#fff">
      <animate attributeName="cy" dur="8s" values="40;260;40" repeatCount="indefinite"/>
      <animate attributeName="cx" dur="14s" values="1100;200;1100" repeatCount="indefinite"/>
    </circle>
    <circle cx="80" cy="180" r="40" fill="#fff">
      <animate attributeName="cy" dur="10s" values="180;40;180" repeatCount="indefinite"/>
      <animate attributeName="cx" dur="12s" values="80;900;80" repeatCount="indefinite"/>
    </circle>
  </g>

  <!-- Başlık metni -->
  <text x="50%" y="45%" dominant-baseline="middle" text-anchor="middle" font-family="Segoe UI, Roboto, Arial" font-size="56" font-weight="700" fill="url(#g)">
    Hüseyin Yaman
  </text>

  <!-- alt satır -->
  <text x="50%" y="70%" dominant-baseline="middle" text-anchor="middle" font-family="Segoe UI, Roboto, Arial" font-size="20" fill="#9aa4b2">
    Mobile Developer • Unity & .NET MAUI • Game maker
  </text>

  <!-- parlayan ışık bandı -->
  <rect x="-400" y="20" width="400" height="260" fill="white" opacity="0.06">
    <animate attributeName="x" from="-400" to="1200" dur="3.6s" repeatCount="indefinite" />
  </rect>
</svg>
