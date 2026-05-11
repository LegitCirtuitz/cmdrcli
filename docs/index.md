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
      <a href="main/setup/" class="md-button md-button--primary">Get Started</a>
      <a href="https://github.com/LegitCirtuitz/cmdrcli" class="md-button">View on GitHub</a>
    </div>
  </div>
  
  <div class="scroll-arrow" onclick="document.getElementById('anchor').scrollIntoView({behavior: 'smooth'})">
    <span class="md-icon">
      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M7.41 8.58L12 13.17l4.59-4.59L18 10l-6 6-6-6 1.41-1.42Z"/></svg>
    </span>
  </div>
</div>

<div id="anchor"></div>

## Why Commandr?

Commandr CLI is built for speed and simplicity. Written in **pure Python** with minimal dependencies, it bridges the gap between complex shell scripts and intuitive user commands.

<div class="grid-container">
  <div class="feature-card">
    <h3>🚀 Lightning Fast</h3>
    <p>Zero-bloat architecture ensures commands execute in milliseconds.</p>
  </div>
  <div class="feature-card">
    <h3>🐍 Python Powered</h3>
    <p>Extensible and easy to customize using the language you already love.</p>
  </div>
  <div class="feature-card">
    <h3>🛠️ Developer First</h3>
    <p>Built-in automation for git workflows, environment setups, and more.</p>
  </div>
</div>

---

## See it in Action

<div class="terminal-window">
  <div class="terminal-header">
    <span class="dot red"></span>
    <span class="dot yellow"></span>
    <span class="dot green"></span>
    <span class="terminal-title">bash — 80x24</span>
  </div>
  <div class="terminal-body">
    <div class="typewriter-line"><span class="prompt">$</span> cmdr init project-alpha</div>
    <div class="response">[!!] Configuration initialized.</div>
    <div class="typewriter-line delay-1"><span class="prompt">$</span> cmdr deploy --prod</div>
    <div class="response delay-1">🚀 Deploying to production... Done!</div>
  </div>
</div>

<style>
  /* Hero Section */
  .hero-section {
    position: relative;
    height: 90vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
    background: radial-gradient(circle at center, var(--md-primary-fg-color--transparent) 0%, transparent 70%);
  }

  .hero-title {
    font-size: 4rem !important;
    font-weight: 900 !important;
    margin-bottom: 0.5rem !important;
    background: linear-gradient(45deg, var(--md-primary-fg-color), #40b1ff);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }

  .reveal { animation: fadeInUp 1.2s ease-out; }

  @keyframes fadeInUp {
    from { opacity: 0; transform: translateY(30px); }
    to { opacity: 1; transform: translateY(0); }
  }

  /* Grid & Cards */
  .grid-container {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 20px;
    margin: 40px 0;
  }

  .feature-card {
    padding: 1.5rem;
    border-radius: 12px;
    background: rgba(255, 255, 255, 0.05);
    border: 1px solid rgba(255, 255, 255, 0.1);
    backdrop-filter: blur(10px);
    transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
  }

  .feature-card:hover {
    transform: translateY(-8px);
    background: rgba(255, 255, 255, 0.1);
    border-color: var(--md-primary-fg-color);
    box-shadow: 0 10px 20px rgba(0,0,0,0.2);
  }

  /* Terminal with Typing Animation */
  .terminal-window {
    background: #121212;
    border-radius: 10px;
    box-shadow: 0 20px 50px rgba(0,0,0,0.4);
    overflow: hidden;
    margin: 2rem 0;
    font-family: 'Fira Code', monospace;
  }

  .terminal-header {
    background: #252525;
    padding: 12px;
    display: flex;
    align-items: center;
    gap: 8px;
  }

  .terminal-title {
    color: #888;
    font-size: 12px;
    margin-left: auto;
    margin-right: auto;
  }

  .dot { height: 12px; width: 12px; border-radius: 50%; }
  .red { background: #ff5f56; }
  .yellow { background: #ffbd2e; }
  .green { background: #27c93f; }

  .terminal-body { padding: 25px; color: #f8f8f2; line-height: 1.6; }
  .prompt { color: #bd93f9; margin-right: 10px; }
  .response { color: #50fa7b; font-weight: bold; margin-bottom: 10px; opacity: 0; animation: fadeIn 0.1s forwards; animation-delay: 1.5s; }
  .response.delay-1 { animation-delay: 3.5s; }

  .typewriter-line {
    overflow: hidden;
    white-space: nowrap;
    border-right: 2px solid var(--md-primary-fg-color);
    width: 0;
    animation: typing 1.5s steps(30, end) forwards, blink 0.8s infinite;
  }

  .typewriter-line.delay-1 { animation-delay: 2s; }

  @keyframes typing { from { width: 0 } to { width: 100% } }
  @keyframes blink { from, to { border-color: transparent } 50% { border-color: var(--md-primary-fg-color) } }
  @keyframes fadeIn { to { opacity: 1; } }

  .scroll-arrow {
    position: absolute;
    bottom: 40px;
    left: 50%;
    transform: translateX(-50%);
    cursor: pointer;
    color: var(--md-primary-fg-color);
    animation: bounce 2s infinite;
  }

  @keyframes bounce {
    0%, 20%, 50%, 80%, 100% {transform: translateX(-50%) translateY(0);}
    40% {transform: translateX(-50%) translateY(-15px);}
    60% {transform: translateX(-50%) translateY(-7px);}
  }
</style>
