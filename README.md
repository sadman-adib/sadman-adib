<!--  N E U R A L   H E A D E R  -->
<div align="center">

<svg width="860" height="220" viewBox="0 0 860 220" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <radialGradient id="bg" cx="50%" cy="50%" r="50%">
      <stop offset="0%"  stop-color="#0d1b2a"/>
      <stop offset="100%" stop-color="#050d14"/>
    </radialGradient>

    <!-- pulse animation along edges -->
    <style>
      .edge { stroke:#1e4d6b; stroke-width:1; opacity:0.5; }
      .node { fill:#0d1b2a; stroke:#1e88e5; stroke-width:1.5; }
      .node-core { fill:#1e88e5; }

      /* traveling dot per edge */
      @keyframes travel0  { 0%{offset-distance:0%} 100%{offset-distance:100%} }
      @keyframes travel1  { 0%{offset-distance:0%} 100%{offset-distance:100%} }
      @keyframes pulse    { 0%,100%{r:2;opacity:.9} 50%{r:3.5;opacity:1} }
      @keyframes glow     { 0%,100%{opacity:.35} 50%{opacity:.9} }

      .dot { fill:#58c4ff; r:2.5; }
      .node-core { animation: pulse 2.4s ease-in-out infinite; }

      /* staggered glow on edges */
      .e0  { animation: glow 2.8s ease-in-out infinite 0.0s; }
      .e1  { animation: glow 2.8s ease-in-out infinite 0.3s; }
      .e2  { animation: glow 2.8s ease-in-out infinite 0.6s; }
      .e3  { animation: glow 2.8s ease-in-out infinite 0.9s; }
      .e4  { animation: glow 2.8s ease-in-out infinite 1.2s; }
      .e5  { animation: glow 2.8s ease-in-out infinite 1.5s; }
      .e6  { animation: glow 2.8s ease-in-out infinite 1.8s; }
      .e7  { animation: glow 2.8s ease-in-out infinite 2.1s; }
      .e8  { animation: glow 2.8s ease-in-out infinite 2.4s; }
      .e9  { animation: glow 2.8s ease-in-out infinite 2.7s; }
      .e10 { animation: glow 2.8s ease-in-out infinite 0.2s; }
      .e11 { animation: glow 2.8s ease-in-out infinite 0.5s; }
      .e12 { animation: glow 2.8s ease-in-out infinite 0.8s; }
      .e13 { animation: glow 2.8s ease-in-out infinite 1.1s; }
      .e14 { animation: glow 2.8s ease-in-out infinite 1.4s; }
      .e15 { animation: glow 2.8s ease-in-out infinite 1.7s; }

      /* traveling signal dots */
      .sig { fill:#58c4ff; opacity:0; }
      @keyframes sig0  { 0%{opacity:0} 5%{opacity:1} 95%{opacity:1} 100%{opacity:0} }
      .sd0  { animation: sig0 2.8s linear infinite 0.0s; }
      .sd1  { animation: sig0 2.8s linear infinite 0.3s; }
      .sd2  { animation: sig0 2.8s linear infinite 0.6s; }
      .sd3  { animation: sig0 2.8s linear infinite 0.9s; }
      .sd4  { animation: sig0 2.8s linear infinite 1.2s; }
      .sd5  { animation: sig0 2.8s linear infinite 1.5s; }
      .sd6  { animation: sig0 2.8s linear infinite 1.8s; }
      .sd7  { animation: sig0 2.8s linear infinite 2.1s; }
      .sd8  { animation: sig0 2.8s linear infinite 2.4s; }
      .sd9  { animation: sig0 2.8s linear infinite 0.7s; }
      .sd10 { animation: sig0 2.8s linear infinite 1.0s; }
      .sd11 { animation: sig0 2.8s linear infinite 1.3s; }

      /* node pulse stagger */
      .np0  { animation: pulse 2.4s ease-in-out infinite 0.0s; }
      .np1  { animation: pulse 2.4s ease-in-out infinite 0.4s; }
      .np2  { animation: pulse 2.4s ease-in-out infinite 0.8s; }
      .np3  { animation: pulse 2.4s ease-in-out infinite 1.2s; }
      .np4  { animation: pulse 2.4s ease-in-out infinite 1.6s; }
      .np5  { animation: pulse 2.4s ease-in-out infinite 2.0s; }
      .np6  { animation: pulse 2.4s ease-in-out infinite 0.2s; }
      .np7  { animation: pulse 2.4s ease-in-out infinite 0.6s; }
      .np8  { animation: pulse 2.4s ease-in-out infinite 1.0s; }
      .np9  { animation: pulse 2.4s ease-in-out infinite 1.4s; }
    </style>
  </defs>

  <!-- background -->
  <rect width="860" height="220" fill="url(#bg)" rx="12"/>

  <!--
    Layer 0 (input):  x=100   nodes at y=50,90,130,170
    Layer 1 (hidden): x=280   nodes at y=60,100,140
    Layer 2 (hidden): x=460   nodes at y=55,95,135,175
    Layer 3 (hidden): x=640   nodes at y=65,105,145
    Layer 4 (output): x=780   nodes at y=85,125
  -->

  <!-- ── EDGES layer 0 → 1 ── -->
  <line class="edge e0"  x1="100" y1="50"  x2="280" y2="60"/>
  <line class="edge e1"  x1="100" y1="50"  x2="280" y2="100"/>
  <line class="edge e2"  x1="100" y1="90"  x2="280" y2="60"/>
  <line class="edge e3"  x1="100" y1="90"  x2="280" y2="100"/>
  <line class="edge e4"  x1="100" y1="90"  x2="280" y2="140"/>
  <line class="edge e5"  x1="100" y1="130" x2="280" y2="100"/>
  <line class="edge e6"  x1="100" y1="130" x2="280" y2="140"/>
  <line class="edge e7"  x1="100" y1="170" x2="280" y2="140"/>

  <!-- ── EDGES layer 1 → 2 ── -->
  <line class="edge e8"  x1="280" y1="60"  x2="460" y2="55"/>
  <line class="edge e9"  x1="280" y1="60"  x2="460" y2="95"/>
  <line class="edge e10" x1="280" y1="100" x2="460" y2="95"/>
  <line class="edge e11" x1="280" y1="100" x2="460" y2="135"/>
  <line class="edge e12" x1="280" y1="140" x2="460" y2="135"/>
  <line class="edge e13" x1="280" y1="140" x2="460" y2="175"/>

  <!-- ── EDGES layer 2 → 3 ── -->
  <line class="edge e14" x1="460" y1="55"  x2="640" y2="65"/>
  <line class="edge e15" x1="460" y1="95"  x2="640" y2="65"/>
  <line class="edge e0"  x1="460" y1="95"  x2="640" y2="105"/>
  <line class="edge e1"  x1="460" y1="135" x2="640" y2="105"/>
  <line class="edge e2"  x1="460" y1="135" x2="640" y2="145"/>
  <line class="edge e3"  x1="460" y1="175" x2="640" y2="145"/>

  <!-- ── EDGES layer 3 → 4 ── -->
  <line class="edge e4"  x1="640" y1="65"  x2="780" y2="85"/>
  <line class="edge e5"  x1="640" y1="105" x2="780" y2="85"/>
  <line class="edge e6"  x1="640" y1="105" x2="780" y2="125"/>
  <line class="edge e7"  x1="640" y1="145" x2="780" y2="125"/>

  <!-- ── SIGNAL DOTS (traveling along edges) ── -->
  <!-- Each animateMotion travels one edge; staggered begins give flow effect -->
  <circle class="sig sd0" r="2.5"><animateMotion dur="2.8s" repeatCount="indefinite" begin="0.0s"><mpath href="#p_e0"/></animateMotion></circle>
  <circle class="sig sd1" r="2.5"><animateMotion dur="2.8s" repeatCount="indefinite" begin="0.3s"><mpath href="#p_e1"/></animateMotion></circle>
  <circle class="sig sd2" r="2.5"><animateMotion dur="2.8s" repeatCount="indefinite" begin="0.6s"><mpath href="#p_e2"/></animateMotion></circle>
  <circle class="sig sd3" r="2.5"><animateMotion dur="2.8s" repeatCount="indefinite" begin="0.9s"><mpath href="#p_e3"/></animateMotion></circle>
  <circle class="sig sd4" r="2.5"><animateMotion dur="2.8s" repeatCount="indefinite" begin="1.2s"><mpath href="#p_e4"/></animateMotion></circle>
  <circle class="sig sd5" r="2.5"><animateMotion dur="2.8s" repeatCount="indefinite" begin="1.5s"><mpath href="#p_e5"/></animateMotion></circle>
  <circle class="sig sd6" r="2.5"><animateMotion dur="2.8s" repeatCount="indefinite" begin="1.8s"><mpath href="#p_e6"/></animateMotion></circle>
  <circle class="sig sd7" r="2.5"><animateMotion dur="2.8s" repeatCount="indefinite" begin="2.1s"><mpath href="#p_e7"/></animateMotion></circle>
  <circle class="sig sd8" r="2.5"><animateMotion dur="2.8s" repeatCount="indefinite" begin="0.5s"><mpath href="#p_e8"/></animateMotion></circle>
  <circle class="sig sd9" r="2.5"><animateMotion dur="2.8s" repeatCount="indefinite" begin="1.0s"><mpath href="#p_e9"/></animateMotion></circle>
  <circle class="sig sd10" r="2.5"><animateMotion dur="2.8s" repeatCount="indefinite" begin="1.6s"><mpath href="#p_e10"/></animateMotion></circle>
  <circle class="sig sd11" r="2.5"><animateMotion dur="2.8s" repeatCount="indefinite" begin="2.2s"><mpath href="#p_e11"/></animateMotion></circle>

  <!-- hidden paths for animateMotion -->
  <path id="p_e0"  d="M100,50  L280,60"  fill="none"/>
  <path id="p_e1"  d="M100,50  L280,100" fill="none"/>
  <path id="p_e2"  d="M100,90  L280,60"  fill="none"/>
  <path id="p_e3"  d="M100,90  L280,100" fill="none"/>
  <path id="p_e4"  d="M280,60  L460,55"  fill="none"/>
  <path id="p_e5"  d="M280,100 L460,95"  fill="none"/>
  <path id="p_e6"  d="M280,140 L460,135" fill="none"/>
  <path id="p_e7"  d="M460,55  L640,65"  fill="none"/>
  <path id="p_e8"  d="M460,95  L640,105" fill="none"/>
  <path id="p_e9"  d="M460,135 L640,145" fill="none"/>
  <path id="p_e10" d="M640,65  L780,85"  fill="none"/>
  <path id="p_e11" d="M640,105 L780,125" fill="none"/>

  <!-- ── NODES ── -->
  <!-- Layer 0 -->
  <circle class="node" cx="100" cy="50"  r="7"/>  <circle class="np0" cx="100" cy="50"  r="3.5" fill="#1e88e5"/>
  <circle class="node" cx="100" cy="90"  r="7"/>  <circle class="np1" cx="100" cy="90"  r="3.5" fill="#1e88e5"/>
  <circle class="node" cx="100" cy="130" r="7"/>  <circle class="np2" cx="100" cy="130" r="3.5" fill="#1e88e5"/>
  <circle class="node" cx="100" cy="170" r="7"/>  <circle class="np3" cx="100" cy="170" r="3.5" fill="#1e88e5"/>
  <!-- Layer 1 -->
  <circle class="node" cx="280" cy="60"  r="7"/>  <circle class="np4" cx="280" cy="60"  r="3.5" fill="#1e88e5"/>
  <circle class="node" cx="280" cy="100" r="7"/>  <circle class="np5" cx="280" cy="100" r="3.5" fill="#1e88e5"/>
  <circle class="node" cx="280" cy="140" r="7"/>  <circle class="np6" cx="280" cy="140" r="3.5" fill="#1e88e5"/>
  <!-- Layer 2 -->
  <circle class="node" cx="460" cy="55"  r="7"/>  <circle class="np7" cx="460" cy="55"  r="3.5" fill="#1e88e5"/>
  <circle class="node" cx="460" cy="95"  r="7"/>  <circle class="np8" cx="460" cy="95"  r="3.5" fill="#1e88e5"/>
  <circle class="node" cx="460" cy="135" r="7"/>  <circle class="np9" cx="460" cy="135" r="3.5" fill="#1e88e5"/>
  <circle class="node" cx="460" cy="175" r="7"/>  <circle class="np0" cx="460" cy="175" r="3.5" fill="#1e88e5"/>
  <!-- Layer 3 -->
  <circle class="node" cx="640" cy="65"  r="7"/>  <circle class="np1" cx="640" cy="65"  r="3.5" fill="#1e88e5"/>
  <circle class="node" cx="640" cy="105" r="7"/>  <circle class="np2" cx="640" cy="105" r="3.5" fill="#1e88e5"/>
  <circle class="node" cx="640" cy="145" r="7"/>  <circle class="np3" cx="640" cy="145" r="3.5" fill="#1e88e5"/>
  <!-- Layer 4 (output) — slightly larger, accent colour -->
  <circle class="node" cx="780" cy="85"  r="9" stroke="#58c4ff"/>  <circle class="np4" cx="780" cy="85"  r="4.5" fill="#58c4ff"/>
  <circle class="node" cx="780" cy="125" r="9" stroke="#58c4ff"/>  <circle class="np5" cx="780" cy="125" r="4.5" fill="#58c4ff"/>

  <!-- ── TEXT OVERLAY ── -->
  <text x="430" y="198" text-anchor="middle" font-family="'Courier New', monospace" font-size="11" fill="#1e4d6b" letter-spacing="4">INPUT · REASON · INTERPRET · OUTPUT</text>
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
