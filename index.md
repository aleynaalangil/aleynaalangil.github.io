---
layout: default
title: "Home"
---

<style>
:root {
  --neon: #00ff8a;
  --neon-dim: #00c26b;
  --bg: #070b08;
  --panel: #0b130f;
  --grid: rgba(0, 255, 138, 0.08);
  --warn: #ff6b35;
}
.hacker-shell {
  position: relative;
  overflow: hidden;
  border: 1px solid var(--neon);
  background: linear-gradient(135deg, var(--panel), #050a07);
  box-shadow: 0 0 20px rgba(0, 255, 138, 0.2);
  padding: 24px;
  margin: 12px 0 24px;
}
.hacker-shell::before {
  content: "";
  position: absolute;
  inset: 0;
  background: repeating-linear-gradient(
    0deg,
    rgba(0, 255, 138, 0.07),
    rgba(0, 255, 138, 0.07) 1px,
    transparent 1px,
    transparent 3px
  );
  pointer-events: none;
}
.hacker-shell > * {
  position: relative;
}
.hacker-header {
  display: flex;
  justify-content: space-between;
  font-size: 12px;
  letter-spacing: 0.24em;
  text-transform: uppercase;
  color: var(--neon);
  margin-bottom: 18px;
}
.blink {
  animation: blink 1.4s steps(2, start) infinite;
}
@keyframes blink {
  to { visibility: hidden; }
}
.hero-grid {
  display: grid;
  grid-template-columns: 1fr 1.2fr;
  gap: 24px;
  align-items: start;
}
.ascii {
  margin: 0;
  color: var(--neon);
  text-shadow: 0 0 14px rgba(0, 255, 138, 0.35);
  font-size: 12px;
  line-height: 1.1;
}
.profile-title {
  font-size: 18px;
  font-weight: 700;
  text-transform: uppercase;
  letter-spacing: 0.08em;
  color: var(--neon);
  margin: 0 0 10px;
}
.profile-meta {
  display: grid;
  gap: 6px;
  color: #b7ffe0;
}
.profile-meta span {
  color: var(--neon-dim);
}
.panel {
  border-left: 3px solid var(--neon);
  padding: 12px 16px;
  margin: 18px 0;
  background: rgba(4, 9, 6, 0.6);
  box-shadow: inset 0 0 0 1px rgba(0, 255, 138, 0.15);
}
.panel-title {
  text-transform: uppercase;
  letter-spacing: 0.2em;
  font-size: 12px;
  color: var(--neon);
  margin-bottom: 10px;
}
.process-list {
  list-style: none;
  padding: 0;
  margin: 0;
}
.process-list li {
  margin: 8px 0;
}
.process-list strong {
  color: var(--neon);
}
.links a {
  color: var(--neon);
  text-decoration: none;
  border-bottom: 1px solid rgba(0, 255, 138, 0.5);
}
.links a:hover {
  color: #ffffff;
  border-bottom-color: #ffffff;
}
@media (max-width: 860px) {
  .hero-grid {
    grid-template-columns: 1fr;
  }
}
</style>

<div class="hacker-shell">
  <div class="hacker-header">
    <div class="blink">Access Granted</div>
    <div>Session: Live</div>
  </div>
  <div class="hero-grid">
    <pre class="ascii">
    ___    _      ________  __    __  ______
   /   |  | | /| / /_  __/ / /   / / / ____/
  / /| |  | |/ |/ / / /   / /   / / / /     
 / ___ |  |__/|__/ / /   / /___/ / / /___   
/_/  |_|         /_/   /_____/_/  \____/    
    </pre>
    <div>
      <div class="profile-title">Blockchain Backend Engineer // Solana</div>
      <div class="profile-meta">
        <div><span>IDENTITY:</span> Aleyna Alangil</div>
        <div><span>STATUS:</span> Developing for Mexico Release</div>
        <div><span>FOCUS:</span> High-performance decentralized architecture</div>
        <div><span>STACK:</span> Rust, Solana, Systems Design</div>
      </div>
    </div>
  </div>
</div>

<div class="panel">
  <div class="panel-title">About</div>
  <div>I am a <strong>Blockchain Backend Engineer</strong> specializing in the Solana ecosystem. I build high-performance systems using Rust and focus on scalable decentralized architecture.</div>
</div>

<div class="panel">
  <div class="panel-title">Active Processes</div>
  <ul class="process-list">
    <li><strong>Open Source:</strong> Contributing to Rust-based tooling and CLI crates.</li>
    <li><strong>Research:</strong> Exploring advanced Solana smart contract optimizations.</li>
  </ul>
</div>

<div class="panel links">
  <div class="panel-title">Primary Link</div>
  <a href="https://github.com/aleynaalangil">github.com/aleynaalangil</a>
</div>
