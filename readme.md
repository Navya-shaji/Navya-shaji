<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Navya C S — MERN Developer</title>
<link href="https://fonts.googleapis.com/css2?family=DM+Mono:wght@400;500&family=DM+Sans:wght@300;400;500;600&display=swap" rel="stylesheet"/>
<style>
  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

  :root {
    --bg: #F5F3EE;
    --ink: #1A1A1A;
    --muted: #7A7570;
    --accent: #2563EB;
    --line: #DDD9D3;
    --card: #FFFFFF;
  }

  body {
    font-family: 'DM Sans', sans-serif;
    background: var(--bg);
    color: var(--ink);
    min-height: 100vh;
    padding: 48px 24px;
  }

  .wrap {
    max-width: 680px;
    margin: 0 auto;
  }

  /* Header */
  .header {
    border-bottom: 1px solid var(--line);
    padding-bottom: 32px;
    margin-bottom: 40px;
    display: flex;
    justify-content: space-between;
    align-items: flex-end;
    gap: 24px;
    flex-wrap: wrap;
  }

  .name {
    font-size: 28px;
    font-weight: 600;
    letter-spacing: -0.5px;
    line-height: 1.1;
  }

  .title {
    font-family: 'DM Mono', monospace;
    font-size: 13px;
    color: var(--accent);
    margin-top: 6px;
    letter-spacing: 0.02em;
  }

  .location {
    font-size: 13px;
    color: var(--muted);
    margin-top: 4px;
  }

  .links {
    display: flex;
    gap: 10px;
    flex-wrap: wrap;
  }

  .link-btn {
    font-family: 'DM Mono', monospace;
    font-size: 11px;
    padding: 6px 12px;
    border-radius: 4px;
    text-decoration: none;
    border: 1px solid var(--line);
    color: var(--ink);
    background: var(--card);
    transition: border-color 0.15s, color 0.15s;
    letter-spacing: 0.03em;
  }

  .link-btn:hover { border-color: var(--accent); color: var(--accent); }

  /* Section */
  .section { margin-bottom: 40px; }

  .section-label {
    font-family: 'DM Mono', monospace;
    font-size: 11px;
    color: var(--muted);
    letter-spacing: 0.1em;
    text-transform: uppercase;
    margin-bottom: 16px;
  }

  /* About */
  .about-text {
    font-size: 15px;
    line-height: 1.75;
    color: #3A3A3A;
  }

  /* Stack */
  .stack-row {
    display: flex;
    gap: 8px;
    flex-wrap: wrap;
    margin-bottom: 8px;
    align-items: center;
  }

  .stack-cat {
    font-size: 12px;
    color: var(--muted);
    width: 72px;
    flex-shrink: 0;
  }

  .tag {
    font-family: 'DM Mono', monospace;
    font-size: 12px;
    background: var(--card);
    border: 1px solid var(--line);
    border-radius: 3px;
    padding: 3px 9px;
    color: var(--ink);
  }

  /* Stats */
  .stats-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 12px;
  }

  .stat-card {
    background: var(--card);
    border: 1px solid var(--line);
    border-radius: 8px;
    padding: 18px 16px;
    text-align: center;
  }

  .stat-num {
    font-family: 'DM Mono', monospace;
    font-size: 22px;
    font-weight: 500;
    color: var(--accent);
    line-height: 1;
  }

  .stat-lbl {
    font-size: 12px;
    color: var(--muted);
    margin-top: 5px;
  }

  /* Focus */
  .focus-list {
    display: flex;
    flex-direction: column;
    gap: 10px;
  }

  .focus-item {
    display: flex;
    align-items: center;
    gap: 12px;
    font-size: 14px;
    color: #3A3A3A;
  }

  .focus-dot {
    width: 6px;
    height: 6px;
    border-radius: 50%;
    background: var(--accent);
    flex-shrink: 0;
  }

  /* Footer */
  .footer {
    border-top: 1px solid var(--line);
    padding-top: 24px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: gap;
    gap: 12px;
  }

  .footer-note {
    font-family: 'DM Mono', monospace;
    font-size: 11px;
    color: var(--muted);
  }

  .portfolio-link {
    font-family: 'DM Mono', monospace;
    font-size: 11px;
    color: var(--accent);
    text-decoration: none;
    letter-spacing: 0.03em;
  }

  .portfolio-link:hover { text-decoration: underline; }

  /* Animate in */
  @keyframes fadeUp {
    from { opacity: 0; transform: translateY(12px); }
    to   { opacity: 1; transform: translateY(0); }
  }

  .wrap > * {
    animation: fadeUp 0.4s ease both;
  }

  .wrap > *:nth-child(1) { animation-delay: 0s; }
  .wrap > *:nth-child(2) { animation-delay: 0.07s; }
  .wrap > *:nth-child(3) { animation-delay: 0.14s; }
  .wrap > *:nth-child(4) { animation-delay: 0.21s; }
  .wrap > *:nth-child(5) { animation-delay: 0.28s; }
  .wrap > *:nth-child(6) { animation-delay: 0.35s; }
</style>
</head>
<body>
<div class="wrap">

  <!-- Header -->
  <header class="header">
    <div>
      <div class="name">Navya C S</div>
      <div class="title">Full MERN Stack Developer</div>
      <div class="location">Kochi, Kerala, India</div>
    </div>
    <nav class="links">
      <a class="link-btn" href="https://github.com/Navya-shaji" target="_blank">GitHub</a>
      <a class="link-btn" href="https://www.linkedin.com/in/navya-shaji-b3b81b325" target="_blank">LinkedIn</a>
      <a class="link-btn" href="https://leetcode.com/u/Navyacs/" target="_blank">LeetCode</a>
      <a class="link-btn" href="mailto:navyacs122511@gmail.com">Email</a>
    </nav>
  </header>

  <!-- About -->
  <section class="section">
    <div class="section-label">About</div>
    <p class="about-text">
      Mathematics graduate turned full-stack developer, building production-ready MERN applications with clean architecture. I blend mathematical logic with creative problem-solving — from system design to pixel-perfect UIs.
    </p>
  </section>

  <!-- Stack -->
  <section class="section">
    <div class="section-label">Tech Stack</div>
    <div class="stack-row">
      <span class="stack-cat">Frontend</span>
      <span class="tag">React</span>
      <span class="tag">TypeScript</span>
      <span class="tag">Tailwind CSS</span>
    </div>
    <div class="stack-row">
      <span class="stack-cat">Backend</span>
      <span class="tag">Node.js</span>
      <span class="tag">Express.js</span>
      <span class="tag">MongoDB</span>
    </div>
    <div class="stack-row">
      <span class="stack-cat">Tools</span>
      <span class="tag">Git</span>
      <span class="tag">Postman</span>
      <span class="tag">Vercel</span>
      <span class="tag">Figma</span>
    </div>
  </section>

  <!-- Stats -->
  <section class="section">
    <div class="section-label">LeetCode</div>
    <div class="stats-grid">
      <div class="stat-card">
        <div class="stat-num">365</div>
        <div class="stat-lbl">Day Streak</div>
      </div>
      <div class="stat-card">
        <div class="stat-num">200+</div>
        <div class="stat-lbl">Days Badge</div>
      </div>
      <div class="stat-card">
        <div class="stat-num">100+</div>
        <div class="stat-lbl">Problems</div>
      </div>
    </div>
  </section>

  <!-- Currently -->
  <section class="section">
    <div class="section-label">Currently</div>
    <div class="focus-list">
      <div class="focus-item"><div class="focus-dot"></div>Advanced Data Structures & Algorithms</div>
      <div class="focus-item"><div class="focus-dot"></div>System Design for scalable MERN apps</div>
      <div class="focus-item"><div class="focus-dot"></div>Clean Architecture & performance optimization</div>
    </div>
  </section>

  <!-- Footer -->
  <footer class="footer">
    <span class="footer-note">navyacs122511@gmail.com</span>
    <a class="portfolio-link" href="https://navya-one.vercel.app/" target="_blank">navya-one.vercel.app →</a>
  </footer>

</div>
</body>
</html>
