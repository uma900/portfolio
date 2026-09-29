<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Venkata Uma Mahesh | VLSI & Embedded Systems Engineer</title>
  <meta name="description" content="Portfolio of Venkata Uma Mahesh Tamarana - ECE Undergraduate (AIoT), VLSI Design Intern, and Hardware Innovator." />

  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Sora:wght@300;400;500;600;700;800&family=Inter:wght@300;400;500;600;700&family=JetBrains+Mono:wght@400;500;600&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

  <style>
    :root {
      --bg: #0f0a1f;
      --surface: #1c1438;
      --surface-2: #241a45;
      --border: rgba(167, 139, 250, 0.18);
      --border-hover: rgba(167, 139, 250, 0.5);

      --violet-200: #ddd6fe;
      --violet-300: #c4b5fd;
      --violet-400: #a78bfa;
      --violet-500: #8b5cf6;
      --violet-600: #7c3aed;
      --fuchsia: #d946ef;
      --amber: #fbbf24;

      --text: #f5f3ff;
      --text-muted: #a89bc4;
      --text-dim: #786a96;

      --font-sans: 'Inter', -apple-system, sans-serif;
      --font-display: 'Sora', sans-serif;
      --font-mono: 'JetBrains Mono', monospace;

      --radius: 14px;
      --radius-sm: 10px;
      --transition: all 0.25s ease;
    }

    * { margin: 0; padding: 0; box-sizing: border-box; }
    html { scroll-behavior: smooth; }

    /* ─── Custom Cursor (Logic Gate) ─── */
    body, a, button, .card, .tag, .skill-block, .social-btn, .modal-close, .timeline-item, .project-card {
      cursor: none !important;
    }

    .cursor-gate {
      position: fixed;
      top: 0; left: 0;
      width: 34px; height: 34px;
      pointer-events: none;
      z-index: 9999;
      transform: translate(-50%, -50%);
      transition: transform 0.15s ease, opacity 0.2s ease;
      filter: drop-shadow(0 0 6px rgba(167, 139, 250, 0.9));
    }
    .cursor-gate svg {
      width: 100%; height: 100%;
      display: block;
    }
    .cursor-gate svg path,
    .cursor-gate svg line,
    .cursor-gate svg circle,
    .cursor-gate svg polygon {
      stroke: var(--violet-300);
      stroke-width: 1.8;
      fill: none;
      transition: stroke 0.2s ease;
    }
    .cursor-gate.hover svg path,
    .cursor-gate.hover svg line,
    .cursor-gate.hover svg circle,
    .cursor-gate.hover svg polygon {
      stroke: var(--fuchsia);
    }
    .cursor-gate.hover {
      transform: translate(-50%, -50%) scale(1.35) rotate(6deg);
    }

    /* Small trailing dot for accuracy */
    .cursor-dot {
      position: fixed;
      top: 0; left: 0;
      width: 5px; height: 5px;
      background: var(--fuchsia);
      border-radius: 50%;
      pointer-events: none;
      z-index: 9998;
      transform: translate(-50%, -50%);
      box-shadow: 0 0 8px rgba(217, 70, 239, 0.9);
    }

    @media (pointer: coarse) {
      body, a, button, .card, .tag, .skill-block, .social-btn, .modal-close, .timeline-item, .project-card {
        cursor: auto !important;
      }
      .cursor-gate, .cursor-dot { display: none; }
    }

    /* ─── Body with Electronics Circuit Background ─── */
    body {
      background-color: var(--bg);
      background-image:
        /* Base radial gradients */
        radial-gradient(circle at 15% 10%, rgba(139, 92, 246, 0.14), transparent 45%),
        radial-gradient(circle at 85% 80%, rgba(217, 70, 239, 0.09), transparent 45%),
        /* Circuit grid lines */
        linear-gradient(rgba(167, 139, 250, 0.055) 1px, transparent 1px),
        linear-gradient(90deg, rgba(167, 139, 250, 0.055) 1px, transparent 1px),
        /* Fine dot pattern (PCB vias) */
        radial-gradient(rgba(167, 139, 250, 0.18) 1.2px, transparent 1.2px);
      background-size:
        100% 100%,
        100% 100%,
        42px 42px,
        42px 42px,
        42px 42px;
      background-position:
        0 0,
        0 0,
        0 0,
        0 0,
        0 0;
      background-attachment: fixed;
      color: var(--text);
      font-family: var(--font-sans);
      line-height: 1.65;
      -webkit-font-smoothing: antialiased;
      overflow-x: hidden;
    }

    /* Decorative circuit overlay using SVG pattern */
    .circuit-bg {
      position: fixed;
      inset: 0;
      z-index: -1;
      pointer-events: none;
      opacity: 0.55;
      background-image: url("data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' width='260' height='260' viewBox='0 0 260 260'><g fill='none' stroke='%23a78bfa' stroke-width='1' opacity='0.35'><path d='M 20 20 H 100 V 60 H 160 V 30 H 220'/><path d='M 40 120 H 90 V 180 H 180 V 140 H 240'/><path d='M 20 220 H 80 V 240 H 200 V 200 H 240'/><circle cx='100' cy='60' r='3'/><circle cx='160' cy='30' r='3'/><circle cx='90' cy='180' r='3'/><circle cx='180' cy='140' r='3'/><circle cx='80' cy='240' r='3'/><circle cx='200' cy='200' r='3'/><rect x='112' y='52' width='18' height='16' rx='2'/><rect x='100' y='172' width='18' height='16' rx='2'/></g></svg>");
      background-repeat: repeat;
      animation: circuitMove 60s linear infinite;
    }
    @keyframes circuitMove {
      from { background-position: 0 0; }
      to { background-position: 260px 260px; }
    }

    /* ─── Navigation ─── */
    nav {
      position: sticky;
      top: 0;
      z-index: 100;
      background: rgba(15, 10, 31, 0.85);
      backdrop-filter: blur(20px);
      -webkit-backdrop-filter: blur(20px);
      border-bottom: 1px solid var(--border);
    }
    .nav-inner {
      max-width: 1180px;
      margin: 0 auto;
      padding: 1rem 1.5rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
    .logo {
      font-family: var(--font-display);
      font-size: 1.05rem;
      font-weight: 700;
      color: var(--text);
      text-decoration: none;
      display: flex;
      align-items: center;
      gap: 0.55rem;
    }
    .logo-dot {
      width: 10px; height: 10px;
      border-radius: 50%;
      background: linear-gradient(135deg, var(--violet-400), var(--fuchsia));
      box-shadow: 0 0 12px rgba(167, 139, 250, 0.6);
    }
    .nav-links {
      display: flex;
      gap: 1.6rem;
      list-style: none;
    }
    .nav-links a {
      color: var(--text-muted);
      text-decoration: none;
      font-size: 0.86rem;
      font-weight: 500;
      transition: var(--transition);
    }
    .nav-links a:hover { color: var(--violet-300); }

    /* ─── Layout ─── */
    .container {
      max-width: 1180px;
      margin: 0 auto;
      padding: 0 1.5rem;
    }
    section {
      padding: 5rem 0;
      border-bottom: 1px solid rgba(167, 139, 250, 0.06);
    }

    /* ─── Section Header ─── */
    .section-head {
      display: grid;
      grid-template-columns: auto 1fr auto;
      align-items: baseline;
      gap: 1.25rem;
      margin-bottom: 2.75rem;
      padding-bottom: 1rem;
      border-bottom: 1px dashed rgba(167, 139, 250, 0.15);
    }
    .section-num {
      font-family: var(--font-mono);
      font-size: 0.78rem;
      color: var(--violet-400);
      letter-spacing: 0.1em;
    }
    .section-head h2 {
      font-family: var(--font-display);
      font-size: 1.65rem;
      font-weight: 700;
      letter-spacing: -0.02em;
      color: var(--text);
    }
    .section-head .section-note {
      font-family: var(--font-mono);
      font-size: 0.72rem;
      color: var(--text-dim);
      text-transform: uppercase;
      letter-spacing: 0.1em;
    }

    /* ─── Hero ─── */
    .hero { padding: 4rem 0 5rem; }
    .hero-grid {
      display: grid;
      grid-template-columns: 1.4fr 1fr;
      gap: 4rem;
      align-items: center;
    }
    .hero-tag {
      display: inline-flex;
      align-items: center;
      gap: 0.5rem;
      background: rgba(139, 92, 246, 0.1);
      border: 1px solid var(--border);
      color: var(--violet-300);
      padding: 0.4rem 0.9rem;
      border-radius: 999px;
      font-family: var(--font-mono);
      font-size: 0.72rem;
      margin-bottom: 1.4rem;
    }
    .hero h1 {
      font-family: var(--font-display);
      font-size: 3rem;
      font-weight: 800;
      line-height: 1.12;
      letter-spacing: -0.03em;
      margin-bottom: 1.25rem;
    }
    .hero h1 .accent {
      background: linear-gradient(120deg, var(--violet-400) 0%, var(--fuchsia) 100%);
      -webkit-background-clip: text;
      -webkit-text-fill-color: transparent;
    }
    .hero p {
      font-size: 1rem;
      color: var(--text-muted);
      max-width: 540px;
      margin-bottom: 2rem;
    }
    .hero-actions {
      display: flex;
      flex-wrap: wrap;
      gap: 0.7rem;
    }

    .btn {
      padding: 0.72rem 1.3rem;
      border-radius: var(--radius-sm);
      font-size: 0.88rem;
      font-weight: 600;
      text-decoration: none;
      display: inline-flex;
      align-items: center;
      gap: 0.5rem;
      cursor: none;
      border: 1px solid transparent;
      transition: var(--transition);
      font-family: var(--font-sans);
    }
    .btn-primary {
      background: linear-gradient(135deg, var(--violet-600), var(--violet-500));
      color: #fff;
      box-shadow: 0 6px 20px rgba(124, 58, 237, 0.35);
    }
    .btn-primary:hover {
      transform: translateY(-2px);
      box-shadow: 0 10px 28px rgba(124, 58, 237, 0.5);
    }
    .btn-ghost {
      background: rgba(167, 139, 250, 0.07);
      border-color: var(--border);
      color: var(--violet-200);
    }
    .btn-ghost:hover {
      background: rgba(167, 139, 250, 0.15);
      border-color: var(--border-hover);
      transform: translateY(-2px);
    }

    .hero-photo { display: flex; justify-content: center; }
    .photo-frame {
      position: relative;
      width: 250px;
      height: 250px;
      border-radius: 50%;
      padding: 4px;
      background: conic-gradient(from 200deg, var(--violet-500), var(--fuchsia), var(--violet-500));
      box-shadow: 0 20px 50px rgba(124, 58, 237, 0.3);
    }
    .photo-frame::before {
      content: '';
      position: absolute;
      inset: -8px;
      border-radius: 50%;
      border: 1px dashed rgba(167, 139, 250, 0.28);
      animation: spin 30s linear infinite;
    }
    @keyframes spin { to { transform: rotate(360deg); } }
    .photo-frame img {
      width: 100%;
      height: 100%;
      border-radius: 50%;
      object-fit: cover;
      border: 4px solid var(--bg);
      display: block;
    }

    /* ─── Timeline ─── */
    .timeline {
      position: relative;
      padding-left: 2rem;
    }
    .timeline::before {
      content: '';
      position: absolute;
      left: 7px;
      top: 8px;
      bottom: 8px;
      width: 1px;
      background: linear-gradient(to bottom, var(--violet-500), transparent);
    }
    .timeline-item {
      position: relative;
      padding: 1.25rem 1.5rem;
      margin-bottom: 1.2rem;
      background: var(--surface);
      border: 1px solid var(--border);
      border-radius: var(--radius);
      transition: var(--transition);
      cursor: none;
    }
    .timeline-item::before {
      content: '';
      position: absolute;
      left: -2rem;
      top: 1.6rem;
      width: 15px;
      height: 15px;
      border-radius: 50%;
      background: var(--surface);
      border: 2px solid var(--violet-500);
      box-shadow: 0 0 12px rgba(139, 92, 246, 0.5);
    }
    .timeline-item:hover {
      border-color: var(--border-hover);
      background: var(--surface-2);
      transform: translateX(6px);
    }
    .timeline-item .item-head {
      display: flex;
      justify-content: space-between;
      align-items: flex-start;
      gap: 1rem;
      margin-bottom: 0.45rem;
    }
    .timeline-item .item-title {
      font-family: var(--font-display);
      font-size: 1.08rem;
      font-weight: 600;
      color: var(--text);
      line-height: 1.4;
    }
    .timeline-item .item-date {
      font-family: var(--font-mono);
      font-size: 0.74rem;
      color: var(--violet-400);
      white-space: nowrap;
      padding: 0.2rem 0.6rem;
      background: rgba(139, 92, 246, 0.08);
      border: 1px solid var(--border);
      border-radius: 6px;
    }
    .timeline-item .item-sub {
      font-family: var(--font-mono);
      font-size: 0.78rem;
      color: var(--violet-300);
      margin-bottom: 0.5rem;
      display: flex;
      align-items: center;
      gap: 0.45rem;
    }
    .timeline-item .item-desc {
      font-size: 0.92rem;
      color: var(--text-muted);
      line-height: 1.6;
      margin-bottom: 0.85rem;
    }
    .tag-list {
      display: flex;
      flex-wrap: wrap;
      gap: 0.4rem;
    }
    .tag {
      background: rgba(139, 92, 246, 0.09);
      border: 1px solid var(--border);
      color: var(--violet-200);
      padding: 0.28rem 0.65rem;
      border-radius: 7px;
      font-size: 0.72rem;
      font-family: var(--font-mono);
      transition: var(--transition);
      cursor: none;
    }
    .tag-highlight {
      background: rgba(217, 70, 239, 0.14) !important;
      border-color: rgba(217, 70, 239, 0.45) !important;
      color: #f5b8ff !important;
    }
    .tag-ongoing {
      background: rgba(251, 191, 36, 0.12) !important;
      border-color: rgba(251, 191, 36, 0.4) !important;
      color: #fcd34d !important;
    }

    /* ─── Projects ─── */
    .project-grid {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 1.35rem;
    }
    .project-grid .project-card:first-child {
      grid-column: span 2;
    }
    .project-card {
      background: var(--surface);
      border: 1px solid var(--border);
      border-radius: var(--radius);
      padding: 1.75rem;
      transition: var(--transition);
      cursor: none;
      display: flex;
      flex-direction: column;
      gap: 0.85rem;
      position: relative;
      overflow: hidden;
    }
    .project-card::after {
      content: '';
      position: absolute;
      top: 0; left: 0;
      width: 100%;
      height: 3px;
      background: linear-gradient(90deg, var(--violet-500), var(--fuchsia));
      transform: scaleX(0);
      transform-origin: left;
      transition: transform 0.35s ease;
    }
    .project-card:hover {
      background: var(--surface-2);
      border-color: var(--border-hover);
      transform: translateY(-4px);
      box-shadow: 0 16px 40px rgba(0, 0, 0, 0.4);
    }
    .project-card:hover::after { transform: scaleX(1); }
    .project-card .p-head {
      display: flex;
      justify-content: space-between;
      align-items: flex-start;
      gap: 0.85rem;
    }
    .project-card .p-title {
      font-family: var(--font-display);
      font-size: 1.12rem;
      font-weight: 600;
      color: var(--text);
      line-height: 1.4;
    }
    .project-card .p-meta {
      font-family: var(--font-mono);
      font-size: 0.76rem;
      color: var(--violet-400);
      display: flex;
      align-items: center;
      gap: 0.4rem;
      margin-bottom: 0.2rem;
    }
    .project-card .p-desc {
      font-size: 0.92rem;
      color: var(--text-muted);
      line-height: 1.6;
    }

    /* ─── Skills ─── */
    .skills-grid {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 1.35rem;
    }
    .skill-block {
      background: var(--surface);
      border: 1px solid var(--border);
      border-radius: var(--radius);
      padding: 1.5rem;
      transition: var(--transition);
    }
    .skill-block:hover {
      border-color: var(--border-hover);
      background: var(--surface-2);
    }
    .skill-block h3 {
      font-family: var(--font-display);
      font-size: 0.95rem;
      font-weight: 600;
      color: var(--violet-200);
      margin-bottom: 1rem;
      display: flex;
      align-items: center;
      gap: 0.5rem;
      padding-bottom: 0.75rem;
      border-bottom: 1px dashed rgba(167, 139, 250, 0.15);
    }
    .skill-block h3 i { color: var(--violet-400); }

    /* ─── About ─── */
    .about-strip {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 2rem;
      padding: 1.75rem;
      background: linear-gradient(135deg, rgba(139, 92, 246, 0.08), rgba(217, 70, 239, 0.04));
      border: 1px solid var(--border);
      border-radius: var(--radius);
    }
    .about-item h4 {
      font-family: var(--font-display);
      font-size: 0.9rem;
      color: var(--violet-300);
      margin-bottom: 0.5rem;
      display: flex;
      align-items: center;
      gap: 0.5rem;
    }
    .about-item p {
      font-size: 0.9rem;
      color: var(--text-muted);
    }

    /* ─── Footer ─── */
    footer {
      padding: 3rem 0 2.5rem;
      text-align: center;
    }
    footer .footer-name {
      font-family: var(--font-display);
      font-size: 1.15rem;
      font-weight: 700;
      color: var(--text);
      margin-bottom: 0.4rem;
    }
    footer .footer-info {
      font-size: 0.88rem;
      color: var(--text-muted);
      margin-bottom: 1.5rem;
    }
    .socials {
      display: flex;
      justify-content: center;
      gap: 0.85rem;
      margin-bottom: 1.5rem;
    }
    .social-btn {
      width: 42px; height: 42px;
      border-radius: 11px;
      background: var(--surface);
      border: 1px solid var(--border);
      color: var(--violet-300);
      display: flex;
      align-items: center;
      justify-content: center;
      text-decoration: none;
      transition: var(--transition);
      font-size: 1.05rem;
    }
    .social-btn:hover {
      background: var(--violet-600);
      color: #fff;
      border-color: var(--violet-500);
      transform: translateY(-3px);
      box-shadow: 0 8px 20px rgba(124, 58, 237, 0.4);
    }
    .copyright {
      font-family: var(--font-mono);
      font-size: 0.76rem;
      color: var(--text-dim);
    }

    /* ─── Modal ─── */
    .modal-overlay {
      position: fixed;
      inset: 0;
      background: rgba(10, 6, 22, 0.85);
      backdrop-filter: blur(12px);
      -webkit-backdrop-filter: blur(12px);
      z-index: 1000;
      display: none;
      align-items: center;
      justify-content: center;
      padding: 1.5rem;
    }
    .modal-overlay.active { display: flex; }
    .modal-card {
      background: var(--surface);
      border: 1px solid var(--border-hover);
      border-radius: var(--radius);
      max-width: 560px;
      width: 100%;
      padding: 2rem;
      position: relative;
      box-shadow: 0 25px 60px rgba(0, 0, 0, 0.6);
      animation: modalIn 0.25s ease;
    }
    @keyframes modalIn {
      from { transform: translateY(16px); opacity: 0; }
      to { transform: translateY(0); opacity: 1; }
    }
    .modal-close {
      position: absolute;
      top: 1rem; right: 1rem;
      width: 34px; height: 34px;
      border-radius: 50%;
      background: rgba(167, 139, 250, 0.08);
      border: 1px solid var(--border);
      color: var(--text-muted);
      display: flex;
      align-items: center;
      justify-content: center;
      cursor: none;
      transition: var(--transition);
    }
    .modal-close:hover {
      background: var(--violet-600);
      color: #fff;
      border-color: var(--violet-500);
    }
    .modal-head {
      display: flex;
      align-items: center;
      gap: 1rem;
      margin-bottom: 1.25rem;
    }
    .modal-icon {
      width: 48px; height: 48px;
      border-radius: 12px;
      background: linear-gradient(135deg, rgba(139, 92, 246, 0.22), rgba(217, 70, 239, 0.12));
      border: 1px solid var(--border);
      display: flex;
      align-items: center;
      justify-content: center;
      color: var(--violet-300);
      font-size: 1.3rem;
      flex-shrink: 0;
    }
    .modal-title {
      font-family: var(--font-display);
      font-size: 1.2rem;
      font-weight: 700;
      color: var(--text);
      line-height: 1.3;
    }
    .modal-sub {
      font-family: var(--font-mono);
      font-size: 0.75rem;
      color: var(--violet-400);
      margin-top: 0.15rem;
    }
    .modal-body {
      color: var(--text-muted);
      font-size: 0.92rem;
      line-height: 1.7;
      margin-bottom: 1.5rem;
    }
    .modal-specs {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 0.85rem;
      padding: 1.1rem;
      background: rgba(15, 10, 31, 0.6);
      border: 1px solid var(--border);
      border-radius: var(--radius-sm);
    }
    .spec-label {
      font-size: 0.7rem;
      color: var(--text-dim);
      text-transform: uppercase;
      letter-spacing: 0.06em;
      margin-bottom: 0.15rem;
    }
    .spec-val {
      font-family: var(--font-mono);
      font-size: 0.82rem;
      color: var(--violet-200);
      font-weight: 500;
    }

    /* ─── Responsive ─── */
    @media (max-width: 900px) {
      .hero-grid { grid-template-columns: 1fr; gap: 2.5rem; text-align: center; }
      .hero p { margin-left: auto; margin-right: auto; }
      .hero-actions { justify-content: center; }
      .hero h1 { font-size: 2.2rem; }
      .nav-links { display: none; }
      .about-strip { grid-template-columns: 1fr; }
      .skills-grid { grid-template-columns: 1fr; }
      .project-grid { grid-template-columns: 1fr; }
      .project-grid .project-card:first-child { grid-column: span 1; }
      .section-head { grid-template-columns: auto 1fr; }
      .section-head .section-note { display: none; }
    }
  </style>
</head>
<body>

  <!-- Custom Logic Gate Cursor (AND gate shape) -->
  <div class="cursor-gate" id="cursorGate">
    <svg viewBox="0 0 40 40" xmlns="http://www.w3.org/2000/svg">
      <!-- AND gate body -->
      <path d="M 6 8 H 20 A 12 12 0 0 1 20 32 H 6 Z" />
      <!-- Input lines -->
      <line x1="0" y1="14" x2="6" y2="14" />
      <line x1="0" y1="26" x2="6" y2="26" />
      <!-- Output line -->
      <line x1="32" y1="20" x2="40" y2="20" />
    </svg>
  </div>
  <div class="cursor-dot" id="cursorDot"></div>

  <!-- Circuit background overlay -->
  <div class="circuit-bg"></div>

  <nav>
    <div class="nav-inner">
      <a href="#" class="logo">
        <span class="logo-dot"></span>
        Venkata Uma Mahesh
      </a>
      <ul class="nav-links">
        <li><a href="#research">Research</a></li>
        <li><a href="#projects">Projects</a></li>
        <li><a href="#internships">Internships</a></li>
        <li><a href="#certifications">Certifications</a></li>
        <li><a href="#skills">Skills</a></li>
        <li><a href="#achievements">Achievements</a></li>
        <li><a href="#education">Education</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </div>
  </nav>

  <!-- Hero -->
  <header class="hero">
    <div class="container hero-grid">
      <div>
        <div class="hero-tag"><i class="fas fa-microchip"></i> VLSI · RTL Verification · AIoT · Embedded</div>
        <h1>Hi, I'm <span class="accent">Venkata Uma Mahesh</span></h1>
        <p>Electronics and Communication Engineering student specializing in AIoT, embedded systems, and VLSI design. Experienced in RTL design using Verilog and building hardware-based solutions.</p>
        <div class="hero-actions">
          <a href="https://www.linkedin.com/in/venkatamamahesh-tamarana-a6418128a" target="_blank" rel="noopener" class="btn btn-primary"><i class="fab fa-linkedin"></i> LinkedIn</a>
          <a href="https://github.com/uma900" target="_blank" rel="noopener" class="btn btn-ghost"><i class="fab fa-github"></i> GitHub</a>
          <a href="mailto:tamaranavenkatamamahesh@gmail.com" class="btn btn-ghost"><i class="fas fa-envelope"></i> Email</a>
        </div>
      </div>
      <div class="hero-photo">
        <div class="photo-frame">
          <img src="profile.jpg" alt="Venkata Uma Mahesh" onerror="this.src='https://github.com/uma900.png';" />
        </div>
      </div>
    </div>
  </header>

  <!-- About -->
  <section>
    <div class="container">
      <div class="section-head">
        <span class="section-num">00 /</span>
        <h2>About</h2>
        <span class="section-note">Quick Intro</span>
      </div>
      <div class="about-strip">
        <div class="about-item">
          <h4><i class="fas fa-bolt"></i> Strengths</h4>
          <p>Problem-Solving · Quick Learner · Adaptable · Disciplined · Self-Motivated</p>
        </div>
        <div class="about-item">
          <h4><i class="fas fa-language"></i> Languages</h4>
          <p>Telugu · English · Hindi · German (Basic)</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Research & IP -->
  <section id="research">
    <div class="container">
      <div class="section-head">
        <span class="section-num">01 /</span>
        <h2>Research & Intellectual Property</h2>
        <span class="section-note">Publication · Patents</span>
      </div>
      <div class="timeline">
        <div class="timeline-item" onclick="openModal('ieee')">
          <div class="item-head">
            <div class="item-title">IEEE Published Research Paper</div>
            <span class="item-date">2025</span>
          </div>
          <div class="item-sub"><i class="fas fa-book"></i> IEEE Xplore</div>
          <p class="item-desc">"A Review of Gesture-Based Wireless Pen Interfaces for Human-Computer Interaction: Sensors, Algorithms, and Applications."</p>
          <div class="tag-list">
            <a href="https://ieeexplore.ieee.org/document/11400200" target="_blank" rel="noopener" onclick="event.stopPropagation()" class="tag tag-highlight">View Paper →</a>
          </div>
        </div>

        <div class="timeline-item" onclick="openModal('pen')">
          <div class="item-head">
            <div class="item-title">Gesture-Based Wireless Pen Interface</div>
            <span class="item-date">19/05/2025</span>
          </div>
          <div class="item-sub"><i class="fas fa-award"></i> Utility Patent · App No: 459423-001</div>
          <p class="item-desc">Utility patent for a wireless pen interface enabling gesture-based human-computer interaction through spatial motion tracking.</p>
          <div class="tag-list">
            <span class="tag">HCI</span><span class="tag">Wireless</span><span class="tag">Gesture Recognition</span>
          </div>
        </div>

        <div class="timeline-item" onclick="openModal('table')">
          <div class="item-head">
            <div class="item-title">IoT Smart Table Call & Tracking</div>
            <span class="item-date">01/04/2026</span>
          </div>
          <div class="item-sub"><i class="fas fa-award"></i> Design Patent · App No: 202611028457</div>
          <p class="item-desc">Design patent for IoT-based smart table call and tracking service automation for restaurant and hospitality environments.</p>
          <div class="tag-list">
            <span class="tag">IoT</span><span class="tag">Automation</span><span class="tag">Hospitality</span>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Projects -->
  <section id="projects">
    <div class="container">
      <div class="section-head">
        <span class="section-num">02 /</span>
        <h2>Featured Projects</h2>
        <span class="section-note">Engineering Work</span>
      </div>
      <div class="project-grid">
        <div class="project-card" onclick="openModal('soc')">
          <div class="p-head">
            <div class="p-title">SoC Architecture using AMBA Protocol</div>
            <span class="tag tag-ongoing">Ongoing · 2026</span>
          </div>
          <div class="p-meta"><i class="fas fa-microchip"></i> VLSI Architecture</div>
          <p class="p-desc">Developing a complete SoC architecture leveraging AMBA bus protocols (AXI, AHB, APB) for on-chip communication between master and slave peripherals.</p>
          <div class="tag-list">
            <span class="tag">AMBA</span><span class="tag">AXI / AHB / APB</span><span class="tag">Verilog RTL</span>
          </div>
        </div>

        <div class="project-card" onclick="openModal('fruit')">
          <div class="p-head">
            <div class="p-title">Deep Learning Fruit Sorting System</div>
            <span class="tag">PLC + Jetson Nano</span>
          </div>
          <div class="p-meta"><i class="fas fa-industry"></i> Edge AI · 2026</div>
          <p class="p-desc">Deep learning-based automated fruit sorting combining Mitsubishi PLC with Nvidia Jetson Nano edge AI inference.</p>
          <div class="tag-list">
            <span class="tag">Jetson Nano</span><span class="tag">PLC</span><span class="tag">Deep Learning</span>
          </div>
        </div>

        <div class="project-card" onclick="openModal('alert')">
          <div class="p-head">
            <div class="p-title">IoT Emergency Alert System</div>
            <span class="tag">ESP32</span>
          </div>
          <div class="p-meta"><i class="fas fa-bell"></i> IoT Safety · 2025</div>
          <p class="p-desc">IoT-based emergency alert system using the ESP32 Wi-Fi module for real-time notifications.</p>
          <div class="tag-list">
            <span class="tag">ESP32</span><span class="tag">Wi-Fi</span><span class="tag">IoT</span>
          </div>
        </div>

        <div class="project-card" onclick="openModal('smarttable')">
          <div class="p-head">
            <div class="p-title">IoT Smart Table Call & Tracking</div>
            <span class="tag">Restaurant IoT</span>
          </div>
          <div class="p-meta"><i class="fas fa-utensils"></i> Service Automation · 2025</div>
          <p class="p-desc">IoT smart table call and tracking system for restaurant automation with real-time order tracking.</p>
          <div class="tag-list">
            <span class="tag">IoT</span><span class="tag">Automation</span><span class="tag">Tracking</span>
          </div>
        </div>

        <div class="project-card" onclick="openModal('prenatal')">
          <div class="p-head">
            <div class="p-title">IoT Prenatal Monitoring System</div>
            <span class="tag tag-highlight">Health Tech</span>
          </div>
          <div class="p-meta"><i class="fas fa-heartbeat"></i> Biomedical IoT · 2024</div>
          <p class="p-desc">IoT-based prenatal monitoring for pregnant women using BPM, vibration, and temperature sensors.</p>
          <div class="tag-list">
            <span class="tag">BPM</span><span class="tag">Vibration</span><span class="tag">Temperature</span>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Internships -->
  <section id="internships">
    <div class="container">
      <div class="section-head">
        <span class="section-num">03 /</span>
        <h2>Internships</h2>
        <span class="section-note">Professional Experience</span>
      </div>
      <div class="timeline">
        <div class="timeline-item" onclick="openModal('hmies')">
          <div class="item-head">
            <div class="item-title">VLSI Intern</div>
            <span class="item-date">Jun 2025</span>
          </div>
          <div class="item-sub"><i class="fas fa-building"></i> HMIES Solutions Pvt. Ltd</div>
          <p class="item-desc">Assisted in RTL design and verification using Verilog and SystemVerilog for digital circuit implementations.</p>
          <div class="tag-list">
            <span class="tag">Verilog</span><span class="tag">SystemVerilog</span><span class="tag">RTL</span>
          </div>
        </div>

        <div class="timeline-item" onclick="openModal('ntpc')">
          <div class="item-head">
            <div class="item-title">Engineering Intern</div>
            <span class="item-date">Jul 2025</span>
          </div>
          <div class="item-sub"><i class="fas fa-industry"></i> NTPC (National Thermal Power Corporation)</div>
          <p class="item-desc">Worked under the turbine and boiler department gaining hands-on exposure to industrial power plant operations and control systems.</p>
          <div class="tag-list">
            <span class="tag">Turbine</span><span class="tag">Boiler</span><span class="tag">Industrial</span>
          </div>
        </div>

        <div class="timeline-item" onclick="openModal('unlox')">
          <div class="item-head">
            <div class="item-title">Intern & Campus Ambassador</div>
            <span class="item-date">Oct 2025</span>
          </div>
          <div class="item-sub"><i class="fas fa-users"></i> UNLOX Academy</div>
          <p class="item-desc">Served as an intern and campus ambassador, promoting technical learning and engagement among student communities.</p>
          <div class="tag-list">
            <span class="tag">Outreach</span><span class="tag">Leadership</span>
          </div>
        </div>

        <div class="timeline-item" onclick="openModal('opbhalla')">
          <div class="item-head">
            <div class="item-title">Vertical Member – Design</div>
            <span class="item-date">Jul 2023 – Dec 2024</span>
          </div>
          <div class="item-sub"><i class="fas fa-palette"></i> OP Bhalla Foundation</div>
          <p class="item-desc">Designed articles, posters, and creative content for social initiatives and outreach programs.</p>
          <div class="tag-list">
            <span class="tag">Canva</span><span class="tag">Graphic Design</span><span class="tag">Social Impact</span>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Certifications -->
  <section id="certifications">
    <div class="container">
      <div class="section-head">
        <span class="section-num">04 /</span>
        <h2>Training & Certifications</h2>
        <span class="section-note">Continuous Learning</span>
      </div>
      <div class="timeline">
        <div class="timeline-item" onclick="openModal('verilogfpga')">
          <div class="item-head">
            <div class="item-title">Learning Verilog for FPGA Development</div>
            <span class="item-date">January 2025</span>
          </div>
          <div class="item-sub"><i class="fas fa-certificate"></i> LinkedIn Learning</div>
          <p class="item-desc">FPGA development fundamentals using Verilog HDL for digital logic implementation on reconfigurable hardware.</p>
        </div>

        <div class="timeline-item" onclick="openModal('leadership')">
          <div class="item-head">
            <div class="item-title">Leadership Foundation</div>
            <span class="item-date">March 2026</span>
          </div>
          <div class="item-sub"><i class="fas fa-certificate"></i> LinkedIn Learning</div>
          <p class="item-desc">Foundational leadership principles including team motivation, decision-making, and effective communication.</p>
        </div>

        <div class="timeline-item" onclick="openModal('arduino')">
          <div class="item-head">
            <div class="item-title">Hands on Arduino</div>
            <span class="item-date">April 2024</span>
          </div>
          <div class="item-sub"><i class="fas fa-certificate"></i> Udemy</div>
          <p class="item-desc">Practical Arduino programming and interfacing with sensors, actuators, and embedded peripherals.</p>
        </div>

        <div class="timeline-item" onclick="openModal('raspberry')">
          <div class="item-head">
            <div class="item-title">Raspberry Pi 4 using Python Programming</div>
            <span class="item-date">March 2025</span>
          </div>
          <div class="item-sub"><i class="fas fa-certificate"></i> LinkedIn Learning</div>
          <p class="item-desc">Python-based development on Raspberry Pi 4 for embedded Linux projects and GPIO hardware interfacing.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Skills -->
  <section id="skills">
    <div class="container">
      <div class="section-head">
        <span class="section-num">05 /</span>
        <h2>Technical Skills</h2>
        <span class="section-note">Capabilities</span>
      </div>
      <div class="skills-grid">
        <div class="skill-block">
          <h3><i class="fas fa-microchip"></i> Hardware</h3>
          <div class="tag-list">
            <span class="tag">Circuit Designing</span>
            <span class="tag">Arduino</span>
            <span class="tag">ESP</span>
            <span class="tag">Zero PCB Designing</span>
            <span class="tag">Proteus</span>
            <span class="tag">TinkerCAD</span>
          </div>
        </div>

        <div class="skill-block">
          <h3><i class="fas fa-laptop-code"></i> Software & EDA Tools</h3>
          <div class="tag-list">
            <span class="tag">Fusion 360</span>
            <span class="tag">MATLAB</span>
            <span class="tag">Arduino IDE</span>
            <span class="tag">Vivado</span>
            <span class="tag">Eagle</span>
            <span class="tag">AutoCAD</span>
            <span class="tag">GX Works3</span>
            <span class="tag">SolidWorks</span>
            <span class="tag">Cadence Genus</span>
            <span class="tag">Virtuoso</span>
          </div>
        </div>

        <div class="skill-block">
          <h3><i class="fas fa-code"></i> Programming</h3>
          <div class="tag-list">
            <span class="tag">Arduino</span>
            <span class="tag">PLC</span>
            <span class="tag">C</span>
            <span class="tag">Python</span>
            <span class="tag">Verilog</span>
          </div>
        </div>

        <div class="skill-block">
          <h3><i class="fas fa-paint-brush"></i> Other Tools</h3>
          <div class="tag-list">
            <span class="tag">Fusion 360</span>
            <span class="tag">Blender</span>
            <span class="tag">Canva</span>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Achievements -->
  <section id="achievements">
    <div class="container">
      <div class="section-head">
        <span class="section-num">06 /</span>
        <h2>Awards & Achievements</h2>
        <span class="section-note">Recognition</span>
      </div>
      <div class="timeline">
        <div class="timeline-item" onclick="openModal('mitsubishi')">
          <div class="item-head">
            <div class="item-title">6th Mitsubishi Electric Cup – National Level</div>
            <span class="item-date">Feb 2026</span>
          </div>
          <div class="item-sub"><i class="fas fa-trophy"></i> Appreciation Award · 15th Position Nationally</div>
          <p class="item-desc">Received Appreciation Award and achieved 15th position nationally at the 6th Mitsubishi Electric Cup.</p>
        </div>

        <div class="timeline-item" onclick="openModal('innoskill')">
          <div class="item-head">
            <div class="item-title">Build a Circuit – INNOSKILL 2025</div>
            <span class="item-date">04/04/2025</span>
          </div>
          <div class="item-sub"><i class="fas fa-medal"></i> 2nd Prize</div>
          <p class="item-desc">Won Second Prize in the Build a Circuit competition at INNOSKILL 2025.</p>
        </div>

        <div class="timeline-item" onclick="openModal('healthtech')">
          <div class="item-head">
            <div class="item-title">Health Tech Innovation (CHI, MRIIRS)</div>
            <span class="item-date">08/04/2024</span>
          </div>
          <div class="item-sub"><i class="fas fa-trophy"></i> 1st Prize</div>
          <p class="item-desc">Won First Prize in Health Tech Innovation for the IoT-based prenatal monitoring system.</p>
        </div>

        <div class="timeline-item" onclick="openModal('ntpccert')">
          <div class="item-head">
            <div class="item-title">NTPC Certificate of Satisfaction</div>
            <span class="item-date">2025</span>
          </div>
          <div class="item-sub"><i class="fas fa-certificate"></i> Industrial Recognition</div>
          <p class="item-desc">Received Certificate of Satisfactory work from NTPC under turbine and boiler department (RLI).</p>
        </div>

        <div class="timeline-item" onclick="openModal('loa')">
          <div class="item-head">
            <div class="item-title">Letter of Appreciation – Dr. NC Wadhwa, IAS</div>
            <span class="item-date">2024</span>
          </div>
          <div class="item-sub"><i class="fas fa-award"></i> OP Bhalla Foundation</div>
          <p class="item-desc">Received LOA from Dr. NC Wadhwa, IAS, for dedicated volunteer service under OP Bhalla Foundation.</p>
        </div>

        <div class="timeline-item" onclick="openModal('volunteer')">
          <div class="item-head">
            <div class="item-title">Highly Dedicated Volunteer</div>
            <span class="item-date">Recognition</span>
          </div>
          <div class="item-sub"><i class="fas fa-hands-helping"></i> MR OP Bhalla Foundation</div>
          <p class="item-desc">Recognized as Highly Dedicated Volunteer for consistent contribution to foundation initiatives.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Education -->
  <section id="education">
    <div class="container">
      <div class="section-head">
        <span class="section-num">07 /</span>
        <h2>Education</h2>
        <span class="section-note">Academic Background</span>
      </div>
      <div class="timeline">
        <div class="timeline-item" onclick="openModal('btech')">
          <div class="item-head">
            <div class="item-title">B.Tech ECE (AIoT)</div>
            <span class="item-date">2023 – 2027</span>
          </div>
          <div class="item-sub"><i class="fas fa-university"></i> MRIIRS, Faridabad · CGPA: 66%</div>
          <p class="item-desc">3rd Year B.Tech in Electronics & Communication Engineering (AIoT) at SET, Manav Rachna International Institute of Research and Studies.</p>
        </div>

        <div class="timeline-item" onclick="openModal('twelfth')">
          <div class="item-head">
            <div class="item-title">Senior Secondary (12th)</div>
            <span class="item-date">2021 – 2023</span>
          </div>
          <div class="item-sub"><i class="fas fa-school"></i> NARAYANA Educational Institutes · 90%</div>
          <p class="item-desc">Completed Senior Secondary at NARAYANA Educational Institutes, Visakhapatnam, Andhra Pradesh with 90%.</p>
        </div>

        <div class="timeline-item" onclick="openModal('tenth')">
          <div class="item-head">
            <div class="item-title">Secondary (10th)</div>
            <span class="item-date">2021</span>
          </div>
          <div class="item-sub"><i class="fas fa-book"></i> NARAYANA HIGH School · 99%</div>
          <p class="item-desc">Completed Secondary at NARAYANA HIGH School, Visakhapatnam, Andhra Pradesh with 99%.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Footer -->
  <footer id="contact">
    <div class="container">
      <div class="footer-name">Venkata Uma Mahesh Tamarana</div>
      <div class="footer-info">Vishakhapatnam, Andhra Pradesh · tamaranavenkatamamahesh@gmail.com · +91 9533444338</div>
      <div class="socials">
        <a href="https://www.linkedin.com/in/venkatamamahesh-tamarana-a6418128a" target="_blank" rel="noopener" class="social-btn" title="LinkedIn"><i class="fab fa-linkedin"></i></a>
        <a href="https://github.com/uma900" target="_blank" rel="noopener" class="social-btn" title="GitHub"><i class="fab fa-github"></i></a>
        <a href="mailto:tamaranavenkatamamahesh@gmail.com" class="social-btn" title="Email"><i class="fas fa-envelope"></i></a>
      </div>
      <div class="copyright">© 2026 Venkata Uma Mahesh Tamarana · Built with care</div>
    </div>
  </footer>

  <!-- Modal -->
  <div class="modal-overlay" id="modal" onclick="closeModal(event)">
    <div class="modal-card" onclick="event.stopPropagation()">
      <button class="modal-close" onclick="closeModal()"><i class="fas fa-times"></i></button>
      <div class="modal-head">
        <div class="modal-icon" id="mIcon"><i class="fas fa-info"></i></div>
        <div>
          <div class="modal-title" id="mTitle">Title</div>
          <div class="modal-sub" id="mSub">Category</div>
        </div>
      </div>
      <div class="modal-body" id="mBody">Description</div>
      <div class="modal-specs" id="mSpecs"></div>
    </div>
  </div>

  <script>
    /* ─── Logic Gate Cursor ─── */
    const gate = document.getElementById('cursorGate');
    const dot = document.getElementById('cursorDot');
    let mouseX = 0, mouseY = 0;
    let gateX = 0, gateY = 0;

    document.addEventListener('mousemove', e => {
      mouseX = e.clientX;
      mouseY = e.clientY;
      dot.style.left = mouseX + 'px';
      dot.style.top = mouseY + 'px';
    });

    function animateGate() {
      gateX += (mouseX - gateX) * 0.22;
      gateY += (mouseY - gateY) * 0.22;
      gate.style.left = gateX + 'px';
      gate.style.top = gateY + 'px';
      requestAnimationFrame(animateGate);
    }
    animateGate();

    const hoverTargets = document.querySelectorAll('a, button, .timeline-item, .project-card, .skill-block, .tag, .social-btn, .modal-close');
    hoverTargets.forEach(el => {
      el.addEventListener('mouseenter', () => gate.classList.add('hover'));
      el.addEventListener('mouseleave', () => gate.classList.remove('hover'));
    });

    /* ─── Modal Data ─── */
    const data = {
      ieee: { icon: 'fas fa-book', title: 'IEEE Published Research Paper', sub: 'IEEE Xplore · 2025', body: 'A Review of Gesture-Based Wireless Pen Interfaces for Human-Computer Interaction: Sensors, Algorithms, and Applications.', specs: [['Title','Gesture-Based Wireless Pen Interfaces'],['Platform','IEEE Xplore'],['Domain','HCI'],['Status','Published (2025)']] },
      pen: { icon: 'fas fa-pen-nib', title: 'Gesture-Based Wireless Pen Interface', sub: 'Granted Utility Patent', body: 'Utility patent for a wireless pen interface enabling gesture-based human-computer interaction through spatial motion tracking.', specs: [['Type','Utility Patent'],['App No.','459423-001'],['Date','19/05/2025'],['Status','Granted']] },
      table: { icon: 'fas fa-utensils', title: 'IoT Smart Table Call & Tracking', sub: 'Granted Design Patent', body: 'Design patent for IoT-based smart table call and tracking service automation.', specs: [['Type','Design Patent'],['App No.','202611028457'],['Date','01/04/2026'],['Status','Granted']] },
      soc: { icon: 'fas fa-microchip', title: 'SoC Architecture using AMBA Protocol', sub: 'Ongoing VLSI Project', body: 'Developing a complete SoC architecture leveraging AMBA bus protocols for on-chip communication.', specs: [['Protocols','AXI, AHB, APB'],['Language','Verilog RTL'],['Year','2026'],['Status','Ongoing']] },
      fruit: { icon: 'fas fa-industry', title: 'Deep Learning Fruit Sorting System', sub: 'Edge AI + Industrial Automation', body: 'Deep learning automated fruit sorting using PLC and Jetson Nano.', specs: [['AI Platform','Jetson Nano'],['Controller','Mitsubishi PLC'],['Domain','Industrial Automation'],['Year','2026']] },
      alert: { icon: 'fas fa-bell', title: 'IoT Emergency Alert System', sub: 'IoT Safety Project', body: 'IoT-based emergency alert system using ESP32 Wi-Fi module.', specs: [['Module','ESP32'],['Connectivity','Wi-Fi'],['Domain','IoT Safety'],['Year','2025']] },
      smarttable: { icon: 'fas fa-utensils', title: 'IoT Smart Table Call & Tracking', sub: 'Restaurant Automation', body: 'IoT smart table call and tracking system for restaurant service automation.', specs: [['Domain','Hospitality'],['Technology','IoT'],['Year','2025']] },
      prenatal: { icon: 'fas fa-heartbeat', title: 'IoT Prenatal Monitoring System', sub: 'Biomedical IoT', body: 'IoT-based prenatal monitoring for pregnant women using BPM, vibration, and temperature sensors.', specs: [['Sensors','BPM, Vibration, Temp'],['Domain','Health Tech'],['Year','2024'],['Award','1st Prize CHI']] },
      hmies: { icon: 'fas fa-microchip', title: 'VLSI Intern', sub: 'HMIES Solutions Pvt. Ltd', body: 'Assisted in RTL design and verification using Verilog/SystemVerilog.', specs: [['Company','HMIES Solutions'],['Duration','Jun 2025'],['Skills','Verilog, SystemVerilog'],['Focus','RTL Design & Verification']] },
      ntpc: { icon: 'fas fa-industry', title: 'Engineering Intern – NTPC', sub: 'National Thermal Power Corporation', body: 'Worked under turbine and boiler department at NTPC.', specs: [['Organization','NTPC'],['Department','Turbine & Boiler'],['Duration','Jul 2025'],['Recognition','Certificate of Satisfaction']] },
      unlox: { icon: 'fas fa-users', title: 'Intern & Campus Ambassador', sub: 'UNLOX Academy', body: 'Intern and campus ambassador promoting technical learning.', specs: [['Organization','UNLOX Academy'],['Role','Intern & Campus Ambassador'],['Duration','Oct 2025']] },
      opbhalla: { icon: 'fas fa-palette', title: 'Vertical Member – Design', sub: 'OP Bhalla Foundation', body: 'Designed articles and posters for social initiatives.', specs: [['Organization','OP Bhalla Foundation'],['Role','Vertical Member – Design'],['Duration','Jul 2023 – Dec 2024'],['Tools','Canva, Graphic Design']] },
      verilogfpga: { icon: 'fas fa-microchip', title: 'Learning Verilog for FPGA Development', sub: 'LinkedIn Learning', body: 'FPGA development using Verilog HDL.', specs: [['Platform','LinkedIn Learning'],['Completed','January 2025'],['Focus','FPGA + Verilog']] },
      leadership: { icon: 'fas fa-users-cog', title: 'Leadership Foundation', sub: 'LinkedIn Learning', body: 'Foundational leadership principles.', specs: [['Platform','LinkedIn Learning'],['Completed','March 2026']] },
      arduino: { icon: 'fas fa-infinity', title: 'Hands on Arduino', sub: 'Udemy', body: 'Practical Arduino programming and interfacing.', specs: [['Platform','Udemy'],['Completed','April 2024']] },
      raspberry: { icon: 'fab fa-python', title: 'Raspberry Pi 4 using Python', sub: 'LinkedIn Learning', body: 'Python development on Raspberry Pi 4.', specs: [['Platform','LinkedIn Learning'],['Completed','March 2025'],['Language','Python 3']] },
      mitsubishi: { icon: 'fas fa-trophy', title: '6th Mitsubishi Electric Cup', sub: 'National Level', body: 'Appreciation Award and 15th position nationally.', specs: [['Event','6th Mitsubishi Electric Cup'],['Level','National'],['Position','15th'],['Date','20–21 Feb 2026']] },
      innoskill: { icon: 'fas fa-medal', title: 'Build a Circuit – INNOSKILL 2025', sub: 'Competition', body: 'Second Prize in Build a Circuit competition.', specs: [['Event','INNOSKILL 2025'],['Prize','2nd Prize'],['Date','04/04/2025']] },
      healthtech: { icon: 'fas fa-trophy', title: 'Health Tech Innovation', sub: 'CHI, MRIIRS', body: 'First Prize for IoT-based prenatal monitoring.', specs: [['Event','Health Tech Innovation'],['Institution','CHI, MRIIRS'],['Prize','1st Prize'],['Date','08/04/2024']] },
      ntpccert: { icon: 'fas fa-certificate', title: 'NTPC Certificate of Satisfaction', sub: 'Industrial Recognition', body: 'Certificate of Satisfactory work from NTPC.', specs: [['Organization','NTPC'],['Year','2025'],['Department','Turbine & Boiler (RLI)']] },
      loa: { icon: 'fas fa-award', title: 'Letter of Appreciation', sub: 'Dr. NC Wadhwa, IAS', body: 'LOA for dedicated volunteer service under OP Bhalla Foundation.', specs: [['From','Dr. NC Wadhwa, IAS'],['Foundation','OP Bhalla'],['Year','2024']] },
      volunteer: { icon: 'fas fa-hands-helping', title: 'Highly Dedicated Volunteer', sub: 'MR OP Bhalla Foundation', body: 'Recognized for consistent contribution to foundation initiatives.', specs: [['Foundation','MR OP Bhalla'],['Role','Volunteer']] },
      btech: { icon: 'fas fa-user-graduate', title: 'B.Tech ECE (AIoT)', sub: 'MRIIRS, Faridabad', body: '3rd Year B.Tech in Electronics & Communication Engineering (AIoT).', specs: [['Institution','MRIIRS, Faridabad'],['Duration','2023–2027'],['CGPA','66%'],['Specialization','AIoT']] },
      twelfth: { icon: 'fas fa-school', title: 'Senior Secondary (12th)', sub: 'NARAYANA Educational Institutes', body: 'Completed 12th with 90%.', specs: [['Institution','NARAYANA Educational Institutes'],['Location','Visakhapatnam'],['Score','90%'],['Duration','2021–2023']] },
      tenth: { icon: 'fas fa-book-reader', title: 'Secondary (10th)', sub: 'NARAYANA HIGH School', body: 'Completed 10th with 99%.', specs: [['Institution','NARAYANA HIGH School'],['Location','Visakhapatnam'],['Score','99%'],['Year','2021']] }
    };

    function openModal(key) {
      const d = data[key];
      if (!d) return;
      document.getElementById('mIcon').innerHTML = `<i class="${d.icon}"></i>`;
      document.getElementById('mTitle').textContent = d.title;
      document.getElementById('mSub').textContent = d.sub;
      document.getElementById('mBody').textContent = d.body;
      let specs = '';
      d.specs.forEach(s => {
        specs += `<div><div class="spec-label">${s[0]}</div><div class="spec-val">${s[1]}</div></div>`;
      });
      document.getElementById('mSpecs').innerHTML = specs;
      document.getElementById('modal').classList.add('active');
    }

    function closeModal(e) {
      if (!e || e.target.id === 'modal' || e.target.closest('.modal-close')) {
        document.getElementById('modal').classList.remove('active');
      }
    }

    document.addEventListener('keydown', e => {
      if (e.key === 'Escape') document.getElementById('modal').classList.remove('active');
    });
  </script>
</body>
</html>
