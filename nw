<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Bene'nw — Ethiopian Gift Registry & Contribution Platform</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=DM+Sans:ital,opsz,wght@0,9..40,300;0,9..40,400;0,9..40,500;0,9..40,600;0,9..40,700;1,9..40,400&family=Fraunces:ital,opsz,wght@0,9..144,300;0,9..144,400;0,9..144,500;0,9..144,600;0,9..144,700;1,9..144,400&display=swap" rel="stylesheet">
  <script>
    tailwind.config = {
      theme: {
        extend: {
          colors: {
            espresso: '#2C1810',
            'espresso-light': '#4A3228',
            ivory: '#FAF6F1',
            'ivory-dark': '#F0E9E0',
            terracotta: '#C45D3E',
            'terracotta-dark': '#A84832',
            gold: '#D4A574',
            'gold-dark': '#B8895A',
            cream: '#FFF8F0',
            sage: '#8B9A7D',
            border: '#E8DFD5',
            muted: '#6B5A4E',
          },
          fontFamily: {
            display: ['Fraunces', 'serif'],
            sans: ['DM Sans', 'sans-serif'],
          }
        }
      }
    }
  </script>
  <style>
    /* ========== BASE STYLES ========== */
    :root {
      --bg: #FAF6F1;
      --fg: #e9e9e96f;
      --muted: #6B5A4E;
      --accent: #C45D3E;
      --accent-hover: #A84832;
      --card: #FFFFFF;
      --border: #E8DFD5;
      --gold: #D4A574;
    }

    * { box-sizing: border-box; margin: 0; padding: 0; }
    html { scroll-behavior: smooth; }
    html[lang="en"] .text-am { display: none; }
    html[lang="am"] .text-en { display: none; }
    
    .text-en, .text-am { transition: opacity 0.3s ease; }

    body {
      font-family: 'DM Sans', sans-serif;
      background-color: var(--bg);
      color: var(--fg);
      overflow-x: hidden;
      line-height: 1.6;
    }

    ::-webkit-scrollbar { width: 10px; }
    ::-webkit-scrollbar-track { background: var(--bg); }
    ::-webkit-scrollbar-thumb { background: var(--border); border-radius: 5px; }
    ::-webkit-scrollbar-thumb:hover { background: var(--muted); }

    /* ========== BACKGROUND PATTERNS ========== */
    .ethiopian-pattern {
      background-image: url("image/svg+xml,%3Csvg width='60' height='60' viewBox='0 0 60 60' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M30 0L60 30L30 60L0 30z' fill='none' stroke='%23D4A574' stroke-width='0.5' opacity='0.15'/%3E%3C/svg%3E");
      background-size: 30px 30px;
    }

    /* ========== ANIMATED ORBS ========== */
    .orb {
      position: absolute;
      border-radius: 50%;
      filter: blur(80px);
      opacity: 0.35;
      pointer-events: none;
    }
    .orb-1 {
      width: 500px; height: 500px;
      background: linear-gradient(135deg, #C45D3E 0%, #D4A574 100%);
      animation: float-1 20s ease-in-out infinite;
    }
    .orb-2 {
      width: 400px; height: 400px;
      background: linear-gradient(135deg, #D4A574 0%, #8B9A7D 100%);
      animation: float-2 25s ease-in-out infinite;
    }
    @keyframes float-1 {
      0%, 100% { transform: translate(0, 0) scale(1); }
      33% { transform: translate(50px, -30px) scale(1.1); }
      66% { transform: translate(-30px, 50px) scale(0.95); }
    }
    @keyframes float-2 {
      0%, 100% { transform: translate(0, 0) scale(1); }
      33% { transform: translate(-40px, 40px) scale(1.05); }
      66% { transform: translate(30px, -20px) scale(0.9); }
    }

    /* ========== SCROLL REVEAL ANIMATIONS ========== */
    .reveal {
      opacity: 0;
      transform: translateY(40px);
      transition: opacity 0.8s cubic-bezier(0.16, 1, 0.3, 1), transform 0.8s cubic-bezier(0.16, 1, 0.3, 1);
    }
    .reveal.visible { opacity: 1; transform: translateY(0); }
    .reveal-delay-1 { transition-delay: 0.1s; }
    .reveal-delay-2 { transition-delay: 0.2s; }
    .reveal-delay-3 { transition-delay: 0.3s; }
    .reveal-delay-4 { transition-delay: 0.4s; }

    @keyframes slide-up {
      from { opacity: 0; transform: translateY(60px); }
      to { opacity: 1; transform: translateY(0); }
    }
    .hero-animate {
      animation: slide-up 1s cubic-bezier(0.16, 1, 0.3, 1) forwards;
      opacity: 0;
    }
    .hero-delay-1 { animation-delay: 0.2s; }
    .hero-delay-2 { animation-delay: 0.4s; }
    .hero-delay-3 { animation-delay: 0.6s; }
    .hero-delay-4 { animation-delay: 0.8s; }

    /* ========== BUTTONS ========== */
    .btn-primary {
      background: linear-gradient(135deg, #C45D3E 0%, #A84832 100%);
      color: rgb(255, 255, 255);
      padding: 1rem 2rem;
      border-radius: 100px;
      font-weight: 600;
      transition: all 0.3s cubic-bezier(0.16, 1, 0.3, 1);
      box-shadow: 0 4px 20px rgba(196, 93, 62, 0.3);
      position: relative;
      overflow: hidden;
      display: inline-flex;
      align-items: center;
      justify-content: center;
      gap: 0.5rem;
      text-align: center;
      text-decoration: none;
      border: none;
      cursor: pointer;
      font-family: inherit;
    }
    .btn-primary:hover {
      transform: translateY(-2px);
      box-shadow: 0 8px 30px rgba(196, 93, 62, 0.4);
    }

    .btn-secondary {
      background: transparent;
      color: var(--fg);
      padding: 1rem 2rem;
      border-radius: 100px;
      font-weight: 600;
      transition: all 0.3s cubic-bezier(0.16, 1, 0.3, 1);
      border: 2px solid var(--border);
      display: inline-flex;
      align-items: center;
      justify-content: center;
      gap: 0.5rem;
      text-align: center;
      text-decoration: none;
      cursor: pointer;
      font-family: inherit;
    }
    .btn-secondary:hover {
      background: var(--fg);
      color: var(--bg);
      border-color: var(--fg);
    }

    .btn-sm {
      padding: 0.5rem 1.25rem;
      font-size: 0.875rem;
    }

    /* ========== NAVIGATION ========== */
    .nav-link {
      position: relative;
      color: rgba(199, 115, 20, 0.7);
      font-weight: 500;
      transition: color 0.3s;
      text-decoration: none;
      cursor: pointer;
      font-size: 0.95rem;
    }
    .nav-link:hover { color: #FAF6F1; }

    .lang-toggle {
      display: flex;
      background: rgba(255, 255, 255, 0.214);
      border-radius: 100px;
      padding: 3px;
      position: relative;
      border: 1px solid rgba(255,255,255,0.1);
    }
    .lang-toggle button {
      padding: 0.4rem 0.85rem;
      border-radius: 100px;
      font-weight: 500;
      font-size: 0.8rem;
      transition: all 0.3s;
      position: relative;
      z-index: 1;
      background: transparent;
      border: none;
      cursor: pointer;
      color: rgba(250, 246, 241, 0.6);
    }
    .lang-toggle button.active { color: #2C1810; background: #C45D3E; }

    /* ========== MOBILE MENU ========== */
    .mobile-menu {
      position: fixed;
      top: 0; right: 0;
      width: 100%;
      height: 100vh;
      background: var(--bg);
      z-index: 100;
      transform: translateX(100%);
      transition: transform 0.4s cubic-bezier(0.16, 1, 0.3, 1);
      overflow-y: auto;
    }
    .mobile-menu.open { transform: translateX(0); }

    /* ========== OCCASION CARDS ========== */
    .occasion-card {
      background: white;
      border-radius: 24px;
      padding: 2rem;
      transition: all 0.4s cubic-bezier(0.16, 1, 0.3, 1);
      border: 1px solid var(--border);
      position: relative;
      overflow: hidden;
      text-decoration: none;
      display: block;
      color: inherit;
    }
    .occasion-card::before {
      content: '';
      position: absolute;
      top: 0; left: 0; right: 0;
      height: 4px;
      background: linear-gradient(90deg, #C45D3E 0%, #D4A574 100%);
      transform: scaleX(0);
      transform-origin: left;
      transition: transform 0.4s cubic-bezier(0.16, 1, 0.3, 1);
    }
    .occasion-card:hover {
      transform: translateY(-8px);
      box-shadow: 0 20px 40px rgba(44, 24, 16, 0.1);
      border-color: transparent;
    }
    .occasion-card:hover::before { transform: scaleX(1); }

    /* ========== MODALS ========== */
    .modal-overlay {
      position: fixed; inset: 0;
      background: rgba(255, 255, 255, 0.5);
      backdrop-filter: blur(4px);
      z-index: 100;
      display: flex;
      align-items: center;
      justify-content: center;
      opacity: 0;
      visibility: hidden;
      transition: opacity 0.3s, visibility 0.3s;
    }
    .modal-overlay.open { opacity: 1; visibility: visible; }
    .modal-content {
      background: white;
      border-radius: 24px;
      width: 100%;
      max-width: 500px;
      max-height: 90vh;
      overflow-y: auto;
      transform: scale(0.9);
      transition: transform 0.3s;
      box-shadow: 0 25px 50px -12px rgba(0, 0, 0, 0.25);
    }
    .modal-overlay.open .modal-content { transform: scale(1); }
    .modal-content-lg { max-width: 700px; }

    /* ========== MARQUEE ========== */
    .marquee-container { overflow: hidden; white-space: nowrap; }
    .marquee-content {
      display: inline-flex;
      animation: marquee 30s linear infinite;
    }
    @keyframes marquee {
      from { transform: translateX(0); }
      to { transform: translateX(-50%); }
    }

    /* ========== 3D CARD GALLERY ========== */
    .hero-gallery-container {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      min-height: 700px;
      position: relative;
    }
    
    .gallery-title-small {
      text-align: center;
      margin-bottom: 2rem;
    }
    .gallery-title-small h3 {
      font-family: 'Fraunces', serif;
      font-size: 1.5rem;
      font-weight: 600;
      color: var(--fg);
      margin-bottom: 0.25rem;
    }
    .gallery-title-small p {
      color: var(--muted);
      font-size: 0.95rem;
    }

    .slider-hero {
      width: 100%;
      max-width: 850px;
      height: 520px;
      position: relative;
      perspective: 1400px;
      display: flex;
      justify-content: center;
      align-items: center;
    }

    .wrapper-hero {
      transform-style: preserve-3d;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      position: relative;
      width: 580px;
      height: 520px;
    }

    .slide-hero {
      position: absolute;
      width: 420px;
      height: 460px;
      border-radius: 20px;
      overflow: hidden;
      transform-origin: bottom;
      animation: cardCycle 12s infinite;
      box-shadow: 0 20px 50px rgba(0,0,0,0.18);
      display: flex;
      flex-direction: column;
      justify-content: flex-end;
      color: white;
      font-weight: 500;
      font-size: 1.05rem;
      text-align: center;
      cursor: pointer;
      transition: transform 0.3s, box-shadow 0.3s;
      background-color: #2C1810;
    }
    .slide-hero:hover {
      transform: scale(1.05);
      z-index: 10 !important;
      box-shadow: 0 25px 60px rgba(0,0,0,0.25);
    }

    .slide-hero img {
      position: absolute;
      inset: 0;
      width: 100%;
      height: 100%;
      object-fit: cover;
      object-position: center;
      pointer-events: none;
      z-index: 1;
    }

    .slide-hero .card-overlay {
      position: absolute;
      inset: 0;
      background: linear-gradient(to top, rgba(0,0,0,0.75) 0%, rgba(0,0,0,0.15) 35%, transparent 65%);
      z-index: 2;
      pointer-events: none;
    }

    .slide-hero .card-label {
      position: relative;
      z-index: 3;
      text-shadow: 0 2px 8px rgba(0,0,0,0.5);
      font-family: 'Fraunces', serif;
      font-weight: 600;
      padding: 1.25rem 1.5rem;
    }

    .slide-hero:nth-child(1) { animation-delay: 10s; }
    .slide-hero:nth-child(2) { animation-delay: 8s; }
    .slide-hero:nth-child(3) { animation-delay: 6s; }
    .slide-hero:nth-child(4) { animation-delay: 4s; }
    .slide-hero:nth-child(5) { animation-delay: 2s; }
    .slide-hero:nth-child(6) { animation-delay: 0s; }

    @keyframes cardCycle {
      0% { transform: translateZ(0) rotateX(0); z-index: 2; opacity: 1; }
      13.88% { transform: translateZ(600px) rotateX(90deg); z-index: 3; opacity: 1; }
      16.66% { transform: translateZ(0px) rotateX(90deg); z-index: 1; opacity: 0; }
      83.33% { transform: translateZ(0px) rotateX(0); z-index: 1; opacity: 0; }
      97.22% { transform: translateZ(0) rotateX(0); z-index: 2; opacity: 1; }
      100% { transform: translateZ(0) rotateX(0); z-index: 2; opacity: 1; }
    }

    @media (max-width: 1024px) {
      .hero-gallery-container { min-height: 520px; margin-top: 3rem; }
      .slider-hero { height: 420px; }
      .wrapper-hero { width: 300px; height: 420px; }
      .slide-hero { width: 250px; height: 370px; font-size: 0.95rem; }
      .slide-hero .card-label { padding: 1rem 1.25rem; }
    }

    @media (max-width: 768px) {
      .hero-gallery-container { min-height: 450px; }
      .slider-hero { height: 360px; max-width: 100%; }
      .wrapper-hero { width: 260px; height: 360px; }
      .slide-hero { width: 210px; height: 310px; font-size: 0.85rem; }
      .gallery-title-small h3 { font-size: 1.2rem; }
      .gallery-title-small p { font-size: 0.85rem; }
    }

    /* ========== FEATURE CARDS ========== */
    .feature-card {
      background: white;
      border-radius: 16px;
      padding: 1.5rem;
      border: 1px solid var(--border);
      transition: all 0.3s;
    }
    .feature-card:hover {
      transform: translateY(-4px);
      box-shadow: 0 10px 30px rgba(0,0,0,0.08);
    }

    /* ========== PRICING CARDS ========== */
    .pricing-card {
      transition: all 0.3s;
    }
    .pricing-card:hover {
      transform: translateY(-4px);
    }

    /* ========== TESTIMONIAL CARDS ========== */
    .testimonial-card {
      background: white;
      border-radius: 20px;
      padding: 2rem;
      border: 1px solid var(--border);
    }

    /* ========== DASHBOARD PREVIEW ========== */
    .dashboard-preview {
      background: linear-gradient(135deg, #2C1810 0%, #4A3228 100%);
      border-radius: 20px;
      padding: 2rem;
      color: white;
    }

    /* ========== TRUST BADGES ========== */
    .trust-badge {
      display: inline-flex;
      align-items: center;
      gap: 0.5rem;
      padding: 0.5rem 1rem;
      background: white;
      border: 1px solid var(--border);
      border-radius: 100px;
      font-size: 0.875rem;
      font-weight: 500;
      color: var(--muted);
      transition: all 0.3s;
    }
    .trust-badge:hover {
      border-color: #C45D3E;
      color: #C45D3E;
    }

    /* ========== FORM INPUTS ========== */
    .input-field {
      width: 100%;
      padding: 0.75rem 1rem;
      border: 1px solid var(--border);
      border-radius: 12px;
      background: white;
      font-family: inherit;
      transition: border-color 0.3s;
    }
    .input-field:focus {
      outline: none;
      border-color: #C45D3E;
      box-shadow: 0 0 0 3px rgba(196, 93, 62, 0.1);
    }

    /* ========== SOCIAL SHARE BUTTONS ========== */
    .social-share-btn {
      display: inline-flex;
      align-items: center;                   
      gap: 0.5rem;
      padding: 0.6rem 1rem;
      border-radius: 12px;
      font-weight: 500;
      font-size: 0.875rem;
      transition: all 0.3s;
      cursor: pointer;
      border: none;
    }
    .social-share-btn.whatsapp { background: #25D366; color: white; }
    .social-share-btn.telegram { background: #0088cc; color: white; }
    .social-share-btn.facebook { background: #1877F2; color: white; }
    .social-share-btn:hover { transform: translateY(-2px); }

    /* ========== LOGO ========== */
    .logo-img {
      height: auto;
      max-height: 100%;
    }

    /* ========== SECTION UTILITIES ========== */
    section {
      position: relative;
    }

    .section-padding {
      padding: 6rem 1rem;
    }

    @media (min-width: 1024px) {
      .section-padding {
        padding: 8rem 1rem;
      }
    }
  </style>
</head>
<body class="antialiased">

  <!-- ========== NAVIGATION ========== -->
  <nav class="fixed top-0 left-0 right-0 z-50 bg-espresso">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex items-center justify-between h-16">
        <!-- Logo -->
        <a href="#" class="flex items-center gap-2 group flex-shrink-0" aria-label="Bene'nw Home">
          <img src="Benenew-01.png" alt="Bene'nw Logo" class="h-9 w-auto transition-transform group-hover:scale-105">
        </a>

        <!-- Desktop Navigation Links -->
        <div class="hidden lg:flex items-center gap-8">
          <a href="#occasions" class="nav-link">
            <span class="text-en">Occasions</span>
            <span class="text-am">አጋጣሚዎች</span>
          </a>
          <a href="#how-it-works" class="nav-link">
            <span class="text-en">How It Works</span>
            <span class="text-am">እንዴት እንደሚሰ</span>
          </a>
          <a href="#pricing" class="nav-link">
            <span class="text-en">Pricing</span>
            <span class="text-am">ዋጋ</span>
          </a>
          <button onclick="openModal('searchModal')" class="nav-link">
            <span class="text-en">Find a List</span>
            <span class="text-am">ዝርዝር ይፈልጉ</span>
          </button>
        </div>

        <!-- Right Side: Language Toggle + Auth Buttons -->
        <div class="hidden lg:flex items-center gap-4">
          <div class="lang-toggle" role="tablist" aria-label="Language selection">
            <button role="tab" aria-selected="true" class="active" data-lang="en">EN</button>
            <button role="tab" aria-selected="false" data-lang="am">አማ</button>
          </div>
          <button onclick="openModal('loginModal')" class="text-sm font-medium text-ivory/70 hover:text-ivory transition-colors">
            <span class="text-en">Log in</span>
            <span class="text-am">ግባ</span>
          </button>
          <button onclick="openModal('signupModal')" class="inline-flex items-center gap-2 bg-terracotta hover:bg-terracotta-dark text-white text-sm font-semibold px-5 py-2.5 rounded-full transition-all hover:shadow-lg hover:shadow-terracotta/20">
            <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round">
              <path d="M15 3h4a2 2 0 0 1 2 2v14a2 2 0 0 1-2 2h-4"/>
              <polyline points="10 17 15 12 10 7"/>
              <line x1="15" y1="12" x2="3" y2="12"/>
            </svg>
            <span class="text-en">Sign In</span>
            <span class="text-am">ይግቡ</span>
          </button>
        </div>

        <!-- Mobile Menu Button -->
        <button class="lg:hidden p-2 -mr-2 text-ivory/70 hover:text-ivory" id="menuBtn" aria-label="Open menu" aria-expanded="false">
          <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
            <line x1="3" y1="6" x2="21" y2="6"/>
            <line x1="3" y1="12" x2="21" y2="12"/>
            <line x1="3" y1="18" x2="21" y2="18"/>
          </svg>
        </button>
      </div>
    </div>
  </nav>

  <!-- ========== MOBILE MENU ========== -->
  <div class="mobile-menu" id="mobileMenu" aria-hidden="true">
    <div class="p-6">
      <div class="flex justify-between items-center mb-8">
        <img src="Benenew-01.png" alt="Bene'nw Logo" class="h-10 w-auto">
        <button id="closeMenuBtn" aria-label="Close menu">
          <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
            <line x1="18" y1="6" x2="6" y2="18"/>
            <line x1="6" y1="6" x2="18" y2="18"/>
          </svg>
        </button>
      </div>
      <div class="flex flex-col gap-4">
        <a href="#occasions" class="text-xl font-medium py-3 border-b border-border">
            <span class="text-en">Occasions</span>
            <span class="text-am">አጋጣሚዎች</span>
        </a>
        <a href="#how-it-works" class="text-xl font-medium py-3 border-b border-border">
            <span class="text-en">How It Works</span>
            <span class="text-am">እንዴት እንደሚሰራ</span>
        </a>
        <a href="#pricing" class="text-xl font-medium py-3 border-b border-border">
            <span class="text-en">Pricing</span>
            <span class="text-am">ዋጋ</span>
        </a>
        <button onclick="openModal('searchModal'); closeMobileMenu();" class="text-xl font-medium py-3 border-b border-border text-left">
            <span class="text-en">Find a List</span>
            <span class="text-am">ዝርዝር ይፈል</span>
        </button>
        <div class="mt-4 flex flex-col gap-3">
          <button onclick="openModal('loginModal'); closeMobileMenu();" class="btn-secondary text-center">
             <span class="text-en">Log In</span>
             <span class="text-am">ግባ</span>
          </button>
          <button onclick="openModal('signupModal'); closeMobileMenu();" class="btn-primary text-center text-white">
             <span class="text-en">Sign In</span>
             <span class="text-am">ይግቡ</span>
          </button>
        </div>
        <div class="mt-4">
          <div class="lang-toggle" role="tablist" aria-label="Language selection">
            <button role="tab" aria-selected="true" class="active" data-lang="en">EN</button>
            <button role="tab" aria-selected="false" data-lang="am">አማ</button>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- ========== MODALS ========== -->

  <!-- Login Modal -->
  <div id="loginModal" class="modal-overlay">
    <div class="modal-content p-8 m-4">
      <div class="text-center mb-6">
        <img src="Benenew-01.png" alt="Bene'nw Logo" class="h-16 w-auto mx-auto mb-3">
        <h2 class="font-display text-2xl font-semibold text-espresso">
          <span class="text-en">Welcome back</span>
          <span class="text-am">እንኳን ደህና መጡ</span>
        </h2>
        <p class="text-muted mt-2 text-sm">
          <span class="text-en">Log in to manage your gift lists</span>
          <span class="text-am">የስጦታ ዝርዝሮችን ለማስተዳደር ይግቡ</span>
        </p>
      </div>
      <form class="space-y-4" onsubmit="event.preventDefault(); closeModal('loginModal');">
        <div>
          <label class="block text-sm font-medium text-muted mb-1">
            <span class="text-en">Email address</span>
            <span class="text-am">ኢሜይል</span>
          </label>
          <input type="email" id="loginEmail" placeholder="you@example.com" class="input-field" required>
        </div>
        <div>
          <label class="block text-sm font-medium text-muted mb-1">
            <span class="text-en">Password</span>
            <span class="text-am">የይለፍ ቃል</span>
          </label>
          <input type="password" id="loginPassword" placeholder="••••••••" class="input-field" required>
        </div>
        <div class="flex justify-between items-center">
          <label class="flex items-center gap-2 text-sm text-muted">
            <input type="checkbox" class="w-4 h-4 rounded border-border text-terracotta focus:ring-terracotta">
            <span class="text-en">Remember me</span>
            <span class="text-am">አስታውሰኝ</span>
          </label>
          <button type="button" onclick="closeModal('loginModal'); openModal('forgotModal');" class="text-sm text-terracotta hover:underline font-medium">
            <span class="text-en">Forgot password?</span>
            <span class="text-am">የይለፍ ቃል ሱ?</span>
          </button>
        </div>
        <button type="submit" class="w-full btn-primary py-3 rounded-full">
          <span class="text-en">Log In</span>
          <span class="text-am">ግባ</span>
        </button>
        <p class="text-center text-sm text-muted">
          <span class="text-en">Don't have an account?</span>
          <span class="text-am">መለያ የለዎትም?</span>
          <button type="button" onclick="closeModal('loginModal'); openModal('signupModal');" class="text-terracotta font-semibold ml-1 hover:underline">
            <span class="text-en">Sign Up</span>
            <span class="text-am">ይመዝገቡ</span>
          </button>
        </p>
      </form>
    </div>
  </div>

  <!-- Sign Up Modal -->
  <div id="signupModal" class="modal-overlay">
    <div class="modal-content p-8 m-4">
      <div class="text-center mb-6">
        <img src="Benenew-01.png" alt="Bene'nw Logo" class="h-16 w-auto mx-auto mb-3">
        <h2 class="font-display text-2xl font-semibold text-espresso">
          <span class="text-en">Create your account</span>
          <span class="text-am">መለያ ይፍጠሩ</span>
        </h2>
        <p class="text-muted mt-2 text-sm">
          <span class="text-en">Start your gift registry in minutes</span>
          <span class="text-am">የስጦታ ዝርዝርዎን በቂቃች ይጀምሩ</span>
        </p>
      </div>
      <form class="space-y-4" onsubmit="event.preventDefault(); closeModal('signupModal');">
        <div class="grid grid-cols-2 gap-4">
          <div>
            <label class="block text-sm font-medium text-muted mb-1">
              <span class="text-en">First Name</span>
              <span class="text-am">ስም</span>
            </label>
            <input type="text" id="signupFirst" placeholder="First name" class="input-field" required>
          </div>
          <div>
            <label class="block text-sm font-medium text-muted mb-1">
              <span class="text-en">Last Name</span>
              <span class="text-am">የአባት ስም</span>
            </label>
            <input type="text" id="signupLast" placeholder="Last name" class="input-field" required>
          </div>
        </div>
        <div>
          <label class="block text-sm font-medium text-muted mb-1">
            <span class="text-en">Email address</span>
            <span class="text-am">ኢሜይል</span>
          </label>
          <input type="email" id="signupEmail" placeholder="you@example.com" class="input-field" required>
        </div>
        <div>
          <label class="block text-sm font-medium text-muted mb-1">
            <span class="text-en">Phone (optional)</span>
            <span class="text-am">ስልክ (አማራጭ)</span>
          </label>
          <input type="tel" id="signupPhone" placeholder="+251 9XX XXX XXX" class="input-field">
        </div>
        <div>
          <label class="block text-sm font-medium text-muted mb-1">
            <span class="text-en">Password</span>
            <span class="text-am">የይለፍ ቃል</span>
          </label>
          <input type="password" id="signupPassword" placeholder="Min 8 characters" class="input-field" required minlength="8">
        </div>
        <div>
          <label class="flex items-start gap-2 text-sm text-muted">
            <input type="checkbox" id="signupTerms" class="w-4 h-4 mt-0.5 rounded border-border text-terracotta focus:ring-terracotta" required>
            <span class="text-en">I agree to the <a href="#" class="text-terracotta hover:underline">Terms of Service</a> and <a href="#" class="text-terracotta hover:underline">Privacy Policy</a></span>
            <span class="text-am"><a href="#" class="text-terracotta hover:underline">የአገልሎት ደን</a> እና <a href="#" class="text-terracotta hover:underline">የግላነት ፖሊሲ</a> ተስማምቻለሁ</span>
          </label>
        </div>
        <button type="submit" class="w-full btn-primary py-3 rounded-full">
          <span class="text-en">Create Account</span>
          <span class="text-am">መለያ ይፍጠሩ</span>
        </button>
        <p class="text-center text-sm text-muted">
          <span class="text-en">Already have an account?</span>
          <span class="text-am">መለያ አለዎት?</span>
          <button type="button" onclick="closeModal('signupModal'); openModal('loginModal');" class="text-terracotta font-semibold ml-1 hover:underline">
            <span class="text-en">Log In</span>
            <span class="text-am">ግባ</span>
          </button>
        </p>
      </form>
    </div>
  </div>

  <!-- Forgot Password Modal -->
  <div id="forgotModal" class="modal-overlay">
    <div class="modal-content p-8 m-4">
      <div class="text-center mb-6">
        <img src="Benenew-01.png" alt="Bene'nw Logo" class="h-16 w-auto mx-auto mb-3">
        <h2 class="font-display text-2xl font-semibold text-espresso">
          <span class="text-en">Reset password</span>
          <span class="text-am">የይለፍ ቃል ዳግም ያስቀም</span>
        </h2>
        <p class="text-muted mt-2 text-sm">
          <span class="text-en">Enter your email and we'll send you a reset link</span>
          <span class="text-am">ኢሜይልን ያስገቡ እና የማስተካከያ ሊንክ እንልክልዎታለን</span>
        </p>
      </div>
      <form class="space-y-4" onsubmit="event.preventDefault(); closeModal('forgotModal');">
        <div>
          <label class="block text-sm font-medium text-muted mb-1">
            <span class="text-en">Email address</span>
            <span class="text-am">ኢሜይል</span>
          </label>
          <input type="email" placeholder="you@example.com" class="input-field" required>
        </div>
        <button type="submit" class="w-full btn-primary py-3 rounded-full">
          <span class="text-en">Send Reset Link</span>
          <span class="text-am">ማስተካከያ ሊንክ ይላኩ</span>
        </button>
        <button type="button" onclick="closeModal('forgotModal'); openModal('loginModal');" class="w-full btn-secondary py-3 rounded-full">
          <span class="text-en">Back to Login</span>
          <span class="text-am">ወደ መግቢያ ተመለስ</span>
        </button>
      </form>
    </div>
  </div>

  <!-- Create List Modal -->
  <div id="createModal" class="modal-overlay">
    <div class="modal-content p-8 m-4">
      <div class="text-center mb-6">
        <img src="Benenew-01.png" alt="Bene'nw Logo" class="h-16 w-auto mx-auto mb-3">
        <h2 class="font-display text-2xl font-semibold text-espresso">
          <span class="text-en">Create your list</span>
          <span class="text-am">ዝርዝርዎን ይፍሩ</span>
        </h2>
      </div>
      <form class="space-y-4" onsubmit="event.preventDefault(); closeModal('createModal');">
        <div>
          <label class="block text-sm font-medium text-muted mb-1">
            <span class="text-en">Occasion Type</span>
            <span class="text-am">የአጋጣሚ ዓይነት</span>
          </label>
          <select class="input-field" required>
            <option value="">Select occasion...</option>
            <option value="wedding">Wedding / ሰርግ</option>
            <option value="baby">Baby / ልደት</option>
            <option value="birthday">Birthday / ልደት በዓል</option>
            <option value="graduation">Graduation / ምረቃ</option>
            <option value="housewarming">Housewarming / አዲስ ቤት</option>
            <option value="group">Group Fund / የቡድን ፈን</option>
            <option value="holiday">Holiday / በዓል</option>
          </select>
        </div>
        <div>
          <label class="block text-sm font-medium text-muted mb-1">
            <span class="text-en">List Title</span>
            <span class="text-am">የዝርዝር ርዕስ</span>
          </label>
          <input type="text" placeholder="e.g., Abebe & Sara's Wedding" class="input-field" required>
        </div>
        <div>
          <label class="block text-sm font-medium text-muted mb-1">
            <span class="text-en">Event Date</span>
            <span class="text-am">የክስተት ቀን</span>
          </label>
          <input type="date" class="input-field" required>
        </div>
        <div class="flex gap-3 pt-4">
          <button type="button" onclick="closeModal('createModal')" class="flex-1 btn-secondary py-3 rounded-full">
            <span class="text-en">Cancel</span>
            <span class="text-am">ሰርዝ</span>
          </button>
          <button type="submit" class="flex-1 btn-primary py-3 rounded-full">
            <span class="text-en">Create List</span>
            <span class="text-am">ዝርዝር ይፍጠሩ</span>
          </button>
        </div>
      </form>
    </div>
  </div>

  <!-- Find a List Modal -->
  <div id="searchModal" class="modal-overlay">
    <div class="modal-content p-8 m-4">
      <div class="text-center mb-6">
        <img src="Benenew-01.png" alt="Bene'nw Logo" class="h-16 w-auto mx-auto mb-3">
        <h2 class="font-display text-2xl font-semibold text-espresso">
          <span class="text-en">Find a gift list</span>
          <span class="text-am">ዝርዝር ይፈል</span>
        </h2>
        <p class="text-muted mt-2 text-sm">
          <span class="text-en">Search by name, occasion, or private invite code</span>
          <span class="text-am">በስም፣ በአጣሚ ይም በግል ግብዣ ድ ይፈልጉ</span>
        </p>
      </div>
      <form class="space-y-4" onsubmit="event.preventDefault(); closeModal('searchModal');">
        <div>
          <label class="block text-sm font-medium text-muted mb-1">
            <span class="text-en">First Name</span>
            <span class="text-am">ስም</span>
          </label>
          <input type="text" placeholder="Search by first name..." class="input-field text-lg">
        </div>
        <div>
          <label class="block text-sm font-medium text-muted mb-1">
            <span class="text-en">Last Name</span>
            <span class="text-am">የአባት ስም</span>
          </label>
          <input type="text" placeholder="Search by last name..." class="input-field">
        </div>
        <div>
          <label class="block text-sm font-medium text-muted mb-1">
            <span class="text-en">Occasion</span>
            <span class="text-am">አጋጣሚ</span>
          </label>
          <select class="input-field">
            <option value="">All occasions</option>
            <option value="wedding">Wedding / ሰርግ</option>
            <option value="baby">Baby / ልደት</option>
            <option value="birthday">Birthday / ልደት በዓል</option>
            <option value="graduation">Graduation / ምረቃ</option>
            <option value="housewarming">Housewarming / አዲስ ቤት</option>
          </select>
        </div>
        <div>
          <label class="block text-sm font-medium text-muted mb-1">
            <span class="text-en">Invite Code (optional)</span>
            <span class="text-am">የግብዣ ድ (አማራጭ)</span>
          </label>
          <input type="text" placeholder="e.g., BEN-XXXX" class="input-field font-mono">
        </div>
        <div class="flex gap-3">
          <button type="button" onclick="closeModal('searchModal')" class="flex-1 btn-secondary py-3 rounded-full">
             <span class="text-en">Cancel</span>
             <span class="text-am">ሰርዝ</span>
          </button>
          <button type="submit" class="flex-1 btn-primary py-3 rounded-full">
             <span class="text-en">Search</span>
             <span class="text-am">ፈል</span>
          </button>
        </div>
      </form>
    </div>
  </div>

  <!-- Share Modal -->
  <div id="shareModal" class="modal-overlay">
    <div class="modal-content p-8 m-4">
      <div class="text-center mb-6">
        <div class="w-16 h-16 mx-auto bg-terracotta/10 rounded-full flex items-center justify-center mb-4">
          <svg width="32" height="32" viewBox="0 0 24 24" fill="none" stroke="#C45D3E" stroke-width="2"><circle cx="18" cy="5" r="3"/><circle cx="6" cy="12" r="3"/><circle cx="18" cy="19" r="3"/><line x1="8.59" y1="13.51" x2="15.42" y2="17.49"/><line x1="15.41" y1="6.51" x2="8.59" y2="10.49"/></svg>
        </div>
        <h2 class="font-display text-2xl font-semibold text-espresso">
          <span class="text-en">Share your list</span>
          <span class="text-am">ዝርዝርዎን ያጋሩ</span>
        </h2>
        <p class="text-muted mt-2 text-sm">
          <span class="text-en">Share with family and friends</span>
          <span class="text-am">ከቤተሰብና ከጓኞች ጋር ያጋሩ</span>
        </p>
      </div>
      <div class="space-y-4">
        <div class="flex gap-2">
          <input type="text" value="https://benenw.com/list/abebe-sara" readonly class="input-field flex-1 font-mono text-sm">
          <button onclick="copyToClipboard()" class="btn-primary btn-sm whitespace-nowrap">
            <span class="text-en">Copy</span>
            <span class="text-am">ቅዳ</span>
          </button>
        </div>
        <div class="flex flex-wrap gap-2">
          <button class="social-share-btn whatsapp">
            <svg width="18" height="18" viewBox="0 0 24 24" fill="white"><path d="M17.472 14.382c-.297-.149-1.758-.867-2.03-.967-.273-.099-.471-.148-.67.15-.197.297-.767.966-.94 1.164-.173.199-.347.223-.644.075-.297-.15-1.255-.463-2.39-1.475-.883-.788-1.48-1.761-1.653-2.059-.173-.297-.018-.458.13-.606.134-.133.298-.347.446-.52.149-.174.198-.298.298-.497.099-.198.05-.371-.025-.52-.075-.149-.669-1.612-.916-2.207-.242-.579-.487-.5-.669-.51-.173-.008-.371-.01-.57-.01-.198 0-.52.074-.792.372-.272.297-1.04 1.016-1.04 2.479 0 1.462 1.065 2.875 1.213 3.074.149.198 2.096 3.2 5.077 4.487.709.306 1.262.489 1.694.625.712.227 1.36.195 1.871.118.571-.085 1.758-.719 2.006-1.413.248-.694.248-1.289.173-1.413-.074-.124-.272-.198-.57-.347z"/><path d="M12 2C6.477 2 2 6.477 2 12c0 1.89.525 3.66 1.438 5.168L2 22l4.832-1.438A9.955 9.955 0 0 0 12 22c5.523 0 10-4.477 10-10S17.523 2 12 2zm0 18a8 8 0 0 1-4.243-1.214l-.29-.174-3.054.906.906-3.054-.174-.29A8 8 0 1 1 12 20z"/></svg>
            WhatsApp
          </button>
          <button class="social-share-btn telegram">
            <svg width="18" height="18" viewBox="0 0 24 24" fill="white"><path d="M21.198 2.433a2.242 2.242 0 0 0-1.022.215l-17.15 6.57a1.9 1.9 0 0 0 .085 3.54l4.15 1.62 2.25 6.65a1.32 1.32 0 0 0 2.26.32l3.07-3.38 4.35 3.2a1.88 1.88 0 0 0 2.94-1.22l2.75-13.74a2.24 2.24 0 0 0-1.68-2.77z"/></svg>
            Telegram
          </button>
          <button class="social-share-btn facebook">
            <svg width="18" height="18" viewBox="0 0 24 24" fill="white"><path d="M18 2h-3a5 5 0 0 0-5 5v3H7v4h3v8h4v-8h3l1-4h-4V7a1 1 0 0 1 1-1h3z"/></svg>
            Facebook
          </button>
        </div>
        <div class="text-center pt-2">
          <button class="text-sm text-terracotta hover:underline font-medium">
            <span class="text-en">Download QR Code</span>
            <span class="text-am">QR ኮድ ያውርዱ</span>
          </button>
        </div>
      </div>
    </div>
  </div>

  <!-- Contact Modal -->
  <div id="contactModal" class="modal-overlay">
    <div class="modal-content modal-content-lg p-8 m-4">
      <div class="text-center mb-6">
        <img src="Benenew-01.png" alt="Bene'nw Logo" class="h-16 w-auto mx-auto mb-3">
        <h2 class="font-display text-2xl font-semibold text-espresso">
          <span class="text-en">Contact Us</span>
          <span class="text-am">አግኙን</span>
        </h2>
      </div>
      <form class="space-y-4" onsubmit="event.preventDefault(); closeModal('contactModal');">
        <div class="grid grid-cols-2 gap-4">
          <div>
            <label class="block text-sm font-medium text-muted mb-1"><span class="text-en">Name</span><span class="text-am">ስም</span></label>
            <input type="text" placeholder="Your name" class="input-field" required>
          </div>
          <div>
            <label class="block text-sm font-medium text-muted mb-1"><span class="text-en">Email</span><span class="text-am">ኢሜይል</span></label>
            <input type="email" placeholder="you@example.com" class="input-field" required>
          </div>
        </div>
        <div>
          <label class="block text-sm font-medium text-muted mb-1"><span class="text-en">Subject</span><span class="text-am">ርዕስ</span></label>
          <select class="input-field">
            <option>General Inquiry</option>
            <option>Technical Support</option>
            <option>Partnership</option>
            <option>Vendor Registration</option>
          </select>
        </div>
        <div>
          <label class="block text-sm font-medium text-muted mb-1"><span class="text-en">Message</span><span class="text-am">መልዕክት</span></label>
          <textarea rows="4" placeholder="How can we help?" class="input-field" required></textarea>
        </div>
        <div class="flex gap-3">
          <button type="button" onclick="closeModal('contactModal')" class="flex-1 btn-secondary py-3 rounded-full">
            <span class="text-en">Cancel</span><span class="text-am">ሰርዝ</span>
          </button>
          <button type="submit" class="flex-1 btn-primary py-3 rounded-full">
            <span class="text-en">Send Message</span><span class="text-am">መልዕክት ይላ</span>
          </button>
        </div>
      </form>
    </div>
  </div>

  <!-- ========== HERO SECTION ========== -->
  <section class="relative min-h-screen flex items-center pt-16 overflow-hidden">
    <div class="orb orb-1 -top-20 -right-20" aria-hidden="true"></div>
    <div class="orb orb-2 top-1/3 -left-32" aria-hidden="true"></div>
    <div class="absolute inset-0 ethiopian-pattern opacity-30" aria-hidden="true"></div>

    <div class="relative max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-20 lg:py-32">
      <div class="grid lg:grid-cols-2 gap-12 lg:gap-20 items-center">
        <!-- Left Content -->
        <div class="text-center lg:text-left">
          <div class="inline-flex items-center gap-2 px-4 py-2 bg-terracotta/10 rounded-full text-terracotta text-sm font-semibold mb-6 hero-animate">
            <span class="w-2 h-2 bg-terracotta rounded-full animate-pulse"></span>
            <span class="text-en">Ethiopia's #1 Gift Registry Platform</span>
            <span class="text-am">የኢትዮጵያ ቁጥር 1 የስጦታ ዝርዝር መድረክ</span>
          </div>
          <h1 class="hero-animate font-display text-5xl sm:text-6xl lg:text-7xl font-semibold text-espresso leading-[1.08] tracking-tight">
            <span class="text-en">Create your gift list, <span class="text-terracotta">your way</span></span>
            <span class="text-am">የስጦታ ዝርዝርዎን <span class="text-terracotta">በእርስዎ መንገድ</span> ይፍሩ</span>
          </h1>
          <p class="hero-animate hero-delay-1 mt-6 text-xl text-espresso/65 max-w-xl mx-auto lg:mx-0 leading-relaxed">
            <span class="text-en">One beautiful link for weddings, babies, birthdays, graduations, and life's special moments. Add gifts from anywhere, collect support securely, and share with the people who matter most.</span>
            <span class="text-am">ለሰርግ፣ ደት፣ ደት በዓል፣ ምረቃ አዲስ ቤት እና ለሌሎች ልዩ አጋጣሚዎች አንድ ውብ ሊንክ።</span>
          </p>
          <div class="hero-animate hero-delay-2 mt-10 flex flex-col sm:flex-row gap-4 justify-center lg:justify-start">
            <button onclick="openModal('signupModal')" class="btn-primary text-lg">
               <span class="text-en">Create Your List — It's Free</span>
               <span class="text-am">ዝርዝር ይፍጠሩ — ነጻ ነው</span>
            </button>
            <button onclick="openModal('searchModal')" class="btn-secondary text-lg">
               <span class="text-en">Find a List</span>
               <span class="text-am">ዝርዝር ይፈልጉ</span>
            </button>
          </div>
          <div class="hero-animate hero-delay-3 mt-10 flex flex-wrap gap-3 justify-center lg:justify-start">
            <span class="trust-badge">
              <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"/></svg>
              <span class="text-en">Secure payments</span>
              <span class="text-am">ደህንነ የተጠበ ክፍያ</span>
            </span>
            <span class="trust-badge">
              <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M17 21v-2a4 4 0 0 0-4-4H5a4 4 0 0 0-4 4v2"/><circle cx="9" cy="7" r="4"/></svg>
              <span class="text-en">One link to share</span>
              <span class="text-am">አንድ ሊንክ ለማጋራት</span>
            </span>
            <span class="trust-badge">
              <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"/><polyline points="22 4 12 14.01 9 11.01"/></svg>
              <span class="text-en">Built for Ethiopia</span>
              <span class="text-am">ለኢትዮጵያ የተሰራ</span>
            </span>
            <span class="trust-badge">
              <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="10"/><line x1="2" y1="12" x2="22" y2="12"/><path d="M12 2a15.3 15.3 0 0 1 4 10 15.3 15.3 0 0 1-4 10 15.3 15.3 0 0 1-4-10 15.3 15.3 0 0 1 4-10z"/></svg>
              <span class="text-en">Diaspora-friendly</span>
              <span class="text-am">ለዲያስፖራ ቹ</span>
            </span>
          </div>
        </div>

        <!-- Right Side - 3D Card Gallery -->
        <div class="hero-animate hero-delay-4">
          <div class="hero-gallery-container">
            <div class="gallery-title-small">
              <h3><span class="text-en">Celebrations on Bene'nw</span><span class="text-am">በBene'nw ላይ ያሉ ክረ በዓሎች</span></h3>
              <p><span class="text-en">See how families celebrate together</span><span class="text-am">ቤተሰቦች እንዴት አብረው እንደሚያከብሩ ይመልከቱ</span></p>
            </div>
            
            <div class="slider-hero">
              <div class="wrapper-hero">
                <div class="slide-hero">
                  <img src="images (2).jpg" alt="Wedding celebration">
                  <div class="card-overlay"></div>
                  <div class="card-label"><span class="text-en">Wedding 💍</span><span class="text-am">ሰርግ 💍</span></div>
                </div>
                <div class="slide-hero">
                  <img src="download (7).jpg" alt="Baby celebration">
                  <div class="card-overlay"></div>
                  <div class="card-label"><span class="text-en">Baby 👶</span><span class="text-am">ልደት 👶</span></div>
                </div>
                <div class="slide-hero">
                  <img src="download (8).jpg" alt="Birthday celebration">
                  <div class="card-overlay"></div>
                  <div class="card-label"><span class="text-en">Birthday 🎂</span><span class="text-am">ልደት በዓል 🎂</span></div>
                </div>
                <div class="slide-hero">
                  <img src="download.jpg" alt="Graduation celebration">
                  <div class="card-overlay"></div>
                  <div class="card-label"><span class="text-en">Graduation 🎓</span><span class="text-am">ምረቃ </span></div>
                </div>
                <div class="slide-hero">
                  <img src="download (1).jpg" alt="Housewarming celebration">
                  <div class="card-overlay"></div>
                  <div class="card-label"><span class="text-en">Housewarming 🏠</span><span class="text-am">አዲስ ቤት </span></div>
                </div>
                <div class="slide-hero">
                  <img src="download (6).jpg" alt="Group contribution">
                  <div class="card-overlay"></div>
                  <div class="card-label"><span class="text-en">Group Fund 🎁</span><span class="text-am">የቡድን አስተዋፅኦ 🎁</span></div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- ========== STATS MARQUEE ========== -->
  <section class="bg-espresso py-8 relative overflow-hidden">
    <div class="marquee-container">
      <div class="marquee-content">
        <div class="flex items-center gap-16 px-8">
          <div class="flex items-center gap-3 text-white/80">
            <span class="font-display text-3xl font-semibold text-gold">2,500+</span>
            <span class="text-sm"><span class="text-en">Lists Created</span><span class="text-am">ዝርዝሮች ተፈረዋል</span></span>
          </div>
          <div class="w-px h-8 bg-white/20"></div>
          <div class="flex items-center gap-3 text-white/80">
            <span class="font-display text-3xl font-semibold text-gold">15M+</span>
            <span class="text-sm">ETB <span class="text-en">Contributed</span><span class="text-am">ተሰብስቧል</span></span>
          </div>
          <div class="w-px h-8 bg-white/20"></div>
          <div class="flex items-center gap-3 text-white/80">
            <span class="font-display text-3xl font-semibold text-gold">50+</span>
            <span class="text-sm"><span class="text-en">Cities Covered</span><span class="text-am">ከተሞች</span></span>
          </div>
          <div class="w-px h-8 bg-white/20"></div>
          <div class="flex items-center gap-3 text-white/80">
            <span class="font-display text-3xl font-semibold text-gold">4.9 ★</span>
            <span class="text-sm"><span class="text-en">User Rating</span><span class="text-am">ደረጃ</span></span>
          </div>
          <div class="w-px h-8 bg-white/20"></div>
          <div class="flex items-center gap-3 text-white/80">
            <span class="font-display text-3xl font-semibold text-gold">3</span>
            <span class="text-sm"><span class="text-en">Payment Options</span><span class="text-am">የክፍያ አማራጮች</span></span>
          </div>
          <div class="w-px h-8 bg-white/20"></div>
        </div>
        <div class="flex items-center gap-16 px-8" aria-hidden="true">
          <div class="flex items-center gap-3 text-white/80">
            <span class="font-display text-3xl font-semibold text-gold">2,500+</span>
            <span class="text-sm"><span class="text-en">Lists Created</span><span class="text-am">ዝርዝሮች ተፈጥረዋል</span></span>
          </div>
          <div class="w-px h-8 bg-white/20"></div>
          <div class="flex items-center gap-3 text-white/80">
            <span class="font-display text-3xl font-semibold text-gold">15M+</span>
            <span class="text-sm">ETB <span class="text-en">Contributed</span><span class="text-am">ተሰብስቧል</span></span>
          </div>
          <div class="w-px h-8 bg-white/20"></div>
          <div class="flex items-center gap-3 text-white/80">
            <span class="font-display text-3xl font-semibold text-gold">50+</span>
            <span class="text-sm"><span class="text-en">Cities Covered</span><span class="text-am">ከተሞች</span></span>
          </div>
          <div class="w-px h-8 bg-white/20"></div>
          <div class="flex items-center gap-3 text-white/80">
            <span class="font-display text-3xl font-semibold text-gold">4.9 ★</span>
            <span class="text-sm"><span class="text-en">User Rating</span><span class="text-am">ደረ</span></span>
          </div>
          <div class="w-px h-8 bg-white/20"></div>
          <div class="flex items-center gap-3 text-white/80">
            <span class="font-display text-3xl font-semibold text-gold">3</span>
            <span class="text-sm"><span class="text-en">Payment Options</span><span class="text-am">የክፍያ አማራጮች</span></span>
          </div>
          <div class="w-px h-8 bg-white/20"></div>
        </div>
      </div>
    </div>
  </section>

  <!-- ========== HOW IT WORKS ========== -->
  <section id="how-it-works" class="py-24 lg:py-32 relative">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center mb-16">
        <div class="inline-flex items-center gap-2 px-4 py-2 bg-terracotta/10 rounded-full text-terracotta text-sm font-semibold mb-4 reveal">
          <span class="text-en">How It Works</span>
          <span class="text-am">እንዴት እንደሚሰራ</span>
        </div>
        <h2 class="reveal font-display text-4xl sm:text-5xl font-semibold text-espresso">
          <span class="text-en">Simple to create. Easy to share. Better to receive.</span>
          <span class="text-am">ለመፍጠር ቀላል። ለማጋራት ቹ። መቀበል የተሻለ።</span>
        </h2>
        <p class="reveal reveal-delay-1 mt-4 text-lg text-espresso/60 max-w-2xl mx-auto">
          <span class="text-en">Create a personalized list, add gifts or contribution goals, and send one link to friends and family.</span>
          <span class="text-am">የእርስዎን የስጦታ ርዝር ይጠሩ፣ ስታዎችን ይም የገንዘብ አስተዋፅኦ ግቦችን ያክሉ እና በአን ሊንክ ወዳችዎ ያጋሩ።</span>
        </p>
      </div>

      <div class="grid sm:grid-cols-2 lg:grid-cols-4 gap-8">
        <!-- Step 1 -->
        <div class="reveal reveal-delay-1 relative">
          <div class="text-center">
            <div class="w-20 h-20 mx-auto bg-gradient-to-br from-terracotta to-terracotta-dark rounded-2xl flex items-center justify-center text-white mb-6 shadow-lg">
              <svg width="32" height="32" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/><polyline points="14 2 14 8 20 8"/></svg>
            </div>
            <div class="font-display text-sm font-semibold text-terracotta mb-2"><span class="text-en">Step 1</span><span class="text-am">ደረጃ 1</span></div>
            <h3 class="font-display text-xl font-semibold text-espresso mb-3"><span class="text-en">Create</span><span class="text-am">ይፍሩ</span></h3>
            <p class="text-espresso/60"><span class="text-en">Open your list and choose your occasion.</span><span class="text-am">ዝርዝርዎን ይክፈቱ እና አጋሚን ይምረጡ</span></p>
          </div>
        </div>
        <!-- Step 2 -->
        <div class="reveal reveal-delay-2 relative">
          <div class="text-center">
            <div class="w-20 h-20 mx-auto bg-gradient-to-br from-gold to-gold-dark rounded-2xl flex items-center justify-center text-white mb-6 shadow-lg">
              <svg width="32" height="32" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="9" cy="21" r="1"/><circle cx="20" cy="21" r="1"/><path d="M1 1h4l2.68 13.39a2 2 0 0 0 2 1.61h9.72a2 2 0 0 0 2-1.61L23 6H6"/></svg>
            </div>
            <div class="font-display text-sm font-semibold text-gold-dark mb-2"><span class="text-en">Step 2</span><span class="text-am">ደረጃ 2</span></div>
            <h3 class="font-display text-xl font-semibold text-espresso mb-3"><span class="text-en">Add</span><span class="text-am">ያክሉ</span></h3>
            <p class="text-espresso/60"><span class="text-en">Add gifts, contribution goals, or personal wishes from anywhere.</span><span class="text-am">ስጦታችን፣ የንዘብ አስተዋፅኦ ቦችን ወይም ግላዊ ምኞቶችን ያክሉ።</span></p>
          </div>
        </div>
        <!-- Step 3 -->
        <div class="reveal reveal-delay-3 relative">
          <div class="text-center">
            <div class="w-20 h-20 mx-auto bg-gradient-to-br from-sage to-green-700 rounded-2xl flex items-center justify-center text-white mb-6 shadow-lg">
              <svg width="32" height="32" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="18" cy="5" r="3"/><circle cx="6" cy="12" r="3"/><circle cx="18" cy="19" r="3"/><line x1="8.59" y1="13.51" x2="15.42" y2="17.49"/><line x1="15.41" y1="6.51" x2="8.59" y2="10.49"/></svg>
            </div>
            <div class="font-display text-sm font-semibold text-sage mb-2"><span class="text-en">Step 3</span><span class="text-am">ደረ 3</span></div>
            <h3 class="font-display text-xl font-semibold text-espresso mb-3"><span class="text-en">Share</span><span class="text-am">ያጋሩ</span></h3>
            <p class="text-espresso/60"><span class="text-en">Send your list through WhatsApp, Telegram, email, or QR code.</span><span class="text-am">ዝርዝርዎን በWhatsApp፣ Telegram ኢሜይል ወይም QR ኮድ ያሩ።</span></p>
          </div>
        </div>
        <!-- Step 4 -->
        <div class="reveal reveal-delay-4">
          <div class="text-center">
            <div class="w-20 h-20 mx-auto bg-gradient-to-br from-espresso to-espresso-light rounded-2xl flex items-center justify-center text-white mb-6 shadow-lg">
              <svg width="32" height="32" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 2v20M17 5H9.5a3.5 3.5 0 0 0 0 7h5a3.5 3.5 0 0 1 0 7H6"/></svg>
            </div>
            <div class="font-display text-sm font-semibold text-espresso mb-2"><span class="text-en">Step 4</span><span class="text-am">ደረ 4</span></div>
            <h3 class="font-display text-xl font-semibold text-espresso mb-3"><span class="text-en">Receive</span><span class="text-am">ተቀበሉ</span></h3>
            <p class="text-espresso/60"><span class="text-en">Track gifts and contributions in one simple dashboard.</span><span class="text-am">ስጦታችን እና አስተዋፅኦችን በአንድ ቀላል ዳሽቦርድ ይከታተሉ።</span></p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- ========== OCCASIONS ========== -->
  <section id="occasions" class="py-24 lg:py-32 bg-gradient-to-b from-ivory to-ivory-dark relative overflow-hidden">
    <div class="absolute inset-0 ethiopian-pattern opacity-20" aria-hidden="true"></div>
    <div class="relative max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center mb-16">
        <div class="inline-flex items-center gap-2 px-4 py-2 bg-terracotta/10 rounded-full text-terracotta text-sm font-semibold mb-4 reveal">
          <span class="text-en">For Every Moment</span>
          <span class="text-am">ለሁሉም ጊዜ</span>
        </div>
        <h2 class="reveal font-display text-4xl sm:text-5xl font-semibold text-espresso">
          <span class="text-en">Made for every celebration</span>
          <span class="text-am">ለሁሉም ክብረ በዓል የተሰራ</span>
        </h2>
        <p class="reveal reveal-delay-1 mt-4 text-lg text-espresso/60 max-w-2xl mx-auto">
          <span class="text-en">From weddings and births to birthdays, graduations, and housewarmings — collect the gifts and support that matter most.</span>
          <span class="text-am">ከሰርግና ልደት እስከ ልደት በዓል፣ ምረቃና አዲስ ቤት — የሚያስፈልጉትን ስጦታዎችና ድጋፍ ሰብስቡ።</span>
        </p>
      </div>
      <div class="grid sm:grid-cols-2 lg:grid-cols-3 gap-6">
        <!-- Wedding -->
        <a href="#" onclick="openModal('createModal'); return false;" class="reveal reveal-delay-1 occasion-card group">
          <div class="w-14 h-14 bg-gradient-to-br from-terracotta/10 to-gold/10 rounded-2xl flex items-center justify-center mb-4 group-hover:scale-110 transition-transform">
            <svg width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="#C45D3E" stroke-width="2"><path d="M20.84 4.61a5.5 5.5 0 0 0-7.78 0L12 5.67l-1.06-1.06a5.5 5.5 0 0 0-7.78 7.78l1.06 1.06L12 21.23l7.78-7.78 1.06-1.06a5.5 5.5 0 0 0 0-7.78z"/></svg>
          </div>
          <h3 class="font-display text-xl font-semibold text-espresso mb-2"><span class="text-en">Wedding Registry</span><span class="text-am">የሰርግ ዝርዝር</span></h3>
          <p class="text-espresso/60 text-sm"><span class="text-en">Create a list for your new chapter — from home essentials to honeymoon support.</span><span class="text-am">ለአዲሱ ምዕራፍ ዝርዝር ይፍሩ — ከቤት እቃዎች እስከ ማር ጋፍ</span></p>
        </a>
        <!-- Baby -->
        <a href="#" onclick="openModal('createModal'); return false;" class="reveal reveal-delay-2 occasion-card group">
          <div class="w-14 h-14 bg-gradient-to-br from-gold/10 to-cream rounded-2xl flex items-center justify-center mb-4 group-hover:scale-110 transition-transform">
            <svg width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="#D4A574" stroke-width="2"><circle cx="12" cy="12" r="10"/><path d="M8 14s1.5 2 4 2 4-2 4-2"/><line x1="9" y1="9" x2="9.01" y2="9"/><line x1="15" y1="9" x2="15.01" y2="9"/></svg>
          </div>
          <h3 class="font-display text-xl font-semibold text-espresso mb-2"><span class="text-en">Baby Registry</span><span class="text-am">የልጅ ዝርዝር</span></h3>
          <p class="text-espresso/60 text-sm"><span class="text-en">Collect the items and support you need before and after your baby arrives.</span><span class="text-am">ልጅዎ መወለዱ በፊትና በኋላ የሚያስፈልትን እቃዎች ይሰብስቡ።</span></p>
        </a>
        <!-- Birthday -->
        <a href="#" onclick="openModal('createModal'); return false;" class="reveal reveal-delay-3 occasion-card group">
          <div class="w-14 h-14 bg-gradient-to-br from-sage/10 to-sage/5 rounded-2xl flex items-center justify-center mb-4 group-hover:scale-110 transition-transform">
            <svg width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="#8B9A7D" stroke-width="2"><path d="M8 2v4"/><path d="M16 2v4"/><path d="M21 13V8a2 2 0 0 0-2-2H5a2 2 0 0 0-2 2v6"/></svg>
          </div>
          <h3 class="font-display text-xl font-semibold text-espresso mb-2"><span class="text-en">Birthday Wishlist</span><span class="text-am">የልደት በዓል ምር</span></h3>
          <p class="text-espresso/60 text-sm"><span class="text-en">Make birthdays easier with a shareable wishlist your friends and family can actually use.</span><span class="text-am">ልደት በዓልን ቀላል ያድርጉት — ጓደኞችና ቤተሰብ የሚጠቀሙበት ዝርዝር ያጋሩ።</span></p>
        </a>
        <!-- Graduation -->
        <a href="#" onclick="openModal('createModal'); return false;" class="reveal reveal-delay-4 occasion-card group">
          <div class="w-14 h-14 bg-gradient-to-br from-espresso/10 to-espresso/5 rounded-2xl flex items-center justify-center mb-4 group-hover:scale-110 transition-transform">
            <svg width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="#2C1810" stroke-width="2"><path d="M22 10v6M2 10l10-5 10 5-10 5z"/><path d="M6 12v5c3 3 9 3 12 0v-5"/></svg>
          </div>
          <h3 class="font-display text-xl font-semibold text-espresso mb-2"><span class="text-en">Graduation List</span><span class="text-am">የምረቃ ዝርዝር</span></h3>
          <p class="text-espresso/60 text-sm"><span class="text-en">Celebrate achievement with gifts, tools, and support for the next step.</span><span class="text-am">ስኬትን በስጦታዎች፣ በመሳሪያዎችና በድጋፍ ያክሩ።</span></p>
        </a>
        <!-- Housewarming -->
        <a href="#" onclick="openModal('createModal'); return false;" class="reveal reveal-delay-5 occasion-card group">
          <div class="w-14 h-14 bg-gradient-to-br from-terracotta/10 to-sage/10 rounded-2xl flex items-center justify-center mb-4 group-hover:scale-110 transition-transform">
            <svg width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="#C45D3E" stroke-width="2"><path d="M3 9l9-7 9 7v11a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2z"/><polyline points="9 22 9 12 15 12 15 22"/></svg>
          </div>
          <h3 class="font-display text-xl font-semibold text-espresso mb-2"><span class="text-en">Housewarming</span><span class="text-am">አዲስ ቤት</span></h3>
          <p class="text-espresso/60 text-sm"><span class="text-en">Build your new space with thoughtful gifts and contributions from loved ones.</span><span class="text-am">አዲሱን ቤትዎን ከወጆችና ከቤተሰብ ጦታች ጋር ገንቡ</span></p>
        </a>
        <!-- Group Contribution -->
        <a href="#" onclick="openModal('createModal'); return false;" class="reveal reveal-delay-6 occasion-card group">
          <div class="w-14 h-14 bg-gradient-to-br from-gold/20 to-terracotta/10 rounded-2xl flex items-center justify-center mb-4 group-hover:scale-110 transition-transform">
            <svg width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="#D4A574" stroke-width="2"><path d="M17 21v-2a4 4 0 0 0-4-4H5a4 4 0 0 0-4 4v2"/><circle cx="9" cy="7" r="4"/><path d="M23 21v-2a4 4 0 0 0-3-3.87"/><path d="M16 3.13a4 4 0 0 1 0 7.75"/></svg>
          </div>
          <h3 class="font-display text-xl font-semibold text-espresso mb-2"><span class="text-en">Group Contribution</span><span class="text-am">የቡድን አስተዋፅኦ</span></h3>
          <p class="text-espresso/60 text-sm"><span class="text-en">Create a shared goal — a trip, project fund, gift pool, or personal milestone.</span><span class="text-am">የጋራ ግብ ፍጠ — ጉዞ ፕሮክት ፈንድ፣ የስታ ፑል ወይም ግላዊ ኬት</span></p>
        </a>
      </div>
    </div>
  </section>

  <!-- ========== ADD ANYTHING SECTION ========== -->
  <section class="py-24 lg:py-32 relative">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center mb-16">
        <div class="inline-flex items-center gap-2 px-4 py-2 bg-terracotta/10 rounded-full text-terracotta text-sm font-semibold mb-4 reveal">
          <span class="text-en">Add Anything</span>
          <span class="text-am">ማንኛውንም ያክሉ</span>
        </div>
        <h2 class="reveal font-display text-4xl sm:text-5xl font-semibold text-espresso">
          <span class="text-en">Not tied to one store. Not limited to one idea.</span>
          <span class="text-am">ለአንድ ሱቅ አይገደቡ ለአንድ ሀሳብ አይወሰኑ።</span>
        </h2>
        <p class="reveal reveal-delay-1 mt-4 text-lg text-espresso/60 max-w-2xl mx-auto">
          <span class="text-en">Add products, cash contributions, shared goals, or even meaningful experiences. Your list should reflect your life, not someone else's catalog.</span>
          <span class="text-am">ምርቶችን፣ የንዘብ አስተዋፅኦ የጋራ ግቦች ይም ትርም ያላቸው ልምዶች ያክሉ።</span>
        </p>
      </div>

      <div class="grid md:grid-cols-3 gap-8">
        <div class="reveal reveal-delay-1 feature-card text-center">
          <div class="w-16 h-16 mx-auto bg-terracotta/10 rounded-2xl flex items-center justify-center mb-4">
            <svg width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="#C45D3E" stroke-width="2"><circle cx="9" cy="21" r="1"/><circle cx="20" cy="21" r="1"/><path d="M1 1h4l2.68 13.39a2 2 0 0 0 2 1.61h9.72a2 2 0 0 0 2-1.61L23 6H6"/></svg>
          </div>
          <h3 class="font-display text-xl font-semibold text-espresso mb-2"><span class="text-en">Add Gifts from Any Store</span><span class="text-am">ከማንኛውም ሱቅ ስጦታ ያሉ</span></h3>
          <p class="text-espresso/60 text-sm"><span class="text-en">Paste a product link or add custom items. No store restrictions.</span><span class="text-am">የምርት ሊን ይለፉ ወይም ብጁ ቃዎች ያክሉ።</span></p>
        </div>
        <div class="reveal reveal-delay-2 feature-card text-center">
          <div class="w-16 h-16 mx-auto bg-gold/10 rounded-2xl flex items-center justify-center mb-4">
            <svg width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="#D4A574" stroke-width="2"><path d="M12 2v20M17 5H9.5a3.5 3.5 0 0 0 0 7h5a3.5 3.5 0 0 1 0 7H6"/></svg>
          </div>
          <h3 class="font-display text-xl font-semibold text-espresso mb-2"><span class="text-en">Cash Goals & Contributions</span><span class="text-am">የገንዘብ ግቦችና አስተዋፅኦ</span></h3>
          <p class="text-espresso/60 text-sm"><span class="text-en">Set funding goals for weddings, travel, education, or any project.</span><span class="text-am">ለሰርግ፣ ዞ፣ ትምህርት ወይም ማንኛውም ፕሮጀክት የገንዘብ ግብ ያስቀምጡ</span></p>
        </div>
        <div class="reveal reveal-delay-3 feature-card text-center">
          <div class="w-16 h-16 mx-auto bg-sage/10 rounded-2xl flex items-center justify-center mb-4">
            <svg width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="#8B9A7D" stroke-width="2"><path d="M20.84 4.61a5.5 5.5 0 0 0-7.78 0L12 5.67l-1.06-1.06a5.5 5.5 0 0 0-7.78 7.78l1.06 1.06L12 21.23l7.78-7.78 1.06-1.06a5.5 5.5 0 0 0 0-7.78z"/></svg>
          </div>
          <h3 class="font-display text-xl font-semibold text-espresso mb-2"><span class="text-en">Custom Ideas & Experiences</span><span class="text-am">ብጁ ሳቦችና ምዶች</span></h3>
          <p class="text-espresso/60 text-sm"><span class="text-en">Add experiences, services, or anything that matters to you.</span><span class="text-am">ልምዶችን አገልግሎቶችን ወይም ለእርስዎ ጠቃሚ ማንኛውንም ነገር ያክሉ</span></p>
        </div>
      </div>
    </div>
  </section>

  <!-- ========== BUILT FOR ETHIOPIA ========== -->
  <section class="py-24 lg:py-32 bg-gradient-to-b from-ivory to-ivory-dark relative overflow-hidden">
    <div class="absolute inset-0 ethiopian-pattern opacity-20" aria-hidden="true"></div>
    <div class="relative max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center mb-16">
        <div class="inline-flex items-center gap-2 px-4 py-2 bg-terracotta/10 rounded-full text-terracotta text-sm font-semibold mb-4 reveal">
          <span class="text-en">Built for Ethiopia</span>
          <span class="text-am">ለኢትዮጵያ የተሰራ</span>
        </div>
        <h2 class="reveal font-display text-4xl sm:text-5xl font-semibold text-espresso">
          <span class="text-en">Designed for how Ethiopia gives</span>
          <span class="text-am">ለኢትዮጵያ አቀራረብ የተሰራ</span>
        </h2>
        <p class="reveal reveal-delay-1 mt-4 text-lg text-espresso/60 max-w-2xl mx-auto">
          <span class="text-en">Built for mobile, local payments, and modern sharing. Easy for loved ones in Ethiopia — and easy for supporters abroad too.</span>
          <span class="text-am">ለሞባይል፣ ለአባቢያዊ ክፍያዎችና ለዘመና ማጋት የተሰ።</span>
        </p>
      </div>

      <div class="grid sm:grid-cols-2 lg:grid-cols-5 gap-6">
        <div class="reveal reveal-delay-1 feature-card text-center">
          <div class="w-12 h-12 mx-auto bg-green-50 rounded-xl flex items-center justify-center mb-3">
            <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#10B981" stroke-width="2"><rect x="2" y="4" width="20" height="16" rx="2"/><path d="M12 14h.01"/><path d="M2 10h20"/></svg>
          </div>
          <h3 class="font-semibold text-espresso mb-1 text-sm"><span class="text-en">telebirr</span><span class="text-am">ቴሌብር</span></h3>
          <p class="text-espresso/50 text-xs"><span class="text-en">Mobile payments</span><span class="text-am">ሞባይል ክፍያ</span></p>
        </div>
        <div class="reveal reveal-delay-2 feature-card text-center">
          <div class="w-12 h-12 mx-auto bg-blue-50 rounded-xl flex items-center justify-center mb-3">
            <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#3B82F6" stroke-width="2"><path d="M3 3h18v18H3zM12 8v8M8 12h8"/></svg>
          </div>
          <h3 class="font-semibold text-espresso mb-1 text-sm"><span class="text-en">CBE Birr</span><span class="text-am">ንግድ ብር</span></h3>
          <p class="text-espresso/50 text-xs"><span class="text-en">Bank mobile</span><span class="text-am">ባንክ ሞባይል</span></p>
        </div>
        <div class="reveal reveal-delay-3 feature-card text-center">
          <div class="w-12 h-12 mx-auto bg-amber-50 rounded-xl flex items-center justify-center mb-3">
            <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#F59E0B" stroke-width="2"><path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"/></svg>
          </div>
          <h3 class="font-semibold text-espresso mb-1 text-sm"><span class="text-en">Bank Transfer</span><span class="text-am">የባንክ ዝውውር</span></h3>
          <p class="text-espresso/50 text-xs"><span class="text-en">Direct deposit</span><span class="text-am">ቀጥተኛ ተቀማጭ</span></p>
        </div>
        <div class="reveal reveal-delay-4 feature-card text-center">
          <div class="w-12 h-12 mx-auto bg-purple-50 rounded-xl flex items-center justify-center mb-3">
            <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#8B5CF6" stroke-width="2"><circle cx="12" cy="12" r="10"/><line x1="2" y1="12" x2="22" y2="12"/><path d="M12 2a15.3 15.3 0 0 1 4 10 15.3 15.3 0 0 1-4 10 15.3 15.3 0 0 1-4-10 15.3 15.3 0 0 1 4-10z"/></svg>
          </div>
          <h3 class="font-semibold text-espresso mb-1 text-sm"><span class="text-en">Diaspora Support</span><span class="text-am">ዲያስራ ድፍ</span></h3>
          <p class="text-espresso/50 text-xs"><span class="text-en">International</span><span class="text-am">ዓለም አቀፍ</span></p>
        </div>
        <div class="reveal reveal-delay-5 feature-card text-center">
          <div class="w-12 h-12 mx-auto bg-red-50 rounded-xl flex items-center justify-center mb-3">
            <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#EF4444" stroke-width="2"><path d="M4 11a9 9 0 0 1 9 9"/><path d="M4 4a16 16 0 0 1 16 16"/><circle cx="5" cy="19" r="1"/></svg>
          </div>
          <h3 class="font-semibold text-espresso mb-1 text-sm"><span class="text-en">ETB Pricing</span><span class="text-am">ብር ዋጋ</span></h3>
          <p class="text-espresso/50 text-xs"><span class="text-en">Local currency</span><span class="text-am">የአካባቢ ገንዘብ</span></p>
        </div>
      </div>
    </div>
  </section>

  <!-- ========== DASHBOARD PREVIEW ========== -->
  <section class="py-24 lg:py-32 relative">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="grid lg:grid-cols-2 gap-12 items-center">
        <div class="reveal">
          <div class="inline-flex items-center gap-2 px-4 py-2 bg-terracotta/10 rounded-full text-terracotta text-sm font-semibold mb-4">
            <span class="text-en">Your Dashboard</span>
            <span class="text-am">ዳሽቦርድዎ</span>
          </div>
          <h2 class="font-display text-4xl sm:text-5xl font-semibold text-espresso mb-4">
            <span class="text-en">Everything in one place</span>
            <span class="text-am">ሁሉም ነገር በአንድ ቦታ</span>
          </h2>
          <p class="text-espresso/60 text-lg mb-8">
            <span class="text-en">Track contributions, manage gifts, send thank-you notes, and share your list — all from a beautiful, simple dashboard.</span>
            <span class="text-am">አስተዋፅኦዎችን ከታተሉ፣ ስታዎችን ስተዳድሩ፣ የምስጋና መልዕክች ይላ፣ ዝርዝርዎን ያጋሩ</span>
          </p>
          <div class="space-y-4">
            <div class="flex items-center gap-3">
              <div class="w-8 h-8 bg-terracotta/10 rounded-lg flex items-center justify-center flex-shrink-0">
                <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="#C45D3E" stroke-width="2"><polyline points="20 6 9 17 4 12"/></svg>
              </div>
              <span class="text-espresso/70"><span class="text-en">Real-time contribution tracking</span><span class="text-am">በቀጥታ አስተዋፅኦ ትትል</span></span>
            </div>
            <div class="flex items-center gap-3">
              <div class="w-8 h-8 bg-terracotta/10 rounded-lg flex items-center justify-center flex-shrink-0">
                <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="#C45D3E" stroke-width="2"><polyline points="20 6 9 17 4 12"/></svg>
              </div>
              <span class="text-espresso/70"><span class="text-en">Gift reservation management</span><span class="text-am">የስጦታ ሪዘርቬሽን አስተዳደር</span></span>
            </div>
            <div class="flex items-center gap-3">
              <div class="w-8 h-8 bg-terracotta/10 rounded-lg flex items-center justify-center flex-shrink-0">
                <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="#C45D3E" stroke-width="2"><polyline points="20 6 9 17 4 12"/></svg>
              </div>
              <span class="text-espresso/70"><span class="text-en">WhatsApp & Telegram sharing</span><span class="text-am">WhatsApp & Telegram ማጋራት</span></span>
            </div>
            <div class="flex items-center gap-3">
              <div class="w-8 h-8 bg-terracotta/10 rounded-lg flex items-center justify-center flex-shrink-0">
                <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="#C45D3E" stroke-width="2"><polyline points="20 6 9 17 4 12"/></svg>
              </div>
              <span class="text-espresso/70"><span class="text-en">Thank-you messages & guest list</span><span class="text-am">የምስጋና መልዕክቶችና የእንግዶች ዝርዝር</span></span>
            </div>
            <div class="flex items-center gap-3">
              <div class="w-8 h-8 bg-terracotta/10 rounded-lg flex items-center justify-center flex-shrink-0">
                <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="#C45D3E" stroke-width="2"><polyline points="20 6 9 17 4 12"/></svg>
              </div>
              <span class="text-espresso/70"><span class="text-en">Payout to your bank or mobile wallet</span><span class="text-am">ወደ ንክ ወይም ሞባይል ዋሌት ክፍያ</span></span>
            </div>
          </div>
          <div class="mt-8">
            <button onclick="openModal('signupModal')" class="btn-primary">
              <span class="text-en">Get Started Free</span>
              <span class="text-am">ነጻ ይጀምሩ</span>
            </button>
          </div>
        </div>

        <div class="reveal reveal-delay-2">
          <div class="dashboard-preview">
            <div class="flex items-center justify-between mb-6">
              <div>
                <h3 class="font-display text-lg font-semibold">Abebe & Sara's Wedding</h3>
                <p class="text-white/50 text-sm">June 15, 2026 · Addis Ababa</p>
              </div>
              <button onclick="openModal('shareModal')" class="px-3 py-1.5 bg-white/10 rounded-lg text-sm hover:bg-white/20 transition-colors">
                <span class="text-en">Share</span>
              </button>
            </div>
            <div class="grid grid-cols-2 gap-4 mb-6">
              <div class="bg-white/10 rounded-xl p-4">
                <p class="text-white/50 text-xs mb-1"><span class="text-en">Total Received</span><span class="text-am">ጠቅላ</span></p>
                <p class="text-2xl font-bold">45,200 <span class="text-sm font-normal text-white/50">ETB</span></p>
              </div>
              <div class="bg-white/10 rounded-xl p-4">
                <p class="text-white/50 text-xs mb-1"><span class="text-en">Goal Progress</span><span class="text-am">የግብ ሂደት</span></p>
                <p class="text-2xl font-bold">75%</p>
              </div>
              <div class="bg-white/10 rounded-xl p-4">
                <p class="text-white/50 text-xs mb-1"><span class="text-en">Gifts Reserved</span><span class="text-am">የተያዙ ጦታች</span></p>
                <p class="text-2xl font-bold">12</p>
              </div>
              <div class="bg-white/10 rounded-xl p-4">
                <p class="text-white/50 text-xs mb-1"><span class="text-en">Contributors</span><span class="text-am">አስተዋጽኦ አድራጊዎች</span></p>
                <p class="text-2xl font-bold">28</p>
              </div>
            </div>
            <div class="bg-white/5 rounded-xl p-4">
              <p class="text-white/50 text-xs mb-3"><span class="text-en">Recent Activity</span><span class="text-am">የቅርብ ጊዜ</span></p>
              <div class="space-y-3">
                <div class="flex items-center justify-between text-sm">
                  <div class="flex items-center gap-2">
                    <div class="w-8 h-8 bg-green-500/20 rounded-full flex items-center justify-center text-green-400 text-xs font-bold">T</div>
                    <span>Tigist contributed</span>
                  </div>
                  <span class="font-semibold">2,000 ETB</span>
                </div>
                <div class="flex items-center justify-between text-sm">
                  <div class="flex items-center gap-2">
                    <div class="w-8 h-8 bg-blue-500/20 rounded-full flex items-center justify-center text-blue-400 text-xs font-bold">D</div>
                    <span>Daniel reserved a gift</span>
                  </div>
                  <span class="text-white/50">Coffee Set</span>
                </div>
                <div class="flex items-center justify-between text-sm">
                  <div class="flex items-center gap-2">
                    <div class="w-8 h-8 bg-purple-500/20 rounded-full flex items-center justify-center text-purple-400 text-xs font-bold">M</div>
                    <span>Meron contributed</span>
                  </div>
                  <span class="font-semibold">1,500 ETB</span>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- ========== TESTIMONIALS ========== -->
  <section class="py-24 lg:py-32 bg-gradient-to-b from-ivory to-ivory-dark relative">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center mb-16">
        <div class="inline-flex items-center gap-2 px-4 py-2 bg-terracotta/10 rounded-full text-terracotta text-sm font-semibold mb-4 reveal">
          <span class="text-en">Testimonials</span>
          <span class="text-am">ምስክርነቶች</span>
        </div>
        <h2 class="reveal font-display text-4xl sm:text-5xl font-semibold text-espresso">
          <span class="text-en">Loved by Ethiopian families</span>
          <span class="text-am">የኢትዮጵያ ቤተሰቦች ደዱት</span>
        </h2>
      </div>

      <div class="grid md:grid-cols-3 gap-8">
        <div class="reveal reveal-delay-1 testimonial-card">
          <div class="flex items-center gap-1 mb-3">
            <svg width="16" height="16" viewBox="0 0 24 24" fill="#F59E0B"><path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01L12 2z"/></svg>
            <svg width="16" height="16" viewBox="0 0 24 24" fill="#F59E0B"><path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01L12 2z"/></svg>
            <svg width="16" height="16" viewBox="0 0 24 24" fill="#F59E0B"><path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01L12 2z"/></svg>
            <svg width="16" height="16" viewBox="0 0 24 24" fill="#F59E0B"><path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01L12 2z"/></svg>
            <svg width="16" height="16" viewBox="0 0 24 24" fill="#F59E0B"><path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01L12 2z"/></svg>
          </div>
          <p class="text-espresso/70 mb-4 text-sm">"Bene'nw made our wedding registry so easy. Family from Addis and diaspora relatives all contributed through one link. The telebirr integration was seamless!"</p>
          <div class="flex items-center gap-3">
            <div class="w-10 h-10 bg-terracotta/10 rounded-full flex items-center justify-center text-terracotta font-bold">SA</div>
            <div>
              <p class="font-semibold text-sm text-espresso">Sara & Abebe</p>
              <p class="text-xs text-muted">Wedding · Addis Ababa</p>
            </div>
          </div>
        </div>
        <div class="reveal reveal-delay-2 testimonial-card">
          <div class="flex items-center gap-1 mb-3">
            <svg width="16" height="16" viewBox="0 0 24 24" fill="#F59E0B"><path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01L12 2z"/></svg>
            <svg width="16" height="16" viewBox="0 0 24 24" fill="#F59E0B"><path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01L12 2z"/></svg>
            <svg width="16" height="16" viewBox="0 0 24 24" fill="#F59E0B"><path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01L12 2z"/></svg>
            <svg width="16" height="16" viewBox="0 0 24 24" fill="#F59E0B"><path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01L12 2z"/></svg>
            <svg width="16" height="16" viewBox="0 0 24 24" fill="#F59E0B"><path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01L12 2z"/></svg>
          </div>
          <p class="text-espresso/70 mb-4 text-sm">"We used it for our baby shower and it was beautiful. Everyone could contribute towards the items we actually needed. The QR code on our invitation was genius!"</p>
          <div class="flex items-center gap-3">
            <div class="w-10 h-10 bg-gold/10 rounded-full flex items-center justify-center text-gold-dark font-bold">FT</div>
            <div>
              <p class="font-semibold text-sm text-espresso">Fikadu & Tsion</p>
              <p class="text-xs text-muted">Baby Registry · Bahir Dar</p>
            </div>
          </div>
        </div>
        <div class="reveal reveal-delay-3 testimonial-card">
          <div class="flex items-center gap-1 mb-3">
            <svg width="16" height="16" viewBox="0 0 24 24" fill="#F59E0B"><path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01L12 2z"/></svg>
            <svg width="16" height="16" viewBox="0 0 24 24" fill="#F59E0B"><path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01L12 2z"/></svg>
            <svg width="16" height="16" viewBox="0 0 24 24" fill="#F59E0B"><path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01L12 2z"/></svg>
            <svg width="16" height="16" viewBox="0 0 24 24" fill="#F59E0B"><path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01L12 2z"/></svg>
            <svg width="16" height="16" viewBox="0 0 24 24" fill="#F59E0B"><path d="M12 2l3.09 6.26L22 9.27l-5 4.87 1.18 6.88L12 17.77l-6.18 3.25L7 14.14 2 9.27l6.91-1.01L12 2z"/></svg>
          </div>
          <p class="text-espresso/70 mb-4 text-sm">"I contributed from the US to my friend's graduation fund. The international payment worked perfectly. This platform is exactly what Ethiopia needed."</p>
          <div class="flex items-center gap-3">
            <div class="w-10 h-10 bg-sage/10 rounded-full flex items-center justify-center text-sage font-bold">DH</div>
            <div>
              <p class="font-semibold text-sm text-espresso">Daniel H.</p>
              <p class="text-xs text-muted">Contributor · Washington DC</p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- ========== FOR VENDORS ========== -->
  <section class="py-24 lg:py-32 relative">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="grid lg:grid-cols-2 gap-12 items-center">
        <div class="reveal">
          <div class="inline-flex items-center gap-2 px-4 py-2 bg-gold/10 rounded-full text-gold-dark text-sm font-semibold mb-4">
            <span class="text-en">For Vendors & Shops</span>
            <span class="text-am">ለሻጮችና ሱቆች</span>
          </div>
          <h2 class="font-display text-4xl sm:text-5xl font-semibold text-espresso mb-4">
            <span class="text-en">Grow your business with Bene'nw</span>
            <span class="text-am">ንግድን ከBene'nw ጋር ያሳድጉ</span>
          </h2>
          <p class="text-espresso/60 text-lg mb-8">
            <span class="text-en">List your products on Bene'nw and reach thousands of Ethiopian families creating gift registries. Simple onboarding, no technical skills needed.</span>
            <span class="text-am">ምርቶችዎን በBene'nw ይዘርዝሩ እና ሺዎች የኢትዮጵያ ተሰቦችን ይድረሱ። ቀላል ምዝገባ።</span>
          </p>
          <div class="space-y-3 mb-8">
            <div class="flex items-center gap-3">
              <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="#C45D3E" stroke-width="2"><polyline points="20 6 9 17 4 12"/></svg>
              <span class="text-espresso/70"><span class="text-en">Reach engaged couples & families</span><span class="text-am">ሰር እና ቤተቦችን ይረሱ</span></span>
            </div>
            <div class="flex items-center gap-3">
              <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="#C45D3E" stroke-width="2"><polyline points="20 6 9 17 4 12"/></svg>
              <span class="text-espresso/70"><span class="text-en">Simple product listing dashboard</span><span class="text-am">ቀላል የምርት ዝርዝር ዳሽቦርድ</span></span>
            </div>
            <div class="flex items-center gap-3">
              <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="#C45D3E" stroke-width="2"><polyline points="20 6 9 17 4 12"/></svg>
              <span class="text-espresso/70"><span class="text-en">No upfront costs</span><span class="text-am">ቅድመ ክፍያ የለም</span></span>
            </div>
          </div>
          <button onclick="openModal('contactModal')" class="btn-secondary">
            <span class="text-en">Register as Vendor</span>
            <span class="text-am">እንደ ጭ ይመዝገቡ</span>
          </button>
        </div>

        <div class="reveal reveal-delay-2">
          <div class="bg-white rounded-2xl border border-border p-8 shadow-lg">
            <div class="text-center mb-6">
              <div class="w-16 h-16 mx-auto bg-gold/10 rounded-2xl flex items-center justify-center mb-4">
                <svg width="32" height="32" viewBox="0 0 24 24" fill="none" stroke="#D4A574" stroke-width="2"><path d="M6 2L3 6v14a2 2 0 0 0 2 2h14a2 2 0 0 0 2-2V6l-3-4z"/><line x1="3" y1="6" x2="21" y2="6"/><path d="M16 10a4 4 0 0 1-8 0"/></svg>
              </div>
              <h3 class="font-display text-xl font-semibold text-espresso"><span class="text-en">Vendor Benefits</span><span class="text-am">የሻጭ ጥቅሞች</span></h3>
            </div>
            <div class="space-y-4">
              <div class="flex items-start gap-3 p-3 bg-ivory rounded-xl">
                <span class="text-2xl">📦</span>
                <div>
                  <p class="font-semibold text-sm text-espresso"><span class="text-en">Product Visibility</span><span class="text-am">የምርት ታይነት</span></p>
                  <p class="text-xs text-muted"><span class="text-en">Your products appear in relevant gift lists</span><span class="text-am">ምርቶችዎ በተገቢ የስጦታ ዝርዝሮች ውስጥ ይታያሉ</span></p>
                </div>
              </div>
              <div class="flex items-start gap-3 p-3 bg-ivory rounded-xl">
                <span class="text-2xl">📊</span>
                <div>
                  <p class="font-semibold text-sm text-espresso"><span class="text-en">Sales Analytics</span><span class="text-am">የሽያጭ ንተና</span></p>
                  <p class="text-xs text-muted"><span class="text-en">Track which products are most popular</span><span class="text-am">ትልቅ ተወዳጅ የሆኑ ምርቶችን ይከታተሉ</span></p>
                </div>
              </div>
              <div class="flex items-start gap-3 p-3 bg-ivory rounded-xl">
                <span class="text-2xl">🤝</span>
                <div>
                  <p class="font-semibold text-sm text-espresso"><span class="text-en">Direct Customer Connection</span><span class="text-am">ቀጥተኛ ደንበ ግንኙነት</span></p>
                  <p class="text-xs text-muted"><span class="text-en">Connect with customers planning events</span><span class="text-am">ክስተቶችን ከሚያቅዱ ደንበኞች ጋር ይገናኙ</span></p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- ========== TRUST & SECURITY ========== -->
  <section class="py-24 lg:py-32 bg-gradient-to-b from-ivory to-ivory-dark relative overflow-hidden">
    <div class="absolute inset-0 ethiopian-pattern opacity-20" aria-hidden="true"></div>
    <div class="relative max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center mb-16">
        <div class="inline-flex items-center gap-2 px-4 py-2 bg-sage/10 rounded-full text-sage text-sm font-semibold mb-4 reveal">
          <span class="text-en">Trust & Security</span>
          <span class="text-am">ታማኝነትና ደህንነት</span>
        </div>
        <h2 class="reveal font-display text-4xl sm:text-5xl font-semibold text-espresso">
          <span class="text-en">Designed with trust in mind</span>
          <span class="text-am">ከታማኝነት ጋር የተሰራ</span>
        </h2>
        <p class="reveal reveal-delay-1 mt-4 text-lg text-espresso/60 max-w-2xl mx-auto">
          <span class="text-en">From payment protection to privacy settings and clear payout records, every part of the platform helps users feel secure.</span>
          <span class="text-am">ከክፍያ ጥበቃ እስከ የግላዊነት ቅንብሮችና ግል የክያ መዝቦች።</span>
        </p>
      </div>

      <div class="grid sm:grid-cols-2 lg:grid-cols-4 gap-6">
        <div class="reveal reveal-delay-1 feature-card text-center">
          <div class="w-14 h-14 mx-auto bg-green-50 rounded-2xl flex items-center justify-center mb-4">
            <svg width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="#10B981" stroke-width="2"><path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"/></svg>
          </div>
          <h3 class="font-semibold text-espresso mb-1"><span class="text-en">Secure Payments</span><span class="text-am">ደህንነቱ የተጠበቀ ክፍያ</span></h3>
          <p class="text-espresso/60 text-sm"><span class="text-en">Bank-grade encryption on all transactions</span><span class="text-am">በሁሉም ግብይቶች የባንክ ደረጃ ስጠራ</span></p>
        </div>
        <div class="reveal reveal-delay-2 feature-card text-center">
          <div class="w-14 h-14 mx-auto bg-blue-50 rounded-2xl flex items-center justify-center mb-4">
            <svg width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="#3B82F6" stroke-width="2"><path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"/><polyline points="22 4 12 14.01 9 11.01"/></svg>
          </div>
          <h3 class="font-semibold text-espresso mb-1"><span class="text-en">Verified Payouts</span><span class="text-am">የተረጋገጠ ክፍያ</span></h3>
          <p class="text-espresso/60 text-sm"><span class="text-en">Clear payout records and timeline</span><span class="text-am">ግል የክያ መዝቦችና ጊዜ</span></p>
        </div>
        <div class="reveal reveal-delay-3 feature-card text-center">
          <div class="w-14 h-14 mx-auto bg-purple-50 rounded-2xl flex items-center justify-center mb-4">
            <svg width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="#8B5CF6" stroke-width="2"><rect x="3" y="11" width="18" height="11" rx="2" ry="2"/><path d="M7 11V7a5 5 0 0 1 10 0v4"/></svg>
          </div>
          <h3 class="font-semibold text-espresso mb-1"><span class="text-en">Privacy Controls</span><span class="text-am">የግላነት ቁጥጥሮች</span></h3>
          <p class="text-espresso/60 text-sm"><span class="text-en">You control who sees your list</span><span class="text-am">ዝርዝርዎን ማን እንደሚያይ ይቆጣጠሩ</span></p>
        </div>
        <div class="reveal reveal-delay-4 feature-card text-center">
          <div class="w-14 h-14 mx-auto bg-amber-50 rounded-2xl flex items-center justify-center mb-4">
            <svg width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="#F59E0B" stroke-width="2"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/><polyline points="14 2 14 8 20 8"/><line x1="16" y1="13" x2="8" y2="13"/><line x1="16" y1="17" x2="8" y2="17"/></svg>
          </div>
          <h3 class="font-semibold text-espresso mb-1"><span class="text-en">Transparent Fees</span><span class="text-am">ግልጽ ክፍያዎች</span></h3>
          <p class="text-espresso/60 text-sm"><span class="text-en">No hidden charges, ever</span><span class="text-am">ድብቅ ክፍያች በፍጹም የሉም</span></p>
        </div>
      </div>
    </div>
  </section>

  <!-- ========== PRICING ========== -->
  <section id="pricing" class="py-24 lg:py-32 relative">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center mb-16">
        <div class="inline-flex items-center gap-2 px-4 py-2 bg-terracotta/10 rounded-full text-terracotta text-sm font-semibold mb-4 reveal">
          <span class="text-en">Pricing</span>
          <span class="text-am">ዋጋ</span>
        </div>
        <h2 class="reveal font-display text-4xl sm:text-5xl font-semibold text-espresso">
          <span class="text-en">Start free. Grow with you.</span>
          <span class="text-am">ነጻ ይጀምሩ። አረን እናድጋለን።</span>
        </h2>
      </div>
      <div class="grid md:grid-cols-3 gap-8 max-w-5xl mx-auto">
        <!-- Free -->
        <div class="reveal reveal-delay-1 pricing-card bg-white rounded-2xl p-8 border border-border hover:border-terracotta/30 transition-colors">
          <h3 class="font-display text-xl font-semibold text-espresso mb-2"><span class="text-en">Free</span><span class="text-am">ነጻ</span></h3>
          <p class="text-muted text-sm mb-6"><span class="text-en">Perfect for personal use</span><span class="text-am">ለግል አቃቀም</span></p>
          <div class="font-display text-4xl font-bold text-espresso mb-6">0 <span class="text-lg font-normal text-muted">ETB</span></div>
          <ul class="space-y-3 mb-8">
            <li class="flex items-center gap-2 text-sm text-espresso/70">
              <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="#C45D3E" stroke-width="2"><polyline points="20 6 9 17 4 12"/></svg>
              <span class="text-en">1 active list</span><span class="text-am">1 ንቁ ዝርዝር</span>
            </li>
            <li class="flex items-center gap-2 text-sm text-espresso/70">
              <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="#C45D3E" stroke-width="2"><polyline points="20 6 9 17 4 12"/></svg>
              <span class="text-en">Shareable link</span><span class="text-am">የሚጋራ ሊንክ</span>
            </li>
            <li class="flex items-center gap-2 text-sm text-espresso/70">
              <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="#C45D3E" stroke-width="2"><polyline points="20 6 9 17 4 12"/></svg>
              <span class="text-en">Basic customization</span><span class="text-am">መሰረታዊ ብጁ ማድግ</span>
            </li>
            <li class="flex items-center gap-2 text-sm text-espresso/70">
              <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="#C45D3E" stroke-width="2"><polyline points="20 6 9 17 4 12"/></svg>
              <span class="text-en">Basic dashboard</span><span class="text-am">መሰረታዊ ዳሽርድ</span>
            </li>
            <li class="flex items-center gap-2 text-sm text-espresso/70">
              <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="#C45D3E" stroke-width="2"><polyline points="20 6 9 17 4 12"/></svg>
              <span class="text-en">Guest messages</span><span class="text-am">የእንግዶች መልዕክቶች</span>
            </li>
          </ul>
          <button onclick="openModal('signupModal')" class="w-full btn-secondary py-3 rounded-full">
            <span class="text-en">Get Started</span>
            <span class="text-am">ይጀምሩ</span>
          </button>
        </div>
        <!-- Plus -->
        <div class="reveal reveal-delay-2 pricing-card bg-terracotta rounded-2xl p-8 border border-terracotta text-white relative shadow-xl shadow-terracotta/20">
          <div class="absolute -top-3 left-1/2 -translate-x-1/2 px-4 py-1 bg-gold text-espresso text-xs font-bold rounded-full">
            <span class="text-en">POPULAR</span>
            <span class="text-am">ታዋቂ</span>
          </div>
          <h3 class="font-display text-xl font-semibold mb-2"><span class="text-en">Plus</span><span class="text-am">ፕላስ</span></h3>
          <p class="text-white/70 text-sm mb-6"><span class="text-en">For families & events</span><span class="text-am">ለቤተሰቦችና ክስተቶች</span></p>
          <div class="font-display text-4xl font-bold mb-6">299 <span class="text-lg font-normal text-white/70">ETB</span></div>
          <ul class="space-y-3 mb-8">
            <li class="flex items-center gap-2 text-sm text-white/90">
              <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="white" stroke-width="2"><polyline points="20 6 9 17 4 12"/></svg>
              <span class="text-en">Multiple payment options</span><span class="text-am">ብዙ የክፍያ አማራጮች</span>
            </li>
            <li class="flex items-center gap-2 text-sm text-white/90">
              <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="white" stroke-width="2"><polyline points="20 6 9 17 4 12"/></svg>
              <span class="text-en">Contribution collection</span><span class="text-am">የአስተዋፅኦ ብሰ</span>
            </li>
            <li class="flex items-center gap-2 text-sm text-white/90">
              <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="white" stroke-width="2"><polyline points="20 6 9 17 4 12"/></svg>
              <span class="text-en">Custom cover & colors</span><span class="text-am">ብጁ ሽፋንና ቀለሞች</span>
            </li>
            <li class="flex items-center gap-2 text-sm text-white/90">
              <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="white" stroke-width="2"><polyline points="20 6 9 17 4 12"/></svg>
              <span class="text-en">QR invite code</span><span class="text-am">QR የግብ ኮድ</span>
            </li>
            <li class="flex items-center gap-2 text-sm text-white/90">
              <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="white" stroke-width="2"><polyline points="20 6 9 17 4 12"/></svg>
              <span class="text-en">Thank-you notes</span><span class="text-am">የምስጋና ማስታወሻች</span>
            </li>
            <li class="flex items-center gap-2 text-sm text-white/90">
              <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="white" stroke-width="2"><polyline points="20 6 9 17 4 12"/></svg>
              <span class="text-en">Better analytics</span><span class="text-am">የተሻለ ትንተና</span>
            </li>
          </ul>
          <button onclick="openModal('signupModal')" class="w-full bg-white text-terracotta font-semibold py-3 rounded-full hover:bg-ivory transition-colors">
            <span class="text-en">Start Free Trial</span>
            <span class="text-am">ነጻ ከራ ጀምሩ</span>
          </button>
        </div>
        <!-- Premium -->
        <div class="reveal reveal-delay-3 pricing-card bg-white rounded-2xl p-8 border border-border hover:border-terracotta/30 transition-colors">
          <h3 class="font-display text-xl font-semibold text-espresso mb-2"><span class="text-en">Premium</span><span class="text-am">ፕሪየም</span></h3>
          <p class="text-muted text-sm mb-6"><span class="text-en">For planners & businesses</span><span class="text-am">ለአስተባባዎች</span></p>
          <div class="font-display text-4xl font-bold text-espresso mb-6">599 <span class="text-lg font-normal text-muted">ETB</span></div>
          <ul class="space-y-3 mb-8">
            <li class="flex items-center gap-2 text-sm text-espresso/70">
              <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="#C45D3E" stroke-width="2"><polyline points="20 6 9 17 4 12"/></svg>
              <span class="text-en">Everything in Plus</span><span class="text-am">ሁሉም በፕላስ</span>
            </li>
            <li class="flex items-center gap-2 text-sm text-espresso/70">
              <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="#C45D3E" stroke-width="2"><polyline points="20 6 9 17 4 12"/></svg>
              <span class="text-en">Custom short link</span><span class="text-am">ብጁ አር ሊንክ</span>
            </li>
            <li class="flex items-center gap-2 text-sm text-espresso/70">
              <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="#C45D3E" stroke-width="2"><polyline points="20 6 9 17 4 12"/></svg>
              <span class="text-en">Multiple admins</span><span class="text-am">ብዙ አስተዳዳዎች</span>
            </li>
            <li class="flex items-center gap-2 text-sm text-espresso/70">
              <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="#C45D3E" stroke-width="2"><polyline points="20 6 9 17 4 12"/></svg>
              <span class="text-en">Scheduled reminders</span><span class="text-am">የተቀጠሩ ማስታወሻዎች</span>
            </li>
            <li class="flex items-center gap-2 text-sm text-espresso/70">
              <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="#C45D3E" stroke-width="2"><polyline points="20 6 9 17 4 12"/></svg>
              <span class="text-en">Payout dashboard</span><span class="text-am">የክፍያ ዳሽቦርድ</span>
            </li>
            <li class="flex items-center gap-2 text-sm text-espresso/70">
              <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="#C45D3E" stroke-width="2"><polyline points="20 6 9 17 4 12"/></svg>
              <span class="text-en">Priority support</span><span class="text-am">ቅድያ ድጋፍ</span>
            </li>
          </ul>
          <button onclick="openModal('contactModal')" class="w-full btn-secondary py-3 rounded-full">
            <span class="text-en">Contact Sales</span>
            <span class="text-am">ይገናኙ</span>
          </button>
        </div>
      </div>
    </div>
  </section>

  <!-- ========== FAQ ========== -->
  <section id="faq" class="py-24 lg:py-32 bg-gradient-to-b from-ivory to-ivory-dark">
    <div class="max-w-3xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="text-center mb-12">
        <h2 class="reveal font-display text-4xl font-semibold text-espresso">
          <span class="text-en">Frequently Asked Questions</span>
          <span class="text-am">በተደጋጋሚ የሚጠየ ጥያቄች</span>
        </h2>
      </div>
      <div class="space-y-4">
        <div class="reveal reveal-delay-1 bg-white rounded-2xl border border-border overflow-hidden">
          <button class="faq-btn w-full px-6 py-5 text-left flex justify-between items-center" onclick="toggleFaq(this)">
            <span class="font-medium text-espresso"><span class="text-en">What is Bene'nw?</span><span class="text-am">Bene'nw ምንን ነው?</span></span>
            <svg class="faq-icon w-5 h-5 text-muted transition-transform" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="6 9 12 15 18 9"/></svg>
          </button>
          <div class="faq-content hidden px-6 pb-5 text-espresso/60">
            <p><span class="text-en">Bene'nw is an Ethiopian gift registry and contribution platform designed for modern celebrations. It helps individuals and families create personalized lists, receive support securely, and share one simple link with loved ones across Ethiopia and beyond.</span><span class="text-am">Bene'nw ለዘመና ክብረ በዓሎች የተሰራ የኢትዮጵያ የስጦታ ዝርዝርና አስተዋፅኦ መድረ ነው።</span></p>
          </div>
        </div>
        <div class="reveal reveal-delay-2 bg-white rounded-2xl border border-border overflow-hidden">
          <button class="faq-btn w-full px-6 py-5 text-left flex justify-between items-center" onclick="toggleFaq(this)">
            <span class="font-medium text-espresso"><span class="text-en">Is it free to create a list?</span><span class="text-am">ዝርዝር መፍጠር ነጻ ነው?</span></span>
            <svg class="faq-icon w-5 h-5 text-muted transition-transform" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="6 9 12 15 18 9"/></svg>
          </button>
          <div class="faq-content hidden px-6 pb-5 text-espresso/60">
            <p><span class="text-en">Yes! Our basic plan is completely free. You can create lists, share them, and receive contributions without any hidden fees.</span><span class="text-am">አዎ! መሰረታዊ እቅዳችን ሙሉ በሙሉ ነ ነው።</span></p>
          </div>
        </div>
        <div class="reveal reveal-delay-3 bg-white rounded-2xl border border-border overflow-hidden">
          <button class="faq-btn w-full px-6 py-5 text-left flex justify-between items-center" onclick="toggleFaq(this)">
            <span class="font-medium text-espresso"><span class="text-en">Which payment methods are supported?</span><span class="text-am">የትኞቹ የክፍያ ዴዎች ይደገሉ?</span></span>
            <svg class="faq-icon w-5 h-5 text-muted transition-transform" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="6 9 12 15 18 9"/></svg>
          </button>
          <div class="faq-content hidden px-6 pb-5 text-espresso/60">
            <p><span class="text-en">We support telebirr, CBE Birr, bank transfer, and international card payments for diaspora contributors. More payment options are being added regularly.</span><span class="text-am">ቴሌር፣ ንግድ ር፣ የባንክ ዝውውርና ለዲያስፖራ ዓለም አቀፍ ርድ ክያ እንደግፋለን።</span></p>
          </div>
        </div>
        <div class="reveal reveal-delay-4 bg-white rounded-2xl border border-border overflow-hidden">
          <button class="faq-btn w-full px-6 py-5 text-left flex justify-between items-center" onclick="toggleFaq(this)">
            <span class="font-medium text-espresso"><span class="text-en">Can I add items from any store?</span><span class="text-am">ከማንኛውም ሱቅ ዕቃች ማከል እችላለሁ?</span></span>
            <svg class="faq-icon w-5 h-5 text-muted transition-transform" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="6 9 12 15 18 9"/></svg>
          </button>
          <div class="faq-content hidden px-6 pb-5 text-espresso/60">
            <p><span class="text-en">Absolutely! You can add products from any online store by pasting the link, or create custom gift items with your own descriptions and prices.</span><span class="text-am">በእርግ! ከማንኛውም የመስመር ላይ ቅ ሊንክ በማጣበቅ ምርች ማከል ይችላሉ።</span></p>
          </div>
        </div>
        <div class="reveal reveal-delay-5 bg-white rounded-2xl border border-border overflow-hidden">
          <button class="faq-btn w-full px-6 py-5 text-left flex justify-between items-center" onclick="toggleFaq(this)">
            <span class="font-medium text-espresso"><span class="text-en">How do payouts work?</span><span class="text-am">ክፍያዎች እንዴት ይሰራሉ?</span></span>
            <svg class="faq-icon w-5 h-5 text-muted transition-transform" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="6 9 12 15 18 9"/></svg>
          </button>
          <div class="faq-content hidden px-6 pb-5 text-espresso/60">
            <p><span class="text-en">Contributions are collected securely and can be transferred to your registered bank account or mobile wallet. You can track everything from your dashboard.</span><span class="text-am">አስተዋፅኦዎች በደህና ይሰበሰባሉ እና ደ ባንክ ሂሳብ ወይም ሞባይል ዋሌት ይዛወራሉ።</span></p>
          </div>
        </div>
        <div class="reveal reveal-delay-6 bg-white rounded-2xl border border-border overflow-hidden">
          <button class="faq-btn w-full px-6 py-5 text-left flex justify-between items-center" onclick="toggleFaq(this)">
            <span class="font-medium text-espresso"><span class="text-en">Can people abroad contribute?</span><span class="text-am">ከውጭ ያሉ ዎች ማስተዋፅኦ ይችላሉ?</span></span>
            <svg class="faq-icon w-5 h-5 text-muted transition-transform" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="6 9 12 15 18 9"/></svg>
          </button>
          <div class="faq-content hidden px-6 pb-5 text-espresso/60">
            <p><span class="text-en">Yes! Our platform supports international payments so diaspora friends and family can contribute easily from anywhere in the world.</span><span class="text-am">አዎ! ዓለም አቀፍ ክፍያዎችን እንደግፋለን ስለሆነ ዲያስፖራ ጓኞችና ቤተሰቦች ከማንኛውም ቦታ ማስተዋፅኦ ችላሉ።</span></p>
          </div>
        </div>
        <div class="reveal reveal-delay-7 bg-white rounded-2xl border border-border overflow-hidden">
          <button class="faq-btn w-full px-6 py-5 text-left flex justify-between items-center" onclick="toggleFaq(this)">
            <span class="font-medium text-espresso"><span class="text-en">Can more than one person manage a list?</span><span class="text-am">ከአንድ በላይ ሰው ርዝር ማስተዳደር ይችላል?</span></span>
            <svg class="faq-icon w-5 h-5 text-muted transition-transform" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="6 9 12 15 18 9"/></svg>
          </button>
          <div class="faq-content hidden px-6 pb-5 text-espresso/60">
            <p><span class="text-en">Yes! With our Plus and Premium plans, you can add multiple admins (like couples or family members) to manage the list together.</span><span class="text-am">አዎ! በፕላስና ፕሪሚየም እቅዶች ብዙ አስተዳዳዎች (እን ጥንች ወይም ተሰብ) ርዝሩን አብረው ማስተዳደር ይችላሉ።</span></p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- ========== FINAL CTA ========== -->
  <section class="py-24 lg:py-32 relative overflow-hidden">
    <div class="absolute inset-0 bg-gradient-to-br from-terracotta/5 to-gold/5" aria-hidden="true"></div>
    <div class="relative max-w-4xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
      <div class="reveal">
        <img src="Benenew-01.png" alt="Bene'nw Logo" class="h-20 w-auto mx-auto mb-6">
      </div>
      <h2 class="reveal font-display text-4xl sm:text-5xl lg:text-6xl font-semibold text-espresso leading-tight">
        <span class="text-en">Ready to create your list?</span>
        <span class="text-am">ዝርዝርዎን ለመፍጠር ዝግጁ ነዎት?</span>
      </h2>
      <p class="reveal reveal-delay-1 mt-6 text-xl text-espresso/60 max-w-2xl mx-auto">
        <span class="text-en">Join thousands of Ethiopian families celebrating with personalized gift registries. It's free to start.</span>
        <span class="text-am">በግላዊ የስጦታ ዝርዝሮች ዎች የኢትዮጵያ ቤተሰቦች ር ይቀላቀሉ። መነሻ ነጻ ነው።</span>
      </p>
      <div class="reveal reveal-delay-2 mt-10 flex flex-col sm:flex-row gap-4 justify-center">
        <button onclick="openModal('signupModal')" class="btn-primary text-lg">
          <span class="text-en">Create Your List Today</span>
          <span class="text-am">ዝርዝርዎን ዛሬ ይፍሩ</span>
        </button>
        <button onclick="openModal('searchModal')" class="btn-secondary text-lg">
          <span class="text-en">Find a List</span>
          <span class="text-am">ዝርዝር ይፈልጉ</span>
        </button>
      </div>
      <p class="reveal reveal-delay-3 mt-4 text-sm text-espresso/40">
        <span class="text-en">No credit card required · Free forever plan available</span>
        <span class="text-am">ክሬዲት ካርድ አያስፈልም · ነ ዘላ እቅድ ይገኛል</span>
      </p>
    </div>
  </section>

  <!-- ========== FOOTER ========== -->
  <footer class="bg-espresso text-white py-16">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="grid md:grid-cols-4 gap-12 mb-12">
        <!-- Brand -->
        <div class="md:col-span-2">
          <div class="flex items-center gap-3 mb-4">
            <img src="Benenew-01.png" alt="Bene'nw Logo" class="h-14 w-auto">
          </div>
          <p class="text-white/50 text-sm max-w-sm mb-4">
            <span class="text-en">Bene'nw is an Ethiopian gift registry and contribution platform designed for modern celebrations. Create personalized lists, receive support securely, and share one simple link with loved ones.</span>
            <span class="text-am">Bene'nw ለዘመናዊ ክብረ በዓሎች የተሰራ የኢትዮጵያ የስጦታ ዝርዝርና አስተዋፅኦ መድረ ነው።</span>
          </p>
          <div class="flex gap-3">
            <a href="#" class="w-10 h-10 bg-white/10 rounded-lg flex items-center justify-center hover:bg-terracotta transition-colors" aria-label="Facebook">
              <svg width="18" height="18" viewBox="0 0 24 24" fill="white"><path d="M18 2h-3a5 5 0 0 0-5 5v3H7v4h3v8h4v-8h3l1-4h-4V7a1 1 0 0 1 1-1h3z"/></svg>
            </a>
            <a href="#" class="w-10 h-10 bg-white/10 rounded-lg flex items-center justify-center hover:bg-terracotta transition-colors" aria-label="Instagram">
              <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="white" stroke-width="2"><rect x="2" y="2" width="20" height="20" rx="5"/><circle cx="12" cy="12" r="5"/><circle cx="17.5" cy="6.5" r="1.5" fill="white" stroke="none"/></svg>
            </a>
            <a href="#" class="w-10 h-10 bg-white/10 rounded-lg flex items-center justify-center hover:bg-terracotta transition-colors" aria-label="Telegram">
              <svg width="18" height="18" viewBox="0 0 24 24" fill="white"><path d="M21.198 2.433a2.242 2.242 0 0 0-1.022.215l-17.15 6.57a1.9 1.9 0 0 0 .085 3.54l4.15 1.62 2.25 6.65a1.32 1.32 0 0 0 2.26.32l3.07-3.38 4.35 3.2a1.88 1.88 0 0 0 2.94-1.22l2.75-13.74a2.24 2.24 0 0 0-1.68-2.77zM10.5 14.5l-1.5 4.5-1-3 7.5-5.5-5 4z"/></svg>
            </a>
            <a href="#" class="w-10 h-10 bg-white/10 rounded-lg flex items-center justify-center hover:bg-terracotta transition-colors" aria-label="TikTok">
              <svg width="18" height="18" viewBox="0 0 24 24" fill="white"><path d="M19.59 6.69a4.83 4.83 0 0 1-3.77-4.25V2h-3.45v13.67a2.89 2.89 0 0 1-2.88 2.5 2.89 2.89 0 0 1-2.89-2.89 2.89 2.89 0 0 1 2.89-2.89c.28 0 .54.04.79.1v-3.5a6.37 6.37 0 0 0-.79-.05A6.34 6.34 0 0 0 3.15 15.2a6.34 6.34 0 0 0 6.34 6.34 6.34 6.34 0 0 0 6.34-6.34V8.73a8.19 8.19 0 0 0 4.76 1.52V6.8a4.84 4.84 0 0 1-1-.11z"/></svg>
            </a>
          </div>
        </div>
        <!-- Product Links -->
        <div>
          <h4 class="font-semibold text-white mb-4"><span class="text-en">Product</span><span class="text-am">ምርት</span></h4>
          <ul class="space-y-2 text-sm text-white/50">
            <li><a href="#how-it-works" class="hover:text-white transition-colors"><span class="text-en">How It Works</span><span class="text-am">እንዴት እንደሚሰራ</span></a></li>
            <li><a href="#occasions" class="hover:text-white transition-colors"><span class="text-en">Occasions</span><span class="text-am">አጋጣሚዎች</span></a></li>
            <li><a href="#pricing" class="hover:text-white transition-colors"><span class="text-en">Pricing</span><span class="text-am">ዋጋ</span></a></li>
            <li><button onclick="openModal('searchModal')" class="hover:text-white transition-colors text-left"><span class="text-en">Find a List</span><span class="text-am">ዝርዝር ይፈል</span></button></li>
            <li><a href="#" class="hover:text-white transition-colors"><span class="text-en">Trust & Security</span><span class="text-am">ታማኝነትና ደህንነት</span></a></li>
            <li><button onclick="openModal('contactModal')" class="hover:text-white transition-colors text-left"><span class="text-en">For Vendors</span><span class="text-am">ለሻጮች</span></button></li>
          </ul>
        </div>
        <!-- Support Links -->
        <div>
          <h4 class="font-semibold text-white mb-4"><span class="text-en">Support</span><span class="text-am">ድጋ</span></h4>
          <ul class="space-y-2 text-sm text-white/50">
            <li><a href="#faq" class="hover:text-white transition-colors"><span class="text-en">FAQ</span><span class="text-am">ጥያቄ</span></a></li>
            <li><button onclick="openModal('contactModal')" class="hover:text-white transition-colors text-left"><span class="text-en">Contact Us</span><span class="text-am">አግኙን</span></button></li>
            <li><a href="#" class="hover:text-white transition-colors"><span class="text-en">Privacy Policy</span><span class="text-am">የግላዊነት ፖሊ</span></a></li>
            <li><a href="#" class="hover:text-white transition-colors"><span class="text-en">Terms of Service</span><span class="text-am">የአገልግሎት ደንብ</span></a></li>
          </ul>
          <div class="mt-6">
            <div class="lang-toggle" role="tablist" aria-label="Language selection">
              <button role="tab" aria-selected="true" class="active" data-lang="en">EN</button>
              <button role="tab" aria-selected="false" data-lang="am">አማ</button>
            </div>
          </div>
        </div>
      </div>
      <div class="pt-8 border-t border-white/10 flex flex-col sm:flex-row justify-between items-center gap-4">
        <p class="text-white/30 text-sm">© 2026 Bene'nw. All rights reserved.</p>
        <div class="flex gap-6 text-sm text-white/30">
          <a href="#" class="hover:text-white/60 transition-colors"><span class="text-en">Privacy</span><span class="text-am">ግላዊነት</span></a>
          <a href="#" class="hover:text-white/60 transition-colors"><span class="text-en">Terms</span><span class="text-am">ደንብ</span></a>
        </div>
      </div>
    </div>
  </footer>

  <!-- ========== JAVASCRIPT ========== -->
  <script>
    // ========== MODAL FUNCTIONS ==========
    function openModal(id) {
        const modal = document.getElementById(id);
        if(modal) {
            modal.classList.add('open');
            document.body.style.overflow = 'hidden';
        }
    }

    function closeModal(id) {
        const modal = document.getElementById(id);
        if(modal) {
            modal.classList.remove('open');
            document.body.style.overflow = '';
        }
    }

    // Close modal when clicking outside
    document.querySelectorAll('.modal-overlay').forEach(modal => {
        modal.addEventListener('click', (e) => {
            if (e.target === modal) {
                modal.classList.remove('open');
                document.body.style.overflow = '';
            }
        });
    });

    // ========== MOBILE MENU ==========
    const menuBtn = document.getElementById('menuBtn');
    const closeMenuBtn = document.getElementById('closeMenuBtn');
    const mobileMenu = document.getElementById('mobileMenu');

    if (menuBtn && mobileMenu && closeMenuBtn) {
      menuBtn.addEventListener('click', () => {
        mobileMenu.classList.add('open');
        document.body.style.overflow = 'hidden';
      });
      closeMenuBtn.addEventListener('click', () => {
        mobileMenu.classList.remove('open');
        document.body.style.overflow = '';
      });
    }

    function closeMobileMenu() {
      if (mobileMenu) {
        mobileMenu.classList.remove('open');
        document.body.style.overflow = '';
      }
    }

    // Close mobile menu on link click
    if (mobileMenu) {
      mobileMenu.querySelectorAll('a, button').forEach(link => {
        link.addEventListener('click', () => {
            if(!link.onclick && link.getAttribute('href')) {
                closeMobileMenu();
            }
        });
      });
    }

    window.closeMobileMenu = closeMobileMenu;

    // ========== LANGUAGE TOGGLE ==========
    function setLanguage(lang) {
        document.documentElement.setAttribute('lang', lang);
        document.querySelectorAll('.lang-toggle').forEach(toggle => {
            const buttons = toggle.querySelectorAll('button');
            buttons.forEach(btn => {
                btn.classList.toggle('active', btn.dataset.lang === lang);
            });
        });
    }

    document.querySelectorAll('.lang-toggle').forEach(toggle => {
        toggle.querySelectorAll('button').forEach(btn => {
            btn.addEventListener('click', () => setLanguage(btn.dataset.lang));
        });
    });

    // ========== SCROLL REVEAL ==========
    const observer = new IntersectionObserver((entries) => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          entry.target.classList.add('visible');
          observer.unobserve(entry.target);
        }
      });
    }, { threshold: 0.1 });

    document.querySelectorAll('.reveal').forEach(el => observer.observe(el));

    // ========== FAQ TOGGLE ==========
    function toggleFaq(btn) {
      const content = btn.nextElementSibling;
      const icon = btn.querySelector('.faq-icon');
      const isOpen = !content.classList.contains('hidden');
      
      // Close all FAQs first
      document.querySelectorAll('.faq-content').forEach(c => c.classList.add('hidden'));
      document.querySelectorAll('.faq-icon').forEach(i => i.style.transform = 'rotate(0deg)');
      
      // Open clicked one if it was closed
      if (!isOpen) {
        content.classList.remove('hidden');
        icon.style.transform = 'rotate(180deg)';
      }
    }

    // ========== COPY TO CLIPBOARD ==========
    function copyToClipboard() {
        const input = document.querySelector('#shareModal input[type="text"]');
        if (input) {
            navigator.clipboard.writeText(input.value).then(() => {
                const btn = input.nextElementSibling;
                const originalText = btn.innerHTML;
                btn.innerHTML = '<span class="text-en">Copied!</span><span class="text-am">ተቀድቷል!</span>';
                setTimeout(() => { btn.innerHTML = originalText; }, 2000);
            });
        }
    }
  </script>
</body>
</html>

