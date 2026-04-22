<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Vibhore Sharma – Full Stack Developer</title>
<link href="https://fonts.googleapis.com/css2?family=Rajdhani:wght@600;700&family=Nunito:wght@400;600;700&display=swap" rel="stylesheet"/>
<style>
  :root {
    --bg: #0a0a0a;
    --card-bg: #0f0f0f;
    --pink: #ff2d78;
    --pink-glow: rgba(255,45,120,0.35);
    --pink-dim: rgba(255,45,120,0.18);
    --white: #f0f0f0;
    --grey: #aaaaaa;
    --border: rgba(255,45,120,0.55);
  }

  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }

  body {
    background: var(--bg);
    color: var(--white);
    font-family: 'Nunito', sans-serif;
    min-height: 100vh;
    display: flex;
    justify-content: center;
    padding: 32px 16px 48px;
  }

  .wrapper {
    width: 100%;
    max-width: 860px;
  }

  /* ── TOP HERO ── */
  .hero {
    display: grid;
    grid-template-columns: auto 1fr auto;
    align-items: flex-start;
    gap: 28px;
    margin-bottom: 36px;
  }

  /* Avatar */
  .avatar-wrap {
    position: relative;
    width: 155px;
    height: 155px;
    flex-shrink: 0;
  }
  .avatar-wrap::before {
    content: '';
    position: absolute;
    inset: -5px;
    border-radius: 50%;
    background: conic-gradient(var(--pink) 0%, transparent 40%, var(--pink) 70%, transparent 100%);
    animation: spin 4s linear infinite;
    filter: blur(1px);
  }
  .avatar-wrap::after {
    content: '';
    position: absolute;
    inset: -5px;
    border-radius: 50%;
    border: 3px solid var(--pink);
    box-shadow: 0 0 22px var(--pink-glow), inset 0 0 22px var(--pink-glow);
  }
  @keyframes spin { to { transform: rotate(360deg); } }
  .avatar-img {
    width: 100%;
    height: 100%;
    border-radius: 50%;
    object-fit: cover;
    position: relative;
    z-index: 1;
    background: #1a0a14;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 56px;
    overflow: hidden;
  }
  /* Placeholder person icon */
  .avatar-img svg { width: 80px; height: 80px; opacity: 0.7; }

  /* Name block */
  .identity { padding-top: 6px; }
  .identity h1 {
    font-family: 'Rajdhani', sans-serif;
    font-size: 2rem;
    font-weight: 700;
    letter-spacing: 1px;
    color: #fff;
    line-height: 1.1;
  }
  .identity .title {
    color: var(--pink);
    font-size: 0.82rem;
    font-weight: 700;
    letter-spacing: 3px;
    text-transform: uppercase;
    margin: 6px 0 10px;
  }
  .identity .location {
    display: flex;
    align-items: center;
    gap: 6px;
    color: var(--grey);
    font-size: 0.82rem;
  }
  .identity .location svg { color: var(--pink); }
  .identity .location span.sep { color: var(--border); margin: 0 4px; }

  /* Speech bubble */
  .bubble-wrap {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    padding-top: 4px;
  }
  .speech {
    position: relative;
    background: #130c10;
    border: 1.5px solid var(--pink);
    box-shadow: 0 0 14px var(--pink-glow);
    border-radius: 14px;
    padding: 14px 18px;
    max-width: 260px;
  }
  .speech::after {
    content: '';
    position: absolute;
    bottom: -14px;
    left: 28px;
    border: 7px solid transparent;
    border-top-color: var(--pink);
  }
  .speech::before {
    content: '';
    position: absolute;
    bottom: -11px;
    left: 29px;
    border: 6px solid transparent;
    border-top-color: #130c10;
    z-index: 1;
  }
  .speech h2 { font-size: 0.95rem; font-weight: 700; margin-bottom: 6px; }
  .speech p { font-size: 0.78rem; color: var(--grey); line-height: 1.55; }

  /* Social links */
  .socials {
    display: flex;
    flex-direction: column;
    gap: 10px;
    min-width: 210px;
  }
  .social-btn {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 10px;
    background: #0f0f0f;
    border: 1.5px solid rgba(255,255,255,0.12);
    border-radius: 10px;
    padding: 11px 16px;
    color: var(--white);
    font-size: 0.88rem;
    font-weight: 600;
    cursor: pointer;
    transition: border-color 0.2s, box-shadow 0.2s;
    text-decoration: none;
  }
  .social-btn:hover {
    border-color: var(--pink);
    box-shadow: 0 0 12px var(--pink-glow);
  }
  .social-btn .icon-label { display: flex; align-items: center; gap: 10px; }
  .social-btn .icon-box {
    width: 28px; height: 28px;
    border-radius: 6px;
    background: #1c1c1c;
    display: flex; align-items: center; justify-content: center;
    font-size: 16px;
  }
  .social-btn .chevron { color: var(--grey); font-size: 14px; }

  /* ── DIVIDER ── */
  .divider {
    height: 1px;
    background: linear-gradient(to right, transparent, var(--pink) 30%, var(--pink) 70%, transparent);
    margin-bottom: 28px;
    box-shadow: 0 0 8px var(--pink-glow);
  }

  /* ── CARDS GRID ── */
  .cards {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 18px;
    margin-bottom: 28px;
  }
  .card {
    background: var(--card-bg);
    border: 1.5px solid var(--border);
    border-radius: 14px;
    padding: 22px 24px 26px;
    position: relative;
    overflow: hidden;
    box-shadow: 0 0 18px var(--pink-dim);
    transition: box-shadow 0.25s;
  }
  .card:hover { box-shadow: 0 0 32px var(--pink-glow); }
  /* dot pattern */
  .card::after {
    content: '';
    position: absolute;
    right: 16px; bottom: 16px;
    width: 80px; height: 80px;
    background-image: radial-gradient(circle, rgba(255,45,120,0.25) 1px, transparent 1px);
    background-size: 8px 8px;
    pointer-events: none;
  }
  .card-header {
    display: flex;
    align-items: center;
    gap: 14px;
    margin-bottom: 14px;
  }
  .card-icon {
    width: 48px; height: 48px;
    border: 1.5px solid var(--pink);
    border-radius: 10px;
    display: flex; align-items: center; justify-content: center;
    flex-shrink: 0;
  }
  .card-icon svg { width: 24px; height: 24px; stroke: var(--pink); fill: none; stroke-width: 1.8; }
  .card-header h3 {
    font-family: 'Rajdhani', sans-serif;
    font-size: 1.25rem;
    font-weight: 700;
    letter-spacing: 0.5px;
  }
  .underline {
    width: 30px; height: 2.5px;
    background: var(--pink);
    border-radius: 2px;
    margin: 2px 0 14px;
    box-shadow: 0 0 6px var(--pink);
  }
  .card p {
    color: var(--grey);
    font-size: 0.88rem;
    line-height: 1.7;
  }

  /* ── FOOTER STRIP ── */
  .footer-tagline {
    text-align: center;
    margin-bottom: 22px;
    font-size: 0.9rem;
    font-weight: 700;
    color: var(--pink);
    letter-spacing: 1px;
  }

  .tech-stack {
    display: flex;
    justify-content: center;
    gap: 12px;
    flex-wrap: wrap;
  }
  .tech-icon {
    width: 52px; height: 52px;
    background: #111;
    border: 1.5px solid rgba(255,255,255,0.1);
    border-radius: 12px;
    display: flex; align-items: center; justify-content: center;
    font-size: 26px;
    transition: border-color 0.2s, box-shadow 0.2s;
    cursor: default;
  }
  .tech-icon:hover {
    border-color: var(--pink);
    box-shadow: 0 0 12px var(--pink-glow);
  }

  @media (max-width: 660px) {
    .hero { grid-template-columns: 1fr; grid-template-rows: auto auto auto; }
    .socials { min-width: unset; }
    .cards { grid-template-columns: 1fr; }
    .avatar-wrap { margin: 0 auto; }
  }
</style>
</head>
<body>
<div class="wrapper">

  <!-- HERO -->
  <div class="hero">
    <!-- Avatar -->
    <div>
      <div class="avatar-wrap">
        <div class="avatar-img">
          <svg viewBox="0 0 80 80" fill="none" xmlns="http://www.w3.org/2000/svg">
            <circle cx="40" cy="30" r="16" fill="#ff2d78" opacity="0.7"/>
            <ellipse cx="40" cy="65" rx="24" ry="14" fill="#ff2d78" opacity="0.5"/>
          </svg>
        </div>
      </div>
      <div style="margin-top:14px;">
        <div class="identity">
          <h1>VIBHORE SHARMA</h1>
          <div class="title">Full Stack Developer</div>
          <div class="location">
            <svg width="13" height="13" viewBox="0 0 24 24" fill="var(--pink)" xmlns="http://www.w3.org/2000/svg"><path d="M12 2C8.13 2 5 5.13 5 9c0 5.25 7 13 7 13s7-7.75 7-13c0-3.87-3.13-7-7-7zm0 9.5c-1.38 0-2.5-1.12-2.5-2.5s1.12-2.5 2.5-2.5 2.5 1.12 2.5 2.5-1.12 2.5-2.5 2.5z"/></svg>
            India
            <span class="sep">|</span>
            Available for Opportunities
          </div>
        </div>
      </div>
    </div>

    <!-- Speech bubble -->
    <div class="bubble-wrap" style="padding-top:0; align-self:flex-start;">
      <div class="speech">
        <h2>Hi, I'm Vibhore! 👋</h2>
        <p>I build modern, scalable and user-friendly web applications with clean code and great user experiences.</p>
      </div>
    </div>

    <!-- Social links -->
    <div class="socials">
      <a class="social-btn" href="#">
        <span class="icon-label">
          <span class="icon-box">🐙</span>
          GitHub
        </span>
        <span class="chevron">›</span>
      </a>
      <a class="social-btn" href="#">
        <span class="icon-label">
          <span class="icon-box" style="background:#0a66c2;">🔗</span>
          LinkedIn
        </span>
        <span class="chevron">›</span>
      </a>
      <a class="social-btn" href="#">
        <span class="icon-label">
          <span class="icon-box">🌐</span>
          Portfolio
        </span>
        <span class="chevron">›</span>
      </a>
      <a class="social-btn" href="#">
        <span class="icon-label">
          <span class="icon-box">✉️</span>
          Email Me
        </span>
        <span class="chevron">›</span>
      </a>
    </div>
  </div>

  <!-- DIVIDER -->
  <div class="divider"></div>

  <!-- CARDS -->
  <div class="cards">
    <!-- My Projects -->
    <div class="card">
      <div class="card-header">
        <div class="card-icon">
          <svg viewBox="0 0 24 24"><path d="M22 19a2 2 0 0 1-2 2H4a2 2 0 0 1-2-2V5a2 2 0 0 1 2-2h5l2 3h9a2 2 0 0 1 2 2z"/></svg>
        </div>
        <h3>My Projects</h3>
      </div>
      <div class="underline"></div>
      <p>AI-Powered Resume Builder<br>&amp; E-Commerce Platform</p>
    </div>

    <!-- Tech Focus -->
    <div class="card">
      <div class="card-header">
        <div class="card-icon">
          <svg viewBox="0 0 24 24"><polyline points="16 18 22 12 16 6"/><polyline points="8 6 2 12 8 18"/></svg>
        </div>
        <h3>Tech Focus</h3>
      </div>
      <div class="underline"></div>
      <p>MERN Stack<br>Django &nbsp;|&nbsp; Java DSA</p>
    </div>

    <!-- Experience -->
    <div class="card">
      <div class="card-header">
        <div class="card-icon">
          <svg viewBox="0 0 24 24"><rect x="2" y="7" width="20" height="14" rx="2"/><path d="M16 7V5a2 2 0 0 0-2-2h-4a2 2 0 0 0-2 2v2"/></svg>
        </div>
        <h3>Experience</h3>
      </div>
      <div class="underline"></div>
      <p>Full-Stack Intern<br>@ WebArclight</p>
    </div>

    <!-- Connect -->
    <div class="card">
      <div class="card-header">
        <div class="card-icon">
          <svg viewBox="0 0 24 24"><path d="M17 21v-2a4 4 0 0 0-4-4H5a4 4 0 0 0-4 4v2"/><circle cx="9" cy="7" r="4"/><path d="M23 21v-2a4 4 0 0 0-3-3.87"/><path d="M16 3.13a4 4 0 0 1 0 7.75"/></svg>
        </div>
        <h3>Connect</h3>
      </div>
      <div class="underline"></div>
      <p>Available for collaboration<br>&amp; open source</p>
    </div>
  </div>

  <!-- FOOTER -->
  <div class="footer-tagline">⚡ &nbsp; Building. Learning. Growing. &nbsp; ⚡</div>

  <div class="tech-stack">
    <div class="tech-icon" title="React">⚛️</div>
    <div class="tech-icon" title="Node.js">🟢</div>
    <div class="tech-icon" title="Express" style="font-size:18px; font-weight:800; color:#ccc; font-family:monospace;">ex</div>
    <div class="tech-icon" title="MongoDB">🍃</div>
    <div class="tech-icon" title="Python">🐍</div>
    <div class="tech-icon" title="Django" style="font-size:20px; font-weight:800; color:#0c4b33; background:#fff;">dj</div>
    <div class="tech-icon" title="Java">☕</div>
    <div class="tech-icon" title="Git">🔀</div>
  </div>

</div>
</body>
</html>
