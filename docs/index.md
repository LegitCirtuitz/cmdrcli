---
hide:
  - navigation
  - toc
---

<div class="hero-section">
  <div class="reveal">
    <h1 class="hero-title">Commandr CLI</h1>
    <p class="hero-subtitle">The ultimate automation tool for modern developers.</p>
    <div class="hero-buttons">
      <a href="main/setup/" class="md-button md-button--primary custom-btn">Get Started</a>
      <a href="https://github.com/LegitCirtuitz/cmdrcli" class="md-button outline-btn">View on GitHub</a>
    </div>
  </div>
  
  <div class="scroll-arrow" onclick="document.getElementById('features-section').scrollIntoView({behavior: 'smooth'})">
    <span class="md-icon">
      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M7.41 8.58L12 13.17l4.59-4.59L18 10l-6 6-6-6 1.41-1.42Z"/></svg>
    </span>
  </div>
</div>

<div id="features-section" class="main-content">

  <h2 class="section-header">Technical Excellence</h2>
  
  <p class="section-text">
    Commandr CLI is engineered for performance. Built with a zero-dependency mindset in Python, 
    it provides a robust framework for automating complex local and cloud workflows.
  </p>

  <div class="grid-container">
    <div class="feature-card">
      <h3 class="card-title">High Performance</h3>
      <p>The core engine is optimized for sub-millisecond execution times and minimal memory footprint.</p>
    </div>
    <div class="feature-card">
      <h3 class="card-title">Pythonic Architecture</h3>
      <p>Leverage the full power of the Python ecosystem to extend functionality with custom plugins.</p>
    </div>
    <div class="feature-card">
      <h3 class="card-title">DevOps Integrated</h3>
      <p>Standardized hooks for Git, Docker, and CI/CD pipelines come pre-configured out of the box.</p>
    </div>
  </div>

  <hr class="section-divider">

  <h2 class="section-header">Live Preview</h2>

  <div class="terminal-window">
    <div class="terminal-header">
      <span class="dot red"></span>
      <span class="dot yellow"></span>
      <span class="dot green"></span>
      <span class="terminal-label">zsh — cmdr</span>
    </div>
    <div class="terminal-body">
      <div class="typewriter-line"><span class="prompt">$</span> cmdr init project-alpha</div>
      <div class="response">[INFO] Environment configuration successfully generated.</div>
      <div class="typewriter-line delay-1"><span class="prompt">$</span> cmdr deploy --prod</div>
      <div class="response delay-1">[SUCCESS] Production deployment sequence complete.</div>
    </div>
  </div>

</div>

<style>
  /* Fixes for Black Primary Color Theme */
  :root {
    --text-bright: #ffffff;
    --text-dim: #b0b0b0;
    --accent-blue: #40b1ff;
  }

  .main-content {
    max-width: 1100px;
    margin: 0 auto;
    padding: 40px 20px;
  }

  /* Typography Fixes */
  .section-header {
    font-size: 2.2rem !important;
    font-weight: 700 !important;
    text-align: center;
    margin-top: 4rem !important;
    color: var(--text-bright) !important;
    border-bottom: none !important;
  }

  .section-text {
    text-align: center;
    color: var(--text-dim);
    max-width: 800px;
    margin: 1.5rem auto 4rem;
    font-size: 1.1rem;
  }

  /* Hero Section */
  .hero-section {
    position: relative;
    height: 80vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
  }

  .hero-title {
    font-size: 4.5rem !important;
    font-weight: 900 !important;
    color: var(--text-bright) !important;
    margin-bottom: 0.5rem !important;
    text-shadow: 0 0 20px rgba(255,255,255,0.1);
  }

  .hero-subtitle {
    color: var(--text-dim) !important;
    font-size: 1.5rem;
  }

  /* Button Fixes */
  .custom-btn {
    background-color: var(--text-bright) !important;
    color: #000 !important;
    border: none !important;
  }

  .outline-btn {
    border: 1px solid #444 !important;
    color: var(--text-bright) !important;
  }

  /* Card Fixes */
  .feature-card {
    padding: 2.5rem;
    border-radius: 12px;
    background: #161616;
    border: 1px solid #333;
    transition: all 0.3s ease;
  }

  .feature-card:hover {
    transform: translateY(-10px);
    border-color: var(--accent-blue);
    box-shadow: 0 10px 30px rgba(64, 177, 255, 0.1);
  }

  .card-title {
    color: var(--accent-blue) !important;
    margin-top: 0 !important;
  }

  /* Terminal */
  .terminal-window {
    background: #000;
    border-radius: 10px;
    box-shadow: 0 0 40px rgba(0,0,0,0.8), 0 0 2px #333;
    margin: 4rem 0;
    overflow: hidden;
  }

  .terminal-header { background: #1a1a1a; padding: 12px 20px; display: flex; align-items: center; gap: 10px; }
  .terminal-body { padding: 30px; font-family: monospace; color: #eee; line-height: 1.8; }
  .prompt { color: var(--accent-blue); }
  .response { color: #00ff9d; opacity: 0; animation: fadeIn 0.4s forwards 1.5s; }
  .response.delay-1 { animation-delay: 3.5s; }

  /* Animations */
  .reveal { animation: fadeInUp 1s ease-out; }
  @keyframes fadeInUp {
    from { opacity: 0; transform: translateY(30px); }
    to { opacity: 1; transform: translateY(0); }
  }

  .typewriter-line {
    overflow: hidden;
    white-space: nowrap;
    width: 0;
    animation: typing 1.5s steps(40, end) forwards;
  }
  .typewriter-line.delay-1 { animation-delay: 2s; }

  @keyframes typing { from { width: 0 } to { width: 100% } }
  @keyframes fadeIn { to { opacity: 1; } }

  .scroll-arrow {
    position: absolute;
    bottom: 40px;
    color: var(--text-dim);
    animation: bounce 2.5s infinite;
  }

  @keyframes bounce {
    0%, 20%, 50%, 80%, 100% { transform: translateY(0); }
    40% { transform: translateY(-15px); }
  }

  .section-divider { border-top: 1px solid #222; margin: 5rem 0; }
</style>
