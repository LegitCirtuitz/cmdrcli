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
  
  <!-- The Scroll Arrow -->
  <div class="scroll-arrow" onclick="document.getElementById('features').scrollIntoView({behavior: 'smooth'})">
    <span class="md-icon">
      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M7.41 8.58L12 13.17l4.59-4.59L18 10l-6 6-6-6 1.41-1.42Z"/></svg>
    </span>
  </div>
</div>

<div id="features" class="content-wrapper">

## Why Commandr?

Commandr CLI is built for speed and simplicity. Written in **pure Python** with minimal dependencies, it bridges the gap between complex shell scripts and intuitive user commands.

<!-- Feature Grid -->
<div class="grid-container">
  <div class="feature-card">
    <h3> Lightning Fast</h3>
    <p>Zero-bloat architecture ensures commands execute in milliseconds.</p>
  </div>
  <div class="feature-card">
    <h3> Python Powered</h3>
    <p>Extensible and easy to customize using the language you already love.</p>
  </div>
  <div class="feature-card">
    <h3> Developer First</h3>
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
  </div>
  <div class="terminal-body">
    <code class="typewriter">$ cmdr init project-alpha</code><br>
    <code class="response">[!!] Configuration initialized.</code><br>
    <code class="typewriter">$ cmdr deploy --prod</code><br>
    <code class="response"> Deploying to production... Done!</code>
  </div>
</div>

</div>

<style>
  /* Hero Section Enhancements */
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
    margin-bottom: 0 !important;
    background: linear-gradient(45deg, var(--md-primary-fg-color), #40b1ff);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }

  /* Reveal Animation */
  .reveal {
    animation: fadeInUp 1.2s ease-out;
  }

  @keyframes fadeInUp {
    from { opacity: 0; transform: translateY(30px); }
    to { opacity: 1; transform: translateY(0); }
  }

  /* Feature Grid */
  .grid-container {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 20px;
    margin-top: 40px;
  }

  .feature-card {
    padding: 1.5rem;
    border-radius: 8px;
    background: var(--md-code-bg-color);
    border: 1px solid var(--md-typeset-table-color);
    transition: transform 0.3s ease;
  }

  .feature-card:hover {
    transform: translateY(-5px);
    border-color: var(--md-primary-fg-color);
  }

  /* Terminal Mockup */
  .terminal-window {
    background: #1e1e1e;
    border-radius: 10px;
    box-shadow: 0 20px 50px rgba(0,0,0,0.3);
    overflow: hidden;
    margin: 2rem 0;
    font-family: 'Courier New', Courier, monospace;
  }

  .terminal-header {
    background: #333;
    padding: 10px;
    display: flex;
    gap: 8px;
  }

  .dot { height: 12px; width: 12px; border-radius: 50%; display: inline-block; }
  .red { background: #ff5f56; }
  .yellow { background: #ffbd2e; }
  .green { background: #27c93f; }

  .terminal-body {
    padding: 20px;
    color: #f8f8f2;
  }

  .response { color: #50fa7b; font-weight: bold; }

  /* Arrow Animation */
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
