<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>MD JAMSHED SIFAT · Premium Red</title>
  <!-- Font Awesome (icons) -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      background: #0b0a0c;
      font-family: 'Inter', 'Segoe UI', system-ui, -apple-system, sans-serif;
      display: flex;
      justify-content: center;
      padding: 2rem 1rem;
      color: #f0ece9;
    }

    .premium-card {
      max-width: 1100px;
      width: 100%;
      background: radial-gradient(circle at 10% 20%, #1a1014, #0d080a);
      border-radius: 3.5rem;
      padding: 2rem 2.5rem 2.5rem;
      box-shadow: 0 25px 50px -8px rgba(200, 0, 0, 0.3), 0 0 0 1px rgba(200, 30, 30, 0.2);
      backdrop-filter: blur(2px);
      transition: all 0.2s ease;
      border: 1px solid rgba(200, 20, 20, 0.25);
    }

    /* ----- red bold accents ----- */
    .red-glow {
      color: #ff1a1a;
      font-weight: 800;
      text-shadow: 0 0 12px rgba(255, 20, 20, 0.7);
    }

    .red-border-bottom {
      border-bottom: 3px solid #d91a1a;
      padding-bottom: 0.3rem;
      display: inline-block;
    }

    .badge-red {
      background: #b01010;
      color: white;
      font-weight: 700;
      padding: 0.2rem 1rem;
      border-radius: 40px;
      letter-spacing: 0.3px;
      box-shadow: 0 0 15px #b01010aa;
    }

    .section-title {
      font-size: 1.8rem;
      font-weight: 700;
      letter-spacing: -0.02em;
      display: flex;
      align-items: center;
      gap: 0.6rem;
      color: #f2e8e4;
    }
    .section-title i {
      color: #e31b1b;
      font-size: 1.8rem;
      filter: drop-shadow(0 0 6px #ff2a2a);
    }

    hr {
      margin: 2rem 0 1.5rem;
      border: 0;
      height: 2px;
      background: linear-gradient(90deg, #b01010, #4a1010, #b01010);
      opacity: 0.6;
    }

    /* header wave + avatar */
    .header-wave {
      position: relative;
      margin-top: -1rem;
    }

    .avatar-ring {
      display: inline-block;
      background: #1f1215;
      padding: 0.4rem;
      border-radius: 999px;
      border: 2px solid #d91a1a;
      box-shadow: 0 0 30px #b0101088;
    }

    .avatar-ring img {
      width: 90px;
      height: 90px;
      border-radius: 999px;
      object-fit: cover;
      background: #1e1316;
      display: block;
    }

    .name-title {
      font-size: 3.2rem;
      font-weight: 800;
      background: linear-gradient(135deg, #ffd9d9, #ffb3b3);
      -webkit-background-clip: text;
      background-clip: text;
      color: transparent;
      letter-spacing: -0.02em;
      text-shadow: 0 0 20px #ff222266;
    }

    .subhead {
      color: #d4c9c9;
      font-weight: 400;
      letter-spacing: 0.3px;
      border-left: 4px solid #e31b1b;
      padding-left: 1rem;
      background: linear-gradient(90deg, #2f1515, transparent);
    }

    .typing-wrapper {
      background: #1b1012;
      padding: 0.8rem 1.5rem;
      border-radius: 60px;
      display: inline-block;
      border: 1px solid #b0101066;
      box-shadow: 0 0 25px #b0101044;
    }

    /* tech icons */
    .tech-pill {
      background: #1c1114;
      border-radius: 60px;
      padding: 0.4rem 1.2rem;
      border: 1px solid #b0101070;
      font-weight: 500;
      color: #f0e0e0;
      display: inline-flex;
      align-items: center;
      gap: 8px;
      backdrop-filter: blur(4px);
    }

    .tech-pill i {
      color: #ff3a3a;
      font-size: 1.1rem;
    }

    /* table cards */
    .project-card {
      background: #130c0e;
      border-radius: 2rem;
      padding: 1.6rem 1.5rem;
      border-left: 8px solid #b01010;
      box-shadow: 0 10px 25px -8px #00000088;
      transition: 0.15s ease;
      height: 100%;
      border: 1px solid #3a1818;
    }

    .project-card:hover {
      border-left-width: 10px;
      border-color: #ff2a2a;
      box-shadow: 0 0 30px #b0101066;
      transform: translateY(-3px);
    }

    .project-card .tech-tag {
      background: #201316;
      border-radius: 30px;
      padding: 0.2rem 0.9rem;
      font-size: 0.75rem;
      font-weight: 600;
      color: #ffbaba;
      border: 1px solid #b0101080;
      display: inline-block;
    }

    .engineering-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
      gap: 0.8rem 1.2rem;
      background: #120b0d;
      padding: 1.5rem;
      border-radius: 2.5rem;
      border: 1px solid #3d1818;
    }

    .engineering-item {
      font-weight: 500;
      border-bottom: 1px dashed #642222;
      padding: 0.4rem 0;
      display: flex;
      align-items: center;
      gap: 0.5rem;
    }
    .engineering-item i {
      color: #ff3a3a;
      width: 1.6rem;
      font-size: 1.2rem;
    }

    .focus-bar {
      background: #1e1215;
      border-radius: 50px;
      padding: 0.2rem 0.2rem 0.2rem 1rem;
      border: 1px solid #b0101060;
      display: flex;
      align-items: center;
      justify-content: space-between;
      flex-wrap: wrap;
    }

    .focus-bar .label {
      font-weight: 600;
      color: #f0d6d6;
    }
    .focus-bar .bar-track {
      background: #2a1a1a;
      height: 10px;
      width: 140px;
      border-radius: 30px;
      overflow: hidden;
      margin: 0 0.5rem;
    }
    .focus-bar .bar-fill {
      height: 100%;
      background: linear-gradient(90deg, #b01010, #ff3a3a);
      border-radius: 30px;
      box-shadow: 0 0 15px #ff1a1a;
    }

    .game-section {
      background: #140a0c;
      border-radius: 2.5rem;
      padding: 1.5rem 2rem;
      border: 1px solid #b0101060;
      box-shadow: inset 0 0 40px #b0101020;
    }

    .game-btn {
      background: #b01010;
      border: none;
      color: white;
      font-weight: 700;
      padding: 0.6rem 1.8rem;
      border-radius: 60px;
      font-size: 1rem;
      cursor: pointer;
      transition: all 0.15s;
      box-shadow: 0 0 20px #b01010aa;
      border: 1px solid #ff5a5a;
    }
    .game-btn:hover {
      background: #d91a1a;
      transform: scale(1.02);
      box-shadow: 0 0 35px #ff2a2a;
    }

    .game-result {
      font-size: 1.5rem;
      font-weight: 700;
      color: #ffd0d0;
    }

    /* footer */
    .footer-wave {
      margin-top: 1rem;
      background: linear-gradient(90deg, #b01010, #1f0f0f, #b01010);
      height: 4px;
      width: 100%;
      border-radius: 10px;
      opacity: 0.5;
    }

    @media (max-width: 640px) {
      .premium-card { padding: 1.5rem; }
      .name-title { font-size: 2.2rem; }
      .section-title { font-size: 1.4rem; }
      .focus-bar { flex-direction: column; align-items: flex-start; gap: 6px; }
    }
  </style>
</head>
<body>
<div class="premium-card">

  <!-- header -->
  <div class="header-wave" align="center">
    <div style="display: flex; flex-wrap: wrap; align-items: center; justify-content: center; gap: 1rem 2rem;">
      <div class="avatar-ring">
        <img src="https://avatars.githubusercontent.com/u/149657269?s=400&v=4" alt="Jamshed Sifat" />
      </div>
      <div style="text-align: left;">
        <div class="name-title">MD JAMSHED SIFAT</div>
        <div style="display: flex; flex-wrap: wrap; gap: 0.5rem 0.8rem; margin-top: 0.2rem;">
          <span class="badge-red"><i class="fas fa-code"></i> Software Dev</span>
          <span class="badge-red" style="background: #7a0f0f;"><i class="fas fa-robot"></i> Robotics</span>
          <span class="badge-red" style="background: #8f1212;"><i class="fas fa-microchip"></i> IoT</span>
        </div>
      </div>
    </div>

    <div style="margin: 1rem 0 0.5rem;">
      <div class="typing-wrapper">
        <i class="fas fa-terminal" style="color:#ff3a3a; margin-right: 0.5rem;"></i>
        <span style="color:#f0e0e0; font-weight: 400; letter-spacing: 0.3px;">Building software · Exploring intelligence · Engineering ideas</span>
      </div>
    </div>

    <div style="display: flex; flex-wrap: wrap; justify-content: center; gap: 0.4rem 1rem; margin-top: 0.5rem;">
      <span class="tech-pill"><i class="fab fa-react"></i> React</span>
      <span class="tech-pill"><i class="fab fa-python"></i> Python</span>
      <span class="tech-pill"><i class="fab fa-js"></i> TS/JS</span>
      <span class="tech-pill"><i class="fas fa-microchip"></i> ESP32</span>
      <span class="tech-pill"><i class="fas fa-brain"></i> AI</span>
    </div>
  </div>

  <!-- about -->
  <div style="margin: 2rem 0 0.5rem;">
    <div class="section-title"><i class="fas fa-user-astronaut"></i> <span class="red-border-bottom">About</span></div>
    <div style="background: #160d0f; border-radius: 2rem; padding: 1.2rem 1.8rem; border: 1px solid #4a1a1a; margin-top: 0.6rem;">
      <p style="font-size: 1.1rem; line-height: 1.6; color: #e6dada;">
        <span class="red-glow">CSE student</span> & developer. I craft modern full‑stack applications, 
        embed intelligence into hardware, and bridge the gap between <span class="red-glow">software</span> and <span class="red-glow">physical systems</span>.
        Passionate about AI, IoT, and robotics.
      </p>
    </div>
  </div>

  <!-- tech arsenal -->
  <div style="margin: 1.8rem 0;">
    <div class="section-title"><i class="fas fa-tools"></i> <span class="red-border-bottom">Tech Arsenal</span></div>
    <div style="display: flex; flex-wrap: wrap; gap: 0.4rem 0.8rem; margin-top: 0.8rem; justify-content: center;">
      <span class="tech-pill"><i class="fab fa-python"></i> Python</span>
      <span class="tech-pill"><i class="fab fa-js"></i> JavaScript</span>
      <span class="tech-pill"><i class="fab fa-typescript"></i> TypeScript</span>
      <span class="tech-pill"><i class="fab fa-react"></i> React</span>
      <span class="tech-pill"><i class="fab fa-node"></i> Node.js</span>
      <span class="tech-pill"><i class="fas fa-database"></i> MongoDB</span>
      <span class="tech-pill"><i class="fas fa-database"></i> MySQL</span>
      <span class="tech-pill"><i class="fab fa-git-alt"></i> Git</span>
      <span class="tech-pill"><i class="fas fa-microchip"></i> Arduino</span>
      <span class="tech-pill"><i class="fas fa-wifi"></i> ESP32</span>
      <span class="tech-pill"><i class="fas fa-robot"></i> Robotics</span>
    </div>
  </div>

  <!-- featured work (cards) -->
  <div>
    <div class="section-title"><i class="fas fa-star"></i> <span class="red-border-bottom">Featured Work</span></div>
    <div style="display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 1.2rem; margin-top: 1rem;">
      <div class="project-card">
        <div style="display: flex; justify-content: space-between;"><span style="font-weight: 700; font-size: 1.2rem;">🏥 SmartHealthCare</span> <span class="tech-tag">Django</span></div>
        <div style="margin: 0.3rem 0 0.6rem; color: #c9b7b7;">Appointment · Reminders · Diet</div>
        <div><span class="tech-tag">Python</span> <span class="tech-tag">JS</span></div>
      </div>
      <div class="project-card">
        <div style="display: flex; justify-content: space-between;"><span style="font-weight: 700; font-size: 1.2rem;">🛒 SportNest</span> <span class="tech-tag">Django</span></div>
        <div style="margin: 0.3rem 0 0.6rem; color: #c9b7b7;">E‑commerce · Product mgmt</div>
        <div><span class="tech-tag">Python</span> <span class="tech-tag">JS</span></div>
      </div>
      <div class="project-card">
        <div style="display: flex; justify-content: space-between;"><span style="font-weight: 700; font-size: 1.2rem;">🌱 Plant Shop</span> <span class="tech-tag">React</span></div>
        <div style="margin: 0.3rem 0 0.6rem; color: #c9b7b7;">API‑driven · Responsive</div>
        <div><span class="tech-tag">Tailwind</span> <span class="tech-tag">API</span></div>
      </div>
      <div class="project-card">
        <div style="display: flex; justify-content: space-between;"><span style="font-weight: 700; font-size: 1.2rem;">🤖 Robotics Lab</span> <span class="tech-tag">ESP32</span></div>
        <div style="margin: 0.3rem 0 0.6rem; color: #c9b7b7;">Sensors · Motors · Control</div>
        <div><span class="tech-tag">Arduino</span> <span class="tech-tag">IoT</span></div>
      </div>
    </div>
  </div>

  <!-- engineering projects + game -->
  <hr>
  <div style="display: grid; grid-template-columns: 1fr 1fr; gap: 1.5rem; margin: 0.5rem 0;">
    <div>
      <div class="section-title" style="font-size:1.5rem;"><i class="fas fa-microchip"></i> <span class="red-border-bottom">Robotics</span></div>
      <div class="engineering-grid">
        <div class="engineering-item"><i class="fas fa-fire"></i> Fire Fighting Robot</div>
        <div class="engineering-item"><i class="fas fa-route"></i> Obstacle Avoid / Maze</div>
        <div class="engineering-item"><i class="fas fa-balance-scale"></i> Self‑Balancing (PID)</div>
        <div class="engineering-item"><i class="fas fa-traffic-light"></i> Traffic Light System</div>
        <div class="engineering-item"><i class="fas fa-ruler"></i> Ultrasonic Sensor</div>
      </div>
    </div>
    <!-- GAME : REDMI premium + bold red -->
    <div class="game-section">
      <div style="display: flex; align-items: center; gap: 0.8rem; flex-wrap: wrap;">
        <i class="fas fa-gamepad" style="color:#ff2a2a; font-size: 2rem;"></i>
        <span style="font-weight: 700; font-size: 1.5rem; color:#f0d6d6;">🎮 <span class="red-glow">REDMI</span> BOLD</span>
        <span style="background:#b01010; padding:0.1rem 1rem; border-radius:30px; font-weight:600; font-size:0.9rem;">premium</span>
      </div>
      <div style="display: flex; flex-wrap: wrap; align-items: center; gap: 1rem 1.5rem; margin-top: 1rem;">
        <button class="game-btn" id="rollDiceBtn"><i class="fas fa-dice"></i> ROLL FOR RED</button>
        <span class="game-result" id="gameResult">⚡</span>
      </div>
      <div style="margin-top: 0.6rem; color:#b17c7c; font-size:0.9rem; border-top:1px solid #5a1a1a; padding-top:0.6rem;">
        <i class="fas fa-bolt red-glow"></i> every roll glows bold red
      </div>
    </div>
  </div>

  <!-- focus -->
  <div style="margin: 1.8rem 0 0.8rem;">
    <div class="section-title"><i class="fas fa-bullseye"></i> <span class="red-border-bottom">Current Focus</span></div>
    <div style="display: flex; flex-direction: column; gap: 0.7rem; margin-top: 0.6rem;">
      <div class="focus-bar"><span class="label"><i class="fas fa-code"></i> Software Eng</span><div class="bar-track"><div class="bar-fill" style="width:90%"></div></div><span style="color:#d4b0b0; font-weight:600;">90%</span></div>
      <div class="focus-bar"><span class="label"><i class="fab fa-react"></i> React + TS</span><div class="bar-track"><div class="bar-fill" style="width:85%"></div></div><span style="color:#d4b0b0; font-weight:600;">85%</span></div>
      <div class="focus-bar"><span class="label"><i class="fab fa-python"></i> Django</span><div class="bar-track"><div class="bar-fill" style="width:78%"></div></div><span style="color:#d4b0b0; font-weight:600;">78%</span></div>
      <div class="focus-bar"><span class="label"><i class="fas fa-robot"></i> IoT / Robotics</span><div class="bar-track"><div class="bar-fill" style="width:70%"></div></div><span style="color:#d4b0b0; font-weight:600;">70%</span></div>
    </div>
  </div>

  <!-- philosophy + connect -->
  <hr>
  <div style="display: flex; flex-wrap: wrap; justify-content: space-between; align-items: center; gap: 1rem;">
    <div style="font-size: 1.15rem; background:#1c1114; padding:0.6rem 1.8rem; border-radius:60px; border:1px solid #b0101080;">
      <i class="fas fa-quote-left red-glow"></i> Build with purpose. Learn. Improve. <i class="fas fa-quote-right red-glow"></i>
    </div>
    <div>
      <a href="https://github.com/JamshedSifat" target="_blank" style="text-decoration:none; background:#b01010; color:white; padding:0.6rem 1.8rem; border-radius:60px; font-weight:700; display:inline-flex; align-items:center; gap:10px; border:1px solid #ff5a5a; box-shadow:0 0 25px #b01010aa;">
        <i class="fab fa-github"></i> GitHub
      </a>
    </div>
  </div>

  <!-- footer wave -->
  <div class="footer-wave"></div>
  <div align="center" style="margin-top:0.8rem; color:#9f7a7a; font-weight:400; letter-spacing:0.5px;">
    <i class="fas fa-heart red-glow"></i> MD JAMSHED SIFAT · premium red edition
  </div>
</div>

<script>
  (function() {
    const btn = document.getElementById('rollDiceBtn');
    const resultSpan = document.getElementById('gameResult');

    const redPhrases = [
      '🔥 REDMI ROYAL', '❤️ BOLD CRIMSON', '⚡ SCARLET POWER', 
      '♦️ RUBY STRIKE', '🔴 PREMIUM RED', '🟥 DEEP BLOOD'
    ];

    btn.addEventListener('click', function() {
      // dice random 1-6
      const roll = Math.floor(Math.random() * 6) + 1;
      const phrase = redPhrases[Math.floor(Math.random() * redPhrases.length)];
      // bold red effect
      resultSpan.innerHTML = `${roll} · ${phrase}`;
      resultSpan.style.color = '#ff1a1a';
      resultSpan.style.textShadow = '0 0 30px #ff3a3a';
      // extra pulse
      btn.style.transform = 'scale(0.95)';
      setTimeout(() => btn.style.transform = 'scale(1)', 100);
      // glow
      resultSpan.style.transition = '0.2s';
    });
  })();
</script>

</body>
</html>
