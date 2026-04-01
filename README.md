<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Lenna Conley Jasuja — Brand Marketing & Creative Leader</title>
  <meta name="description" content="Lenna Conley Jasuja is a brand marketing and creative leader with Fortune 100 experience spanning healthcare, CPG, and durable goods.">
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,400;0,500;0,600;1,400;1,500&family=Outfit:wght@300;400;500;600&display=swap" rel="stylesheet">
  <style>
    *, *::before, *::after { margin: 0; padding: 0; box-sizing: border-box; }

    :root {
      --ivory: #FAF6F1;
      --cream: #F3EDE4;
      --warm-white: #FFFDFB;
      --charcoal: #2C2824;
      --charcoal-light: #4A4440;
      --terracotta: #B8734A;
      --terracotta-light: #D4956A;
      --terracotta-pale: #F0DFD0;
      --sage: #8B9A7E;
      --sage-light: #C5CEBF;
      --warm-gray: #9E9590;
      --warm-gray-light: #D1CBC5;
    }

    html { scroll-behavior: smooth; }

    body {
      font-family: 'Outfit', sans-serif;
      background: var(--ivory);
      color: var(--charcoal);
      line-height: 1.7;
      font-weight: 300;
      -webkit-font-smoothing: antialiased;
    }

    /* NAV */
    nav {
      position: fixed;
      top: 0;
      left: 0;
      right: 0;
      z-index: 100;
      padding: 1.2rem 2.5rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
      transition: background 0.4s, box-shadow 0.4s;
    }

    nav.scrolled {
      background: rgba(250, 246, 241, 0.92);
      backdrop-filter: blur(12px);
      box-shadow: 0 1px 20px rgba(44, 40, 36, 0.06);
    }

    nav .logo {
      font-family: 'Cormorant Garamond', serif;
      font-size: 1.3rem;
      font-weight: 500;
      letter-spacing: 0.03em;
      color: var(--charcoal);
      text-decoration: none;
    }

    nav ul {
      list-style: none;
      display: flex;
      gap: 2rem;
    }

    nav ul li a {
      font-size: 0.85rem;
      font-weight: 400;
      letter-spacing: 0.06em;
      text-transform: uppercase;
      color: var(--charcoal-light);
      text-decoration: none;
      position: relative;
      transition: color 0.3s;
    }

    nav ul li a::after {
      content: '';
      position: absolute;
      bottom: -4px;
      left: 0;
      width: 0;
      height: 1.5px;
      background: var(--terracotta);
      transition: width 0.3s;
    }

    nav ul li a:hover { color: var(--terracotta); }
    nav ul li a:hover::after { width: 100%; }

    .hamburger {
      display: none;
      flex-direction: column;
      gap: 5px;
      cursor: pointer;
      background: none;
      border: none;
      padding: 4px;
    }

    .hamburger span {
      display: block;
      width: 24px;
      height: 2px;
      background: var(--charcoal);
      transition: transform 0.3s, opacity 0.3s;
    }

    /* HERO */
    .hero {
      min-height: 100vh;
      display: flex;
      align-items: center;
      padding: 8rem 2.5rem 4rem;
      max-width: 1200px;
      margin: 0 auto;
      gap: 4rem;
    }

    .hero-text { flex: 1.2; }

    .hero-text h1 {
      font-family: 'Cormorant Garamond', serif;
      font-size: clamp(2.8rem, 5vw, 4.2rem);
      font-weight: 400;
      line-height: 1.15;
      margin-bottom: 1.5rem;
      color: var(--charcoal);
    }

    .hero-text h1 em {
      font-style: italic;
      color: var(--terracotta);
    }

    .hero-text .tagline {
      font-size: 1.15rem;
      color: var(--charcoal-light);
      margin-bottom: 2rem;
      max-width: 540px;
      font-weight: 300;
      line-height: 1.8;
    }

    .hero-brands {
      display: flex;
      flex-wrap: wrap;
      gap: 0.5rem 1.2rem;
      margin-top: 2rem;
    }

    .hero-brands span {
      font-size: 0.78rem;
      font-weight: 400;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      color: var(--warm-gray);
      padding: 0.35rem 0;
      border-bottom: 1px solid var(--warm-gray-light);
    }

    .hero-photo {
      flex: 0.8;
      display: flex;
      justify-content: center;
    }

    .hero-photo .photo-frame {
      position: relative;
      width: 320px;
      height: 400px;
    }

    .hero-photo .photo-frame::before {
      content: '';
      position: absolute;
      top: 12px;
      left: 12px;
      right: -12px;
      bottom: -12px;
      border: 2px solid var(--terracotta-pale);
      border-radius: 8px;
    }

    .hero-photo img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      object-position: center top;
      border-radius: 8px;
      position: relative;
      z-index: 1;
      filter: saturate(0.9);
    }

    /* SECTION FOUNDATIONS */
    section { padding: 6rem 2.5rem; }

    .section-inner {
      max-width: 1000px;
      margin: 0 auto;
    }

    .section-label {
      font-size: 0.75rem;
      font-weight: 500;
      letter-spacing: 0.15em;
      text-transform: uppercase;
      color: var(--terracotta);
      margin-bottom: 1rem;
    }

    .section-heading {
      font-family: 'Cormorant Garamond', serif;
      font-size: clamp(2rem, 3.5vw, 2.8rem);
      font-weight: 400;
      line-height: 1.25;
      margin-bottom: 2rem;
      color: var(--charcoal);
    }

    /* ABOUT */
    .about { background: var(--warm-white); }

    .about-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 3rem;
      margin-top: 2rem;
    }

    .about-grid p {
      font-size: 1rem;
      color: var(--charcoal-light);
      line-height: 1.85;
    }

    .about-grid p + p { margin-top: 1rem; }

    .about-cta {
      margin-top: 2.5rem;
      display: flex;
      gap: 1.2rem;
      flex-wrap: wrap;
    }

    .about-cta a {
      display: inline-flex;
      align-items: center;
      gap: 0.5rem;
      font-size: 0.85rem;
      font-weight: 500;
      letter-spacing: 0.04em;
      text-decoration: none;
      color: var(--terracotta);
      border-bottom: 1.5px solid var(--terracotta-pale);
      padding-bottom: 2px;
      transition: border-color 0.3s, color 0.3s;
    }

    .about-cta a:hover { border-color: var(--terracotta); }
    .about-cta a svg { width: 14px; height: 14px; }

    /* WORK / SHOWREELS */
    .work { background: var(--ivory); }

    .work-grid {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 2.5rem;
      margin-top: 2.5rem;
    }

    .work-card {
      background: var(--warm-white);
      border-radius: 10px;
      overflow: hidden;
      transition: transform 0.3s, box-shadow 0.3s;
    }

    .work-card:hover {
      transform: translateY(-4px);
      box-shadow: 0 12px 40px rgba(44, 40, 36, 0.08);
    }

    .work-card-visual {
      height: 200px;
      position: relative;
      overflow: hidden;
    }

    .work-card-visual .overlay {
      position: absolute;
      inset: 0;
      display: flex;
      align-items: center;
      justify-content: center;
      z-index: 2;
    }

    .work-card-visual .play-btn {
      width: 56px;
      height: 56px;
      border-radius: 50%;
      background: rgba(255, 255, 255, 0.92);
      display: flex;
      align-items: center;
      justify-content: center;
      transition: transform 0.3s;
    }

    .work-card:hover .play-btn { transform: scale(1.1); }

    .work-card-visual .play-btn svg {
      width: 20px;
      height: 20px;
      fill: var(--terracotta);
      margin-left: 3px;
    }

    .work-card-body { padding: 1.5rem; }

    .work-card-body h3 {
      font-family: 'Cormorant Garamond', serif;
      font-size: 1.3rem;
      font-weight: 500;
      margin-bottom: 0.4rem;
      color: var(--charcoal);
    }

    .work-card-body .card-role {
      font-size: 0.78rem;
      letter-spacing: 0.08em;
      text-transform: uppercase;
      color: var(--terracotta);
      font-weight: 500;
      margin-bottom: 0.6rem;
    }

    .work-card-body p {
      font-size: 0.88rem;
      color: var(--charcoal-light);
      line-height: 1.7;
    }

    .work-card-link {
      display: inline-flex;
      align-items: center;
      gap: 0.4rem;
      font-size: 0.82rem;
      font-weight: 500;
      color: var(--terracotta);
      text-decoration: none;
      margin-top: 0.8rem;
      transition: gap 0.3s;
    }

    .work-card-link:hover { gap: 0.7rem; }
    .work-card-link svg { width: 14px; height: 14px; }

    /* IMPACT NUMBERS */
    .impact {
      background: var(--charcoal);
      color: var(--cream);
      padding: 5rem 2.5rem;
    }

    .impact .section-label { color: var(--terracotta-light); }
    .impact .section-heading { color: var(--cream); }

    .impact-grid {
      display: grid;
      grid-template-columns: repeat(4, 1fr);
      gap: 2rem;
      margin-top: 2.5rem;
    }

    .impact-stat {
      text-align: center;
      padding: 1.5rem;
    }

    .impact-stat .number {
      font-family: 'Cormorant Garamond', serif;
      font-size: 2.8rem;
      font-weight: 400;
      color: var(--terracotta-light);
      line-height: 1;
      margin-bottom: 0.6rem;
    }

    .impact-stat .label {
      font-size: 0.82rem;
      font-weight: 300;
      color: var(--warm-gray-light);
      line-height: 1.5;
    }

    /* CAREER LOGOS */
    .career {
      background: var(--warm-white);
      padding: 5rem 2.5rem;
    }

    .career .section-inner { text-align: center; }

    .logo-bar {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      align-items: center;
      gap: 2.5rem 3.5rem;
      margin-top: 2.5rem;
    }

    .logo-bar img {
      height: 50px;
      width: auto;
      object-fit: contain;
      opacity: 0.6;
      transition: opacity 0.3s;
      filter: grayscale(100%);
    }

    .logo-bar img:hover {
      opacity: 1;
      filter: grayscale(0%);
    }

    /* CONTACT / FOOTER */
    footer {
      background: var(--ivory);
      padding: 5rem 2.5rem 3rem;
    }

    .footer-inner {
      max-width: 1000px;
      margin: 0 auto;
      text-align: center;
    }

    .footer-inner .section-heading { margin-bottom: 1rem; }

    .footer-inner .footer-note {
      font-size: 1rem;
      color: var(--charcoal-light);
      margin-bottom: 2.5rem;
      max-width: 500px;
      margin-left: auto;
      margin-right: auto;
    }

    .footer-links {
      display: flex;
      justify-content: center;
      gap: 2rem;
      flex-wrap: wrap;
      margin-bottom: 3rem;
    }

    .footer-links a {
      display: inline-flex;
      align-items: center;
      gap: 0.5rem;
      font-size: 0.92rem;
      font-weight: 400;
      color: var(--charcoal);
      text-decoration: none;
      padding: 0.8rem 1.6rem;
      border: 1.5px solid var(--warm-gray-light);
      border-radius: 40px;
      transition: border-color 0.3s, background 0.3s, color 0.3s;
    }

    .footer-links a:hover {
      border-color: var(--terracotta);
      background: var(--terracotta);
      color: white;
    }

    .footer-links a svg { width: 16px; height: 16px; }

    .copyright {
      font-size: 0.78rem;
      color: var(--warm-gray);
      margin-top: 3rem;
      padding-top: 2rem;
      border-top: 1px solid var(--warm-gray-light);
    }

    /* ANIMATIONS */
    .fade-in {
      opacity: 0;
      transform: translateY(24px);
      transition: opacity 0.7s ease, transform 0.7s ease;
    }

    .fade-in.visible {
      opacity: 1;
      transform: translateY(0);
    }

    /* RESPONSIVE */
    @media (max-width: 900px) {
      .hero {
        flex-direction: column-reverse;
        padding-top: 7rem;
        gap: 2.5rem;
        min-height: auto;
      }
      .hero-photo .photo-frame { width: 240px; height: 300px; }
      .about-grid { grid-template-columns: 1fr; }
      .work-grid { grid-template-columns: 1fr; }
      .impact-grid { grid-template-columns: 1fr 1fr; }
      .logo-bar { gap: 2rem 2.5rem; }
      .logo-bar img { height: 40px; }
    }

    @media (max-width: 600px) {
      nav ul { display: none; }
      nav ul.open {
        display: flex;
        flex-direction: column;
        position: absolute;
        top: 100%;
        left: 0;
        right: 0;
        background: rgba(250, 246, 241, 0.97);
        backdrop-filter: blur(12px);
        padding: 1.5rem 2.5rem;
        gap: 1.2rem;
        box-shadow: 0 8px 30px rgba(44, 40, 36, 0.08);
      }
      .hamburger { display: flex; }
      section { padding: 4rem 1.5rem; }
      .hero { padding: 6rem 1.5rem 3rem; }
      .impact-grid { grid-template-columns: 1fr 1fr; gap: 1rem; }
      .impact-stat .number { font-size: 2.2rem; }
      .footer-links { flex-direction: column; align-items: center; }
      .logo-bar { gap: 1.5rem 2rem; }
      .logo-bar img { height: 35px; }
    }
  </style>
</head>
<body>

  <!-- NAV -->
  <nav id="nav">
    <a href="#" class="logo">Lenna Conley Jasuja</a>
    <button class="hamburger" onclick="document.querySelector('nav ul').classList.toggle('open')" aria-label="Menu">
      <span></span><span></span><span></span>
    </button>
    <ul>
      <li><a href="#about">About</a></li>
      <li><a href="#work">Work</a></li>
      <li><a href="#career">Career</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>

  <!-- HERO -->
  <section class="hero">
    <div class="hero-text fade-in">
      <h1>Building brands<br>that <em>move</em> people</h1>
      <p class="tagline">I'm Lenna Conley Jasuja — a brand marketing and creative leader who combines Fortune 100 discipline with purpose-driven storytelling. I build teams that turn complex value into campaigns people actually feel while delivering measurable growth.</p>
      <div class="hero-brands">
        <span>City of Hope</span>
        <span>CTCA</span>
        <span>Newell Brands</span>
        <span>Unilever</span>
        <span>Procter &amp; Gamble</span>
        <span>Kraft General Foods</span>
      </div>
    </div>
    <div class="hero-photo fade-in">
      <div class="photo-frame">
        <img src="images/headshot.jpg" alt="Lenna Conley Jasuja" loading="eager">
      </div>
    </div>
  </section>

  <!-- ABOUT -->
  <section class="about" id="about">
    <div class="section-inner fade-in">
      <span class="section-label">About</span>
      <h2 class="section-heading">Strategy meets storytelling</h2>
      <div class="about-grid">
        <div>
          <p>I'm a cross-disciplined marketer with a track record of building and elevating brands at the intersection of strategy, creativity, and purpose. Leading brand strategy in oncology sharpened my ability to market with both rigor and empathy — translating complex clinical value into narratives that move patients to act.</p>
          <p>At City of Hope, a top-10 NCI-designated cancer system, I led enterprise brand marketing and creative across 40+ locations, unifying City of Hope and Cancer Treatment Centers of America into a national brand post-acquisition.</p>
        </div>
        <div>
          <p>Before healthcare, I spent nearly two decades in CPG at Newell Brands, leading marketing for Crock-Pot, Mr. Coffee, Calphalon, and Oster — launching over 100 products and driving both retail and DTC growth. My career began in brand activation at Procter &amp; Gamble and Unilever, where I built the discipline of consumer-led, data-driven marketing.</p>
          <div class="about-cta">
            <a href="https://www.linkedin.com/in/lennaconley/" target="_blank" rel="noopener">
              LinkedIn
              <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><line x1="7" y1="17" x2="17" y2="7"></line><polyline points="7 7 17 7 17 17"></polyline></svg>
            </a>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- WORK -->
  <section class="work" id="work">
    <div class="section-inner fade-in">
      <span class="section-label">Campaign Work</span>
      <h2 class="section-heading">Selected creative</h2>
      <div class="work-grid">

        <a href="https://michaelharkins.slateapp.com/showreel/view/5ec831bbeb48d" target="_blank" rel="noopener" class="work-card" style="text-decoration:none; color:inherit;">
          <div class="work-card-visual">
            <img src="images/showreel-harkins.png" alt="City of Hope campaign still" style="position:absolute;inset:0;width:100%;height:100%;object-fit:cover;z-index:1;">
            <div class="overlay">
              <div class="play-btn">
                <svg viewBox="0 0 24 24"><polygon points="5,3 19,12 5,21"></polygon></svg>
              </div>
            </div>
          </div>
          <div class="work-card-body">
            <div class="card-role">Director's Reel — Michael Harkins</div>
            <h3>City of Hope &amp; CTCA Campaigns</h3>
            <p>National TV spots including "Hope Is Here," "One Call," and "Driven" — produced through the in-house Health Studios team.</p>
            <span class="work-card-link">Watch reel <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><line x1="5" y1="12" x2="19" y2="12"></line><polyline points="12 5 19 12 12 19"></polyline></svg></span>
          </div>
        </a>

        <a href="https://www.matthamill.com/" target="_blank" rel="noopener" class="work-card" style="text-decoration:none; color:inherit;">
          <div class="work-card-visual">
            <img src="images/showreel-hamill.png" alt="Walk for Hope 2025" style="position:absolute;inset:0;width:100%;height:100%;object-fit:cover;z-index:1;">
            <div class="overlay">
              <div class="play-btn">
                <svg viewBox="0 0 24 24"><polygon points="5,3 19,12 5,21"></polygon></svg>
              </div>
            </div>
          </div>
          <div class="work-card-body">
            <div class="card-role">Producer/Editor — Matt Hamill</div>
            <h3>City of Hope Brand Films</h3>
            <p>"Driven," "This is City of Hope," patient stories, and Walk for Hope — editorial and documentary content produced in-house.</p>
            <span class="work-card-link">View work <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><line x1="5" y1="12" x2="19" y2="12"></line><polyline points="12 5 19 12 12 19"></polyline></svg></span>
          </div>
        </a>

      </div>
    </div>
  </section>

  <!-- IMPACT -->
  <section class="impact">
    <div class="section-inner fade-in">
      <span class="section-label">Impact</span>
      <h2 class="section-heading">Numbers that matter</h2>
      <div class="impact-grid">
        <div class="impact-stat">
          <div class="number">6,000+</div>
          <div class="label">Projects delivered annually at City of Hope</div>
        </div>
        <div class="impact-stat">
          <div class="number">26%</div>
          <div class="label">Increase in qualified funnel leads via SEO/content</div>
        </div>
        <div class="impact-stat">
          <div class="number">$550K</div>
          <div class="label">Annual vendor savings through in-house production</div>
        </div>
        <div class="impact-stat">
          <div class="number">40+</div>
          <div class="label">Locations unified under one brand system</div>
        </div>
      </div>
    </div>
  </section>

  <!-- CAREER -->
  <section class="career" id="career">
    <div class="section-inner fade-in">
      <span class="section-label">Career</span>
      <h2 class="section-heading">Where I've built</h2>
      <div class="logo-bar">
        <img src="images/logo-coh.png" alt="City of Hope">
        <img src="images/logo-ctca.png" alt="Cancer Treatment Centers of America">
        <img src="images/logo-newell.png" alt="Newell Brands">
        <img src="images/logo-unilever.png" alt="Unilever">
        <img src="images/logo-pg.png" alt="Procter & Gamble">
        <img src="images/logo-kraft.png" alt="Kraft">
      </div>
    </div>
  </section>

  <!-- CONTACT -->
  <footer id="contact">
    <div class="footer-inner fade-in">
      <span class="section-label">Get in Touch</span>
      <h2 class="section-heading">Let's talk</h2>
      <p class="footer-note">Open to conversations about brand leadership, creative strategy, and the next thing worth building.</p>
      <div class="footer-links">
        <a href="mailto:lennaconley@gmail.com">
          <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"></path><polyline points="22,6 12,13 2,6"></polyline></svg>
          Email
        </a>
        <a href="https://www.linkedin.com/in/lennaconley/" target="_blank" rel="noopener">
          <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"></path><rect x="2" y="9" width="4" height="12"></rect><circle cx="4" cy="4" r="2"></circle></svg>
          LinkedIn
        </a>
        <a href="tel:5613069699">
          <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07 19.5 19.5 0 0 1-6-6 19.79 19.79 0 0 1-3.07-8.67A2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72 12.84 12.84 0 0 0 .7 2.81 2 2 0 0 1-.45 2.11L8.09 9.91a16 16 0 0 0 6 6l1.27-1.27a2 2 0 0 1 2.11-.45 12.84 12.84 0 0 0 2.81.7A2 2 0 0 1 22 16.92z"></path></svg>
          561.306.9699
        </a>
      </div>
      <div class="copyright">
        &copy; 2026 Lenna Conley Jasuja. All rights reserved.
      </div>
    </div>
  </footer>

  <script>
    const nav = document.getElementById('nav');
    window.addEventListener('scroll', () => {
      nav.classList.toggle('scrolled', window.scrollY > 40);
    });

    document.querySelectorAll('nav ul li a').forEach(link => {
      link.addEventListener('click', () => {
        document.querySelector('nav ul').classList.remove('open');
      });
    });

    const observer = new IntersectionObserver((entries) => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          entry.target.classList.add('visible');
        }
      });
    }, { threshold: 0.12 });

    document.querySelectorAll('.fade-in').forEach(el => observer.observe(el));
  </script>

</body>
</html>
