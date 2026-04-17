<div align="center">

<svg width="860" height="220" viewBox="0 0 860 220" xmlns="http://www.w3.org/2000/svg">

  <defs>
    <radialGradient id="bg" cx="50%" cy="50%" r="50%">
      <stop offset="0%" stop-color="#0d1b2a"/>
      <stop offset="100%" stop-color="#050d14"/>
    </radialGradient>
  </defs>

  <!-- BACKGROUND -->
  <rect width="860" height="220" fill="url(#bg)" rx="12"/>

  <!-- EDGES -->
  <g stroke="#1e4d6b" stroke-width="1" opacity="0.5">

    <line x1="100" y1="50" x2="280" y2="60"/>
    <line x1="100" y1="50" x2="280" y2="100"/>
    <line x1="100" y1="90" x2="280" y2="60"/>
    <line x1="100" y1="90" x2="280" y2="100"/>
    <line x1="100" y1="90" x2="280" y2="140"/>
    <line x1="100" y1="130" x2="280" y2="100"/>
    <line x1="100" y1="130" x2="280" y2="140"/>
    <line x1="100" y1="170" x2="280" y2="140"/>

    <line x1="280" y1="60" x2="460" y2="55"/>
    <line x1="280" y1="60" x2="460" y2="95"/>
    <line x1="280" y1="100" x2="460" y2="95"/>
    <line x1="280" y1="100" x2="460" y2="135"/>
    <line x1="280" y1="140" x2="460" y2="135"/>
    <line x1="280" y1="140" x2="460" y2="175"/>

    <line x1="460" y1="55" x2="640" y2="65"/>
    <line x1="460" y1="95" x2="640" y2="65"/>
    <line x1="460" y1="95" x2="640" y2="105"/>
    <line x1="460" y1="135" x2="640" y2="105"/>
    <line x1="460" y1="135" x2="640" y2="145"/>
    <line x1="460" y1="175" x2="640" y2="145"/>

    <line x1="640" y1="65" x2="780" y2="85"/>
    <line x1="640" y1="105" x2="780" y2="85"/>
    <line x1="640" y1="105" x2="780" y2="125"/>
    <line x1="640" y1="145" x2="780" y2="125"/>

  </g>

  <!-- SIGNAL PATH -->
  <path id="netPath"
        d="M100 50 L280 60 L460 55 L640 65 L780 85
           L640 145 L460 135 L280 140 L100 170"
        fill="none"/>

  <!-- SIGNAL PARTICLES -->
  <circle r="2.5" fill="#58c4ff" opacity="0.9">
    <animateMotion dur="3s" repeatCount="indefinite">
      <mpath href="#netPath"/>
    </animateMotion>
  </circle>

  <circle r="2.5" fill="#58c4ff" opacity="0.7">
    <animateMotion dur="4.2s" repeatCount="indefinite">
      <mpath href="#netPath"/>
    </animateMotion>
  </circle>

  <circle r="2.5" fill="#58c4ff" opacity="0.5">
    <animateMotion dur="5s" repeatCount="indefinite">
      <mpath href="#netPath"/>
    </animateMotion>
  </circle>

  <!-- NODES (with inline pulse animation) -->

  <!-- helper function style: radius animation -->
  <!-- Layer 0 -->
  <g fill="#1e88e5">
    <circle cx="100" cy="50" r="7"/>
    <circle cx="100" cy="90" r="7"/>
    <circle cx="100" cy="130" r="7"/>
    <circle cx="100" cy="170" r="7"/>

    <circle cx="280" cy="60" r="7"/>
    <circle cx="280" cy="100" r="7"/>
    <circle cx="280" cy="140" r="7"/>

    <circle cx="460" cy="55" r="7"/>
    <circle cx="460" cy="95" r="7"/>
    <circle cx="460" cy="135" r="7"/>
    <circle cx="460" cy="175" r="7"/>

    <circle cx="640" cy="65" r="7"/>
    <circle cx="640" cy="105" r="7"/>
    <circle cx="640" cy="145" r="7"/>
  </g>

  <!-- PULSE EFFECT (no CSS needed) -->
  <g fill="#1e88e5">
    <circle cx="100" cy="50">
      <animate attributeName="r" values="3;6;3" dur="2s" repeatCount="indefinite"/>
    </circle>

    <circle cx="280" cy="60">
      <animate attributeName="r" values="3;6;3" dur="2.3s" repeatCount="indefinite"/>
    </circle>

    <circle cx="460" cy="95">
      <animate attributeName="r" values="3;6;3" dur="2.4s" repeatCount="indefinite"/>
    </circle>

    <circle cx="640" cy="105">
      <animate attributeName="r" values="3;6;3" dur="2.2s" repeatCount="indefinite"/>
    </circle>
  </g>

  <!-- OUTPUT NODES -->
  <g fill="#58c4ff">
    <circle cx="780" cy="85" r="9"/>
    <circle cx="780" cy="125" r="9"/>
  </g>

  <!-- OUTPUT PULSE -->
  <g fill="#58c4ff">
    <circle cx="780" cy="85">
      <animate attributeName="r" values="4;8;4" dur="2.2s" repeatCount="indefinite"/>
    </circle>

    <circle cx="780" cy="125">
      <animate attributeName="r" values="4;8;4" dur="2.6s" repeatCount="indefinite"/>
    </circle>
  </g>

  <!-- LABEL -->
  <text x="440" y="205" text-anchor="middle"
        font-family="monospace"
        font-size="11"
        fill="#1e4d6b"
        letter-spacing="3">
    INPUT • PROCESS • LEARN • OUTPUT
  </text>

</svg>

</div>

---

<div align="center">

# Md. Sadman Haque

<a href="https://git.io/typing-svg"><img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=17&pause=1000&color=58A6FF&center=true&vCenter=true&width=600&lines=Exploring+Intelligent+Systems;Reasoning+%7C+Interpretability+%7C+Real-World+Impact;Researcher+%26+Engineer" alt="Typing SVG" /></a>

</div>

---

<div align="center">

Passionate about building systems that are not just powerful — but understandable and impactful.
My work sits at the intersection of machine reasoning, interpretability, and practical engineering.

</div>

---

### Tech Stack

<div align="center">

![C](https://img.shields.io/badge/C-00599C?style=flat-square&logo=c&logoColor=white)
![C++](https://img.shields.io/badge/C++-004482?style=flat-square&logo=cplusplus&logoColor=white)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)
![Arduino](https://img.shields.io/badge/Arduino-00979D?style=flat-square&logo=arduino&logoColor=white)
![Raspberry Pi](https://img.shields.io/badge/Raspberry%20Pi-C51A4A?style=flat-square&logo=raspberrypi&logoColor=white)
![Linux](https://img.shields.io/badge/Ubuntu-E95420?style=flat-square&logo=ubuntu&logoColor=white)

</div>

---

### Connect

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/shadib007)
[![Google Scholar](https://img.shields.io/badge/Google%20Scholar-4285F4?style=flat-square&logo=googlescholar&logoColor=white)](https://scholar.google.com/citations?user=3fMbSl8AAAAJ&hl=en)
[![ResearchGate](https://img.shields.io/badge/ResearchGate-00CCBB?style=flat-square&logo=researchgate&logoColor=white)](https://www.researchgate.net/profile/Md-Sadman-Haque)
[![Facebook](https://img.shields.io/badge/Facebook-1877F2?style=flat-square&logo=facebook&logoColor=white)](https://www.facebook.com/shadib007)
[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=flat-square&logo=instagram&logoColor=white)](https://www.instagram.com/sadman.h.adib/)

</div>
