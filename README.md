<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Brain &amp; Mind Academy • DHANANJAYA 10 - Trigonometry (Part 3: Identities &amp; Exercise 8.3)</title>

  <!-- MathJax v3 Configuration & Loader -->
  <script>
    window.MathJax = {
      tex: {
        inlineMath: [['\\(', '\\)']],
        displayMath: [['\\[', '\\]']],
        processEscapes: true
      },
      svg: { fontCache: 'global' }
    };
  </script>
  <script type="text/javascript" id="MathJax-script" async
    src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js">
  </script>

  <style>
    :root {
      --navy-dark: #0c4a6e;
      --brand-blue: #0284c7;
      --accent-cyan: #0ea5e9;
      --bg-tint: #f0f9ff;
      --card-surf: #ffffff;
      --border-accent: #7dd3fc;
      --border-soft: #bae6fd;
      --green-ok: #059669;
      --green-surf: #d1fae5;
      --red-fail: #dc2626;
      --red-surf: #fee2e2;
      --brand-gold: #f59e0b;
      --gold-dark: #d97706;
      --gold-surf: #fef3c7;
      --text-main: #0f172a;
      --text-muted: #475569;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
    }

    body {
      background-color: var(--bg-tint);
      color: var(--text-main);
      display: flex;
      flex-direction: column;
      min-height: 100vh;
    }

    header {
      background: var(--navy-dark);
      color: #fff;
      padding: 12px 24px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      box-shadow: 0 4px 12px rgba(12, 74, 110, 0.15);
      position: sticky;
      top: 0;
      z-index: 100;
    }

    .brand-wrap {
      display: flex;
      align-items: center;
      gap: 14px;
    }

    .logo-badge {
      width: 46px;
      height: 46px;
      background: #ffffff;
      border-radius: 10px;
      display: flex;
      align-items: center;
      justify-content: center;
      box-shadow: 0 2px 6px rgba(0,0,0,0.2);
    }

    .brand-title h1 {
      font-size: 1.15rem;
      font-weight: 700;
      letter-spacing: 0.5px;
    }

    .brand-title p {
      font-size: 0.78rem;
      color: var(--accent-cyan);
      font-weight: 500;
    }

    .header-controls {
      display: flex;
      align-items: center;
      gap: 12px;
    }

    .chip {
      background: rgba(255, 255, 255, 0.12);
      border: 1px solid var(--border-accent);
      padding: 6px 14px;
      border-radius: 20px;
      font-size: 0.85rem;
      font-weight: 600;
      display: flex;
      align-items: center;
      gap: 6px;
    }

    .btn-icon {
      background: transparent;
      border: 1px solid var(--border-accent);
      color: #fff;
      border-radius: 50%;
      width: 36px;
      height: 36px;
      cursor: pointer;
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 1rem;
    }

    nav {
      background: #ffffff;
      border-bottom: 1px solid var(--border-soft);
      display: flex;
      justify-content: center;
      gap: 8px;
      padding: 8px 16px;
    }

    nav button {
      background: none;
      border: none;
      outline: none;
      padding: 10px 20px;
      font-size: 0.95rem;
      font-weight: 600;
      color: var(--text-muted);
      cursor: pointer;
      border-radius: 8px;
      transition: all 0.2s;
    }

    nav button.active {
      background: var(--bg-tint);
      color: var(--brand-blue);
      border-bottom: 3px solid var(--brand-blue);
    }

    main {
      flex: 1;
      padding: 24px;
      max-width: 1400px;
      margin: 0 auto;
      width: 100%;
    }

    .view {
      display: none;
    }

    .view.active {
      display: block;
    }

    #loginGateView {
      position: fixed;
      top: 0;
      left: 0;
      right: 0;
      bottom: 0;
      background: rgba(12, 74, 110, 0.88);
      backdrop-filter: blur(5px);
      z-index: 1000;
      display: flex;
      align-items: center;
      justify-content: center;
    }

    .login-box {
      background: #fff;
      padding: 36px;
      border-radius: 16px;
      width: 100%;
      max-width: 420px;
      text-align: center;
      box-shadow: 0 14px 35px rgba(0,0,0,0.3);
    }

    .login-box h2 {
      font-size: 1.45rem;
      color: var(--navy-dark);
      margin-bottom: 6px;
    }

    .login-box p {
      font-size: 0.88rem;
      color: var(--text-muted);
      margin-bottom: 24px;
    }

    .login-box input {
      width: 100%;
      padding: 12px 16px;
      border: 1px solid var(--border-soft);
      border-radius: 8px;
      font-size: 1rem;
      margin-bottom: 16px;
      outline: none;
    }

    .btn-primary {
      background: var(--brand-blue);
      color: #fff;
      border: none;
      padding: 12px 24px;
      font-size: 1rem;
      font-weight: 600;
      border-radius: 8px;
      cursor: pointer;
      width: 100%;
      transition: background 0.2s;
    }

    .btn-primary:hover {
      background: var(--navy-dark);
    }

    .theory-card {
      background: #fff;
      border-radius: 12px;
      border: 1px solid var(--border-soft);
      padding: 24px;
      margin-bottom: 24px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.02);
    }

    .theory-card h3 {
      color: var(--navy-dark);
      margin-bottom: 14px;
      display: flex;
      align-items: center;
      gap: 8px;
      font-size: 1.25rem;
    }

    .theory-intro-text {
      color: var(--text-main);
      line-height: 1.65;
      margin-bottom: 18px;
      font-size: 0.95rem;
    }

    .compendium-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(360px, 1fr));
      gap: 20px;
      margin: 16px 0;
    }

    .comp-card {
      background: #ffffff;
      border: 1px solid var(--border-soft);
      border-radius: 10px;
      padding: 20px;
      display: flex;
      flex-direction: column;
      box-shadow: 0 2px 6px rgba(12, 74, 110, 0.04);
    }

    .comp-card h4 {
      color: var(--navy-dark);
      border-bottom: 2px solid var(--border-soft);
      padding-bottom: 8px;
      margin-bottom: 12px;
      font-size: 1.05rem;
      display: flex;
      align-items: center;
      gap: 8px;
    }

    .derivation-body {
      font-size: 0.92rem;
      line-height: 1.6;
      color: var(--text-main);
    }

    .ratios-highlight-box {
      background: #f8fafc;
      border-left: 4px solid var(--brand-blue);
      border-radius: 0 6px 6px 0;
      padding: 10px 14px;
      margin-top: 10px;
    }

    .table-container {
      margin: 16px 0;
      overflow-x: auto;
      border-radius: 8px;
      border: 1px solid var(--border-soft);
      background: #ffffff;
    }

    .stat-table {
      width: 100%;
      border-collapse: collapse;
      text-align: center;
      font-size: 0.92rem;
    }

    .stat-table th, .stat-table td {
      border: 1px solid var(--border-soft);
      padding: 10px 14px;
    }

    .stat-table th {
      background: var(--bg-tint);
      color: var(--navy-dark);
      font-weight: 700;
    }

    .stat-table tr:nth-child(even) {
      background: #f8fafc;
    }

    .video-callout-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 14px;
      margin-top: 18px;
    }

    .video-callout {
      display: flex;
      flex-direction: column;
      justify-content: space-between;
      background: #f8fafc;
      border: 1px solid var(--border-soft);
      padding: 14px 16px;
      border-radius: 8px;
      border-left: 4px solid var(--accent-cyan);
    }

    .video-callout a {
      color: var(--brand-blue);
      font-weight: 700;
      text-decoration: none;
      margin-top: 8px;
      font-size: 0.88rem;
    }

    /* Practice Sheet Styles */
    .sheet-grid {
      display: grid;
      grid-template-columns: 1fr 350px;
      gap: 24px;
    }

    @media (max-width: 990px) {
      .sheet-grid {
        grid-template-columns: 1fr;
      }
    }

    .question-card {
      background: #fff;
      border-radius: 12px;
      border: 1px solid var(--border-soft);
      padding: 24px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.03);
    }

    .concept-tag {
      display: inline-block;
      padding: 4px 10px;
      border-radius: 14px;
      font-size: 0.75rem;
      font-weight: 700;
      letter-spacing: 0.4px;
      text-transform: uppercase;
      margin-bottom: 8px;
    }

    .concept-tag.example {
      background: #e0f2fe;
      color: #0369a1;
      border: 1px solid #7dd3fc;
    }

    .concept-tag.proof {
      background: #fef3c7;
      color: #b45309;
      border: 1px solid #fde68a;
    }

    .concept-tag.mcq {
      background: #d1fae5;
      color: #059669;
      border: 1px solid #a7f3d0;
    }

    .svg-container {
      display: flex;
      justify-content: center;
      margin: 18px 0;
      padding: 16px;
      background: var(--bg-tint);
      border-radius: 8px;
      border: 1px solid var(--border-soft);
      overflow-x: auto;
    }

    .step-box {
      margin-top: 16px;
      padding: 18px;
      border: 1px solid var(--border-soft);
      border-radius: 8px;
      background: #fff;
      display: none;
    }

    .step-box.unlocked {
      display: block;
      animation: fadeIn 0.3s ease-in;
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(6px); }
      to { opacity: 1; transform: translateY(0); }
    }

    .step-box.success {
      border-color: var(--green-ok);
      background: var(--green-surf);
    }

    .step-text-wrap {
      font-size: 1rem;
      line-height: 1.8;
      display: flex;
      align-items: center;
      flex-wrap: wrap;
      gap: 8px;
    }

    .inline-blank {
      width: 150px;
      padding: 6px 10px;
      font-size: 0.95rem;
      border: 2px dashed var(--brand-blue);
      border-radius: 6px;
      outline: none;
      background: #fff;
      color: var(--navy-dark);
      font-weight: 600;
      text-align: center;
    }

    .inline-blank:focus {
      border-style: solid;
      border-color: var(--accent-cyan);
      box-shadow: 0 0 0 3px rgba(14,165,233,0.2);
    }

    .inline-blank:disabled {
      border: 1px solid var(--green-ok);
      background: #fff;
      color: var(--green-ok);
      cursor: not-allowed;
    }

    .btn-verify {
      background: var(--accent-cyan);
      color: #fff;
      border: none;
      padding: 7px 16px;
      border-radius: 6px;
      font-weight: 600;
      cursor: pointer;
    }

    .btn-verify:hover {
      background: var(--brand-blue);
    }

    .btn-reveal {
      background: var(--brand-gold);
      color: #fff;
      border: none;
      padding: 6px 12px;
      border-radius: 6px;
      font-weight: 600;
      font-size: 0.85rem;
      cursor: pointer;
      margin-left: 6px;
    }

    .btn-reveal:hover {
      background: var(--gold-dark);
    }

    .attempts-badge {
      font-size: 0.8rem;
      font-weight: 700;
      padding: 3px 8px;
      border-radius: 12px;
      background: #f1f5f9;
      color: #64748b;
      margin-left: 6px;
    }

    .nav-toolbar {
      display: flex;
      justify-content: space-between;
      align-items: center;
      margin-top: 26px;
      padding-top: 18px;
      border-top: 1px solid var(--border-soft);
    }

    .nav-btn-group {
      display: flex;
      gap: 10px;
    }

    .btn-nav-action {
      background: #f8fafc;
      border: 1px solid var(--border-accent);
      color: var(--navy-dark);
      padding: 8px 18px;
      border-radius: 6px;
      font-weight: 600;
      font-size: 0.9rem;
      cursor: pointer;
      display: flex;
      align-items: center;
      gap: 6px;
      transition: all 0.15s;
    }

    .btn-nav-action:hover:not(:disabled) {
      background: var(--bg-tint);
      border-color: var(--brand-blue);
    }

    .btn-nav-action:disabled {
      opacity: 0.45;
      cursor: not-allowed;
    }

    .btn-skip {
      border-color: var(--brand-gold);
      color: var(--gold-dark);
      background: var(--gold-surf);
    }

    .btn-skip:hover {
      background: #fde68a;
    }

    .palette-box {
      background: #fff;
      border: 1px solid var(--border-soft);
      border-radius: 12px;
      padding: 16px;
      margin-bottom: 20px;
    }

    .palette-legend {
      display: flex;
      justify-content: space-between;
      font-size: 0.75rem;
      margin: 8px 0 12px 0;
      padding: 6px 8px;
      background: var(--bg-tint);
      border-radius: 6px;
    }

    .legend-item {
      display: flex;
      align-items: center;
      gap: 4px;
      font-weight: 600;
    }

    .legend-dot {
      width: 10px;
      height: 10px;
      border-radius: 50%;
    }

    .palette-section-title {
      font-size: 0.8rem;
      font-weight: 700;
      color: var(--text-muted);
      text-transform: uppercase;
      letter-spacing: 0.5px;
      margin: 12px 0 6px 0;
    }

    .palette-grid {
      display: grid;
      grid-template-columns: repeat(5, 1fr);
      gap: 6px;
      margin-bottom: 12px;
    }

    .palette-btn {
      aspect-ratio: 1;
      border: 1px solid var(--border-soft);
      background: var(--bg-tint);
      border-radius: 6px;
      font-weight: 600;
      cursor: pointer;
      display: flex;
      align-items: center;
      justify-content: center;
      transition: all 0.15s;
      font-size: 0.82rem;
      color: var(--navy-dark);
    }

    .palette-btn.active {
      border: 2px solid var(--navy-dark) !important;
      background: var(--border-accent);
      color: #fff;
      font-weight: 800;
    }

    .palette-btn.completed {
      background: var(--green-ok) !important;
      color: #fff !important;
      border-color: var(--green-ok) !important;
    }

    .palette-btn.skipped {
      background: var(--brand-gold) !important;
      color: #fff !important;
      border-color: var(--gold-dark) !important;
    }

    .tool-tabs {
      display: flex;
      border-bottom: 1px solid var(--border-soft);
      margin-bottom: 12px;
    }

    .tool-tabs button {
      flex: 1;
      border: none;
      background: none;
      padding: 8px;
      font-weight: 600;
      font-size: 0.85rem;
      cursor: pointer;
      color: var(--text-muted);
    }

    .tool-tabs button.active {
      color: var(--brand-blue);
      border-bottom: 2px solid var(--brand-blue);
    }

    .keypad-grid {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 6px;
    }

    .keypad-btn {
      padding: 8px 4px;
      border: 1px solid var(--border-soft);
      background: #fff;
      border-radius: 4px;
      font-weight: 600;
      font-size: 0.85rem;
      cursor: pointer;
      text-align: center;
    }

    .keypad-btn:hover {
      background: var(--bg-tint);
    }

    #calcDisplay {
      width: 100%;
      padding: 8px;
      border: 1px solid var(--border-soft);
      border-radius: 4px;
      font-size: 1rem;
      text-align: right;
      margin-bottom: 8px;
      background: #f8fafc;
    }

    .hero-score-card {
      background: #fff;
      border-radius: 12px;
      border: 1px solid var(--border-soft);
      padding: 24px;
      text-align: center;
      margin-bottom: 24px;
    }

    .score-badge {
      font-size: 2.4rem;
      font-weight: 800;
      color: var(--brand-blue);
    }

    .toast {
      position: fixed;
      bottom: 20px;
      right: 20px;
      background: var(--navy-dark);
      color: #fff;
      padding: 12px 20px;
      border-radius: 8px;
      box-shadow: 0 4px 16px rgba(0,0,0,0.2);
      display: none;
      z-index: 1000;
    }

    @media print {
      header, nav, .palette-box, #toolsPanel, .btn-primary, .btn-verify, #loginGateView, .nav-toolbar {
        display: none !important;
      }
      body { background: #fff; }
      main { width: 100%; max-width: 100%; padding: 0; }
      .sheet-grid { display: block; }
      .view { display: block !important; }
    }
  </style>
</head>
<body>

  <!-- Brand Header -->
  <header>
    <div class="brand-wrap">
      <div class="logo-badge">
        <svg width="34" height="34" viewBox="0 0 100 100" fill="none">
          <path d="M 20 30 Q 50 10 80 30" stroke="#f59e0b" stroke-width="8" stroke-linecap="round"/>
          <path d="M 26 40 Q 50 22 74 40" stroke="#f59e0b" stroke-width="8" stroke-linecap="round"/>
          <path d="M 32 50 Q 50 36 68 50" stroke="#f59e0b" stroke-width="7" stroke-linecap="round"/>
          <path d="M 18 80 Q 50 68 50 82 Q 50 68 82 80 L 82 52 Q 50 42 50 56 Q 50 42 18 52 Z" fill="#ffffff" stroke="#334155" stroke-width="7" stroke-linejoin="round"/>
        </svg>
      </div>
      <div class="brand-title">
        <h1>Brain &amp; Mind Academy</h1>
        <p>B&amp;M – The Experts • DHANANJAYA 10 (Trigonometric Identities &amp; Exercise 8.3)</p>
      </div>
    </div>
    <div class="header-controls">
      <div class="chip" id="timerChip">⏱️ 00:00</div>
      <div class="chip" id="userPill">Roll No: Guest</div>
      <button class="btn-icon" id="audioToggleBtn" title="Toggle Audio">🔊</button>
    </div>
  </header>

  <!-- Navigation Bar -->
  <nav>
    <button class="tab-btn active" onclick="switchView('theoryView')">📖 Theory &amp; Strategy Guide</button>
    <button class="tab-btn" onclick="switchView('sheetView')">✍️ Interactive Practice Sheet</button>
    <button class="tab-btn" onclick="switchView('solutionsView')">📋 Complete Solutions</button>
  </nav>

  <!-- Login Gate Modal -->
  <div id="loginGateView">
    <div class="login-box">
      <h2>DHANANJAYA 10 Portal</h2>
      <p>Class 10 CBSE Chapter Mastery — Section 8.4 &amp; Exercise 8.3 Identities</p>
      <input type="text" id="rollInput" placeholder="Enter Student ID / Roll No" />
      <input type="password" id="passInput" placeholder="Passcode (Optional)" />
      <button class="btn-primary" onclick="initDirectLogin()">Initialize Workspace</button>
    </div>
  </div>

  <main>
    <!-- View 1: Theory & Strategy Guide -->
    <div id="theoryView" class="view active">
      <div class="theory-card">
        <h3>📐 Theory Compendium: The Three Fundamental Pythagorean Identities</h3>
        <p class="theory-intro-text">
          An equation involving trigonometric ratios of an angle is called a <strong>trigonometric identity</strong> if it remains true for all values of the angles for which the functions are defined. Below is the formal derivation of the three foundational identities using Pythagoras theorem in right-angled triangle \(\triangle ABC\) (with \(\angle B = 90^\circ\)):
        </p>

        <div class="compendium-grid">
          <!-- Identity 1 -->
          <div class="comp-card">
            <h4>1. Primary Identity: \(\sin^2 A + \cos^2 A = 1\)</h4>
            <div class="derivation-body">
              <p>In right \(\triangle ABC\), by Pythagoras Theorem:</p>
              \[AB^2 + BC^2 = AC^2\]
              <p>Dividing each term by \(AC^2\):</p>
              \[\left(\frac{AB}{AC}\right)^2 + \left(\frac{BC}{AC}\right)^2 = \left(\frac{AC}{AC}\right)^2\]
              <p>Since \(\cos A = \frac{AB}{AC}\) and \(\sin A = \frac{BC}{AC}\):</p>
              <div class="ratios-highlight-box">
                \[\cos^2 A + \sin^2 A = 1 \quad (\text{Valid for } 0^\circ \le A \le 90^\circ)\]
                <p style="margin-top:6px; font-size:0.88rem;"><strong>Useful Rearrangements:</strong></p>
                \[\sin^2 A = 1 - \cos^2 A \iff \cos^2 A = 1 - \sin^2 A\]
              </div>
            </div>
          </div>

          <!-- Identity 2 -->
          <div class="comp-card">
            <h4>2. Second Identity: \(1 + \tan^2 A = \sec^2 A\)</h4>
            <div class="derivation-body">
              <p>Dividing \(AB^2 + BC^2 = AC^2\) by \(AB^2\):</p>
              \[\left(\frac{AB}{AB}\right)^2 + \left(\frac{BC}{AB}\right)^2 = \left(\frac{AC}{AB}\right)^2\]
              <p>Since \(\frac{BC}{AB} = \tan A\) and \(\frac{AC}{AB} = \sec A\):</p>
              <div class="ratios-highlight-box">
                \[1 + \tan^2 A = \sec^2 A \quad (\text{Valid for } 0^\circ \le A < 90^\circ)\]
                <p style="margin-top:6px; font-size:0.88rem;"><strong>Useful Rearrangements:</strong></p>
                \[\sec^2 A - \tan^2 A = 1 \iff \tan^2 A = \sec^2 A - 1\]
                \[(\sec A - \tan A)(\sec A + \tan A) = 1 \implies \sec A - \tan A = \frac{1}{\sec A + \tan A}\]
              </div>
            </div>
          </div>

          <!-- Identity 3 -->
          <div class="comp-card">
            <h4>3. Third Identity: \(1 + \cot^2 A = \operatorname{cosec}^2 A\)</h4>
            <div class="derivation-body">
              <p>Dividing \(AB^2 + BC^2 = AC^2\) by \(BC^2\):</p>
              \[\left(\frac{AB}{BC}\right)^2 + \left(\frac{BC}{BC}\right)^2 = \left(\frac{AC}{BC}\right)^2\]
              <p>Since \(\frac{AB}{BC} = \cot A\) and \(\frac{AC}{BC} = \operatorname{cosec} A\):</p>
              <div class="ratios-highlight-box">
                \[\cot^2 A + 1 = \operatorname{cosec}^2 A \quad (\text{Valid for } 0^\circ < A \le 90^\circ)\]
                <p style="margin-top:6px; font-size:0.88rem;"><strong>Useful Rearrangements:</strong></p>
                \[\operatorname{cosec}^2 A - \cot^2 A = 1 \iff \cot^2 A = \operatorname{cosec}^2 A - 1\]
                \[(\operatorname{cosec} A - \cot A)(\operatorname{cosec} A + \cot A) = 1 \implies \operatorname{cosec} A - \cot A = \frac{1}{\operatorname{cosec} A + \cot A}\]
              </div>
            </div>
          </div>
        </div>
      </div>

      <!-- Conversion Matrix Card -->
      <div class="theory-card">
        <h3>📊 Trigonometric Conversion Matrix</h3>
        <p class="theory-intro-text">Expressing each trigonometric ratio in terms of any other ratio:</p>
        <div class="table-container">
          <table class="stat-table">
            <thead>
              <tr>
                <th>Ratio</th>
                <th>In terms of \(\sin A\)</th>
                <th>In terms of \(\cos A\)</th>
                <th>In terms of \(\tan A\)</th>
                <th>In terms of \(\cot A\)</th>
                <th>In terms of \(\sec A\)</th>
              </tr>
            </thead>
            <tbody>
              <tr>
                <td><strong>\(\sin A\)</strong></td>
                <td>\(\sin A\)</td>
                <td>\(\sqrt{1 - \cos^2 A}\)</td>
                <td>\(\frac{\tan A}{\sqrt{1 + \tan^2 A}}\)</td>
                <td>\(\frac{1}{\sqrt{1 + \cot^2 A}}\)</td>
                <td>\(\frac{\sqrt{\sec^2 A - 1}}{\sec A}\)</td>
              </tr>
              <tr>
                <td><strong>\(\cos A\)</strong></td>
                <td>\(\sqrt{1 - \sin^2 A}\)</td>
                <td>\(\cos A\)</td>
                <td>\(\frac{1}{\sqrt{1 + \tan^2 A}}\)</td>
                <td>\(\frac{\cot A}{\sqrt{1 + \cot^2 A}}\)</td>
                <td>\(\frac{1}{\sec A}\)</td>
              </tr>
              <tr>
                <td><strong>\(\tan A\)</strong></td>
                <td>\(\frac{\sin A}{\sqrt{1 - \sin^2 A}}\)</td>
                <td>\(\frac{\sqrt{1 - \cos^2 A}}{\cos A}\)</td>
                <td>\(\tan A\)</td>
                <td>\(\frac{1}{\cot A}\)</td>
                <td>\(\sqrt{\sec^2 A - 1}\)</td>
              </tr>
              <tr>
                <td><strong>\(\operatorname{cosec} A\)</strong></td>
                <td>\(\frac{1}{\sin A}\)</td>
                <td>\(\frac{1}{\sqrt{1 - \cos^2 A}}\)</td>
                <td>\(\frac{\sqrt{1 + \tan^2 A}}{\tan A}\)</td>
                <td>\(\sqrt{1 + \cot^2 A}\)</td>
                <td>\(\frac{\sec A}{\sqrt{\sec^2 A - 1}}\)</td>
              </tr>
              <tr>
                <td><strong>\(\sec A\)</strong></td>
                <td>\(\frac{1}{\sqrt{1 - \sin^2 A}}\)</td>
                <td>\(\frac{1}{\cos A}\)</td>
                <td>\(\sqrt{1 + \tan^2 A}\)</td>
                <td>\(\frac{\sqrt{1 + \cot^2 A}}{\cot A}\)</td>
                <td>\(\sec A\)</td>
              </tr>
              <tr>
                <td><strong>\(\cot A\)</strong></td>
                <td>\(\frac{\sqrt{1 - \sin^2 A}}{\sin A}\)</td>
                <td>\(\frac{\cos A}{\sqrt{1 - \cos^2 A}}\)</td>
                <td>\(\frac{1}{\tan A}\)</td>
                <td>\(\cot A\)</td>
                <td>\(\frac{1}{\sqrt{\sec^2 A - 1}}\)</td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>

      <!-- Master Proof Strategy Guide -->
      <div class="theory-card">
        <h3>💡 Strategic Board Heuristics for Proving Identities</h3>
        <div class="compendium-grid">
          <div class="comp-card">
            <h4>Strategy 1: The \(\sin\) &amp; \(\cos\) Bridge</h4>
            <p>If an expression contains mixed functions (\(\tan, \cot, \sec, \operatorname{cosec}\)), rewrite all terms using \(\sin\theta\) and \(\cos\theta\), take a common algebraic denominator, and simplify.</p>
          </div>
          <div class="comp-card">
            <h4>Strategy 2: Conjugate Multiplication</h4>
            <p>When radical expressions appear, or terms like \(1 \pm \sin A\) or \(\sec A \pm \tan A\) exist in denominators, multiply numerator and denominator by their algebraic conjugates to trigger \(a^2 - b^2\).</p>
          </div>
          <div class="comp-card">
            <h4>Strategy 3: Algebraic Factoring</h4>
            <p>Exploit polynomial identities: \(a^3 \pm b^3 = (a \pm b)(a^2 \mp ab + b^2)\) and \((a + b)^2 = a^2 + b^2 + 2ab\). Look for common factors to factor out and cancel.</p>
          </div>
          <div class="comp-card">
            <h4>Strategy 4: Substituted Ones</h4>
            <p>In expressions like \(\frac{\cos A - \sin A + 1}{\cos A + \sin A - 1}\), replace the standalone constant \(1\) with \((\operatorname{cosec}^2 A - \cot^2 A)\) to unlock common binomial factors.</p>
          </div>
        </div>
      </div>

      <!-- Video Callouts Card -->
      <div class="theory-card">
        <h3>📹 Curated Master Video Lectures (Khan Academy)</h3>
        <div class="video-callout-grid">
          <div class="video-callout">
            <strong>Intro to Pythagorean Trig Identities</strong>
            <p>Geometric derivations and core relationships of the three primary identities.</p>
            <a href="https://www.khanacademy.org/math/ncert-class-10/xd6a17b08edbd2443:introduction-to-trigonometry-ncert-new/xd6a17b08edbd2443:trigonometric-identities/v/intro-to-pythagorean-trigonometric-identities" target="_blank">Watch on Khan Academy →</a>
          </div>
          <div class="video-callout">
            <strong>Writing a Trig Ratio in terms of other ratios</strong>
            <p>Systematic techniques for expressing ratios in terms of a chosen single ratio.</p>
            <a href="https://www.khanacademy.org/math/ncert-class-10/xd6a17b08edbd2443:introduction-to-trigonometry-ncert-new/xd6a17b08edbd2443:trigonometric-identities/v/writing-a-trigonometric-ratio-in-terms-other-ratios" target="_blank">Watch on Khan Academy →</a>
          </div>
          <div class="video-callout">
            <strong>Example 1 Proving Trig Identities</strong>
            <p>Step-by-step proof breakdown using algebraic simplification and conjugate multiplication.</p>
            <a href="https://www.khanacademy.org/math/ncert-class-10/xd6a17b08edbd2443:introduction-to-trigonometry-ncert-new/xd6a17b08edbd2443:trigonometric-identities/v/example-1-proving-trigonometric-identities" target="_blank">Watch on Khan Academy →</a>
          </div>
          <div class="video-callout">
            <strong>Example 2 Proving Trig Identities</strong>
            <p>Working with fraction expansions, common denominators, and reciprocal substitutions.</p>
            <a href="https://www.khanacademy.org/math/ncert-class-10/xd6a17b08edbd2443:introduction-to-trigonometry-ncert-new/xd6a17b08edbd2443:trigonometric-identities/v/example-2-proving-trigonometric-identities" target="_blank">Watch on Khan Academy →</a>
          </div>
        </div>
      </div>
    </div>

    <!-- View 2: Interactive Practice Sheet -->
    <div id="sheetView" class="view">
      <div class="sheet-grid">
        <div class="question-card" id="activeQuestionCard"></div>

        <aside>
          <div class="palette-box">
            <div style="display: flex; justify-content: space-between; align-items: center;">
              <h4>Question Palette</h4>
              <span style="font-size:0.8rem; color:var(--text-muted);" id="paletteCount">0 / 20</span>
            </div>

            <div class="palette-legend">
              <div class="legend-item"><span class="legend-dot" style="background:#059669;"></span> Done</div>
              <div class="legend-item"><span class="legend-dot" style="background:#f59e0b;"></span> Skipped</div>
              <div class="legend-item"><span class="legend-dot" style="background:#7dd3fc;"></span> Active</div>
              <div class="legend-item"><span class="legend-dot" style="background:#f0f9ff; border:1px solid #bae6fd;"></span> Unseen</div>
            </div>
            
            <div class="palette-section-title">Worked Examples (Q1 – Q4)</div>
            <div class="palette-grid" id="paletteExamplesGrid"></div>

            <div class="palette-section-title">Exercise 8.3 Q1 - Q3 (Q5 – Q10)</div>
            <div class="palette-grid" id="paletteExGrid"></div>

            <div class="palette-section-title">Exercise 8.3 Q4 Proofs (Q11 – Q20)</div>
            <div class="palette-grid" id="paletteProofsGrid"></div>
          </div>

          <div class="palette-box" id="toolsPanel">
            <div class="tool-tabs">
              <button id="tabKeypadBtn" class="active" onclick="toggleTool('keypad')">Math Keypad</button>
              <button id="tabCalcBtn" onclick="toggleTool('calc')">Calculator</button>
            </div>

            <div id="toolKeypad">
              <div class="keypad-grid">
                <button class="keypad-btn" onclick="insertSymbol('/')">/</button>
                <button class="keypad-btn" onclick="insertSymbol('√')">√</button>
                <button class="keypad-btn" onclick="insertSymbol('^2')">\(^2\)</button>
                <button class="keypad-btn" onclick="insertSymbol('+')">+</button>
                <button class="keypad-btn" onclick="insertSymbol('-')">-</button>
                <button class="keypad-btn" onclick="insertSymbol('(')">(</button>
                <button class="keypad-btn" onclick="insertSymbol(')')">)</button>
                <button class="keypad-btn" onclick="insertSymbol('1')">1</button>
                <button class="keypad-btn" onclick="insertSymbol('θ')">θ</button>
                <button class="keypad-btn" onclick="insertSymbol('A')">A</button>
                <button class="keypad-btn" onclick="insertSymbol('sin')">sin</button>
                <button class="keypad-btn" onclick="insertSymbol('cos')">cos</button>
                <button class="keypad-btn" onclick="insertSymbol('tan')">tan</button>
                <button class="keypad-btn" onclick="insertSymbol('cot')">cot</button>
                <button class="keypad-btn" onclick="insertSymbol('sec')">sec</button>
                <button class="keypad-btn" onclick="insertSymbol('cosec')">cosec</button>
              </div>
            </div>

            <div id="toolCalc" style="display: none;">
              <input type="text" id="calcDisplay" readonly value="" />
              <div class="keypad-grid">
                <button class="keypad-btn" onclick="pressCalc('7')">7</button>
                <button class="keypad-btn" onclick="pressCalc('8')">8</button>
                <button class="keypad-btn" onclick="pressCalc('9')">9</button>
                <button class="keypad-btn" onclick="pressCalc('/')">/</button>
                <button class="keypad-btn" onclick="pressCalc('4')">4</button>
                <button class="keypad-btn" onclick="pressCalc('5')">5</button>
                <button class="keypad-btn" onclick="pressCalc('6')">6</button>
                <button class="keypad-btn" onclick="pressCalc('*')">*</button>
                <button class="keypad-btn" onclick="pressCalc('1')">1</button>
                <button class="keypad-btn" onclick="pressCalc('2')">2</button>
                <button class="keypad-btn" onclick="pressCalc('3')">3</button>
                <button class="keypad-btn" onclick="pressCalc('-')">-</button>
                <button class="keypad-btn" onclick="pressCalc('0')">0</button>
                <button class="keypad-btn" onclick="pressCalc('.')">.</button>
                <button class="keypad-btn" onclick="calcEval()">=</button>
                <button class="keypad-btn" onclick="pressCalc('+')">+</button>
                <button class="keypad-btn" style="grid-column: span 2;" onclick="calcClear()">C</button>
                <button class="keypad-btn" style="grid-column: span 2;" onclick="calcSqrt()">√</button>
              </div>
            </div>
          </div>
        </aside>
      </div>
    </div>

    <!-- View 3: Complete Solutions -->
    <div id="solutionsView" class="view">
      <div class="hero-score-card">
        <h2>Chapter Performance Report</h2>
        <div class="score-badge" id="scoreValue">0 / 20</div>
        <p id="scoreSubtitle">Complete active questions to review your diagnostic analysis.</p>
        <button class="btn-primary" style="margin-top: 14px; max-width: 200px;" onclick="window.print()">🖨️ Print Solutions</button>
      </div>
      <div id="completeSolutionsContainer"></div>
    </div>
  </main>

  <div class="toast" id="toastMessage"></div>

  <script>
    function renderTable(headers, rows) {
      let ths = headers.map(h => `<th>${h}</th>`).join('');
      let trs = rows.map(r => `<tr>${r.map(c => `<td>${c}</td>`).join('')}</tr>`).join('');
      return `<div class="table-container"><table class="stat-table"><thead><tr>${ths}</tr></thead><tbody>${trs}</tbody></table></div>`;
    }

    const CHAPTER_QUESTIONS = [
      // ========== WORKED EXAMPLES (Q1 - Q4) ==========
      {
        id: 1,
        concept: "example",
        source: "Example 9",
        title: "Express cos A, tan A and sec A in terms of sin A",
        prompt: "Express the trigonometric ratios \\(\\cos A\\), \\(\\tan A\\) and \\(\\sec A\\) in terms of \\(\\sin A\\).",
        table: renderTable(
          ["Target Ratio", "Pythagorean Identity", "Expression in \\(\\sin A\\)"],
          [
            ["\\(\\cos A\\)", "\\(\\cos^2 A = 1 - \\sin^2 A\\)", "\\(\\sqrt{1 - \\sin^2 A}\\)"],
            ["\\(\\tan A\\)", "\\(\\tan A = \\frac{\\sin A}{\\cos A}\\)", "\\(\\frac{\\sin A}{\\sqrt{1 - \\sin^2 A}}\\)"],
            ["\\(\\sec A\\)", "\\(\\sec A = \\frac{1}{\\cos A}\\)", "\\(\\frac{1}{\\sqrt{1 - \\sin^2 A}}\\)"]
          ]
        ),
        svg: `<svg width="200" height="110" viewBox="0 0 120 70">
          <rect x="15" y="15" width="90" height="40" rx="6" fill="#f0f9ff" stroke="#0c4a6e" stroke-width="1.5"/>
          <text x="24" y="38" font-size="8" fill="#0284c7">cos²A + sin²A = 1</text>
        </svg>`,
        steps: [
          { prefix: "Step 1: Using \\(\\cos^2 A = 1 - \\sin^2 A\\), \\(\\cos A = \\sqrt{1 - \\text{?}}\\). Enter the missing term (sin^2 A):", expected: "sin^2 A", suffix: ".", explanation: "\\[\\cos A = \\sqrt{1 - \\sin^2 A}\\]" },
          { prefix: "Step 2: Since \\(\\tan A = \\frac{\\sin A}{\\cos A}\\), denominator in terms of \\(\\sin A\\) is \\(\\sqrt{1 - \\text{?}}\\):", expected: "sin^2 A", suffix: ".", explanation: "\\[\\tan A = \\frac{\\sin A}{\\sqrt{1 - \\sin^2 A}}\\]" },
          { prefix: "Step 3: Reciprocal \\(\\sec A = \\frac{1}{\\cos A} = \\frac{1}{\\sqrt{1 - \\text{?}}}\\):", expected: "sin^2 A", suffix: ".", explanation: "\\[\\sec A = \\frac{1}{\\sqrt{1 - \\sin^2 A}}\\]" }
        ]
      },
      {
        id: 2,
        concept: "example",
        source: "Example 10",
        title: "Proof: sec A (1 - sin A)(sec A + tan A) = 1",
        prompt: "Prove that \\(\\sec A (1 - \\sin A)(\\sec A + \\tan A) = 1\\).",
        table: renderTable(
          ["Expression", "\\(\\sec A(1 - \\sin A)(\\sec A + \\tan A)\\)"],
          [["Conversion", "\\(\\left(\\frac{1}{\\cos A}\\right)(1 - \\sin A)\\left(\\frac{1 + \\sin A}{\\cos A}\\right) = \\frac{1 - \\sin^2 A}{\\cos^2 A}\\)"]]
        ),
        svg: `<svg width="200" height="110" viewBox="0 0 120 70">
          <polygon points="20,55 90,55 90,20" fill="#f0f9ff" stroke="#0c4a6e" stroke-width="1.5"/>
          <text x="35" y="45" font-size="7" fill="#0284c7">LHS = RHS = 1</text>
        </svg>`,
        steps: [
          { prefix: "Step 1: Convert terms to \\(\\sin, \\cos\\): \\(\\sec A + \\tan A = \\frac{1}{\\cos A} + \\frac{\\sin A}{\\cos A} = \\frac{1 + \\sin A}{\\text{?}}\\):", expected: "cos A", suffix: ".", explanation: "\\[\\sec A + \\tan A = \\frac{1 + \\sin A}{\\cos A}\\]" },
          { prefix: "Step 2: Multiply numerators: \\((1 - \\sin A)(1 + \\sin A) = 1 - \\text{?}\\):", expected: "sin^2 A", suffix: ".", explanation: "\\[(1 - \\sin A)(1 + \\sin A) = 1 - \\sin^2 A\\]" },
          { prefix: "Step 3: Since \\(1 - \\sin^2 A = \\cos^2 A\\), the ratio \\(\\frac{\\cos^2 A}{\\cos^2 A} =\\)", expected: "1", suffix: ", completing the proof.", explanation: "\\[\\frac{\\cos^2 A}{\\cos^2 A} = 1\\]" }
        ]
      },
      {
        id: 3,
        concept: "example",
        source: "Example 11",
        title: "Proof: (cot A - cos A)/(cot A + cos A) = (cosec A - 1)/(cosec A + 1)",
        prompt: "Prove that \\(\\frac{\\cot A - \\cos A}{\\cot A + \\cos A} = \\frac{\\operatorname{cosec} A - 1}{\\operatorname{cosec} A + 1}\\).",
        table: renderTable(
          ["Numerator", "\\(\\cot A - \\cos A = \\frac{\\cos A}{\\sin A} - \\cos A = \\cos A\\left(\\frac{1}{\\sin A} - 1\\right)\\)"],
          [["Denominator", "\\(\\cot A + \\cos A = \\frac{\\cos A}{\\sin A} + \\cos A = \\cos A\\left(\\frac{1}{\\sin A} + 1\\right)\\)"]]
        ),
        svg: `<svg width="200" height="110" viewBox="0 0 120 70">
          <rect x="15" y="15" width="90" height="40" rx="4" fill="#f0f9ff" stroke="#0c4a6e" stroke-width="1.5"/>
          <text x="25" y="38" font-size="8" fill="#0284c7">Factor out cos A</text>
        </svg>`,
        steps: [
          { prefix: "Step 1: Write \\(\\cot A = \\frac{\\cos A}{\\sin A}\\). Factoring \\(\\cos A\\) from numerator gives \\(\\cos A\\left(\\frac{1}{\\sin A} - \\text{?}\\right)\\):", expected: "1", suffix: ".", explanation: "\\[\\cos A\\left(\\frac{1}{\\sin A} - 1\\right)\\]" },
          { prefix: "Step 2: Factoring \\(\\cos A\\) from denominator gives \\(\\cos A\\left(\\frac{1}{\\sin A} + \\text{?}\\right)\\):", expected: "1", suffix: ".", explanation: "\\[\\cos A\\left(\\frac{1}{\\sin A} + 1\\right)\\]" },
          { prefix: "Step 3: Cancelling \\(\\cos A\\) and replacing \\(\\frac{1}{\\sin A}\\) by \\(\\operatorname{cosec} A\\) gives \\(\\frac{\\operatorname{cosec} A - 1}{\\operatorname{cosec} A + 1}\\). Is LHS = RHS?", expected: "yes", suffix: "(yes/no)", explanation: "\\[\\frac{\\operatorname{cosec} A - 1}{\\operatorname{cosec} A + 1} = \\text{RHS}\\]" }
        ]
      },
      {
        id: 4,
        concept: "example",
        source: "Example 12",
        title: "Proof: (sin θ - cos θ + 1)/(sin θ + cos θ - 1) = 1/(sec θ - tan θ)",
        prompt: "Prove that \\(\\frac{\\sin\\theta - \\cos\\theta + 1}{\\sin\\theta + \\cos\\theta - 1} = \\frac{1}{\\sec\\theta - \\tan\\theta}\\), using identity \\(\\sec^2\\theta = 1 + \\tan^2\\theta\\).",
        table: renderTable(
          ["Step 1", "Divide numerator and denominator by \\(\\cos\\theta\\)", "\\(\\frac{\\tan\\theta - 1 + \\sec\\theta}{\\tan\\theta + 1 - \\sec\\theta}\\)"],
          [["Step 2", "Multiply and simplify with \\(\\sec\\theta - \\tan\\theta\\)", "RHS: \\(\\frac{1}{\\sec\\theta - \\tan\\theta}\\)"]]
        ),
        svg: `<svg width="200" height="110" viewBox="0 0 120 70">
          <rect x="15" y="15" width="90" height="40" rx="4" fill="#f0f9ff" stroke="#0c4a6e" stroke-width="1.5"/>
          <text x="25" y="38" font-size="8" fill="#0284c7">sec²θ - tan²θ = 1</text>
        </svg>`,
        steps: [
          { prefix: "Step 1: Dividing numerator & denominator by \\(\\cos\\theta\\) gives \\(\\frac{\\tan\\theta - 1 + \\sec\\theta}{\\tan\\theta + 1 - \\sec\\theta}\\). In numerator, grouping \\((\\tan\\theta + \\sec\\theta) - \\text{?}\\):", expected: "1", suffix: ".", explanation: "\\[(\\tan\\theta + \\sec\\theta) - 1\\]" },
          { prefix: "Step 2: Replace constant 1 in numerator by \\(\\sec^2\\theta - \\text{?}\\):", expected: "tan^2 θ", suffix: ".", explanation: "\\[1 = \\sec^2\\theta - \\tan^2\\theta\\]" },
          { prefix: "Step 3: Factoring \\((\\sec\\theta - \\tan\\theta)(\\sec\\theta + \\tan\\theta)\\) and simplifying leaves \\(\\frac{1}{\\sec\\theta - \\text{?}}\\):", expected: "tan θ", suffix: ".", explanation: "\\[\\frac{1}{\\sec\\theta - \\tan\\theta}\\]" }
        ]
      },

      // ========== EXERCISE 8.3 Q1 - Q3 (Q5 - Q10) ==========
      {
        id: 5,
        concept: "proof",
        source: "Exercise 8.3 Q1",
        title: "Express sin A, sec A and tan A in terms of cot A",
        prompt: "Express the trigonometric ratios \\(\\sin A\\), \\(\\sec A\\) and \\(\\tan A\\) in terms of \\(\\cot A\\).",
        table: renderTable(
          ["Ratio", "Primary Identity", "In terms of \\(\\cot A\\)"],
          [
            ["\\(\\sin A\\)", "\\(\\operatorname{cosec}^2 A = 1 + \\cot^2 A\\)", "\\(\\frac{1}{\\sqrt{1 + \\cot^2 A}}\\)"],
            ["\\(\\tan A\\)", "Reciprocal of \\(\\cot A\\)", "\\(\\frac{1}{\\cot A}\\)"],
            ["\\(\\sec A\\)", "\\(\\sec^2 A = 1 + \\tan^2 A = 1 + \\frac{1}{\\cot^2 A}\\)", "\\(\\frac{\\sqrt{1 + \\cot^2 A}}{\\cot A}\\)"]
          ]
        ),
        svg: `<svg width="200" height="110" viewBox="0 0 120 70">
          <text x="20" y="38" font-size="8" fill="#0c4a6e">cosec²A = 1 + cot²A</text>
        </svg>`,
        steps: [
          { prefix: "Step 1: \\(\\operatorname{cosec} A = \\sqrt{1 + \\cot^2 A}\\). Therefore \\(\\sin A = \\frac{1}{\\sqrt{1 + \\text{?}}}\\):", expected: "cot^2 A", suffix: ".", explanation: "\\[\\sin A = \\frac{1}{\\sqrt{1 + \\cot^2 A}}\\]" },
          { prefix: "Step 2: \\(\\tan A = \\frac{1}{\\text{?}}\\):", expected: "cot A", suffix: ".", explanation: "\\[\\tan A = \\frac{1}{\\cot A}\\]" },
          { prefix: "Step 3: \\(\\sec A = \\sqrt{1 + \\frac{1}{\\cot^2 A}} = \\frac{\\sqrt{\\cot^2 A + 1}}{\\text{?}}\\):", expected: "cot A", suffix: ".", explanation: "\\[\\sec A = \\frac{\\sqrt{1 + \\cot^2 A}}{\\cot A}\\]" }
        ]
      },
      {
        id: 6,
        concept: "proof",
        source: "Exercise 8.3 Q2",
        title: "Write All Other Trig Ratios in terms of sec A",
        prompt: "Write all the other trigonometric ratios of \\(\\angle A\\) in terms of \\(\\sec A\\).",
        table: renderTable(
          ["Ratio", "Formula Transformation in \\(\\sec A\\)"],
          [
            ["\\(\\cos A\\)", "\\(\\frac{1}{\\sec A}\\)"],
            ["\\(\\tan A\\)", "\\(\\sqrt{\\sec^2 A - 1}\\)"],
            ["\\(\\sin A\\)", "\\(\\frac{\\sqrt{\\sec^2 A - 1}}{\\sec A}\\)"]
          ]
        ),
        svg: `<svg width="200" height="110" viewBox="0 0 120 70">
          <text x="25" y="38" font-size="8" fill="#0c4a6e">sec²A - tan²A = 1</text>
        </svg>`,
        steps: [
          { prefix: "Step 1: Cosine is the reciprocal: \\(\\cos A = \\frac{1}{\\text{?}}\\):", expected: "sec A", suffix: ".", explanation: "\\[\\cos A = \\frac{1}{\\sec A}\\]" },
          { prefix: "Step 2: Using identity \\(\\tan^2 A = \\sec^2 A - 1\\), \\(\\tan A = \\sqrt{\\sec^2 A - \\text{?}}\\):", expected: "1", suffix: ".", explanation: "\\[\\tan A = \\sqrt{\\sec^2 A - 1}\\]" },
          { prefix: "Step 3: Sine \\(\\sin A = \\tan A \\times \\cos A = \\frac{\\sqrt{\\sec^2 A - 1}}{\\text{?}}\\):", expected: "sec A", suffix: ".", explanation: "\\[\\sin A = \\frac{\\sqrt{\\sec^2 A - 1}}{\\sec A}\\]" }
        ]
      },
      {
        id: 7,
        concept: "mcq",
        source: "Exercise 8.3 Q3(i)",
        title: "Evaluation: 9 sec²A - 9 tan²A",
        prompt: "Choose the correct option: \\(9\\sec^2 A - 9\\tan^2 A =\\) (A) 1, (B) 9, (C) 8, (D) 0.",
        table: renderTable(
          ["Factoring 9", "\\(9(\\sec^2 A - \\tan^2 A)\\)"],
          [["Identity", "\\(\\sec^2 A - \\tan^2 A = 1 \\implies 9(1) = 9\\)"]]
        ),
        svg: `<svg width="180" height="90" viewBox="0 0 100 50">
          <text x="15" y="28" font-size="8" fill="#0c4a6e">9(sec²A - tan²A)</text>
        </svg>`,
        steps: [
          { prefix: "Step 1: Identity \\(\\sec^2 A - \\tan^2 A =\\)", expected: "1", suffix: ".", explanation: "\\[\\sec^2 A - \\tan^2 A = 1\\]" },
          { prefix: "Step 2: Therefore \\(9 \\times 1 =\\)", expected: "9", suffix: "(Option B).", explanation: "\\[9(1) = 9\\]" }
        ]
      },
      {
        id: 8,
        concept: "mcq",
        source: "Exercise 8.3 Q3(ii)",
        title: "Evaluation: (1 + tan θ + sec θ)(1 + cot θ - cosec θ)",
        prompt: "Choose the correct option: \\((1 + \\tan\\theta + \\sec\\theta)(1 + \\cot\\theta - \\operatorname{cosec}\\theta) =\\) (A) 0, (B) 1, (C) 2, (D) -1.",
        table: renderTable(
          ["Term 1", "\\(1 + \\frac{\\sin\\theta}{\\cos\\theta} + \\frac{1}{\\cos\\theta} = \\frac{\\cos\\theta + \\sin\\theta + 1}{\\cos\\theta}\\)"],
          [["Term 2", "\\(1 + \\frac{\\cos\\theta}{\\sin\\theta} - \\frac{1}{\\sin\\theta} = \\frac{\\sin\\theta + \\cos\\theta - 1}{\\sin\\theta}\\)"]]
        ),
        svg: `<svg width="180" height="90" viewBox="0 0 100 50">
          <text x="10" y="28" font-size="7" fill="#0c4a6e">[(sin+cos)² - 1] / sin·cos</text>
        </svg>`,
        steps: [
          { prefix: "Step 1: Numerator is of form \\((a + 1)(a - 1) = a^2 - 1 = (\\cos\\theta + \\sin\\theta)^2 - 1\\). Expanding gives \\(1 + 2\\sin\\theta\\cos\\theta - 1 = 2\\sin\\theta\\cos\\theta\\). In denominator we have \\(\\cos\\theta\\sin\\theta\\). The quotient is", expected: "2", suffix: "(Option C).", explanation: "\\[\\frac{2\\sin\\theta\\cos\\theta}{\sin\\theta\\cos\\theta} = 2\\]" }
        ]
      },
      {
        id: 9,
        concept: "mcq",
        source: "Exercise 8.3 Q3(iii)",
        title: "Evaluation: (sec A + tan A)(1 - sin A)",
        prompt: "Choose the correct option: \\((\\sec A + \\tan A)(1 - \\sin A) =\\) (A) \\(\\sec A\\), (B) \\(\\sin A\\), (C) \\(\\operatorname{cosec} A\\), (D) \\(\\cos A\\).",
        table: renderTable(
          ["Rewrite", "\\(\\left(\\frac{1 + \\sin A}{\\cos A}\\right)(1 - \\sin A)\\)"],
          [["Simplify", "\\(\\frac{1 - \\sin^2 A}{\\cos A} = \\frac{\\cos^2 A}{\\cos A} = \\cos A\\)"]]
        ),
        svg: `<svg width="180" height="90" viewBox="0 0 100 50">
          <text x="15" y="28" font-size="8" fill="#0c4a6e">(1 - sin²A) / cos A</text>
        </svg>`,
        steps: [
          { prefix: "Step 1: Numerator \\((1 + \\sin A)(1 - \\sin A) = 1 - \\sin^2 A = \\cos^2 A\\). Dividing by \\(\\cos A\\) yields", expected: "cos A", suffix: "(Option D).", explanation: "\\[\\frac{\\cos^2 A}{\\cos A} = \\cos A\\]" }
        ]
      },
      {
        id: 10,
        concept: "mcq",
        source: "Exercise 8.3 Q3(iv)",
        title: "Evaluation: (1 + tan²A)/(1 + cot²A)",
        prompt: "Choose the correct option: \\(\\frac{1 + \\tan^2 A}{1 + \\cot^2 A} =\\) (A) \\(\\sec^2 A\\), (B) -1, (C) \\(\\cot^2 A\\), (D) \\(\\tan^2 A\\).",
        table: renderTable(
          ["Numerator", "\\(1 + \\tan^2 A = \\sec^2 A\\)"],
          [["Denominator", "\\(1 + \\cot^2 A = \\operatorname{cosec}^2 A\\)"]]
        ),
        svg: `<svg width="180" height="90" viewBox="0 0 100 50">
          <text x="20" y="28" font-size="8" fill="#0c4a6e">sec²A / cosec²A</text>
        </svg>`,
        steps: [
          { prefix: "Step 1: \\(\\frac{\\sec^2 A}{\\operatorname{cosec}^2 A} = \\frac{1/\\cos^2 A}{1/\\sin^2 A} = \\frac{\\sin^2 A}{\\cos^2 A} =\\)", expected: "tan^2 A", suffix: "(Option D).", explanation: "\\[\\frac{\\sin^2 A}{\\cos^2 A} = \\tan^2 A\\]" }
        ]
      },

      // ========== EXERCISE 8.3 Q4 PROOFS (Q11 - Q20) ==========
      {
        id: 11,
        concept: "proof",
        source: "Exercise 8.3 Q4(i)",
        title: "Proof: (cosec θ - cot θ)² = (1 - cos θ)/(1 + cos θ)",
        prompt: "Prove that \\((\\operatorname{cosec}\\theta - \\cot\\theta)^2 = \\frac{1 - \\cos\\theta}{1 + \\cos\\theta}\\).",
        table: renderTable(
          ["LHS", "\\(\\left(\\frac{1 - \\cos\\theta}{\\sin\\theta}\\right)^2 = \\frac{(1 - \\cos\\theta)^2}{\\sin^2\\theta}\\)"],
          [["RHS", "\\(\\frac{(1 - \\cos\\theta)^2}{1 - \\cos^2\\theta} = \\frac{(1 - \\cos\\theta)^2}{(1 - \\cos\\theta)(1 + \\cos\\theta)}\\)"]]
        ),
        svg: `<svg width="200" height="100" viewBox="0 0 120 60">
          <text x="20" y="32" font-size="8" fill="#0c4a6e">(1 - cos θ) / (1 + cos θ)</text>
        </svg>`,
        steps: [
          { prefix: "Step 1: Write \\(\\operatorname{cosec}\\theta - \\cot\\theta = \\frac{1 - \\cos\\theta}{\\sin\\theta}\\). Squaring gives \\(\\frac{(1 - \\cos\\theta)^2}{\\text{?}}\\):", expected: "sin^2 θ", suffix: ".", explanation: "\\[\\frac{(1 - \\cos\\theta)^2}{\\sin^2\\theta}\\]" },
          { prefix: "Step 2: Replace \\(\\sin^2\\theta = 1 - \\cos^2\\theta = (1 - \\cos\\theta)(1 + \\text{?})\\):", expected: "cos θ", suffix: ".", explanation: "\\[1 - \\cos^2\\theta = (1 - \\cos\\theta)(1 + \\cos\\theta)\\]" },
          { prefix: "Step 3: Cancelling \\((1 - \\cos\\theta)\\) leaves \\(\\frac{1 - \\cos\\theta}{1 + \\cos\\theta}\\). Is LHS = RHS?", expected: "yes", suffix: "(yes/no)", explanation: "Proof complete." }
        ]
      },
      {
        id: 12,
        concept: "proof",
        source: "Exercise 8.3 Q4(ii)",
        title: "Proof: cos A / (1 + sin A) + (1 + sin A) / cos A = 2 sec A",
        prompt: "Prove that \\(\\frac{\\cos A}{1 + \\sin A} + \\frac{1 + \\sin A}{\\cos A} = 2\\sec A\\).",
        table: renderTable(
          ["Common Denominator", "\\(\\cos A(1 + \\sin A)\\)"],
          [["Expanded Numerator", "\\(\\cos^2 A + (1 + \\sin A)^2 = \\cos^2 A + 1 + 2\\sin A + \\sin^2 A\\)"]]
        ),
        svg: `<svg width="200" height="100" viewBox="0 0 120 60">
          <text x="25" y="32" font-size="8" fill="#0c4a6e">2(1 + sin A) / [cos A(1 + sin A)]</text>
        </svg>`,
        steps: [
          { prefix: "Step 1: Numerator \\(\\cos^2 A + \\sin^2 A + 1 + 2\\sin A = 1 + 1 + 2\\sin A = 2 + 2\\sin A = 2(1 + \\text{?})\\):", expected: "sin A", suffix: ".", explanation: "\\[2(1 + \\sin A)\\]" },
          { prefix: "Step 2: Cancelling \\((1 + \\sin A)\\) gives \\(\\frac{2}{\\cos A} = 2 \\times \\text{?}\\):", expected: "sec A", suffix: ".", explanation: "\\[\\frac{2}{\\cos A} = 2\\sec A\\]" }
        ]
      },
      {
        id: 13,
        concept: "proof",
        source: "Exercise 8.3 Q4(iii)",
        title: "Proof: tan θ / (1 - cot θ) + cot θ / (1 - tan θ) = 1 + sec θ cosec θ",
        prompt: "Prove that \\(\\frac{\\tan\\theta}{1 - \\cot\\theta} + \\frac{\\cot\\theta}{1 - \\tan\\theta} = 1 + \\sec\\theta\\operatorname{cosec}\\theta\\).",
        table: renderTable(
          ["In terms of \\(\\sin, \\cos\\)", "\\(\\frac{\\sin^2\\theta}{\\cos\\theta(\\sin\\theta - \\cos\\theta)} - \\frac{\\cos^2\\theta}{\\sin\\theta(\\sin\\theta - \\cos\\theta)}\\)"],
          [["Numerator", "\\(\\sin^3\\theta - \\cos^3\\theta = (\\sin\\theta - \\cos\\theta)(1 + \\sin\\theta\\cos\\theta)\\)"]]
        ),
        svg: `<svg width="200" height="100" viewBox="0 0 120 60">
          <text x="15" y="32" font-size="7" fill="#0c4a6e">sin³θ - cos³θ factoring</text>
        </svg>`,
        steps: [
          { prefix: "Step 1: Combining fractions over \\(\\sin\\theta\\cos\\theta(\\sin\\theta - \\cos\\theta)\\) yields numerator \\(\\sin^3\\theta - \\text{?}\\):", expected: "cos^3 θ", suffix: ".", explanation: "\\[\\sin^3\\theta - \\cos^3\\theta\\]" },
          { prefix: "Step 2: Factoring \\(a^3 - b^3\\) leaves \\(1 + \\sin\\theta\\cos\\theta\\). Dividing by \\(\\sin\\theta\\cos\\theta\\) yields \\(\\frac{1}{\\sin\\theta\\cos\\theta} + \\text{?}\\):", expected: "1", suffix: ".", explanation: "\\[1 + \\sec\\theta\\operatorname{cosec}\\theta\\]" },
          { prefix: "Step 3: Since \\(\\frac{1}{\\sin\\theta\\cos\\theta} = \\operatorname{cosec}\\theta\\sec\\theta\\), LHS = RHS verified?", expected: "yes", suffix: "(yes/no)", explanation: "Verified." }
        ]
      },
      {
        id: 14,
        concept: "proof",
        source: "Exercise 8.3 Q4(iv)",
        title: "Proof: (1 + sec A) / sec A = sin²A / (1 - cos A)",
        prompt: "Prove that \\(\\frac{1 + \\sec A}{\\sec A} = \\frac{\\sin^2 A}{1 - \\cos A}\\).",
        table: renderTable(
          ["LHS", "\\(\\frac{1 + 1/\\cos A}{1/\\cos A} = 1 + \\cos A\\)"],
          [["RHS", "\\(\\frac{\\sin^2 A}{1 - \\cos A} = \\frac{1 - \\cos^2 A}{1 - \\cos A} = \\frac{(1 - \\cos A)(1 + \\cos A)}{1 - \\cos A} = 1 + \\cos A\\)"]]
        ),
        svg: `<svg width="200" height="100" viewBox="0 0 120 60">
          <text x="25" y="32" font-size="8" fill="#0c4a6e">LHS = RHS = 1 + cos A</text>
        </svg>`,
        steps: [
          { prefix: "Step 1: Simplify LHS: \\(\\frac{1 + 1/\\cos A}{1/\\cos A} = 1 + \\text{?}\\):", expected: "cos A", suffix: ".", explanation: "\\[1 + \\cos A\\]" },
          { prefix: "Step 2: Simplify RHS: \\(\\frac{1 - \\cos^2 A}{1 - \\cos A} = \\frac{(1 - \\cos A)(1 + \\cos A)}{1 - \\cos A} = 1 + \\text{?}\\):", expected: "cos A", suffix: ".", explanation: "\\[1 + \\cos A\\]" },
          { prefix: "Step 3: Are LHS and RHS identical?", expected: "yes", suffix: "(yes/no)", explanation: "Both equal 1 + cos A." }
        ]
      },
      {
        id: 15,
        concept: "proof",
        source: "Exercise 8.3 Q4(v)",
        title: "Proof: (cos A - sin A + 1)/(cos A + sin A - 1) = cosec A + cot A",
        prompt: "Prove that \\(\\frac{\\cos A - \\sin A + 1}{\\cos A + \\sin A - 1} = \\operatorname{cosec} A + \\cot A\\), using \\(\\operatorname{cosec}^2 A = 1 + \\cot^2 A\\).",
        table: renderTable(
          ["Divide by \\(\\sin A\\)", "\\(\\frac{\\cot A - 1 + \\operatorname{cosec} A}{\\cot A + 1 - \\operatorname{cosec} A} = \\frac{(\\operatorname{cosec} A + \\cot A) - 1}{\\cot A - \\operatorname{cosec} A + 1}\\)"],
          [["Substitute 1", "\\(1 = \\operatorname{cosec}^2 A - \\cot^2 A = (\\operatorname{cosec} A - \\cot A)(\\operatorname{cosec} A + \\cot A)\\)"]]
        ),
        svg: `<svg width="200" height="100" viewBox="0 0 120 60">
          <text x="20" y="32" font-size="8" fill="#0c4a6e">cosec²A - cot²A = 1</text>
        </svg>`,
        steps: [
          { prefix: "Step 1: Dividing numerator & denominator by \\(\\sin A\\) gives \\(\\frac{\\cot A - 1 + \\operatorname{cosec} A}{\\cot A + 1 - \\operatorname{cosec} A}\\). In numerator, replace 1 by \\(\\operatorname{cosec}^2 A - \\text{?}\\):", expected: "cot^2 A", suffix: ".", explanation: "\\[1 = \\operatorname{cosec}^2 A - \\cot^2 A\\]" },
          { prefix: "Step 2: Factor out \\((\\operatorname{cosec} A + \\cot A)\\). The remaining factor cancels with denominator, leaving \\(\\operatorname{cosec} A + \\text{?}\\):", expected: "cot A", suffix: ".", explanation: "\\[\\operatorname{cosec} A + \\cot A\\]" }
        ]
      },
      {
        id: 16,
        concept: "proof",
        source: "Exercise 8.3 Q4(vi)",
        title: "Proof: √[(1 + sin A)/(1 - sin A)] = sec A + tan A",
        prompt: "Prove that \\(\\sqrt{\\frac{1 + \\sin A}{1 - \\sin A}} = \\sec A + \\tan A\\).",
        table: renderTable(
          ["Conjugate Multiplication", "\\(\\sqrt{\\frac{(1 + \\sin A)(1 + \\sin A)}{(1 - \\sin A)(1 + \\sin A)}} = \\sqrt{\\frac{(1 + \\sin A)^2}{1 - \\sin^2 A}}\\)"],
          [["Square Root", "\\(\\frac{1 + \\sin A}{\\cos A} = \\frac{1}{\\cos A} + \\frac{\\sin A}{\\cos A} = \\sec A + \\tan A\\)"]]
        ),
        svg: `<svg width="200" height="100" viewBox="0 0 120 60">
          <text x="20" y="32" font-size="8" fill="#0c4a6e">√(1 + sin A)² / cos²A</text>
        </svg>`,
        steps: [
          { prefix: "Step 1: Under radical, denominator becomes \\(1 - \\sin^2 A =\\)", expected: "cos^2 A", suffix: ".", explanation: "\\[1 - \\sin^2 A = \\cos^2 A\\]" },
          { prefix: "Step 2: Taking square root gives \\(\\frac{1 + \\sin A}{\\text{?}}\\):", expected: "cos A", suffix: ".", explanation: "\\[\\frac{1 + \\sin A}{\\cos A}\\]" },
          { prefix: "Step 3: Separating terms: \\(\\frac{1}{\\cos A} + \\frac{\\sin A}{\\cos A} = \\sec A + \\text{?}\\):", expected: "tan A", suffix: ".", explanation: "\\[\\sec A + \\tan A\\]" }
        ]
      },
      {
        id: 17,
        concept: "proof",
        source: "Exercise 8.3 Q4(vii)",
        title: "Proof: (sin θ - 2 sin³θ)/(2 cos³θ - cos θ) = tan θ",
        prompt: "Prove that \\(\\frac{\\sin\\theta - 2\\sin^3\\theta}{2\\cos^3\\theta - \\cos\\theta} = \\tan\\theta\\).",
        table: renderTable(
          ["Factor Out", "\\(\\frac{\\sin\\theta(1 - 2\\sin^2\\theta)}{\\cos\\theta(2\\cos^2\\theta - 1)}\\)"],
          [["Simplify", "\\(1 - 2\\sin^2\\theta = \\cos^2\\theta - \\sin^2\\theta = 2\\cos^2\\theta - 1\\)"]]
        ),
        svg: `<svg width="200" height="100" viewBox="0 0 120 60">
          <text x="20" y="32" font-size="8" fill="#0c4a6e">(sin θ / cos θ) × 1 = tan θ</text>
        </svg>`,
        steps: [
          { prefix: "Step 1: Factor out \\(\\sin\\theta\\) from numerator to get \\(\\sin\\theta(1 - 2\\text{?})\\):", expected: "sin^2 θ", suffix: ".", explanation: "\\[\\sin\\theta(1 - 2\\sin^2\\theta)\\]" },
          { prefix: "Step 2: In numerator replace \\(1 = \\sin^2\\theta + \\cos^2\\theta\\) to get \\(\\cos^2\\theta - \\sin^2\\theta\\). Both brackets cancel, leaving \\(\\frac{\\sin\\theta}{\\cos\\theta} =\\)", expected: "tan θ", suffix: ".", explanation: "\\[\\frac{\\sin\\theta}{\\cos\\theta} = \\tan\\theta\\]" }
        ]
      },
      {
        id: 18,
        concept: "proof",
        source: "Exercise 8.3 Q4(viii)",
        title: "Proof: (sin A + cosec A)² + (cos A + sec A)² = 7 + tan²A + cot²A",
        prompt: "Prove that \\((\\sin A + \\operatorname{cosec} A)^2 + (\\cos A + \\sec A)^2 = 7 + \\tan^2 A + \\cot^2 A\\).",
        table: renderTable(
          ["Expansion", "\\(\\sin^2 A + \\operatorname{cosec}^2 A + 2 + \\cos^2 A + \\sec^2 A + 2\\)"],
          [["Combine", "\\((\\sin^2 A + \\cos^2 A) + 4 + (1 + \\cot^2 A) + (1 + \\tan^2 A) = 7 + \\tan^2 A + \\cot^2 A\\)"]]
        ),
        svg: `<svg width="200" height="100" viewBox="0 0 120 60">
          <text x="15" y="32" font-size="8" fill="#0c4a6e">1 + 4 + 1 + 1 = 7</text>
        </svg>`,
        steps: [
          { prefix: "Step 1: Cross terms \\(2\\sin A\\operatorname{cosec} A + 2\\cos A\\sec A = 2(1) + 2(1) =\\)", expected: "4", suffix: ".", explanation: "\\[2 + 2 = 4\\]" },
          { prefix: "Step 2: Add \\(\\sin^2 A + \\cos^2 A = 1\\), \\(\\operatorname{cosec}^2 A = 1 + \\cot^2 A\\), and \\(\\sec^2 A = 1 + \\tan^2 A\\). Constant sum is \\(4 + 1 + 1 + 1 =\\)", expected: "7", suffix: ".", explanation: "\\[7 + \\tan^2 A + \\cot^2 A\\]" }
        ]
      },
      {
        id: 19,
        concept: "proof",
        source: "Exercise 8.3 Q4(ix)",
        title: "Proof: (cosec A - sin A)(sec A - cos A) = 1 / (tan A + cot A)",
        prompt: "Prove that \\((\\operatorname{cosec} A - \\sin A)(\\sec A - \\cos A) = \\frac{1}{\\tan A + \\cot A}\\).",
        table: renderTable(
          ["LHS", "\\(\\left(\\frac{\\cos^2 A}{\\sin A}\\right)\\left(\\frac{\\sin^2 A}{\\cos A}\\right) = \\sin A\\cos A\\)"],
          [["RHS", "\\(\\frac{1}{\\frac{\\sin A}{\\cos A} + \\frac{\\cos A}{\\sin A}} = \\frac{1}{\\frac{\\sin^2 A + \\cos^2 A}{\\sin A\\cos A}} = \\sin A\\cos A\\)"]]
        ),
        svg: `<svg width="200" height="100" viewBox="0 0 120 60">
          <text x="20" y="32" font-size="8" fill="#0c4a6e">LHS = RHS = sin A cos A</text>
        </svg>`,
        steps: [
          { prefix: "Step 1: LHS simplifies to \\(\\frac{\\cos^2 A}{\\sin A} \\times \\frac{\\sin^2 A}{\\cos A} =\\)", expected: "sin A cos A", suffix: ".", explanation: "\\[\\sin A\\cos A\\]" },
          { prefix: "Step 2: RHS denominator \\(\\tan A + \\cot A = \\frac{\\sin^2 A + \\cos^2 A}{\\sin A\\cos A} = \\frac{1}{\\sin A\\cos A}\\). Reciprocal is \\(\\sin A\\cos A\\). Does LHS = RHS?", expected: "yes", suffix: "(yes/no)", explanation: "Both equal sin A cos A." }
        ]
      },
      {
        id: 20,
        concept: "proof",
        source: "Exercise 8.3 Q4(x)",
        title: "Proof: (1 + tan²A)/(1 + cot²A) = [(1 - tan A)/(1 - cot A)]² = tan²A",
        prompt: "Prove that \\(\\frac{1 + \\tan^2 A}{1 + \\cot^2 A} = \\left(\\frac{1 - \\tan A}{1 - \\cot A}\\right)^2 = \\tan^2 A\\).",
        table: renderTable(
          ["Part 1", "\\(\\frac{\\sec^2 A}{\\operatorname{cosec}^2 A} = \\frac{\\sin^2 A}{\\cos^2 A} = \\tan^2 A\\)"],
          [["Part 2", "\\(\\left(\\frac{1 - \\tan A}{1 - 1/\\tan A}\\right)^2 = \\left(\\frac{1 - \\tan A}{\\frac{\\tan A - 1}{\\tan A}}\\right)^2 = (-\\tan A)^2 = \\tan^2 A\\)"]]
        ),
        svg: `<svg width="200" height="100" viewBox="0 0 120 60">
          <text x="25" y="32" font-size="8" fill="#0c4a6e">(-tan A)² = tan²A</text>
        </svg>`,
        steps: [
          { prefix: "Step 1: First expression \\(\\frac{\\sec^2 A}{\\operatorname{cosec}^2 A} =\\)", expected: "tan^2 A", suffix: ".", explanation: "\\[\\tan^2 A\\]" },
          { prefix: "Step 2: In second expression, rewrite \\(\\cot A = \\frac{1}{\\tan A}\\). Simplifying inside brackets gives \\(-\\tan A\\). Squaring gives", expected: "tan^2 A", suffix: ", proving all parts equal.", explanation: "\\[(-\\tan A)^2 = \\tan^2 A\\]" }
        ]
      }
    ];

    let currentAuthUser = null;
    let currentQuestionIndex = 0;
    let stepProgress = CHAPTER_QUESTIONS.map(() => ({ completedSteps: 0, status: "unseen" }));
    let stepAttempts = {}; // Key: "qIdx_sIdx", Value: int
    let audioMuted = false;
    let totalSeconds = 0;
    let timerInterval = null;
    let activeInputRef = null;

    const AudioEngine = {
      ctx: null,
      init() {
        if (!this.ctx) {
          this.ctx = new (window.AudioContext || window.webkitAudioContext)();
        }
      },
      playTone(freq, type, duration, delay = 0) {
        if (audioMuted || !this.ctx) return;
        setTimeout(() => {
          try {
            const osc = this.ctx.createOscillator();
            const gain = this.ctx.createGain();
            osc.type = type;
            osc.frequency.setValueAtTime(freq, this.ctx.currentTime);
            gain.gain.setValueAtTime(0.12, this.ctx.currentTime);
            gain.gain.exponentialRampToValueAtTime(0.0001, this.ctx.currentTime + duration);
            osc.connect(gain);
            gain.connect(this.ctx.destination);
            osc.start();
            osc.stop(this.ctx.currentTime + duration);
          } catch (e) {
            console.warn("AudioContext error", e);
          }
        }, delay * 1000);
      },
      correct() {
        this.init();
        this.playTone(659.25, 'sine', 0.15, 0);
        this.playTone(880.00, 'sine', 0.25, 0.12);
      },
      incorrect() {
        this.init();
        this.playTone(196.00, 'triangle', 0.2, 0);
        this.playTone(146.83, 'triangle', 0.3, 0.12);
      },
      milestone() {
        this.init();
        [523.25, 659.25, 783.99, 1046.50].forEach((freq, idx) => {
          this.playTone(freq, 'sine', 0.25, idx * 0.1);
        });
      }
    };

    function startTimer() {
      if (timerInterval) clearInterval(timerInterval);
      timerInterval = setInterval(() => {
        totalSeconds++;
        const mins = String(Math.floor(totalSeconds / 60)).padStart(2, '0');
        const secs = String(totalSeconds % 60).padStart(2, '0');
        document.getElementById('timerChip').innerText = `⏱️ ${mins}:${secs}`;

        if (totalSeconds === 1200 || (totalSeconds > 1200 && totalSeconds % 300 === 0)) {
          AudioEngine.milestone();
          showToast(`Pacing Check: ${Math.floor(totalSeconds / 60)} minutes elapsed.`);
        }
      }, 1000);
    }

    function showToast(msg) {
      const t = document.getElementById('toastMessage');
      t.innerText = msg;
      t.style.display = 'block';
      setTimeout(() => { t.style.display = 'none'; }, 3500);
    }

    function initDirectLogin() {
      const roll = document.getElementById('rollInput').value.trim() || 'Student-10';
      currentAuthUser = roll;
      sessionStorage.setItem('bm_user', roll);
      document.getElementById('userPill').innerText = `Roll No: ${roll}`;
      document.getElementById('loginGateView').style.display = 'none';
      AudioEngine.init();
      startTimer();
      renderPalettes();
      loadQuestion(0);
      renderSolutions();
    }

    function normalizeInput(str) {
      return str.toLowerCase().replace(/\s+/g, '').replace(/−/g, '-').replace(/theta/g, 'θ');
    }

    function parseNumeric(val) {
      if (val.includes('/')) {
        const parts = val.split('/');
        return parseFloat(parts[0]) / parseFloat(parts[1]);
      }
      return parseFloat(val);
    }

    function checkNumericalTolerance(val1, val2) {
      const n1 = parseNumeric(val1);
      const n2 = parseNumeric(val2);
      if (isNaN(n1) || isNaN(n2)) return false;
      return Math.abs(n1 - n2) <= 0.05;
    }

    function switchView(viewId) {
      document.querySelectorAll('.view').forEach(v => v.classList.remove('active'));
      document.querySelectorAll('nav button').forEach(b => b.classList.remove('active'));
      document.getElementById(viewId).classList.add('active');

      const btnMap = { 'theoryView': 0, 'sheetView': 1, 'solutionsView': 2 };
      document.querySelectorAll('nav button')[btnMap[viewId]].classList.add('active');

      if (window.MathJax && window.MathJax.typesetPromise) {
        MathJax.typesetPromise();
      }
    }

    function renderPalettes() {
      const exGrid = document.getElementById('paletteExamplesGrid');
      const qGrid = document.getElementById('paletteExGrid');
      const proofsGrid = document.getElementById('paletteProofsGrid');
      exGrid.innerHTML = '';
      qGrid.innerHTML = '';
      proofsGrid.innerHTML = '';

      let doneCount = 0;
      CHAPTER_QUESTIONS.forEach((q, idx) => {
        const state = stepProgress[idx];
        if (state.status === "completed") doneCount++;

        const btn = document.createElement('button');
        let stateClass = '';
        if (idx === currentQuestionIndex) {
          stateClass = 'active';
        } else if (state.status === "completed") {
          stateClass = 'completed';
        } else if (state.status === "skipped") {
          stateClass = 'skipped';
        }

        btn.className = `palette-btn ${stateClass}`;
        btn.innerText = idx + 1;
        btn.title = `${q.source}: ${q.title}`;
        btn.onclick = () => loadQuestion(idx);

        if (idx < 4) {
          exGrid.appendChild(btn);
        } else if (idx < 10) {
          qGrid.appendChild(btn);
        } else {
          proofsGrid.appendChild(btn);
        }
      });
      document.getElementById('paletteCount').innerText = `${doneCount} / ${CHAPTER_QUESTIONS.length}`;
    }

    function loadQuestion(idx) {
      currentQuestionIndex = idx;
      renderPalettes();
      const q = CHAPTER_QUESTIONS[idx];
      const prog = stepProgress[idx];

      let stepsHtml = '';
      q.steps.forEach((st, sIdx) => {
        const isUnlocked = sIdx <= prog.completedSteps;
        const isPassed = sIdx < prog.completedSteps;
        const key = `${idx}_${sIdx}`;
        const attempts = stepAttempts[key] || 0;

        stepsHtml += `
          <div class="step-box ${isUnlocked ? 'unlocked' : ''} ${isPassed ? 'success' : ''}" id="stepBox_${idx}_${sIdx}">
            <div class="step-text-wrap">
              <span>${st.prefix}</span>
              <input type="text" class="inline-blank" id="stepInput_${idx}_${sIdx}" 
                value="${isPassed ? st.expected : ''}" 
                placeholder="enter answer"
                ${isPassed ? 'disabled' : ''} 
                onfocus="activeInputRef = this;" />
              <span>${st.suffix}</span>
              ${!isPassed ? `
                <button class="btn-verify" onclick="verifyStep(${idx}, ${sIdx})">Verify</button>
                <span class="attempts-badge" id="attemptBadge_${idx}_${sIdx}">Attempts: ${attempts}/2</span>
                ${attempts >= 2 ? `<button class="btn-reveal" onclick="autoFillStep(${idx}, ${sIdx})">Auto-Fill Correct Answer</button>` : ''}
              ` : `<span style="color: var(--green-ok); font-weight: bold; margin-left: 8px;">✓ Verified</span>`}
            </div>
            ${isPassed ? `<div style="margin-top:10px; padding:10px; background:#eff6ff; border-radius:6px; border-left:4px solid var(--brand-blue); font-size:0.92rem; color:var(--text-main);">${st.explanation}</div>` : ''}
          </div>
        `;
      });

      const tagClass = q.concept === 'example' ? 'example' : (q.concept === 'mcq' ? 'mcq' : 'proof');
      const tagText = q.concept === 'example' ? 'NCERT Worked Example' : (q.concept === 'mcq' ? 'Multiple Choice' : 'Identity Proof');

      const prevDisabled = idx === 0 ? 'disabled' : '';
      const nextDisabled = idx === CHAPTER_QUESTIONS.length - 1 ? 'disabled' : '';

      const html = `
        <span class="concept-tag ${tagClass}">${tagText}</span>
        <span style="font-size:0.85rem; font-weight:700; color:var(--text-muted); margin-left: 8px;">[${q.source}]</span>
        <h2 style="color:var(--navy-dark); margin: 6px 0 10px 0;">Problem ${q.id}: ${q.title}</h2>
        <p style="margin-top: 8px; line-height: 1.65;">${q.prompt}</p>
        ${q.table ? q.table : ''}
        <div class="svg-container">${q.svg}</div>
        <div id="stepsContainer">${stepsHtml}</div>

        <!-- Action Toolbar -->
        <div class="nav-toolbar">
          <button class="btn-nav-action" onclick="navigateQuestion(-1)" ${prevDisabled}>
            ⏮ Previous
          </button>
          <div class="nav-btn-group">
            <button class="btn-nav-action btn-skip" onclick="skipQuestion()">
              ⏭ Skip Question
            </button>
            <button class="btn-nav-action" onclick="navigateQuestion(1)" ${nextDisabled}>
              Next ❯
            </button>
          </div>
        </div>
      `;

      document.getElementById('activeQuestionCard').innerHTML = html;
      if (window.MathJax && window.MathJax.typesetPromise) {
        MathJax.typesetPromise();
      }
    }

    function navigateQuestion(delta) {
      const target = currentQuestionIndex + delta;
      if (target >= 0 && target < CHAPTER_QUESTIONS.length) {
        loadQuestion(target);
      }
    }

    function skipQuestion() {
      if (stepProgress[currentQuestionIndex].status !== "completed") {
        stepProgress[currentQuestionIndex].status = "skipped";
      }
      showToast(`Question ${currentQuestionIndex + 1} marked as Skipped (Amber/Gold).`);
      renderPalettes();
      navigateQuestion(1);
    }

    function autoFillStep(qIdx, sIdx) {
      const inputEl = document.getElementById(`stepInput_${qIdx}_${sIdx}`);
      if (inputEl) {
        inputEl.value = CHAPTER_QUESTIONS[qIdx].steps[sIdx].expected;
        verifyStep(qIdx, sIdx);
      }
    }

    function verifyStep(qIdx, sIdx) {
      const inputEl = document.getElementById(`stepInput_${qIdx}_${sIdx}`);
      const val = normalizeInput(inputEl.value);
      const expected = normalizeInput(CHAPTER_QUESTIONS[qIdx].steps[sIdx].expected);
      const key = `${qIdx}_${sIdx}`;

      const isCorrect = (val === expected) || checkNumericalTolerance(val, expected);

      if (isCorrect) {
        AudioEngine.correct();
        stepProgress[qIdx].completedSteps++;
        if (stepProgress[qIdx].completedSteps >= CHAPTER_QUESTIONS[qIdx].steps.length) {
          stepProgress[qIdx].status = "completed";
          AudioEngine.milestone();
          showToast(`Problem ${qIdx + 1} Fully Completed!`);
        }
        renderPalettes();
        loadQuestion(qIdx);
        renderSolutions();
      } else {
        AudioEngine.incorrect();
        stepAttempts[key] = (stepAttempts[key] || 0) + 1;
        inputEl.style.borderColor = "var(--red-fail)";
        
        if (stepAttempts[key] >= 2) {
          showToast(`Hint: 2 attempts reached. The correct answer is '${CHAPTER_QUESTIONS[qIdx].steps[sIdx].expected}'. You may click Auto-Fill to continue.`);
        } else {
          showToast("Incorrect transformation or answer. Try once more!");
        }
        loadQuestion(qIdx);
      }
    }

    function renderSolutions() {
      const container = document.getElementById('completeSolutionsContainer');
      let completedCount = stepProgress.filter(p => p.status === "completed").length;
      document.getElementById('scoreValue').innerText = `${completedCount} / ${CHAPTER_QUESTIONS.length}`;

      let html = '';
      let lastConcept = '';

      CHAPTER_QUESTIONS.forEach((q) => {
        if (q.concept !== lastConcept) {
          lastConcept = q.concept;
          const sectionHeader = q.concept === 'example' 
            ? 'Section A: NCERT Worked Examples (Section 8.4)'
            : (q.concept === 'mcq' ? 'Section B: Exercise 8.3 Multiple Choice & Short Answer' : 'Section C: Exercise 8.3 Comprehensive Identity Proofs');
          html += `<h2 style="color:var(--navy-dark); margin: 30px 0 14px 0; border-bottom: 2px solid var(--border-soft); padding-bottom: 6px;">${sectionHeader}</h2>`;
        }

        html += `
          <div class="theory-card">
            <span class="concept-tag ${q.concept}">${q.concept.toUpperCase()}</span>
            <span style="font-size:0.8rem; font-weight:bold; color:var(--text-muted); margin-left:6px;">${q.source}</span>
            <h3 style="margin-top:6px;">Problem ${q.id}: ${q.title}</h3>
            <p>${q.prompt}</p>
            ${q.table ? q.table : ''}
            <div class="svg-container" style="max-width: 240px; margin: 12px 0;">${q.svg}</div>
            <div class="proof-section">
              ${q.steps.map((st, sIdx) => `
                <div class="proof-block">
                  <strong>Step ${sIdx + 1}:</strong> ${st.prefix} <strong>[ ${st.expected} ]</strong> ${st.suffix}<br/>
                  <div style="margin-top:6px;">${st.explanation}</div>
                </div>
              `).join('')}
            </div>
          </div>
        `;
      });
      container.innerHTML = html;
      if (window.MathJax && window.MathJax.typesetPromise) {
        MathJax.typesetPromise();
      }
    }

    function toggleTool(tool) {
      if (tool === 'keypad') {
        document.getElementById('toolKeypad').style.display = 'block';
        document.getElementById('toolCalc').style.display = 'none';
        document.getElementById('tabKeypadBtn').classList.add('active');
        document.getElementById('tabCalcBtn').classList.remove('active');
      } else {
        document.getElementById('toolKeypad').style.display = 'none';
        document.getElementById('toolCalc').style.display = 'block';
        document.getElementById('tabCalcBtn').classList.add('active');
        document.getElementById('tabKeypadBtn').classList.remove('active');
      }
    }

    function insertSymbol(sym) {
      if (activeInputRef) {
        activeInputRef.value += sym;
        activeInputRef.focus();
      }
    }

    function pressCalc(val) {
      document.getElementById('calcDisplay').value += val;
    }

    function calcClear() {
      document.getElementById('calcDisplay').value = '';
    }

    function calcEval() {
      try {
        const res = eval(document.getElementById('calcDisplay').value);
        document.getElementById('calcDisplay').value = res;
      } catch (e) {
        document.getElementById('calcDisplay').value = 'Error';
      }
    }

    function calcSqrt() {
      try {
        const val = parseFloat(document.getElementById('calcDisplay').value);
        document.getElementById('calcDisplay').value = Math.sqrt(val);
      } catch (e) {
        document.getElementById('calcDisplay').value = 'Error';
      }
    }

    document.getElementById('audioToggleBtn').onclick = () => {
      audioMuted = !audioMuted;
      document.getElementById('audioToggleBtn').innerText = audioMuted ? '🔇' : '🔊';
    };
  </script>
</body>
</html>
