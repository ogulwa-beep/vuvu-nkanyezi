<!DOCTYPE html>

<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
  <meta name="description" content="Vuvu Nkanyezi — African-inspired first-person game. Collect star-seeds, balance ancestral energies, compose celestial music.">
  <meta name="theme-color" content="#050a1a">
  <meta name="apple-mobile-web-app-capable" content="yes">
  <meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
  <meta name="mobile-web-app-capable" content="yes">

  <!-- Open Graph -->

  <meta property="og:title" content="VUVU ✦ NKANYEZI">
  <meta property="og:description" content="The Starborn Resonance — An African ancestral game of music and balance">
  <meta property="og:type" content="website">

  <!-- Security -->

  <meta http-equiv="X-Content-Type-Options" content="nosniff">
  <meta http-equiv="Referrer-Policy" content="no-referrer">
  <meta http-equiv="Permissions-Policy" content="camera=(), microphone=(), geolocation=()">
  <meta http-equiv="Content-Security-Policy" content="default-src 'none'; script-src 'self' 'unsafe-inline' https://cdnjs.cloudflare.com https://unpkg.com; style-src 'self' 'unsafe-inline' https://fonts.googleapis.com; font-src https://fonts.gstatic.com; connect-src 'none'; img-src 'self' data:; object-src 'none'; base-uri 'none'; form-action 'none';">

  <title>VUVU ✦ NKANYEZI — The Starborn Resonance</title>

  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Cinzel+Decorative:wght@400;700&family=Crimson+Pro:ital,wght@0,300;0,400;1,300&display=swap" rel="stylesheet">

  <style>
    /* ════════════════════════════════════
       TOKENS & RESET
    ════════════════════════════════════ */
    :root {
      --void:          #020509;
      --deep-night:    #050a1a;
      --star-white:    #f0eedd;
      --star-warm:     #ffefc8;
      --star-blue:     #8ab4e8;
      --star-gold:     #f5c842;
      --star-amber:    #e8942a;
      --nebula-purple: #4a2070;
      --gold-glow:     rgba(245,200,66,0.45);
      --text-dim:      rgba(240,238,221,0.5);
      /* joystick sizes */
      --jz: 110px;   /* zone diameter  */
      --jk: 46px;    /* knob diameter  */
    }

    *, *::before, *::after { margin:0; padding:0; box-sizing:border-box; }

    html, body {
      width:100%; height:100%;
      overflow:hidden;
      background: var(--void);
      font-family: 'Crimson Pro', Georgia, serif;
      user-select: none;
      -webkit-tap-highlight-color: transparent;
      touch-action: none;
    }

    /* ════════════════════════════════════
       CANVAS
    ════════════════════════════════════ */
    #game-container { width:100%; height:100%; position:relative; }

    #render-canvas {
      display:block;
      width:100%; height:100%;
      cursor: crosshair;
      touch-action: none;
    }

    /* ════════════════════════════════════
       LOADING SCREEN
    ════════════════════════════════════ */
    #loading-screen {
      position:absolute; inset:0;
      background: radial-gradient(ellipse at 30% 40%, #1a0a2e 0%, #050a1a 40%, #020509 100%);
      display:flex; flex-direction:column;
      align-items:center; justify-content:center;
      z-index:1000;
      transition: opacity 1.2s ease;
      overflow:hidden;
    }
    #loading-screen::before {
      content:'';
      position:absolute; inset:0;
      background-image:
        radial-gradient(circle,#fff 1px,transparent 1px),
        radial-gradient(circle,rgba(255,255,255,.6) 1px,transparent 1px),
        radial-gradient(circle,rgba(138,180,232,.8) 1px,transparent 1px);
      background-size: 150px 150px, 97px 97px, 213px 213px;
      background-position: 0 0, 50px 80px, 120px 30px;
      animation: shimmer 4s infinite;
    }
    #loading-screen.hidden { opacity:0; pointer-events:none; }

    .loading-constellation {
      position:relative; width:100px; height:100px;
      margin-bottom:1.5rem;
      animation: drift 6s infinite ease-in-out;
    }
    .cstar {
      position:absolute; border-radius:50%;
      background: var(--star-gold);
      box-shadow: 0 0 8px var(--star-gold), 0 0 20px rgba(245,200,66,.4);
    }
    .cs1{width:8px;height:8px;top:8px;left:44px;  animation:twinkle 2.1s infinite}
    .cs2{width:6px;height:6px;top:32px;left:16px; animation:twinkle 1.7s .4s infinite}
    .cs3{width:10px;height:10px;top:52px;left:50px;animation:twinkle 2.5s .2s infinite;background:var(--star-warm)}
    .cs4{width:5px;height:5px;top:36px;left:78px; animation:twinkle 1.9s .8s infinite;background:var(--star-blue)}
    .cs5{width:7px;height:7px;top:78px;left:22px; animation:twinkle 2.3s 1.1s infinite}
    .cs6{width:6px;height:6px;top:82px;left:68px; animation:twinkle 1.8s .6s infinite;background:var(--star-blue)}

    .loading-title {
      font-family:'Cinzel Decorative',serif;
      font-size: clamp(2rem,7vw,4rem);
      color: var(--star-gold);
      letter-spacing:.3em;
      text-shadow: 0 0 30px var(--star-gold), 0 0 80px rgba(245,200,66,.3);
      margin-bottom:.3rem;
      position:relative; z-index:1;
      animation: fadeUp 1s ease both;
    }
    .loading-subtitle {
      font-style:italic;
      font-size: clamp(.75rem,2vw,1rem);
      color: var(--star-blue);
      letter-spacing:.2em;
      text-transform:uppercase;
      margin-bottom:1.8rem;
      position:relative; z-index:1;
      animation: fadeUp 1s .3s ease both;
    }
    .loading-ring {
      width:46px; height:46px;
      border:2px solid transparent;
      border-top:2px solid var(--star-gold);
      border-right:2px solid rgba(245,200,66,.3);
      border-radius:50%;
      animation: spin 1.4s linear infinite;
      box-shadow: 0 0 20px var(--gold-glow);
      position:relative; z-index:1;
    }
    .loading-text {
      color:var(--text-dim); font-style:italic;
      font-size:.95rem; margin-top:1rem;
      position:relative; z-index:1;
      animation: shimmer 2.5s infinite;
      letter-spacing:.06em;
    }

    /* ════════════════════════════════════
       CROSSHAIR (desktop only)
    ════════════════════════════════════ */
    #crosshair {
      position:absolute; top:50%; left:50%;
      transform:translate(-50%,-50%);
      width:18px; height:18px;
      pointer-events:none; z-index:100;
    }
    #crosshair::before,#crosshair::after {
      content:''; position:absolute;
      background: rgba(245,200,66,.7);
    }
    #crosshair::before { width:2px;height:10px; top:4px; left:8px; }
    #crosshair::after  { width:10px;height:2px; top:8px; left:4px; }

    /* ════════════════════════════════════
       TOP-LEFT: SEED COUNTER
    ════════════════════════════════════ */
    #star-count {
      position:absolute; top:12px; left:12px;
      font-family:'Cinzel Decorative',serif;
      font-size: clamp(.55rem,.9vw,.72rem);
      letter-spacing:.12em;
      color: var(--star-warm);
      padding:8px 14px;
      background: rgba(5,10,26,.78);
      border:1px solid rgba(245,200,66,.22);
      border-radius:12px;
      backdrop-filter:blur(8px);
      z-index:100;
    }
    #star-count span { color:var(--star-gold); text-shadow: 0 0 8px var(--gold-glow); }

    /* ════════════════════════════════════
       BALANCE HUD (bottom-centre)
    ════════════════════════════════════ */
    #balance-hud {
      position:absolute;
      bottom: env(safe-area-inset-bottom, 16px);
      bottom: calc(env(safe-area-inset-bottom, 0px) + 16px);
      left:50%; transform:translateX(-50%);
      display:flex; gap:20px; align-items:center;
      background: rgba(5,10,26,.82);
      padding:10px 26px;
      border-radius:60px;
      border:1px solid rgba(245,200,66,.28);
      box-shadow: 0 0 30px rgba(0,0,0,.6), inset 0 0 20px rgba(245,200,66,.04);
      z-index:100;
      backdrop-filter:blur(12px);
      -webkit-backdrop-filter:blur(12px);
    }
    .meter { text-align:center; }
    .meter .label {
      display:block;
      font-family:'Cinzel Decorative',serif;
      font-size: clamp(.45rem,.7vw,.6rem);
      letter-spacing:.12em;
      color:var(--star-gold);
      text-shadow: 0 0 8px var(--gold-glow);
      margin-bottom:5px;
    }
    .meter-bar {
      width: clamp(72px,10vw,110px);
      height:7px;
      background: rgba(255,255,255,.06);
      border:1px solid rgba(245,200,66,.18);
      border-radius:10px;
      overflow:hidden;
    }
    .meter-fill {
      height:100%; width:50%;
      transition: width .4s ease;
      border-radius:10px;
    }
    #umsindo-fill  { background: linear-gradient(90deg,var(--star-blue),var(--star-gold)); }
    #isithunzi-fill{ background: linear-gradient(90deg,var(--nebula-purple),var(--star-amber)); }

    #equilibrium-indicator {
      width:42px; height:42px;
      background: rgba(10,20,40,.9);
      border:1px solid rgba(245,200,66,.38);
      border-radius:50%;
      display:flex; align-items:center; justify-content:center;
      font-size:1.3rem; color:var(--star-gold);
      transition: all .4s ease;
    }
    #equilibrium-indicator.balanced {
      background: rgba(245,200,66,.12);
      border-color:var(--star-gold);
      animation: pulseGlow 2.5s infinite;
    }

    /* ════════════════════════════════════
       STAR MAP OVERLAY
    ════════════════════════════════════ */
    #logic-grid-overlay {
      position:absolute; top:50%; left:50%;
      transform:translate(-50%,-50%);
      background: rgba(5,10,26,.96);
      padding: clamp(14px,3vw,26px);
      border:1px solid rgba(245,200,66,.33);
      border-radius:20px;
      box-shadow: 0 0 60px rgba(0,0,0,.8), inset 0 0 40px rgba(245,200,66,.03);
      z-index:300;
      display:none;
      flex-direction:column; align-items:center;
      gap:14px;
      backdrop-filter:blur(20px);
      -webkit-backdrop-filter:blur(20px);
      max-width:95vw;
      max-height:90vh;
      overflow-y:auto;
    }
    #logic-grid-overlay.visible { display:flex; }
    .grid-title {
      font-family:'Cinzel Decorative',serif;
      color:var(--star-gold);
      font-size: clamp(.6rem,1.5vw,.9rem);
      letter-spacing:.18em;
      text-align:center;
      text-shadow: 0 0 12px var(--gold-glow);
    }
    #grid-canvas {
      background: rgba(2,5,9,.95);
      border:1px solid rgba(138,180,232,.22);
      border-radius:10px;
      cursor:pointer;
      max-width:100%;
      height:auto;
    }
    .grid-controls {
      display:flex; gap:8px;
      flex-wrap:wrap; justify-content:center;
    }
    .btn {
      padding:9px 18px;
      background:transparent;
      color:var(--star-warm);
      border:1px solid rgba(245,200,66,.33);
      font-family:'Cinzel Decorative',serif;
      font-size: clamp(.5rem,.9vw,.68rem);
      border-radius:40px;
      cursor:pointer;
      letter-spacing:.1em;
      transition: all .2s ease;
      touch-action:manipulation;
    }
    .btn:hover   { background:rgba(245,200,66,.1); border-color:var(--star-gold); }
    .btn:active  { transform:scale(.95); }
    .btn.gold    { border-color:var(--star-gold); color:var(--star-gold); background:rgba(245,200,66,.08); }
    .btn.gold:hover { background:rgba(245,200,66,.18); }

    /* ════════════════════════════════════
       MESSAGE TOAST
    ════════════════════════════════════ */
    #message-display {
      position:absolute; top:16%; left:50%;
      transform:translateX(-50%);
      background: rgba(5,10,26,.9);
      border:1px solid rgba(245,200,66,.28);
      color:var(--star-warm);
      padding:12px 28px;
      border-radius:50px;
      font-style:italic;
      font-size: clamp(.8rem,1.6vw,1rem);
      letter-spacing:.04em;
      opacity:0; pointer-events:none;
      transition: opacity .5s ease;
      z-index:150;
      backdrop-filter:blur(10px);
      -webkit-backdrop-filter:blur(10px);
      text-align:center;
      max-width:88vw;
      white-space:normal;
    }
    #message-display.show { opacity:1; }

    /* ════════════════════════════════════
       DESKTOP INSTRUCTIONS (landscape ≥ 900px)
    ════════════════════════════════════ */
    #instructions {
      position:absolute; top:12px; right:12px;
      background: rgba(5,10,26,.85);
      border:1px solid rgba(245,200,66,.18);
      padding:16px 18px;
      border-radius:14px;
      font-size:.78rem;
      color:var(--text-dim);
      z-index:100; max-width:200px;
      line-height:1.85;
      backdrop-filter:blur(10px);
      -webkit-backdrop-filter:blur(10px);
    }
    #instructions h4 {
      font-family:'Cinzel Decorative',serif;
      color:var(--star-gold);
      font-size:.58rem;
      letter-spacing:.16em;
      margin-bottom:9px;
      text-shadow: 0 0 8px var(--gold-glow);
    }
    .key {
      display:inline-block;
      background:rgba(245,200,66,.1);
      border:1px solid rgba(245,200,66,.28);
      color:var(--star-gold);
      padding:1px 6px; border-radius:4px;
      font-size:.7rem; font-family:monospace;
      margin-right:3px;
    }

    /* ════════════════════════════════════
       MOBILE TOUCH CONTROLS
       Left side: joystick   Right side: look pad + buttons
    ════════════════════════════════════ */

    /* Joystick zone — bottom-left */
    #joystick-zone {
      display:none;
      position:absolute;
      left: max(env(safe-area-inset-left,0px), 16px);
      bottom: calc(env(safe-area-inset-bottom,0px) + 90px);
      width:var(--jz); height:var(--jz);
      border-radius:50%;
      background: rgba(245,200,66,.06);
      border:1px solid rgba(245,200,66,.22);
      z-index:200;
      touch-action:none;
      pointer-events:none; /* receive injected touch only */
    }
    #joystick-knob {
      position:absolute;
      width:var(--jk); height:var(--jk);
      border-radius:50%;
      background: rgba(245,200,66,.2);
      border:2px solid var(--star-gold);
      box-shadow: 0 0 12px var(--gold-glow);
      top:50%; left:50%;
      transform:translate(-50%,-50%);
      transition: background .15s;
    }

    /* Look / rotate zone — right 50% of screen (no pointer-events on element; captured via JS) */

    /* Action buttons — bottom-right */
    #action-btns {
      display:none;
      position:absolute;
      right: max(env(safe-area-inset-right,0px), 14px);
      bottom: calc(env(safe-area-inset-bottom,0px) + 90px);
      flex-direction:column;
      gap:10px;
      z-index:200;
      align-items:flex-end;
    }
    .act-btn {
      width:58px; height:58px;
      border-radius:50%;
      background: rgba(5,10,26,.85);
      border:1px solid rgba(245,200,66,.38);
      font-size:1.4rem;
      display:flex; align-items:center; justify-content:center;
      color:var(--star-warm);
      box-shadow: 0 0 14px rgba(0,0,0,.4);
      backdrop-filter:blur(5px);
      -webkit-backdrop-filter:blur(5px);
      touch-action:manipulation;
      cursor:pointer;
      transition: background .15s, box-shadow .15s;
    }
    .act-btn:active {
      background:rgba(245,200,66,.18);
      box-shadow:0 0 22px rgba(245,200,66,.35);
    }
    .act-btn .btn-label {
      position:absolute;
      font-family:'Cinzel Decorative',serif;
      font-size:.38rem;
      letter-spacing:.05em;
      color:rgba(245,200,66,.6);
      bottom:-14px; left:50%; transform:translateX(-50%);
      white-space:nowrap;
    }
    .act-btn-wrap { position:relative; }

    /* Balance nudge buttons (landscape: small, top-right on mobile) */
    #balance-btns {
      display:none;
      position:absolute;
      right: max(env(safe-area-inset-right,0px), 14px);
      top:12px;
      flex-direction:row;
      gap:8px;
      z-index:200;
    }
    .bal-btn {
      padding:7px 12px;
      font-family:'Cinzel Decorative',serif;
      font-size:.45rem;
      letter-spacing:.08em;
      color:var(--star-warm);
      background: rgba(5,10,26,.8);
      border:1px solid rgba(245,200,66,.25);
      border-radius:30px;
      cursor:pointer;
      touch-action:manipulation;
      backdrop-filter:blur(5px);
    }
    .bal-btn:active { background:rgba(245,200,66,.15); }

    /* ════════════════════════════════════
       ORIENTATION PROMPT (portrait warning)
    ════════════════════════════════════ */
    #orient-prompt {
      display:none;
      position:absolute; inset:0;
      background: var(--void);
      z-index:900;
      flex-direction:column;
      align-items:center; justify-content:center;
      gap:1.5rem;
      text-align:center;
      padding:2rem;
    }
    #orient-prompt .icon { font-size:3.5rem; animation: rotateHint 2s infinite ease-in-out; }
    #orient-prompt p {
      font-family:'Cinzel Decorative',serif;
      color:var(--star-gold);
      font-size:.85rem;
      letter-spacing:.15em;
      line-height:1.8;
    }
    #orient-prompt small { color:var(--text-dim); font-style:italic; }

    /* ════════════════════════════════════
       RESPONSIVE BREAKPOINTS
    ════════════════════════════════════ */

    /* Mobile portrait — show rotate prompt over game */
    @media (max-width:600px) and (orientation:portrait) {
      #orient-prompt { display:flex; }
    }

    /* Mobile landscape — full touch UI */
    @media (max-height:500px), (max-width:900px) and (pointer:coarse) {
      #instructions  { display:none; }
      #crosshair     { display:none; }
      #joystick-zone { display:block; }
      #action-btns   { display:flex; }
      #balance-btns  { display:flex; }
      #balance-hud   { bottom: calc(env(safe-area-inset-bottom,0px) + 14px); padding:8px 18px; gap:14px; }
      .meter-bar     { width:72px; }
      #star-count    { font-size:.52rem; padding:6px 10px; }
    }

    /* Tablet / large mobile landscape — show everything comfortably */
    @media (min-width:600px) and (max-width:1024px) and (pointer:coarse) {
      --jz: 120px; --jk: 52px;
    }

    /* ════════════════════════════════════
       KEYFRAME ANIMATIONS
    ════════════════════════════════════ */
    @keyframes twinkle  { 0%,100%{opacity:.6;transform:scale(1)} 50%{opacity:1;transform:scale(1.3)} }
    @keyframes drift    { 0%,100%{transform:translateY(0) translateX(0)} 33%{transform:translateY(-6px) translateX(3px)} 66%{transform:translateY(4px) translateX(-3px)} }
    @keyframes shimmer  { 0%,100%{opacity:.4} 50%{opacity:1} }
    @keyframes spin     { to{transform:rotate(360deg)} }
    @keyframes fadeUp   { from{opacity:0;transform:translateY(10px)} to{opacity:1;transform:translateY(0)} }
    @keyframes pulseGlow{ 0%,100%{box-shadow:0 0 15px var(--gold-glow)} 50%{box-shadow:0 0 40px var(--gold-glow),0 0 80px rgba(245,200,66,.18)} }
    @keyframes rotateHint { 0%,100%{transform:rotate(0deg)} 50%{transform:rotate(90deg)} }
  </style>

</head>
<body>
<div id="game-container">

  <!-- Loading -->

  <div id="loading-screen">
    <div class="loading-constellation">
      <div class="cstar cs1"></div><div class="cstar cs2"></div>
      <div class="cstar cs3"></div><div class="cstar cs4"></div>
      <div class="cstar cs5"></div><div class="cstar cs6"></div>
    </div>
    <div class="loading-title">VUVU</div>
    <div class="loading-subtitle">✦ Nkanyezi ✦ The Starborn Resonance</div>
    <div class="loading-ring"></div>
    <div class="loading-text">The star-ancestors are awakening…</div>
  </div>

  <!-- Orientation prompt -->

  <div id="orient-prompt">
    <div class="icon">📱</div>
    <p>ROTATE YOUR DEVICE<br>TO LANDSCAPE</p>
    <small>Vuvu Nkanyezi plays best in landscape mode</small>
  </div>

  <!-- 3D Canvas -->

<canvas id="render-canvas"></canvas>

  <!-- Crosshair -->

  <div id="crosshair"></div>

  <!-- Seed counter -->

  <div id="star-count">✦ INYANKEZANA <span id="seed-counter">0</span>/5</div>

  <!-- Balance HUD -->

  <div id="balance-hud">
    <div class="meter">
      <span class="label">UMSINDO</span>
      <div class="meter-bar"><div class="meter-fill" id="umsindo-fill"></div></div>
    </div>
    <div id="equilibrium-indicator">✦</div>
    <div class="meter">
      <span class="label">ISITHUNZI</span>
      <div class="meter-bar"><div class="meter-fill" id="isithunzi-fill"></div></div>
    </div>
  </div>

  <!-- Star Map overlay -->

  <div id="logic-grid-overlay">
    <div class="grid-title">✦ UHLELO LWEZINKANYEZI — STAR MAP ✦</div>
    <canvas id="grid-canvas" width="360" height="180"></canvas>
    <div class="grid-controls">
      <button class="btn gold" id="play-composition">▶ Vula</button>
      <button class="btn" id="stop-composition">■ Misa</button>
      <button class="btn" id="clear-grid">✕ Sula</button>
      <button class="btn" id="exit-grid">← Phuma</button>
    </div>
  </div>

  <!-- Message toast -->

  <div id="message-display"></div>

  <!-- Desktop instructions -->

  <div id="instructions">
    <h4>✦ CONTROLS</h4>
    <p><span class="key">WASD</span> Move</p>
    <p><span class="key">Mouse</span> Look</p>
    <p><span class="key">E</span> Collect</p>
    <p><span class="key">G</span> Star Map</p>
    <p><span class="key">Q</span> Thunder/Self</p>
    <p><span class="key">R</span> River/Ancestral</p>
    <p><span class="key">Space</span> Sketch</p>
    <p><span class="key">Click</span> Lock cursor</p>
  </div>

  <!-- Virtual joystick (mobile) -->

  <div id="joystick-zone"><div id="joystick-knob"></div></div>

  <!-- Action buttons (mobile right side) -->

  <div id="action-btns">
    <div class="act-btn-wrap">
      <button class="act-btn" id="btn-collect" aria-label="Collect star-seed">✦
        <span class="btn-label">COLLECT</span>
      </button>
    </div>
    <div class="act-btn-wrap">
      <button class="act-btn" id="btn-grid" aria-label="Open star map">🎵
        <span class="btn-label">MAP</span>
      </button>
    </div>
    <div class="act-btn-wrap">
      <button class="act-btn" id="btn-sketch" aria-label="Sketch resonance">✏️
        <span class="btn-label">SKETCH</span>
      </button>
    </div>
  </div>

  <!-- Balance nudge (mobile top-right) -->

  <div id="balance-btns">
    <button class="bal-btn" id="btn-thunder">⚡ THUNDER</button>
    <button class="bal-btn" id="btn-river">🌊 RIVER</button>
  </div>

</div><!-- /game-container -->

<!-- Three.js via importmap -->

<script type="importmap">
  { "imports": { "three": "https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.module.min.js" } }
</script>

<script type="module">
'use strict';
// ═══════════════════════════════════════════════════════
// VUVU NKANYEZI — THE STARBORN RESONANCE
// Mobile-first landscape edition
// Zibekezelele: patient art endures like stars
// ═══════════════════════════════════════════════════════

import * as THREE from 'three';

// ── DOM ────────────────────────────────────────────────
const $ = id => document.getElementById(id);
const loadingScreen       = $('loading-screen');
const messageDisplay      = $('message-display');
const umsindoFill         = $('umsindo-fill');
const isithunziFill       = $('isithunzi-fill');
const equilibriumIndicator= $('equilibrium-indicator');
const logicGridOverlay    = $('logic-grid-overlay');
const gridCanvas          = $('grid-canvas');
const gridCtx             = gridCanvas.getContext('2d');
const seedCounter         = $('seed-counter');
const joystickZone        = $('joystick-zone');
const joystickKnob        = $('joystick-knob');

// ── RENDERER ───────────────────────────────────────────
const canvas = $('render-canvas');
const renderer = new THREE.WebGLRenderer({ canvas, antialias: true });
renderer.setPixelRatio(Math.min(window.devicePixelRatio, 2));
renderer.setSize(window.innerWidth, window.innerHeight);
renderer.shadowMap.enabled = true;
renderer.shadowMap.type = THREE.PCFSoftShadowMap;
renderer.toneMapping = THREE.ACESFilmicToneMapping;
renderer.toneMappingExposure = 1.2;

const scene = new THREE.Scene();
scene.background = new THREE.Color('#020509');
scene.fog = new THREE.FogExp2('#050a1a', 0.022);

const camera = new THREE.PerspectiveCamera(72, window.innerWidth / window.innerHeight, 0.1, 200);
camera.position.set(0, 1.7, 8);

// ── LIGHTING ───────────────────────────────────────────
scene.add(new THREE.AmbientLight('#1a2a5a', 0.5));

const moonLight = new THREE.DirectionalLight('#8ab4e8', 0.65);
moonLight.position.set(-8, 18, 5);
moonLight.castShadow = true;
moonLight.shadow.mapSize.set(1024, 1024);
scene.add(moonLight);

const fireLight = new THREE.PointLight('#e8942a', 1.2, 15);
fireLight.position.set(0, 1.5, -2);
scene.add(fireLight);

// ══════════════════════════════
// AUDIO ENGINE
// ══════════════════════════════
class AudioEngine {
  constructor() {
    this.ctx = null;
    this.masterGain = null;
    this.activeOsc = [];
    this.tempo = 108;
    const init = () => {
      if (this.ctx) return;
      this.ctx = new (window.AudioContext || window.webkitAudioContext)();
      this.masterGain = this.ctx.createGain();
      this.masterGain.gain.value = 0.32;
      this.masterGain.connect(this.ctx.destination);
      document.removeEventListener('click',   init);
      document.removeEventListener('keydown', init);
      document.removeEventListener('touchstart', init);
    };
    document.addEventListener('click',      init, { passive:true });
    document.addEventListener('keydown',    init, { passive:true });
    document.addEventListener('touchstart', init, { passive:true });
  }

  playNote(freq, time, dur = 0.2, type = 'triangle') {
    if (!this.ctx) return;
    const osc = this.ctx.createOscillator();
    const gain = this.ctx.createGain();
    osc.type = type;
    osc.frequency.value = freq;
    gain.gain.setValueAtTime(0, time);
    gain.gain.linearRampToValueAtTime(0.2, time + 0.01);
    gain.gain.exponentialRampToValueAtTime(0.001, time + dur);
    osc.connect(gain);
    gain.connect(this.masterGain);
    osc.start(time);
    osc.stop(time + dur + 0.05);
    this.activeOsc.push(osc);
  }

  playPattern(seeds) {
    if (!this.ctx || !seeds.length) return;
    const now = this.ctx.currentTime;
    const step = 60 / this.tempo / 2;
    const types = ['triangle', 'sine', 'sawtooth'];
    seeds.forEach((s, i) => {
      if (!s) return;
      this.playNote(s.frequency, now + i * step, 0.25, types[i % 3]);
      this.playNote(s.frequency * 2, now + i * step + 0.05, 0.1, 'sine');
    });
  }

  playDrone(baseFreq = 55) {
    if (!this.ctx) return;
    const osc = this.ctx.createOscillator();
    const gain = this.ctx.createGain();
    osc.type = 'sine';
    osc.frequency.value = baseFreq;
    gain.gain.value = 0.035;
    osc.connect(gain);
    gain.connect(this.masterGain);
    osc.start();
  }

  stopAll() {
    this.activeOsc.forEach(o => { try { o.stop(); } catch(e){} });
    this.activeOsc = [];
  }
}

// ══════════════════════════════
// BALANCE SYSTEM
// ══════════════════════════════
class BalanceSystem {
  constructor() { this.umsindo = 0.5; this.isithunzi = 0.5; }

  modify(axis, amt) {
    const cl = v => Math.min(1, Math.max(0, v));
    if (axis === 'thunder')   this.umsindo   = cl(this.umsindo   + amt);
    if (axis === 'river')     this.umsindo   = cl(this.umsindo   - amt);
    if (axis === 'self')      this.isithunzi = cl(this.isithunzi + amt);
    if (axis === 'ancestral') this.isithunzi = cl(this.isithunzi - amt);
    this._ui();
  }

  getState() { return { umsindo: this.umsindo, isithunzi: this.isithunzi }; }
  isBalanced() { return Math.abs(this.umsindo - this.isithunzi) < 0.15; }

  _ui() {
    umsindoFill.style.width   = `${this.umsindo * 100}%`;
    isithunziFill.style.width = `${this.isithunzi * 100}%`;
    equilibriumIndicator.classList.toggle('balanced', this.isBalanced());
  }
}

// ══════════════════════════════
// WORLD BUILDER
// ══════════════════════════════
class WorldBuilder {
  constructor(scene, balance) {
    this.scene = scene;
    this.balance = balance;
    this.seedObjs = [];
    this.collected = 0;
    this._build();
  }

  _build() {
    // Ground
    const ground = new THREE.Mesh(
      new THREE.CircleGeometry(18, 80),
      new THREE.MeshStandardMaterial({ color:'#0a0f1a', roughness:.95, metalness:.04 })
    );
    ground.rotation.x = -Math.PI / 2;
    ground.receiveShadow = true;
    this.scene.add(ground);

    // Zulu ground lines
    for (let i = -14; i <= 14; i += 2.5) {
      const l = new THREE.Mesh(
        new THREE.BoxGeometry(.04, .005, 28),
        new THREE.MeshStandardMaterial({ color:'#1a2440', emissive:'#0a1228', emissiveIntensity:.3 })
      );
      l.position.set(i, .005, 0);
      this.scene.add(l);
    }

    // Starfield dome
    const sv = new Float32Array(1400 * 3);
    for (let i = 0; i < sv.length; i += 3) {
      const th = Math.random() * Math.PI * 2;
      const ph = Math.random() * Math.PI;
      const r  = 80 + Math.random() * 20;
      sv[i]   = r * Math.sin(ph) * Math.cos(th);
      sv[i+1] = Math.abs(r * Math.cos(ph)) + 5;
      sv[i+2] = r * Math.sin(ph) * Math.sin(th);
    }
    const sg = new THREE.BufferGeometry();
    sg.setAttribute('position', new THREE.BufferAttribute(sv, 3));
    this.stars = new THREE.Points(sg, new THREE.PointsMaterial({ color:'#f0eedd', size:.17, sizeAttenuation:true, transparent:true, opacity:.88 }));
    this.scene.add(this.stars);

    this._baobab(0, 0, -2);
    this._stones();
    this._fire();
    this._wisps();
    this._boundary();
  }

  _baobab(x, y, z) {
    const g = new THREE.Group();
    const m = new THREE.MeshStandardMaterial({ color:'#080d18', roughness:.95, emissive:'#0a1228', emissiveIntensity:.2 });
    const trunk = new THREE.Mesh(new THREE.CylinderGeometry(.28,.55,4.5,20), m);
    trunk.position.y = 2.25; trunk.castShadow = true;
    g.add(trunk);
    for (let i = 0; i < 7; i++) {
      const a = (i/7)*Math.PI*2;
      const br = new THREE.Mesh(new THREE.CylinderGeometry(.06,.16,2.2,8), m);
      br.position.set(Math.cos(a)*.4, 4.2, Math.sin(a)*.4);
      br.rotation.z = (Math.random()-.5)*1.8;
      br.rotation.y = a;
      g.add(br);
    }
    g.position.set(x,y,z);
    this.scene.add(g);
  }

  _stones() {
    const sm = new THREE.MeshStandardMaterial({ color:'#12192e', roughness:.9, emissive:'#0d1526', emissiveIntensity:.3 });
    const gm = new THREE.MeshBasicMaterial({ color:'#f5c842', transparent:true, opacity:.11, side:THREE.DoubleSide });
    for (let i = 0; i < 8; i++) {
      const a = (i/8)*Math.PI*2, r = 5.5;
      const s = new THREE.Mesh(new THREE.DodecahedronGeometry(.32), sm);
      s.position.set(Math.cos(a)*r, .22, Math.sin(a)*r - 1);
      s.rotation.set(Math.random(), Math.random(), Math.random());
      s.castShadow = s.receiveShadow = true;
      this.scene.add(s);
      const gr = new THREE.Mesh(new THREE.RingGeometry(.35,.45,16), gm);
      gr.rotation.x = -Math.PI/2;
      gr.position.set(Math.cos(a)*r, .01, Math.sin(a)*r - 1);
      this.scene.add(gr);
    }
  }

  _fire() {
    const fm = new THREE.MeshBasicMaterial({ color:'#f5c842', transparent:true, opacity:.6 });
    this.fire = new THREE.Mesh(new THREE.CircleGeometry(.5,24), fm);
    this.fire.rotation.x = -Math.PI/2;
    this.fire.position.set(0,.02,-2);
    this.scene.add(this.fire);
    const em = new THREE.MeshBasicMaterial({ color:'#e8942a' });
    for (let i = 0; i < 5; i++) {
      const e = new THREE.Mesh(new THREE.SphereGeometry(.08,8,8), em);
      e.position.set((Math.random()-.5)*.3, .15+Math.random()*.4, -2+(Math.random()-.5)*.3);
      this.scene.add(e);
    }
  }

  _wisps() {
    const data = [
      { name:'Grandfather Drum', freq:110, col:'#8ab4e8', em:'#4a6bb0', pos:[ 3.2,1.5, 1.2] },
      { name:'River Song',       freq:165, col:'#f5c842', em:'#b8960f', pos:[-3.1,1.3, 2.1] },
      { name:'Wind Whisper',     freq:220, col:'#e8942a', em:'#8a4a10', pos:[ 2.3,1.9,-3.2] },
      { name:'Ancestor Chant',   freq:277, col:'#c084fc', em:'#6a20c0', pos:[-2.2,1.4,-2.1] },
      { name:'Earth Pulse',      freq:330, col:'#4ade80', em:'#16803a', pos:[ 4.1,1.2,-1.3] },
    ];
    const wg = new THREE.SphereGeometry(.14,20,20);
    data.forEach(d => {
      const mat = new THREE.MeshStandardMaterial({
        color:d.col, emissive:d.em, emissiveIntensity:.8,
        roughness:.1, metalness:.3, transparent:true, opacity:.92
      });
      const wisp = new THREE.Mesh(wg, mat);
      wisp.position.set(...d.pos);
      wisp.userData = { seed:{ name:d.name, frequency:d.freq }, collected:false, baseY:d.pos[1] };
      this.scene.add(wisp);
      this.seedObjs.push(wisp);
      // orbital ring
      const ring = new THREE.Mesh(
        new THREE.TorusGeometry(.25,.02,8,32),
        new THREE.MeshBasicMaterial({ color:d.col, transparent:true, opacity:.38 })
      );
      ring.position.set(...d.pos);
      this.scene.add(ring);
      wisp.userData.ring = ring;
    });
  }

  _boundary() {
    const m = new THREE.MeshStandardMaterial({ color:'#1a2440', emissive:'#f5c842', emissiveIntensity:.13, roughness:.7 });
    for (let i = 0; i < 12; i++) {
      const a = (i/12)*Math.PI*2;
      const mk = new THREE.Mesh(new THREE.ConeGeometry(.25,1.6,8), m);
      mk.position.set(Math.cos(a)*9, .8, Math.sin(a)*9);
      this.scene.add(mk);
    }
  }

  getSeedAt(pos) {
    for (const w of this.seedObjs) {
      if (!w.userData.collected && w.position.distanceTo(pos) < 2.3) {
        w.userData.collected = true;
        w.visible = false;
        if (w.userData.ring) w.userData.ring.visible = false;
        this.collected++;
        seedCounter.textContent = this.collected;
        return w.userData.seed;
      }
    }
    return null;
  }

  update(t) {
    this.seedObjs.forEach((w, i) => {
      if (w.userData.collected) return;
      w.position.y = w.userData.baseY + Math.sin(t*1.8 + i*1.3)*.28;
      w.rotation.y += .015;
      if (w.userData.ring) {
        w.userData.ring.position.y = w.position.y;
        w.userData.ring.rotation.y += .02;
        w.userData.ring.rotation.x = Math.sin(t + i)*.5;
      }
    });
    if (this.fire) {
      this.fire.material.opacity = .5 + Math.sin(t*8)*.12;
      fireLight.intensity = 1.0 + Math.sin(t*6.5)*.35;
    }
    if (this.stars) this.stars.rotation.y = t*.003;
    const s = this.balance.getState();
    moonLight.color.set(s.umsindo > .7 ? '#e8942a' : s.umsindo < .3 ? '#8ab4e8' : '#8ab4e8');
  }
}

// ══════════════════════════════
// LOGIC GRID — STAR MAP
// ══════════════════════════════
class LogicGrid {
  constructor(audio) {
    this.audio = audio;
    this.slots = Array(8).fill(null);
    this._draw();
    this._bind();
  }

  _draw() {
    const ctx = gridCtx, w = gridCanvas.width, h = gridCanvas.height;
    ctx.fillStyle = '#020509'; ctx.fillRect(0,0,w,h);
    const nb = ctx.createRadialGradient(w/2,h/2,8,w/2,h/2,w/2);
    nb.addColorStop(0,'rgba(74,32,112,.18)'); nb.addColorStop(1,'rgba(0,0,0,0)');
    ctx.fillStyle = nb; ctx.fillRect(0,0,w,h);

    const cw = (w-32)/8;
    ctx.strokeStyle = 'rgba(245,200,66,.16)'; ctx.lineWidth = 1;
    for (let i = 0; i <= 8; i++) {
      ctx.beginPath(); ctx.moveTo(i*cw+16,16); ctx.lineTo(i*cw+16,h-16); ctx.stroke();
    }
    for (let j = 0; j <= 2; j++) {
      const y = j*((h-32)/2)+16;
      ctx.beginPath(); ctx.moveTo(16,y); ctx.lineTo(w-16,y); ctx.stroke();
    }
    this.slots.forEach((seed,i) => {
      const x = i*cw+16+cw/2, y = h/2+12;
      if (seed) {
        const grd = ctx.createRadialGradient(x,y-18,2,x,y-18,20);
        grd.addColorStop(0,'rgba(245,200,66,.55)'); grd.addColorStop(1,'rgba(245,200,66,0)');
        ctx.fillStyle = grd; ctx.fillRect(x-20,y-38,40,40);
        ctx.font = 'bold 20px serif'; ctx.fillStyle = '#f5c842'; ctx.textAlign = 'center';
        ctx.fillText('✦', x, y-6);
        ctx.font = '9px sans-serif'; ctx.fillStyle = 'rgba(240,238,221,.65)';
        ctx.fillText(seed.name.split(' ')[0], x, y+7);
      } else {
        ctx.beginPath(); ctx.arc(x,y-12,5,0,Math.PI*2);
        ctx.strokeStyle='rgba(138,180,232,.14)'; ctx.lineWidth=1; ctx.stroke();
      }
    });
  }

  addSeed(seed) {
    const s = this.slots.findIndex(x=>x===null);
    if (s !== -1) this.slots[s] = seed; else this.slots[0] = seed;
    this._draw();
  }
  play() { this.audio.playPattern(this.slots.filter(Boolean)); }
  clear() { this.slots = Array(8).fill(null); this._draw(); }

  _bind() {
    $('play-composition').addEventListener('click', () => this.play());
    $('stop-composition').addEventListener('click', () => this.audio.stopAll());
    $('clear-grid').addEventListener('click',  () => this.clear());
    $('exit-grid').addEventListener('click',   () => logicGridOverlay.classList.remove('visible'));
    gridCanvas.addEventListener('click', e => {
      const r = gridCanvas.getBoundingClientRect();
      const xi = Math.floor((e.clientX - r.left - 16) / ((gridCanvas.width-32)/8));
      if (xi >= 0 && xi < 8 && this.slots[xi]) { this.slots[xi] = null; this._draw(); }
    });
  }
}

// ══════════════════════════════
// PLAYER CONTROLLER (desktop + mobile joystick)
// ══════════════════════════════
class PlayerController {
  constructor(camera) {
    this.camera = camera;
    this.speed  = 0.09;
    this.lookSp = 0.0018;
    this.keys   = {};
    this.locked = false;
    this.euler  = new THREE.Euler(0,0,0,'YXZ');
    // Mobile joystick state
    this.jx = 0; this.jy = 0; // -1..1
    // Mobile look state
    this.lookDx = 0; this.lookDy = 0;
    this._setupKeyboard();
    this._setupPointerLock();
    this._setupMobileJoystick();
    this._setupMobileLook();
  }

  _setupKeyboard() {
    document.addEventListener('keydown', e => {
      this.keys[e.key.toLowerCase()] = true;
      if (e.key==='g'||e.key==='G') logicGridOverlay.classList.toggle('visible');
    });
    document.addEventListener('keyup', e => { this.keys[e.key.toLowerCase()] = false; });
    document.addEventListener('mousemove', e => {
      if (!this.locked) return;
      this.euler.setFromQuaternion(this.camera.quaternion);
      this.euler.y -= e.movementX * this.lookSp;
      this.euler.x  = Math.max(-Math.PI/3, Math.min(Math.PI/3, this.euler.x - e.movementY * this.lookSp));
      this.camera.quaternion.setFromEuler(this.euler);
    });
  }

  _setupPointerLock() {
    canvas.addEventListener('click', () => {
      if (!isMobile()) canvas.requestPointerLock();
    });
    document.addEventListener('pointerlockchange', () => {
      this.locked = document.pointerLockElement === canvas;
    });
  }

  _setupMobileJoystick() {
    // Track touches that start inside the joystick zone (left 45% of screen)
    const JR = parseFloat(getComputedStyle(document.documentElement).getPropertyValue('--jz') || '110') / 2;
    let jTouchId = null;
    let jOriginX, jOriginY;

    const getZoneCenter = () => {
      const r = joystickZone.getBoundingClientRect();
      return { x: r.left + r.width/2, y: r.top + r.height/2 };
    };

    document.addEventListener('touchstart', e => {
      if (!isMobile()) return;
      for (const t of e.changedTouches) {
        // Left 45% of screen → joystick
        if (t.clientX < window.innerWidth * 0.45 && jTouchId === null) {
          jTouchId = t.identifier;
          const c = getZoneCenter();
          jOriginX = c.x; jOriginY = c.y;
          joystickZone.style.opacity = '1';
        }
      }
    }, { passive:true });

    document.addEventListener('touchmove', e => {
      if (!isMobile()) return;
      for (const t of e.changedTouches) {
        if (t.identifier === jTouchId) {
          const maxR = parseFloat(getComputedStyle(document.documentElement)
            .getPropertyValue('--jz').trim()) * 0.38 || 42;
          let dx = t.clientX - jOriginX;
          let dy = t.clientY - jOriginY;
          const dist = Math.sqrt(dx*dx + dy*dy);
          if (dist > maxR) { dx *= maxR/dist; dy *= maxR/dist; }
          this.jx = dx / maxR;
          this.jy = dy / maxR;
          joystickKnob.style.transform = `translate(calc(-50% + ${dx}px), calc(-50% + ${dy}px))`;
        }
      }
    }, { passive:true });

    const endJoy = e => {
      for (const t of e.changedTouches) {
        if (t.identifier === jTouchId) {
          jTouchId = null;
          this.jx = 0; this.jy = 0;
          joystickKnob.style.transform = 'translate(-50%,-50%)';
          joystickZone.style.opacity = '0.7';
        }
      }
    };
    document.addEventListener('touchend',    endJoy, { passive:true });
    document.addEventListener('touchcancel', endJoy, { passive:true });
  }

  _setupMobileLook() {
    // Right 55% of screen (excluding buttons) = look drag
    let lTouchId = null, lLastX, lLastY;

    document.addEventListener('touchstart', e => {
      if (!isMobile()) return;
      if (logicGridOverlay.classList.contains('visible')) return;
      for (const t of e.changedTouches) {
        if (t.clientX >= window.innerWidth * 0.45 && lTouchId === null) {
          // Exclude button areas (right 80px, bottom 220px)
          const fromRight  = window.innerWidth - t.clientX;
          const fromBottom = window.innerHeight - t.clientY;
          if (fromRight < 82 && fromBottom < 230) continue; // action buttons
          lTouchId = t.identifier;
          lLastX = t.clientX; lLastY = t.clientY;
        }
      }
    }, { passive:true });

    document.addEventListener('touchmove', e => {
      if (!isMobile() || lTouchId === null) return;
      for (const t of e.changedTouches) {
        if (t.identifier === lTouchId) {
          const dx = t.clientX - lLastX;
          const dy = t.clientY - lLastY;
          lLastX = t.clientX; lLastY = t.clientY;
          const spd = 0.004;
          this.euler.setFromQuaternion(this.camera.quaternion);
          this.euler.y -= dx * spd;
          this.euler.x  = Math.max(-Math.PI/3, Math.min(Math.PI/3, this.euler.x - dy * spd));
          this.camera.quaternion.setFromEuler(this.euler);
        }
      }
    }, { passive:true });

    const endLook = e => {
      for (const t of e.changedTouches) {
        if (t.identifier === lTouchId) lTouchId = null;
      }
    };
    document.addEventListener('touchend',    endLook, { passive:true });
    document.addEventListener('touchcancel', endLook, { passive:true });
  }

  update() {
    const dir   = new THREE.Vector3();
    const right = new THREE.Vector3();
    this.camera.getWorldDirection(dir);
    right.crossVectors(this.camera.up, dir).normalize();

    // Keyboard
    if (this.locked) {
      if (this.keys['w']) this.camera.position.addScaledVector(dir,   this.speed);
      if (this.keys['s']) this.camera.position.addScaledVector(dir,  -this.speed);
      if (this.keys['a']) this.camera.position.addScaledVector(right,  this.speed);
      if (this.keys['d']) this.camera.position.addScaledVector(right, -this.speed);
    }

    // Joystick
    if (isMobile() && (this.jx !== 0 || this.jy !== 0)) {
      this.camera.position.addScaledVector(dir,  -this.jy * this.speed);
      this.camera.position.addScaledVector(right, -this.jx * this.speed);
    }

    // Clamp to sacred circle
    const p = this.camera.position;
    const d = Math.sqrt(p.x*p.x + p.z*p.z);
    if (d > 8) { p.x *= 8/d; p.z *= 8/d; }
    p.y = 1.7;
  }
}

// ══════════════════════════════
// SKETCH MECHANIC
// ══════════════════════════════
class SketchMechanic {
  constructor() {
    this.active = false;
    this.prog   = 0;
    document.addEventListener('keydown', e => { if (e.code==='Space') { e.preventDefault(); this.start(); } });
    document.addEventListener('keyup',   e => { if (e.code==='Space') this.stop(); });
  }
  start() { if (this.active) return; this.active=true; this.prog=0; msg('✦ Sketching the stellar resonance…'); }
  stop()  { this.active=false; this.prog=0; hideMsg(); }
  update(camera, world, grid) {
    if (!this.active) return;
    this.prog += 0.018;
    if (this.prog >= 1) {
      const s = world.getSeedAt(camera.position);
      if (s) { grid.addSeed(s); msg(`✦ Uthole: ${s.name}`); setTimeout(hideMsg, 3000); }
      this.stop();
    }
  }
}

// ══════════════════════════════
// HELPERS
// ══════════════════════════════
function isMobile() {
  return window.matchMedia('(pointer:coarse)').matches || window.innerWidth < 900;
}
function msg(text)  { messageDisplay.textContent = text; messageDisplay.classList.add('show'); }
function hideMsg()  { messageDisplay.classList.remove('show'); }

// ══════════════════════════════
// GAME INIT
// ══════════════════════════════
async function init() {
  try {
    const audio   = new AudioEngine();
    const balance = new BalanceSystem();
    const world   = new WorldBuilder(scene, balance);
    const grid    = new LogicGrid(audio);
    const player  = new PlayerController(camera);
    const sketch  = new SketchMechanic();

    // Mobile action buttons
    $('btn-collect').addEventListener('click', () => {
      const s = world.getSeedAt(camera.position);
      if (s) { grid.addSeed(s); msg(`✦ Uthole: ${s.name}`); setTimeout(hideMsg,3000); }
      else   { msg('✦ Sondela — draw near to a star-seed'); setTimeout(hideMsg,2000); }
    });
    $('btn-grid').addEventListener('click', () => logicGridOverlay.classList.toggle('visible'));
    $('btn-sketch').addEventListener('click', () => { sketch.start(); setTimeout(()=>sketch.stop(),3000); });

    // Balance nudge (mobile)
    $('btn-thunder').addEventListener('click', () => { balance.modify('thunder',.08); balance.modify('self',.08); });
    $('btn-river').addEventListener('click',   () => { balance.modify('river',.08); balance.modify('ancestral',.08); });

    // Keyboard balance
    document.addEventListener('keydown', e => {
      if (e.key==='q'||e.key==='Q') { balance.modify('thunder',.08); balance.modify('self',.08); }
      if (e.key==='r'||e.key==='R') { balance.modify('river',.08); balance.modify('ancestral',.08); }
      if (e.key==='e'||e.key==='E') {
        const s = world.getSeedAt(camera.position);
        if (s) { grid.addSeed(s); msg(`✦ Uthole umsindo: ${s.name}`); setTimeout(hideMsg,3000); }
      }
    });

    audio.playDrone(55);

    let t = 0;
    function loop() {
      requestAnimationFrame(loop);
      t += 0.016;
      player.update();
      world.update(t);
      sketch.update(camera, world, grid);
      renderer.render(scene, camera);
    }

    setTimeout(() => {
      loadingScreen.classList.add('hidden');
      msg('✦ Wamkelekile — Welcome to the ancestral star-realm');
      setTimeout(hideMsg, 4000);
      loop();
    }, 1800);

    window.addEventListener('resize', () => {
      camera.aspect = window.innerWidth / window.innerHeight;
      camera.updateProjectionMatrix();
      renderer.setSize(window.innerWidth, window.innerHeight);
    }, { passive:true });

  } catch(err) {
    console.error('Vuvu Nkanyezi error:', err);
    loadingScreen.innerHTML = `<div style="color:#e8942a;font-family:serif;text-align:center;padding:2rem"><p>✦</p><p style="margin-top:1rem">The stars could not align. Please refresh.</p></div>`;
  }
}

init();
</script>

</body>
</html>
