---
hide:
  - navigation
  - toc
---

<div class="hero-section">
  <h1 class="hero-title">Commandr CLI</h1>
  <p class="hero-subtitle">The ultimate automation tool for modern developers.</p>
  <div class="hero-buttons">
    <a href="main/setup/" class="md-button md-button--primary">Get Started</a>
    <a href="https://github.com/LegitCirtuitz/cmdrcli" class="md-button">View on GitHub</a>
  </div>
  
  <!-- The Scroll Arrow -->
  <div class="scroll-arrow" onclick="document.getElementById('features').scrollIntoView({behavior: 'smooth'})">
    <span class="md-icon">
      <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24"><path d="M7.41 8.58L12 13.17l4.59-4.59L18 10l-6 6-6-6 1.41-1.42Z"/></svg>
    </span>
  </div>
</div>

<!-- This is where the arrow scrolls to -->
<div id="features" style="padding-top: 50px;"></div>

## Features
*   **Fast:** Built with speed in mind.
*   **Customizable:** Fits your workflow perfectly.

<style>
  .hero-section {
    position: relative;
    height: 80vh; /* Takes up most of the screen height */
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
  }

  .hero-title {
    font-size: 3rem !important;
    font-weight: 800 !important;
    color: var(--md-primary-fg-color);
  }

  /* Arrow Styling & Animation */
  .scroll-arrow {
    position: absolute;
    bottom: 20px;
    left: 50%;
    transform: translateX(-50%);
    cursor: pointer;
    font-size: 2rem;
    color: var(--md-default-fg-color--light);
    animation: bounce 2s infinite;
  }

  .scroll-arrow svg {
    width: 40px;
    fill: currentColor;
  }

  @keyframes bounce {
    0%, 20%, 50%, 80%, 100% {transform: translateX(-50%) translateY(0);}
    40% {transform: translateX(-50%) translateY(-10px);}
    60% {transform: translateX(-50%) translateY(-5px);}
  }
</style>
