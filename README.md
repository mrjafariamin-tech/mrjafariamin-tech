<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Amin's · GitHub Profile</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      background-color: #0d1117;
      font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Noto Sans', Helvetica, Arial, sans-serif;
      color: #e6edf3;
      line-height: 1.5;
      padding: 2rem 1rem;
    }

    .container {
      max-width: 1100px;
      margin: 0 auto;
      background-color: #010409;
      border-radius: 24px;
      padding: 2rem 2rem 3rem;
      box-shadow: 0 8px 24px rgba(0,0,0,0.3);
    }

    /* header row */
    .profile-header {
      display: flex;
      justify-content: space-between;
      align-items: flex-start;
      flex-wrap: wrap;
      margin-bottom: 1.5rem;
      border-bottom: 1px solid #30363d;
      padding-bottom: 1.5rem;
    }

    .title h1 {
      font-size: 2rem;
      font-weight: 600;
      letter-spacing: -0.5px;
    }

    .title p {
      font-size: 1.1rem;
      color: #7d8590;
      margin-top: 0.25rem;
    }

    .edit-badge {
      background-color: #21262d;
      padding: 0.2rem 0.7rem;
      border-radius: 24px;
      font-size: 0.75rem;
      color: #c9d1d9;
      border: 1px solid #30363d;
    }

    /* stats row (followers/following) */
    .stats-row {
      display: flex;
      gap: 1.2rem;
      margin: 1rem 0 1.2rem;
      flex-wrap: wrap;
    }

    .stat-item {
      background: #161b22;
      padding: 0.3rem 0.9rem;
      border-radius: 32px;
      font-size: 0.85rem;
      border: 1px solid #30363d;
    }

    .stat-item strong {
      font-weight: 600;
      margin-right: 0.2rem;
    }

    .location {
      display: flex;
      align-items: center;
      gap: 0.5rem;
      color: #7d8590;
      margin: 0.5rem 0 1rem;
      font-size: 0.9rem;
    }

    .welcome {
      text-align: center;
      font-size: 1.6rem;
      font-weight: 500;
      margin: 2rem 0 1.8rem;
      background: linear-gradient(135deg, #58a6ff, #f0883e);
      background-clip: text;
      -webkit-background-clip: text;
      color: transparent;
    }

    /* section headings */
    .section-title {
      font-size: 1.5rem;
      font-weight: 600;
      margin: 2rem 0 1rem 0;
      border-left: 4px solid #f78166;
      padding-left: 0.8rem;
    }

    .about-text {
      background: #161b22;
      padding: 1.2rem;
      border-radius: 16px;
      border: 1px solid #30363d;
      margin-bottom: 1rem;
    }

    /* tech badges */
    .tech-grid {
      display: flex;
      flex-wrap: wrap;
      gap: 0.7rem;
      margin: 1rem 0 0.5rem;
    }

    .badge {
      background-color: #21262d;
      padding: 0.3rem 0.9rem;
      border-radius: 32px;
      font-size: 0.8rem;
      font-weight: 500;
      color: #e6edf3;
      border: 1px solid #30363d;
      transition: 0.1s ease;
    }

    .badge:hover {
      background-color: #2d333b;
      border-color: #8b949e;
    }

    /* statistics cards */
    .stats-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
      gap: 1rem;
      margin: 1rem 0 1rem;
    }

    .stat-card {
      background: #161b22;
      border: 1px solid #30363d;
      border-radius: 16px;
      padding: 1rem;
      text-align: center;
    }

    .stat-number {
      font-size: 2.2rem;
      font-weight: 700;
      color: #58a6ff;
    }

    .stat-label {
      font-size: 0.75rem;
      text-transform: uppercase;
      letter-spacing: 0.5px;
      color: #7d8590;
    }

    /* contribution & streak */
    .streak-box {
      background: #161b22;
      border-radius: 16px;
      padding: 1rem;
      margin: 1rem 0;
      display: flex;
      flex-wrap: wrap;
      justify-content: space-between;
      gap: 1rem;
      border: 1px solid #30363d;
    }

    .streak-item {
      flex: 1;
      text-align: center;
    }

    .streak-value {
      font-size: 1.8rem;
      font-weight: 700;
    }

    /* mock contribution graph (bars) */
    .graph-container {
      background: #161b22;
      border-radius: 16px;
      padding: 1.2rem;
      margin: 1rem 0;
      border: 1px solid #30363d;
    }

    .graph-bars {
      display: flex;
      align-items: flex-end;
      gap: 6px;
      height: 120px;
      margin-top: 0.8rem;
    }

    .bar {
      flex: 1;
      background-color: #2f81f7;
      min-width: 6px;
      border-radius: 4px 4px 0 0;
      transition: 0.1s;
    }

    .bar:hover {
      background-color: #58a6ff;
    }

    .x-axis {
      display: flex;
      justify-content: space-around;
      margin-top: 8px;
      font-size: 0.7rem;
      color: #7d8590;
    }

    .axis-label {
      text-align: center;
      margin-top: 1rem;
      font-size: 0.75rem;
      color: #8b949e;
    }

    hr {
      border-color: #30363d;
      margin: 1.5rem 0;
    }

    footer {
      text-align: center;
      margin-top: 2.5rem;
      font-size: 0.75rem;
      color: #7d8590;
    }

    @media (max-width: 700px) {
      .container {
        padding: 1.5rem;
      }
      .streak-box {
        flex-direction: column;
      }
    }
  </style>
</head>
<body>
<div class="container">
  <!-- header -->
  <div class="profile-header">
    <div class="title">
      <h1>Amin</h1>
      <p>Full-Stack Web Developer</p>
    </div>
    <div class="edit-badge">✎ Edit profile</div>
  </div>

  <!-- followers/following (static demo – replace with your actual numbers) -->
  <div class="stats-row">
    <div class="stat-item"><strong>6</strong> followers</div>
    <div class="stat-item"><strong>15</strong> following</div>
  </div>

  <div class="location">
    <span>📍</span> San Jose / Costa Rica
    <span style="margin-left: 0.5rem;">📧</span> none
  </div>

  <!-- achievements placeholder (like a mini section) -->
  <div class="section-title">🏆 Achievements</div>
  <div class="tech-grid" style="margin-top: -0.5rem;">
    <div class="badge">🥇 ICPC Regional 2025</div>
    <div class="badge">📘 200+ Codeforces</div>
    <div class="badge">🚀 First PR merged</div>
  </div>

  <!-- welcome banner -->
  <div class="welcome"># Welcome to Benjamin's Github</div>

  <!-- about me -->
  <div class="section-title">👤 About me</div>
  <div class="about-text">
    Hello! I'm Amin, a Systems Engineer student. I enjoy learning new technologies and problem solving at Codeforces and Codechef. Now I'm working on some little and fun projects to put in practice my knowledge about JavaScript, React, Bootstrap and more.
  </div>

  <!-- technologies -->
  <div class="section-title">🛠️ Technologies</div>
  <div class="tech-grid">
    <span class="badge">C++</span> <span class="badge">JAVA</span>
    <span class="badge">PYTHON</span> <span class="badge">JAVASCRIPT</span>
    <span class="badge">HTML</span> <span class="badge">CSS</span>
    <span class="badge">REACT</span> <span class="badge">BOOTSTRAP</span>
    <span class="badge">GIT</span> <span class="badge">GITBASH</span>
    <span class="badge">NODE.JS</span> <span class="badge">JEST</span>
    <span class="badge">POSTGRESQL</span> <span class="badge">MYSQL</span>
  </div>

  <!-- statistics section (matching the image numbers) -->
  <div class="section-title">📊 Statistics</div>
  <div class="stats-grid">
    <div class="stat-card"><div class="stat-number">1</div><div class="stat-label">Total Stars Earned</div></div>
    <div class="stat-card"><div class="stat-number">67</div><div class="stat-label">Total Commits (2025)</div></div>
    <div class="stat-card"><div class="stat-number">0</div><div class="stat-label">Total PR</div></div>
    <div class="stat-card"><div class="stat-number">0</div><div class="stat-label">Total Issues</div></div>
    <div class="stat-card"><div class="stat-number">0</div><div class="stat-label">Contributed (last year)</div></div>
  </div>

  <!-- contributions & streak -->
  <div class="section-title">🔥 Contributions & Streak</div>
  <div class="streak-box">
    <div class="streak-item"><div class="streak-value">119</div><div class="stat-label">Total (2025)</div></div>
    <div class="streak-item"><div class="streak-value">7</div><div class="stat-label">Contributed</div></div>
    <div class="streak-item"><div class="streak-value">7 days</div><div class="stat-label">Longest Streak</div></div>
  </div>
  <div style="margin-top: -0.5rem; font-size: 0.8rem; color:#8b949e; text-align: center;">
    ⏱️ Start: Sep 21, 2023 – End: Sep 15, 2023
  </div>

  <!-- contribution graph (mock) -->
  <div class="section-title">📈 Amin's Contribution Graph</div>
  <div class="graph-container">
    <div class="graph-bars" id="contributionBars"></div>
    <div class="x-axis">
      <span>Mon</span> <span>Tue</span> <span>Wed</span> <span>Thu</span> <span>Fri</span> <span>Sat</span> <span>Sun</span>
    </div>
    <div class="axis-label">X‑axis: Days &nbsp;&nbsp;|&nbsp;&nbsp; Y‑axis: Contributions</div>
  </div>

  <hr />
  <footer>
    🧑‍💻 Built with HTML & CSS — GitHub Pages ready
  </footer>
</div>

<script>
  // generate random-looking contribution bars (just for visual, matches the mock style)
  const barsContainer = document.getElementById('contributionBars');
  if (barsContainer) {
    const heights = [12, 28, 42, 18, 35, 55, 32, 45, 28, 38, 62, 44, 19, 27, 58, 70, 33, 48, 39, 52, 21, 47, 63, 29, 38, 44, 18, 55, 40, 22];
    for (let i = 0; i < heights.length; i++) {
      const bar = document.createElement('div');
      bar.className = 'bar';
      bar.style.height = heights[i] + 'px';
      bar.title = `${heights[i]} contributions`;
      barsContainer.appendChild(bar);
    }
  }
</script>
</body>
</html>
