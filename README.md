<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Andualem Guchi · Portfolio</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,300;14..32,400;14..32,500;14..32,600;14..32,700&family=Playfair+Display:ital,wght@0,500;0,600;0,700;1,600&display=swap" rel="stylesheet">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      background: #f0ece6;
      display: flex;
      flex-direction: column;
      align-items: center;
      padding: 2rem 1rem;
      font-family: 'Inter', sans-serif;
    }

    .portfolio-page {
      max-width: 1000px;
      width: 100%;
      background: #ffffff;
      border-radius: 36px;
      box-shadow: 0 25px 50px -12px rgba(0, 0, 0, 0.15), 0 8px 24px rgba(0, 0, 0, 0.03);
      padding: 2.4rem 2.4rem 1.8rem;
      border: 1px solid rgba(0, 0, 0, 0.04);
    }

    /* ===== HEADER ===== */
    .header-intro {
      margin-bottom: 2rem;
      padding-bottom: 1.2rem;
      border-bottom: 2px solid #f0ebe3;
      display: flex;
      flex-wrap: wrap;
      justify-content: space-between;
      align-items: center;
    }

    .name-title {
      font-family: 'Playfair Display', serif;
      font-weight: 700;
      font-size: 2.2rem;
      color: #0b2b3b;
      letter-spacing: -0.5px;
      line-height: 1.1;
    }

    .name-title small {
      font-family: 'Inter', sans-serif;
      font-weight: 400;
      font-size: 0.95rem;
      color: #3f5d6b;
      background: #ecf0ed;
      padding: 0.1rem 1.2rem;
      border-radius: 60px;
      letter-spacing: 0.3px;
      display: inline-block;
      margin-top: 0.2rem;
    }

    .tagline {
      font-size: 0.95rem;
      color: #2a4a5a;
      margin-top: 0.5rem;
      padding: 0.4rem 1.2rem;
      background: #f9f6f0;
      border-radius: 60px;
      display: inline-block;
      border-left: 4px solid #f5b042;
    }

    .header-right {
      text-align: right;
    }

    .header-right .availability {
      background: #e6f0ea;
      color: #0b3b2b;
      font-weight: 600;
      font-size: 0.75rem;
      padding: 0.3rem 1.2rem;
      border-radius: 60px;
      display: inline-block;
      letter-spacing: 0.5px;
      border: 1px solid #b5cfc0;
    }

    /* ===== ATTRACTIVE DIGITALIZED HERO IMAGE ===== */
    .hero-digital {
      position: relative;
      width: 100%;
      border-radius: 24px;
      overflow: hidden;
      margin-bottom: 2.4rem;
      background: linear-gradient(135deg, #0b2b3b 0%, #1a4a5e 30%, #d4a24e 80%, #4A2E1B 100%);
      min-height: 220px;
      display: flex;
      align-items: center;
      justify-content: center;
      padding: 2rem 1.8rem;
      border: 1px solid rgba(255,255,255,0.08);
      box-shadow: 0 12px 30px -8px rgba(0,0,0,0.25);
    }

    .hero-digital::before {
      content: '';
      position: absolute;
      inset: 0;
      background: 
        radial-gradient(circle at 20% 50%, rgba(212, 175, 55, 0.25) 0%, transparent 50%),
        radial-gradient(circle at 80% 20%, rgba(74, 46, 27, 0.4) 0%, transparent 40%),
        radial-gradient(circle at 60% 80%, rgba(253, 251, 247, 0.1) 0%, transparent 50%);
      background-blend-mode: overlay;
      animation: meshMove 12s ease-in-out infinite alternate;
    }

    @keyframes meshMove {
      0% { background-position: 0% 0%, 0% 0%, 0% 0%; }
      100% { background-position: 10% 20%, -10% 10%, 10% -10%; }
    }

    .hero-digital::after {
      content: '';
      position: absolute;
      inset: 0;
      background: url("data:image/svg+xml,%3Csvg width='60' height='60' viewBox='0 0 60 60' xmlns='http://www.w3.org/2000/svg'%3E%3Cg fill='none' fill-rule='evenodd'%3E%3Cg fill='%23ffffff' fill-opacity='0.04'%3E%3Cpath d='M36 34v-4h-2v4h-4v2h4v4h2v-4h4v-2h-4zm0-30V0h-2v4h-4v2h4v4h2V6h4V4h-4zM6 34v-4H4v4H0v2h4v4h2v-4h4v-2H6zM6 4V0H4v4H0v2h4v4h2V6h4V4H6z'/%3E%3C/g%3E%3C/g%3E%3C/svg%3E");
      opacity: 0.5;
    }

    .hero-digital-content {
      position: relative;
      z-index: 2;
      display: flex;
      flex-wrap: wrap;
      align-items: center;
      justify-content: center;
      gap: 1.8rem;
      width: 100%;
    }

    .hero-digital-content .left {
      flex: 1;
      min-width: 180px;
    }

    .hero-digital-content .left .hero-tagline {
      font-family: 'Playfair Display', serif;
      font-weight: 700;
      font-size: clamp(1.4rem, 3.5vw, 2.4rem);
      color: #FDFBF7;
      line-height: 1.2;
      text-shadow: 0 4px 20px rgba(0,0,0,0.3);
    }

    .hero-digital-content .left .hero-tagline .gold {
      color: #D4AF37;
      font-style: italic;
    }

    .hero-digital-content .left .hero-sub {
      color: rgba(255,255,255,0.8);
      font-size: 0.85rem;
      margin-top: 0.4rem;
      letter-spacing: 0.5px;
      font-weight: 300;
    }

    .hero-digital-content .right {
      display: flex;
      gap: 0.6rem;
      flex-wrap: wrap;
      align-items: center;
      justify-content: center;
    }

    .hero-digital-content .right .glass-card {
      background: rgba(253, 251, 247, 0.08);
      backdrop-filter: blur(12px);
      -webkit-backdrop-filter: blur(12px);
      border: 1px solid rgba(255,255,255,0.12);
      border-radius: 16px;
      padding: 0.6rem 1.2rem;
      display: flex;
      align-items: center;
      gap: 0.6rem;
      font-size: 0.75rem;
      color: #FDFBF7;
      font-weight: 500;
      letter-spacing: 0.3px;
      box-shadow: 0 8px 20px -8px rgba(0,0,0,0.3);
      transition: transform 0.2s ease;
    }

    .hero-digital-content .right .glass-card:hover {
      transform: translateY(-4px) scale(1.02);
    }

    .hero-digital-content .right .glass-card .icon {
      font-size: 1.4rem;
    }

    .hero-digital-content .right .glass-card .badge-dot {
      display: inline-block;
      width: 8px;
      height: 8px;
      background: #D4AF37;
      border-radius: 50%;
      animation: pulse-dot 2s ease-in-out infinite;
    }

    @keyframes pulse-dot {
      0%, 100% { opacity: 1; transform: scale(1); }
      50% { opacity: 0.4; transform: scale(0.7); }
    }

    .hero-digital-content .right .glass-card.gold {
      background: rgba(212, 175, 55, 0.2);
      border-color: rgba(212, 175, 55, 0.3);
    }

    .shape-float {
      position: absolute;
      border-radius: 50%;
      opacity: 0.1;
      pointer-events: none;
      z-index: 1;
    }

    .shape-float.s1 {
      width: 120px;
      height: 120px;
      background: #D4AF37;
      top: -20px;
      right: 10%;
      animation: float 8s ease-in-out infinite alternate;
    }

    .shape-float.s2 {
      width: 80px;
      height: 80px;
      background: #FDFBF7;
      bottom: -10px;
      left: 5%;
      animation: float 10s ease-in-out infinite alternate-reverse;
    }

    @keyframes float {
      0% { transform: translate(0, 0) scale(1); }
      100% { transform: translate(20px, -20px) scale(1.1); }
    }

    /* ===== PROJECTS ===== */
    .project-section {
      margin: 2rem 0 2.4rem;
    }

    .project-headline {
      font-family: 'Playfair Display', serif;
      font-weight: 600;
      font-size: 1.4rem;
      color: #0b2b3b;
      margin-bottom: 1rem;
      display: flex;
      align-items: center;
      gap: 0.8rem;
      flex-wrap: wrap;
    }

    .project-headline .badge {
      background: #0b2b3b;
      color: white;
      font-family: 'Inter', sans-serif;
      font-weight: 500;
      font-size: 0.6rem;
      padding: 0.2rem 1rem;
      border-radius: 40px;
      letter-spacing: 0.6px;
      text-transform: uppercase;
    }

    .project-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 1.8rem;
    }

    @media (max-width: 680px) {
      .project-grid {
        grid-template-columns: 1fr;
      }
      .header-intro {
        flex-direction: column;
        align-items: flex-start;
        gap: 0.6rem;
      }
      .header-right {
        text-align: left;
        width: 100%;
      }
      .portfolio-page {
        padding: 1.2rem;
      }
      .hero-digital-content {
        flex-direction: column;
        text-align: center;
      }
      .hero-digital-content .left .hero-sub {
        text-align: center;
      }
    }

    .project-card {
      background: #faf9f7;
      border-radius: 20px;
      padding: 1.4rem 1.4rem 1.2rem;
      border: 1px solid #e5e0d8;
      transition: 0.15s ease;
      box-shadow: 0 2px 6px rgba(0,0,0,0.02);
      display: flex;
      flex-direction: column;
    }

    .project-card:hover {
      border-color: #c9bfb0;
      box-shadow: 0 8px 16px -8px rgba(0,0,0,0.06);
    }

    .project-card .card-icon {
      font-size: 2rem;
      margin-bottom: 0.2rem;
    }

    .project-card h4 {
      font-family: 'Playfair Display', serif;
      font-weight: 600;
      font-size: 1.2rem;
      color: #0b2b3b;
      margin-bottom: 0.2rem;
    }

    .project-card .card-tag {
      font-size: 0.6rem;
      font-weight: 600;
      text-transform: uppercase;
      letter-spacing: 0.6px;
      color: #4f6d7a;
      background: #eef0ed;
      padding: 0.1rem 0.8rem;
      border-radius: 40px;
      display: inline-block;
      margin-bottom: 0.5rem;
      align-self: flex-start;
    }

    .project-card p {
      color: #2f4a58;
      font-size: 0.9rem;
      line-height: 1.6;
      flex: 1;
    }

    .project-card .preview-badge {
      margin-top: 0.6rem;
      font-size: 0.7rem;
      background: #eae5dc;
      padding: 0.1rem 1rem;
      border-radius: 40px;
      align-self: flex-start;
      color: #2f4a58;
    }

    .project-card .color-swatches {
      display: flex;
      gap: 0.4rem;
      flex-wrap: wrap;
      margin: 0.3rem 0;
    }

    .swatch {
      display: inline-block;
      width: 18px;
      height: 18px;
      border-radius: 4px;
      border: 1px solid rgba(0,0,0,0.08);
    }

    /* ===== CONTACT ===== */
    .contact-section {
      margin-top: 2.4rem;
      padding-top: 2rem;
      border-top: 3px solid #f0ebe3;
      background: #fcfaf7;
      border-radius: 32px;
      padding: 2rem 2rem 1.6rem;
    }

    .contact-headline {
      font-family: 'Playfair Display', serif;
      font-weight: 600;
      font-size: 2rem;
      color: #0b2b3b;
      margin-bottom: 0.2rem;
    }

    .contact-sub {
      font-size: 1rem;
      color: #2f4a58;
      margin-bottom: 1.6rem;
      border-left: 4px solid #f5b042;
      padding-left: 1rem;
    }

    .contact-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(190px, 1fr));
      gap: 1rem;
      margin: 1rem 0 0.8rem;
    }

    .contact-item {
      background: white;
      border-radius: 16px;
      padding: 0.8rem 1.2rem;
      border: 1px solid #e5dfd6;
      box-shadow: 0 1px 4px rgba(0,0,0,0.02);
      display: flex;
      flex-direction: column;
      gap: 0.2rem;
    }

    .contact-item .label {
      font-size: 0.6rem;
      font-weight: 600;
      text-transform: uppercase;
      letter-spacing: 0.8px;
      color: #5a7a8a;
    }

    .contact-item .value {
      font-size: 0.95rem;
      font-weight: 500;
      color: #0b2b3b;
      word-break: break-word;
    }

    .contact-item .value a {
      color: #1d4b5e;
      text-decoration: none;
      border-bottom: 1px dotted #b5aa99;
    }

    .contact-item .value a:hover {
      border-bottom: 2px solid #f5b042;
    }

    .contact-item .telegram-handle {
      background: #eef3f0;
      padding: 0.1rem 0.8rem;
      border-radius: 40px;
      font-weight: 500;
    }

    .footer-divider {
      margin-top: 1.2rem;
      border-top: 1px solid #e3dcd2;
      padding-top: 0.8rem;
      display: flex;
      flex-wrap: wrap;
      justify-content: flex-end;
      align-items: center;
      font-size: 0.7rem;
      color: #4f6d7a;
    }

    .footer-badge {
      background: #eae5dc;
      padding: 0.1rem 1rem;
      border-radius: 40px;
    }

    @media (max-width: 480px) {
      .contact-grid {
        grid-template-columns: 1fr;
      }
      .name-title {
        font-size: 1.8rem;
      }
    }
  </style>
</head>
<body>
  <div class="portfolio-page">

    <!-- ===== HEADER ===== -->
    <header class="header-intro">
      <div>
        <div class="name-title">
          Andualem Guchi <small>Design · Translation</small>
        </div>
        <div class="tagline">
          📍 Addis Ababa · Available for freelance projects
        </div>
      </div>
      <div class="header-right">
        <span class="availability">✦ open for work</span>
        <div style="margin-top:0.3rem; font-size:0.75rem; color:#3f5d6b;">Ethiopia · Global</div>
      </div>
    </header>

    <!-- ===== ATTRACTIVE DIGITALIZED HERO IMAGE ===== -->
    <div class="hero-digital">
      <div class="shape-float s1"></div>
      <div class="shape-float s2"></div>

      <div class="hero-digital-content">
        <div class="left">
          <div class="hero-tagline">
            Crafting <span class="gold">visual stories</span><br>
            &amp; bridging <span class="gold">languages</span>
          </div>
          <div class="hero-sub">
            From coffee branding to solar energy localization
          </div>
        </div>
        <div class="right">
          <div class="glass-card gold">
            <span class="icon">☕</span>
            Brand Design
            <span class="badge-dot"></span>
          </div>
          <div class="glass-card">
            <span class="icon">✍️</span>
            Copywriting
          </div>
          <div class="glass-card gold">
            <span class="icon">🌍</span>
            Localization
          </div>
          <div class="glass-card">
            <span class="icon">📱</span>
            Social Media
          </div>
          <div class="glass-card gold">
            <span class="icon">⚡</span>
            Solar Energy
          </div>
          <div class="glass-card">
            <span class="icon">📝</span>
            Translation
          </div>
        </div>
      </div>
    </div>

    <!-- ===== PROJECTS ===== -->
    <section class="project-section">
      <div class="project-headline">
        📌 Featured Work
        <span class="badge">Portfolio</span>
      </div>
      <div class="project-grid">
        <!-- Project 1: Coffee -->
        <div class="project-card">
          <div class="card-icon">☕</div>
          <h4>Bunna Bites &amp; Brew</h4>
          <span class="card-tag">Design · Copywriting</span>
          <p>
            Social media brand content: Canva design with deep coffee brown, 
            ochre, and off-white palette. Persuasive copy for Ethiopian coffee lovers.
          </p>
          <div class="color-swatches">
            <span class="swatch" style="background:#4A2E1B;"></span>
            <span class="swatch" style="background:#D4AF37;"></span>
            <span class="swatch" style="background:#FDFBF7; border:1px solid #ccc;"></span>
            <span style="font-size:0.65rem; color:#4f6d7a; margin-left:0.2rem;">Tradition Meets Tomorrow</span>
          </div>
          <span class="preview-badge">📸 PNG · caption ready</span>
        </div>

        <!-- Project 2: SolarFlow -->
        <div class="project-card">
          <div class="card-icon">🌍</div>
          <h4>SolarFlow Energy</h4>
          <span class="card-tag">Translation · Localization</span>
          <p>
            E‑Commerce website localization (English → Amharic). Hero, features, 
            and CTA adapted for East African market with technical precision.
          </p>
          <div style="display:flex; gap:0.4rem; flex-wrap:wrap; margin:0.3rem 0;">
            <span style="background:#0b2b3b; color:white; padding:0.05rem 0.6rem; border-radius:40px; font-size:0.6rem;">EN</span>
            <span style="background:#f5b042; color:#0b2b3b; padding:0.05rem 0.6rem; border-radius:40px; font-size:0.6rem;">AM</span>
            <span style="font-size:0.65rem; color:#4f6d7a;">bilingual · technical</span>
          </div>
          <span class="preview-badge">📄 side‑by‑side comparison</span>
        </div>
      </div>
    </section>

    <!-- ===== CONTACT ===== -->
    <section class="contact-section" id="contact">
      <div class="contact-headline">
        📬 Let’s Work Together
      </div>
      <div class="contact-sub">
        Have a project or need a dedicated freelancer? Reach out directly.
      </div>

      <div class="contact-grid">
        <div class="contact-item">
          <span class="label">✉️ Email</span>
          <div class="value">
            <a href="mailto:andualemguchi0@gmail.com">andualemguchi0@gmail.com</a>
          </div>
        </div>
        <div class="contact-item">
          <span class="label">📱 Telegram</span>
          <div class="value">
            <a href="https://t.me/Andualem_digital" target="_blank" class="telegram-handle" style="text-decoration:none; border-bottom:none;">
              @Andualem_digital
            </a>
          </div>
        </div>
        <div class="contact-item">
          <span class="label">💼 Upwork</span>
          <div class="value">
            <a href="https://www.upwork.com/freelancers/~01andualemguchi" target="_blank">Andualem Guchi</a>
          </div>
        </div>
        <div class="contact-item">
          <span class="label">📍 Location</span>
          <div class="value">
            Addis Ababa, Ethiopia <span style="font-size:0.7rem; color:#3f5d6b;">(available)</span>
          </div>
        </div>
      </div>

      <div class="footer-divider">
        <span class="footer-badge">Portfolio</span>
      </div>
    </section>
  </div>
</body>
</html>
