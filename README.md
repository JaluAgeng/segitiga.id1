<!DOCTYPE html>
<html lang="id" class="scroll-smooth">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>segitiga.id — Fakta untuk Warga | Media Hyperlocal Digital Purwasuka</title>
  <meta name="description" content="segitiga.id adalah media informasi hyperlocal digital untuk wilayah Purwakarta, Subang, dan Karawang (Purwasuka). Fakta untuk Warga." />

  <!-- Google Fonts: Plus Jakarta Sans (Editorial Headings) & Inter (Article Body) -->
  <link rel="preconnect" href="https://fonts.googleapis.com" />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&family=Plus+Jakarta+Sans:wght@600;700;800&display=swap" rel="stylesheet" />

  <!-- Tailwind CSS CDN -->
  <script src="https://cdn.tailwindcss.com"></script>
  <script>
    tailwind.config = {
      theme: {
        extend: {
          fontFamily: {
            heading: ['"Plus Jakarta Sans"', 'system-ui', 'sans-serif'],
            sans: ['"Inter"', 'system-ui', '-apple-system', 'sans-serif'],
          },
          colors: {
            navy: {
              DEFAULT: '#0A2239',
              light: '#133557',
              dark: '#061524',
            },
            royal: {
              DEFAULT: '#0D4F8B',
              light: '#1767B0',
            },
            cyanbrand: {
              DEFAULT: '#00B4D8',
              light: '#48CAE4',
              soft: '#E0F7FC',
            },
            ice: '#F4F9FC',
            slatebody: '#334155',
          },
          boxShadow: {
            'soft-navy': '0 20px 45px -15px rgba(10, 34, 57, 0.12)',
            'cyan-glow': '0 14px 30px -8px rgba(0, 180, 216, 0.34)',
            'card-hover': '0 24px 50px -12px rgba(13, 79, 139, 0.16)',
          }
        }
      }
    };
  </script>

  <style>
    body {
      font-family: 'Inter', sans-serif;
      color: #334155;
      background-color: #FFFFFF;
      overflow-x: hidden;
    }

    h1, h2, h3, h4, .font-heading {
      font-family: 'Plus Jakarta Sans', sans-serif;
    }

    /* Pola geometris segitiga editorial */
    .bg-hero-editorial {
      background-color: #FFFFFF;
      background-image:
        radial-gradient(circle at 86% 16%, rgba(0, 180, 216, 0.11) 0%, transparent 44%),
        radial-gradient(circle at 10% 80%, rgba(13, 79, 139, 0.08) 0%, transparent 48%),
        linear-gradient(180deg, #FFFFFF 0%, #F8FAFC 100%);
    }

    .triangle-mesh {
      background-image: url("data:image/svg+xml,%3Csvg width='72' height='64' viewBox='0 0 72 64' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M36 4L68 60H4L36 4Z' fill='none' stroke='%230D4F8B' stroke-opacity='0.04' stroke-width='1'/%3E%3C/svg%3E");
      background-size: 72px 64px;
    }

    /* Glassmorphism Navbar */
    .navbar-glass {
      background: rgba(255, 255, 255, 0.88);
      backdrop-filter: blur(14px);
      -webkit-backdrop-filter: blur(14px);
      border-bottom: 1px solid rgba(10, 34, 57, 0.08);
    }

    /* Animasi Sinyal Antena Logo */
    @keyframes signalPulse {
      0%, 100% { transform: scale(1); opacity: 0.95; }
      50% { transform: scale(1.16); opacity: 1; }
    }
    .animate-signal {
      transform-origin: 172px 52px;
      animation: signalPulse 3s ease-in-out infinite;
    }

    /* Animasi Scroll Reveal */
    .reveal {
      opacity: 0;
      transform: translateY(20px);
      transition: opacity 0.65s cubic-bezier(0.22, 1, 0.36, 1), transform 0.65s cubic-bezier(0.22, 1, 0.36, 1);
    }
    .reveal.is-visible {
      opacity: 1;
      transform: translateY(0);
    }

    /* Tab Filosofi Aktif */
    .philosophy-tab.active {
      border-color: #00B4D8;
      background-color: #FFFFFF;
      box-shadow: 0 16px 32px -12px rgba(10, 34, 57, 0.14);
    }

    /* Hide scrollbar horizontal pada tab rubrik mobile */
    .no-scrollbar::-webkit-scrollbar {
      display: none;
    }
    .no-scrollbar {
      -ms-overflow-style: none;
      scrollbar-width: none;
    }

    /* Custom Scrollbar */
    ::-webkit-scrollbar {
      width: 8px;
      height: 8px;
    }
    ::-webkit-scrollbar-track {
      background: #F8FAFC;
    }
    ::-webkit-scrollbar-thumb {
      background: #CBD5E1;
      border-radius: 9999px;
    }
    ::-webkit-scrollbar-thumb:hover {
      background: #0D4F8B;
    }
  </style>
</head>

<body class="antialiased selection:bg-cyanbrand/20 selection:text-navy">

  <!-- =====================================================================
       DEFINISI GRADASI SVG IDENTITAS SEGITIGA.ID
       ===================================================================== -->
  <svg width="0" height="0" class="hidden" aria-hidden="true">
    <defs>
      <linearGradient id="segitigaLogoGrad" x1="15%" y1="95%" x2="55%" y2="5%">
        <stop offset="0%" stop-color="#0A2239" />
        <stop offset="55%" stop-color="#0D4F8B" />
        <stop offset="100%" stop-color="#00B4D8" />
      </linearGradient>
      <linearGradient id="segitigaPlayGrad" x1="0%" y1="100%" x2="100%" y2="0%">
        <stop offset="0%" stop-color="#0A2239" />
        <stop offset="50%" stop-color="#0D4F8B" />
        <stop offset="100%" stop-color="#00B4D8" />
      </linearGradient>
    </defs>
  </svg>

  <!-- =====================================================================
       TOP EDITORIAL BAR (3 SALURAN RESMI & LOKASI PURWASUKA)
       ===================================================================== -->
  <div class="bg-navy text-white text-xs py-2 border-b border-white/10">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 flex flex-wrap items-center justify-between gap-2">
      <div class="flex items-center gap-2.5">
        <span class="inline-flex items-center gap-1.5 font-heading font-bold text-cyanbrand tracking-wide">
          <span class="w-2 h-2 rounded-full bg-cyanbrand animate-pulse"></span>
          FAKTA UNTUK WARGA
        </span>
        <span class="text-white/30 hidden sm:inline">|</span>
        <span class="text-slate-300 hidden sm:inline">Purwakarta • Subang • Karawang (Purwasuka)</span>
      </div>

      <!-- Hanya 3 Saluran Resmi -->
      <div class="flex items-center gap-3 sm:gap-4 font-medium">
        <span class="text-slate-400 hidden md:inline">Kanal Resmi:</span>
        <a href="https://www.tiktok.com/@redaksi.segitiga?_r=1&_t=ZS-9Bf5fEpCAP0" target="_blank" rel="noopener noreferrer" class="inline-flex items-center gap-1.5 text-slate-200 hover:text-cyanbrand transition-colors">
          <svg class="w-3.5 h-3.5" fill="currentColor" viewBox="0 0 24 24"><path d="M16.6 5.82A4.28 4.28 0 0 1 15.54 3h-3.09v12.4a2.59 2.59 0 0 1-2.59 2.5c-1.42 0-2.6-1.16-2.6-2.6 0-1.72 1.66-3.01 3.37-2.48V9.66c-3.45-.46-6.47 2.22-6.47 5.64 0 3.33 2.76 5.7 5.69 5.7 3.14 0 5.69-2.55 5.69-5.7V9.01a7.35 7.35 0 0 0 4.3 1.38V7.3s-1.88.09-3.24-1.48Z"/></svg>
          <span>TikTok</span>
        </a>
        <span class="text-white/20">•</span>
        <a href="https://www.instagram.com/redaksi.segitiga?gwpx=MWx4eTQ1eG90bmoxdw==" target="_blank" rel="noopener noreferrer" class="inline-flex items-center gap-1.5 text-slate-200 hover:text-cyanbrand transition-colors">
          <svg class="w-3.5 h-3.5" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><rect x="2" y="2" width="20" height="20" rx="5"/><circle cx="12" cy="12" r="4"/><circle cx="17.5" cy="6.5" r="1" fill="currentColor" stroke="none"/></svg>
          <span>Instagram</span>
        </a>
        <span class="text-white/20">•</span>
        <a href="https://whatsapp.com/channel/0029Vb9QOPJ3LdQQIEvpWi0K" target="_blank" rel="noopener noreferrer" class="inline-flex items-center gap-1.5 text-cyanbrand hover:text-white font-semibold transition-colors">
          <svg class="w-3.5 h-3.5" fill="currentColor" viewBox="0 0 24 24"><path d="M12.04 2C6.58 2 2.13 6.45 2.13 11.91c0 1.75.46 3.45 1.32 4.95L2.05 22l5.25-1.38c1.45.79 3.08 1.21 4.74 1.21 5.46 0 9.91-4.45 9.91-9.91C21.95 6.45 17.5 2 12.04 2Zm5.82 14.01c-.24.68-1.41 1.3-1.96 1.38-.51.08-1.15.11-1.86-.11-.43-.14-.99-.32-1.7-.63-2.99-1.29-4.94-4.3-5.09-4.5-.15-.2-1.21-1.61-1.21-3.07 0-1.46.77-2.18 1.04-2.48.27-.3.59-.37.79-.37.2 0 .4 0 .57.01.18.01.43-.07.67.51.24.59.84 2.05.91 2.2.08.15.13.32.02.52-.1.2-.15.32-.3.5-.15.17-.31.38-.45.51-.15.15-.3.31-.13.61.17.3.77 1.27 1.65 2.05 1.13 1.01 2.09 1.32 2.39 1.47.3.15.47.12.65-.08.17-.2.74-.86.94-1.16.2-.3.4-.25.67-.15.27.1 1.73.82 2.03.97.3.15.5.22.57.34.07.12.07.7-.17 1.38Z"/></svg>
          <span>Saluran WhatsApp</span>
        </a>
      </div>
    </div>
  </div>

  <!-- =====================================================================
       1. NAVBAR STICKY
       ===================================================================== -->
  <header id="navbar" class="sticky top-0 z-40 navbar-glass transition-all duration-300">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex items-center justify-between h-20">

        <!-- Logo Horizontal SVG segitiga.id -->
        <a href="#beranda" class="flex items-center gap-3 group focus:outline-none" aria-label="Beranda segitiga.id">
          <!-- Emblem Segitiga + Kurva S + Play + Antena -->
          <svg class="w-10 h-9 sm:w-11 sm:h-10 transition-transform duration-300 group-hover:scale-105" viewBox="0 0 220 200" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M104.2 17.5C106.8 13.1 113.2 13.1 115.8 17.5L196.4 157.2C199.0 161.7 195.8 167.3 190.6 167.3H29.4C24.2 167.3 21.0 161.7 23.6 157.2L104.2 17.5Z" fill="url(#segitigaLogoGrad)" />
            <path d="M62 146C51 134 49 112 58 93C55 113 62 131 76 140L62 146Z" fill="#FFFFFF" />
            <path d="M137 88C128 73 108 65 91 71C75 77 68 95 70 114C72 132 84 143 104 143C115 143 124 140 130 137C121 151 104 162 85 169H103C122 161 138 147 146 130C151 118 147 101 137 88Z" fill="#FFFFFF" />
            <path d="M101 92.5C101 89.8 104.0 88.2 106.3 89.6L127.5 102.6C129.7 103.9 129.7 107.1 127.5 108.4L106.3 121.4C104.0 122.8 101 121.2 101 118.5V92.5Z" fill="url(#segitigaPlayGrad)" />
            <path d="M97 135C121 121 146 93 169 55" stroke="#FFFFFF" stroke-width="14" stroke-linecap="round" />
            <path d="M97 135C121 121 146 93 169 55" stroke="url(#segitigaLogoGrad)" stroke-width="7.5" stroke-linecap="round" />
            <circle cx="172" cy="52" r="10.5" fill="#00B4D8" />
          </svg>

          <!-- Wordmark segitiga.id -->
          <svg class="h-7 sm:h-8 w-auto" viewBox="0 0 245 48" fill="none" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="segitiga.id">
            <text x="0" y="36" fill="#0A2239" font-family="'Plus Jakarta Sans', sans-serif" font-weight="800" font-size="36" letter-spacing="-1.2">segitiga</text>
            <polygon points="154,26 164,31.5 154,37" fill="#0A2239" />
            <rect x="171" y="16" width="7.2" height="20" rx="1.5" fill="#00B4D8" />
            <polygon points="171,4 181.5,9.5 171,15" fill="#00B4D8" />
            <text x="184" y="36" fill="#00B4D8" font-family="'Plus Jakarta Sans', sans-serif" font-weight="800" font-size="36" letter-spacing="-1">d</text>
          </svg>
        </a>

        <!-- Menu Navigasi Desktop -->
        <nav class="hidden lg:flex items-center gap-6" aria-label="Navigasi Utama">
          <a href="#beranda" class="text-sm font-heading font-bold text-slatebody hover:text-navy transition-colors py-2">Beranda</a>
          <a href="#tentang" class="text-sm font-heading font-bold text-slatebody hover:text-navy transition-colors py-2">Tentang Kami</a>
          <a href="#wilayah" class="text-sm font-heading font-bold text-slatebody hover:text-navy transition-colors py-2">Wilayah Purwasuka</a>
          <a href="#rubrik" class="text-sm font-heading font-bold text-slatebody hover:text-navy transition-colors py-2">Rubrik</a>
          <a href="#berita" class="text-sm font-heading font-bold text-slatebody hover:text-navy transition-colors py-2">Berita Terbaru</a>
          <a href="#kontak" class="text-sm font-heading font-bold text-slatebody hover:text-navy transition-colors py-2">Hubungi Kami</a>
        </nav>

        <!-- Tombol CTA Ikuti Saluran & Menu Mobile -->
        <div class="flex items-center gap-3">
          <button
            type="button"
            onclick="openSocialModal()"
            class="inline-flex items-center gap-2 px-4 sm:px-5 py-2.5 rounded-xl bg-navy hover:bg-royal text-white font-heading text-sm font-bold shadow-sm hover:shadow-cyan-glow transition-all duration-300 cursor-pointer"
          >
            <span>Ikuti Saluran</span>
            <svg class="w-3.5 h-3.5 text-cyanbrand" viewBox="0 0 16 16" fill="currentColor">
              <path d="M3 2.5L13.5 8L3 13.5V2.5Z" />
            </svg>
          </button>

          <button
            id="mobileMenuBtn"
            type="button"
            aria-label="Buka Menu Navigasi"
            aria-expanded="false"
            class="lg:hidden p-2.5 rounded-xl text-navy hover:bg-ice border border-slate-200/80 transition-colors cursor-pointer"
          >
            <svg id="hamburgerIcon" class="w-6 h-6" fill="none" stroke="currentColor" stroke-width="2.2" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" d="M4 6h16M4 12h16M4 18h16" />
            </svg>
            <svg id="closeIcon" class="w-6 h-6 hidden" fill="none" stroke="currentColor" stroke-width="2.2" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12" />
            </svg>
          </button>
        </div>
      </div>
    </div>

    <!-- Drawer Navigasi Mobile -->
    <div id="mobileMenu" class="hidden lg:hidden bg-white border-t border-slate-100 shadow-lg">
      <div class="px-4 pt-3 pb-5 space-y-1">
        <a href="#beranda" class="mobile-nav-link block px-4 py-3 rounded-xl text-base font-heading font-bold text-navy hover:bg-ice transition-colors">Beranda</a>
        <a href="#tentang" class="mobile-nav-link block px-4 py-3 rounded-xl text-base font-heading font-bold text-navy hover:bg-ice transition-colors">Tentang Kami</a>
        <a href="#wilayah" class="mobile-nav-link block px-4 py-3 rounded-xl text-base font-heading font-bold text-navy hover:bg-ice transition-colors">Wilayah Purwasuka</a>
        <a href="#rubrik" class="mobile-nav-link block px-4 py-3 rounded-xl text-base font-heading font-bold text-navy hover:bg-ice transition-colors">Rubrik</a>
        <a href="#berita" class="mobile-nav-link block px-4 py-3 rounded-xl text-base font-heading font-bold text-navy hover:bg-ice transition-colors">Berita Terbaru</a>
        <a href="#kontak" class="mobile-nav-link block px-4 py-3 rounded-xl text-base font-heading font-bold text-navy hover:bg-ice transition-colors">Hubungi Kami</a>
      </div>
    </div>
  </header>

  <main>
    <!-- =====================================================================
         2. HERO SECTION (IDENTITAS MEDIA HYPERLOCAL PURWASUKA)
         ===================================================================== -->
    <section id="beranda" class="relative bg-hero-editorial triangle-mesh pt-10 pb-16 sm:pt-14 sm:pb-24 lg:pt-16 lg:pb-28 overflow-hidden border-b border-slate-200/70">
      <div class="pointer-events-none absolute -top-24 -right-24 w-96 h-96 rounded-full bg-cyanbrand/10 blur-3xl"></div>
      <div class="pointer-events-none absolute bottom-0 -left-24 w-80 h-80 rounded-full bg-royal/10 blur-3xl"></div>

      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
        <div class="grid grid-cols-1 lg:grid-cols-12 gap-10 lg:gap-12 items-center">

          <!-- Kolom Kiri: Headline, Subjudul, CTA & 3 Saluran Resmi -->
          <div class="lg:col-span-7 space-y-6 reveal">
            <!-- Badge -->
            <div class="inline-flex items-center gap-2.5 px-4 py-2 rounded-full bg-white border border-cyanbrand/35 shadow-sm">
              <span class="w-2.5 h-2.5 rounded-full bg-cyanbrand animate-pulse"></span>
              <span class="text-[11px] sm:text-xs font-heading font-extrabold tracking-widest text-navy uppercase">
                MEDIA HYPERLOCAL DIGITAL • PURWAKARTA • SUBANG • KARAWANG
              </span>
            </div>

            <!-- Judul Utama -->
            <h1 class="text-4xl sm:text-5xl lg:text-[3.5rem] font-extrabold text-navy leading-[1.12] tracking-tight">
              Fakta untuk Warga
              <span class="block text-transparent bg-clip-text bg-gradient-to-r from-navy via-royal to-cyanbrand">Purwasuka.</span>
            </h1>

            <!-- Subjudul -->
            <p class="text-base sm:text-lg text-slatebody leading-relaxed max-w-2xl">
              <strong class="font-bold text-navy">segitiga.id</strong> adalah media informasi hyperlocal digital terverifikasi bagi masyarakat <strong>Purwakarta, Subang, dan Karawang</strong>. Kami mengemas berita aktual, potensi daerah, dan klarifikasi fakta secara ringkas, visual, serta mudah dipahami di perangkat Anda.
            </p>

            <!-- Tombol CTA Utama & Sekunder -->
            <div class="pt-1 flex flex-col sm:flex-row items-stretch sm:items-center gap-3.5 sm:gap-4">
              <a
                href="#berita"
                class="inline-flex items-center justify-center gap-2.5 px-7 py-4 rounded-2xl bg-gradient-to-r from-navy via-royal to-cyanbrand text-white font-heading font-bold text-sm sm:text-base shadow-cyan-glow hover:opacity-95 hover:-translate-y-0.5 transition-all duration-300"
              >
                <span>Baca Berita Terbaru</span>
                <svg class="w-4 h-4" fill="none" stroke="currentColor" stroke-width="2.5" viewBox="0 0 24 24">
                  <path stroke-linecap="round" stroke-linejoin="round" d="M19 9l-7 7-7-7" />
                </svg>
              </a>

              <a
                href="https://whatsapp.com/channel/0029Vb9QOPJ3LdQQIEvpWi0K"
                target="_blank"
                rel="noopener noreferrer"
                class="inline-flex items-center justify-center gap-2.5 px-7 py-4 rounded-2xl bg-white text-navy font-heading font-bold text-sm sm:text-base border-2 border-navy/15 hover:border-cyanbrand hover:bg-ice transition-all duration-300"
              >
                <svg class="w-5 h-5 text-emerald-600" fill="currentColor" viewBox="0 0 24 24">
                  <path d="M12.04 2C6.58 2 2.13 6.45 2.13 11.91c0 1.75.46 3.45 1.32 4.95L2.05 22l5.25-1.38c1.45.79 3.08 1.21 4.74 1.21 5.46 0 9.91-4.45 9.91-9.91C21.95 6.45 17.5 2 12.04 2Zm5.82 14.01c-.24.68-1.41 1.3-1.96 1.38-.51.08-1.15.11-1.86-.11-.43-.14-.99-.32-1.7-.63-2.99-1.29-4.94-4.3-5.09-4.5-.15-.2-1.21-1.61-1.21-3.07 0-1.46.77-2.18 1.04-2.48.27-.3.59-.37.79-.37.2 0 .4 0 .57.01.18.01.43-.07.67.51.24.59.84 2.05.91 2.2.08.15.13.32.02.52-.1.2-.15.32-.3.5-.15.17-.31.38-.45.51-.15.15-.3.31-.13.61.17.3.77 1.27 1.65 2.05 1.13 1.01 2.09 1.32 2.39 1.47.3.15.47.12.65-.08.17-.2.74-.86.94-1.16.2-.3.4-.25.67-.15.27.1 1.73.82 2.03.97.3.15.5.22.57.34.07.12.07.7-.17 1.38Z"/>
                </svg>
                <span>Gabung Saluran WhatsApp</span>
              </a>
            </div>

            <!-- Quick-Access 3 Kartu Saluran Resmi (TikTok, Instagram, Saluran WhatsApp) -->
            <div class="pt-3">
              <p class="text-xs font-heading font-extrabold uppercase tracking-wider text-slate-400 mb-3">
                Saluran Resmi Distribusi Berita
              </p>
              <div class="grid grid-cols-1 sm:grid-cols-3 gap-3">
                <!-- 1. TikTok -->
                <div class="flex items-center justify-between gap-2 p-3 rounded-2xl bg-white border border-slate-200/90 hover:border-cyanbrand/60 shadow-sm transition-all">
                  <a href="https://www.tiktok.com/@redaksi.segitiga?_r=1&_t=ZS-9Bf5fEpCAP0" target="_blank" rel="noopener noreferrer" class="flex items-center gap-2.5 min-w-0 group">
                    <span class="w-9 h-9 rounded-xl bg-navy text-white flex items-center justify-center shrink-0 group-hover:bg-cyanbrand transition-colors">
                      <svg class="w-4 h-4" fill="currentColor" viewBox="0 0 24 24"><path d="M16.6 5.82A4.28 4.28 0 0 1 15.54 3h-3.09v12.4a2.59 2.59 0 0 1-2.59 2.5c-1.42 0-2.6-1.16-2.6-2.6 0-1.72 1.66-3.01 3.37-2.48V9.66c-3.45-.46-6.47 2.22-6.47 5.64 0 3.33 2.76 5.7 5.69 5.7 3.14 0 5.69-2.55 5.69-5.7V9.01a7.35 7.35 0 0 0 4.3 1.38V7.3s-1.88.09-3.24-1.48Z"/></svg>
                    </span>
                    <div class="truncate">
                      <p class="text-xs font-heading font-extrabold text-navy truncate">TikTok</p>
                      <p class="text-[11px] text-slate-500 truncate">@redaksi.segitiga</p>
                    </div>
                  </a>
                  <button type="button" onclick="copyText('https://www.tiktok.com/@redaksi.segitiga?_r=1&_t=ZS-9Bf5fEpCAP0', 'Tautan TikTok @redaksi.segitiga disalin!')" title="Salin tautan TikTok" aria-label="Salin tautan TikTok" class="p-2 rounded-lg text-slate-400 hover:text-navy hover:bg-ice transition-colors cursor-pointer shrink-0">
                    <svg class="w-4 h-4" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M8 16H6a2 2 0 01-2-2V6a2 2 0 012-2h8a2 2 0 012 2v2m-6 12h8a2 2 0 002-2v-8a2 2 0 00-2-2h-8a2 2 0 00-2 2v8a2 2 0 002 2z"/></svg>
                  </button>
                </div>

                <!-- 2. Instagram -->
                <div class="flex items-center justify-between gap-2 p-3 rounded-2xl bg-white border border-slate-200/90 hover:border-cyanbrand/60 shadow-sm transition-all">
                  <a href="https://www.instagram.com/redaksi.segitiga?gwpx=MWx4eTQ1eG90bmoxdw==" target="_blank" rel="noopener noreferrer" class="flex items-center gap-2.5 min-w-0 group">
                    <span class="w-9 h-9 rounded-xl bg-royal text-white flex items-center justify-center shrink-0 group-hover:bg-cyanbrand transition-colors">
                      <svg class="w-4 h-4" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><rect x="2" y="2" width="20" height="20" rx="5"/><circle cx="12" cy="12" r="4"/><circle cx="17.5" cy="6.5" r="1" fill="currentColor" stroke="none"/></svg>
                    </span>
                    <div class="truncate">
                      <p class="text-xs font-heading font-extrabold text-navy truncate">Instagram</p>
                      <p class="text-[11px] text-slate-500 truncate">@redaksi.segitiga</p>
                    </div>
                  </a>
                  <button type="button" onclick="copyText('https://www.instagram.com/redaksi.segitiga?gwpx=MWx4eTQ1eG90bmoxdw==', 'Tautan Instagram @redaksi.segitiga disalin!')" title="Salin tautan Instagram" aria-label="Salin tautan Instagram" class="p-2 rounded-lg text-slate-400 hover:text-navy hover:bg-ice transition-colors cursor-pointer shrink-0">
                    <svg class="w-4 h-4" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M8 16H6a2 2 0 01-2-2V6a2 2 0 012-2h8a2 2 0 012 2v2m-6 12h8a2 2 0 002-2v-8a2 2 0 00-2-2h-8a2 2 0 00-2 2v8a2 2 0 002 2z"/></svg>
                  </button>
                </div>

                <!-- 3. Saluran WhatsApp -->
                <div class="flex items-center justify-between gap-2 p-3 rounded-2xl bg-white border border-slate-200/90 hover:border-cyanbrand/60 shadow-sm transition-all">
                  <a href="https://whatsapp.com/channel/0029Vb9QOPJ3LdQQIEvpWi0K" target="_blank" rel="noopener noreferrer" class="flex items-center gap-2.5 min-w-0 group">
                    <span class="w-9 h-9 rounded-xl bg-cyanbrand text-white flex items-center justify-center shrink-0 group-hover:bg-navy transition-colors">
                      <svg class="w-4 h-4" fill="currentColor" viewBox="0 0 24 24"><path d="M12.04 2C6.58 2 2.13 6.45 2.13 11.91c0 1.75.46 3.45 1.32 4.95L2.05 22l5.25-1.38c1.45.79 3.08 1.21 4.74 1.21 5.46 0 9.91-4.45 9.91-9.91C21.95 6.45 17.5 2 12.04 2Zm5.82 14.01c-.24.68-1.41 1.3-1.96 1.38-.51.08-1.15.11-1.86-.11-.43-.14-.99-.32-1.7-.63-2.99-1.29-4.94-4.3-5.09-4.5-.15-.2-1.21-1.61-1.21-3.07 0-1.46.77-2.18 1.04-2.48.27-.3.59-.37.79-.37.2 0 .4 0 .57.01.18.01.43-.07.67.51.24.59.84 2.05.91 2.2.08.15.13.32.02.52-.1.2-.15.32-.3.5-.15.17-.31.38-.45.51-.15.15-.3.31-.13.61.17.3.77 1.27 1.65 2.05 1.13 1.01 2.09 1.32 2.39 1.47.3.15.47.12.65-.08.17-.2.74-.86.94-1.16.2-.3.4-.25.67-.15.27.1 1.73.82 2.03.97.3.15.5.22.57.34.07.12.07.7-.17 1.38Z"/></svg>
                    </span>
                    <div class="truncate">
                      <p class="text-xs font-heading font-extrabold text-navy truncate">Saluran WA</p>
                      <p class="text-[11px] text-slate-500 truncate">segitiga.id</p>
                    </div>
                  </a>
                  <button type="button" onclick="copyText('https://whatsapp.com/channel/0029Vb9QOPJ3LdQQIEvpWi0K', 'Tautan Saluran WhatsApp segitiga.id disalin!')" title="Salin tautan Saluran WhatsApp" aria-label="Salin tautan Saluran WhatsApp" class="p-2 rounded-lg text-slate-400 hover:text-navy hover:bg-ice transition-colors cursor-pointer shrink-0">
                    <svg class="w-4 h-4" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M8 16H6a2 2 0 01-2-2V6a2 2 0 012-2h8a2 2 0 012 2v2m-6 12h8a2 2 0 002-2v-8a2 2 0 00-2-2h-8a2 2 0 00-2 2v8a2 2 0 002 2z"/></svg>
                  </button>
                </div>
              </div>
            </div>
          </div>

          <!-- Kolom Kanan: Kartu Interaktif Identitas Logo & 3 Pilar Filosofi -->
          <div class="lg:col-span-5 reveal">
            <div class="bg-white rounded-[2rem] p-6 sm:p-8 shadow-soft-navy border border-slate-200/80">
              <div class="flex items-center justify-between mb-4">
                <span class="text-xs font-heading font-extrabold uppercase tracking-wider text-royal">Identitas Visual & Tiga Sisi</span>
                <div class="flex items-center gap-1.5">
                  <span class="w-2.5 h-2.5 rounded-full bg-navy"></span>
                  <span class="w-2.5 h-2.5 rounded-full bg-royal"></span>
                  <span class="w-2.5 h-2.5 rounded-full bg-cyanbrand"></span>
                </div>
              </div>

              <!-- Diagram SVG Logo Stacked segitiga.id -->
              <div class="flex flex-col items-center justify-center py-3 px-4 rounded-2xl bg-ice/70 border border-slate-200/60">
                <svg class="w-36 h-32 sm:w-40 sm:h-36" viewBox="0 0 240 215" fill="none" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Diagram Filosofi Logo segitiga.id">
                  <g transform="translate(10, 8)">
                    <path d="M104.2 17.5C106.8 13.1 113.2 13.1 115.8 17.5L196.4 157.2C199.0 161.7 195.8 167.3 190.6 167.3H29.4C24.2 167.3 21.0 161.7 23.6 157.2L104.2 17.5Z" fill="url(#segitigaLogoGrad)" />
                    <path d="M62 146C51 134 49 112 58 93C55 113 62 131 76 140L62 146Z" fill="#FFFFFF" />
                    <path d="M137 88C128 73 108 65 91 71C75 77 68 95 70 114C72 132 84 143 104 143C115 143 124 140 130 137C121 151 104 162 85 169H103C122 161 138 147 146 130C151 118 147 101 137 88Z" fill="#FFFFFF" />
                    <path d="M101 92.5C101 89.8 104.0 88.2 106.3 89.6L127.5 102.6C129.7 103.9 129.7 107.1 127.5 108.4L106.3 121.4C104.0 122.8 101 121.2 101 118.5V92.5Z" fill="url(#segitigaPlayGrad)" />
                    <path d="M97 135C121 121 146 93 169 55" stroke="#FFFFFF" stroke-width="14" stroke-linecap="round" />
                    <path d="M97 135C121 121 146 93 169 55" stroke="url(#segitigaLogoGrad)" stroke-width="7.5" stroke-linecap="round" />
                    <circle class="animate-signal" cx="172" cy="52" r="10.5" fill="#00B4D8" />
                  </g>

                  <!-- Penanda 3 Sisi Interaktif -->
                  <g id="highlightSide1" class="transition-opacity duration-300 opacity-100">
                    <circle cx="38" cy="174" r="13" fill="#0A2239" fill-opacity="0.2" />
                    <circle cx="38" cy="174" r="6.5" fill="#0A2239" stroke="#FFFFFF" stroke-width="2" />
                  </g>
                  <g id="highlightSide2" class="transition-opacity duration-300 opacity-40">
                    <circle cx="202" cy="174" r="13" fill="#0D4F8B" fill-opacity="0.2" />
                    <circle cx="202" cy="174" r="6.5" fill="#0D4F8B" stroke="#FFFFFF" stroke-width="2" />
                  </g>
                  <g id="highlightSide3" class="transition-opacity duration-300 opacity-40">
                    <circle cx="120" cy="24" r="13" fill="#00B4D8" fill-opacity="0.24" />
                    <circle cx="120" cy="24" r="6.5" fill="#00B4D8" stroke="#FFFFFF" stroke-width="2" />
                  </g>
                </svg>

                <!-- Wordmark -->
                <svg class="h-8 w-auto mt-1" viewBox="0 0 245 48" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <text x="4" y="36" fill="#0A2239" font-family="'Plus Jakarta Sans', sans-serif" font-weight="800" font-size="36" letter-spacing="-1.2">segitiga</text>
                  <polygon points="158,26 168,31.5 158,37" fill="#0A2239" />
                  <rect x="175" y="16" width="7.2" height="20" rx="1.5" fill="#00B4D8" />
                  <polygon points="175,4 185.5,9.5 175,15" fill="#00B4D8" />
                  <text x="188" y="36" fill="#00B4D8" font-family="'Plus Jakarta Sans', sans-serif" font-weight="800" font-size="36" letter-spacing="-1">d</text>
                </svg>
              </div>

              <!-- 3 Tombol Pilar Filosofi -->
              <div class="mt-4 grid grid-cols-3 gap-2">
                <button type="button" data-side="1" onclick="selectPhilosophy(1)" class="philosophy-tab active p-2.5 rounded-xl border border-slate-200 bg-slate-50/70 text-center transition-all cursor-pointer">
                  <span class="block text-[11px] font-heading font-extrabold text-navy">SISI 01</span>
                  <span class="block text-[11px] font-semibold text-slate-600 mt-0.5">Fakta</span>
                </button>
                <button type="button" data-side="2" onclick="selectPhilosophy(2)" class="philosophy-tab p-2.5 rounded-xl border border-slate-200 bg-slate-50/70 text-center transition-all cursor-pointer">
                  <span class="block text-[11px] font-heading font-extrabold text-royal">SISI 02</span>
                  <span class="block text-[11px] font-semibold text-slate-600 mt-0.5">Perspektif</span>
                </button>
                <button type="button" data-side="3" onclick="selectPhilosophy(3)" class="philosophy-tab p-2.5 rounded-xl border border-slate-200 bg-slate-50/70 text-center transition-all cursor-pointer">
                  <span class="block text-[11px] font-heading font-extrabold text-cyanbrand">SISI 03</span>
                  <span class="block text-[11px] font-semibold text-slate-600 mt-0.5">Konektivitas</span>
                </button>
              </div>

              <!-- Keterangan Dinamis Sisi Aktif -->
              <div class="mt-3 p-4 rounded-2xl bg-ice border border-slate-200/80">
                <div class="flex items-center justify-between gap-2 mb-1">
                  <span id="detailTitle" class="text-xs font-heading font-extrabold text-navy">Sisi 01 — Fakta & Kredibilitas</span>
                  <span id="detailColorBadge" class="px-2 py-0.5 rounded-md text-[10px] font-bold text-white bg-navy">#0A2239</span>
                </div>
                <p id="detailDesc" class="text-xs text-slatebody leading-relaxed">
                  Fondasi berita berdiri di atas verifikasi sumber primer, akurasi data, serta kepatuhan pada Kode Etik Jurnalistik.
                </p>
              </div>
            </div>
          </div>

        </div>
      </div>
    </section>

    <!-- =====================================================================
         3. SECTION "TENTANG SEGITIGA" (#tentang)
         ===================================================================== -->
    <section id="tentang" class="py-16 sm:py-24 bg-white">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="grid grid-cols-1 lg:grid-cols-12 gap-10 lg:gap-12 items-start">

          <!-- Narasi Utama Tentang SEGITIGA (Sesuai Dokumen Lampiran) -->
          <div class="lg:col-span-7 space-y-5 reveal">
            <span class="inline-block px-3.5 py-1.5 rounded-full bg-ice text-royal text-xs font-heading font-extrabold tracking-widest uppercase">
              Profil Redaksi
            </span>
            <h2 class="text-3xl sm:text-4xl font-extrabold text-navy tracking-tight">
              Tentang <span class="text-royal">SEGITIGA</span>
            </h2>

            <div class="space-y-4 text-base sm:text-[1.05rem] text-slatebody leading-relaxed">
              <p>
                <strong class="text-navy font-semibold">SEGITIGA</strong> merupakan media informasi digital yang hadir untuk menyajikan berbagai informasi, berita, dan perkembangan terkini dari tiga wilayah, yaitu <strong class="text-navy font-semibold">Purwakarta, Subang, dan Karawang (Purwasuka)</strong>.
              </p>
              <p>
                Kami hadir sebagai ruang informasi yang mengangkat berbagai peristiwa, potensi, serta dinamika kehidupan masyarakat. Mulai dari perkembangan pendidikan, kebudayaan, pariwisata, sosial, ekonomi, hingga kuliner dan fakta menarik di lingkungan sekitar.
              </p>
              <p>
                Melalui penyajian informasi yang aktual, menarik, dan mudah dipahami, <strong class="text-navy font-semibold">SEGITIGA</strong> berupaya menjadi media yang mendekatkan masyarakat dengan berbagai cerita dan perkembangan di wilayah Purwasuka.
              </p>
            </div>
          </div>

          <!-- 3 Poin Keunggulan Redaksi -->
          <div class="lg:col-span-5 space-y-4 reveal">
            <!-- Poin 1 -->
            <div class="p-5 sm:p-6 rounded-3xl bg-ice/80 border border-slate-200/80 flex items-start gap-4">
              <div class="w-11 h-11 rounded-2xl bg-navy text-cyanbrand flex items-center justify-center shrink-0">
                <svg class="w-6 h-6" fill="none" stroke="currentColor" stroke-width="2.2" viewBox="0 0 24 24">
                  <path stroke-linecap="round" stroke-linejoin="round" d="M9 12l2 2 4-4m5.618-4.016A11.955 11.955 0 0112 2.944a11.955 11.955 0 01-8.618 3.04A12.02 12.02 0 003 9c0 5.591 3.824 10.29 9 11.622 5.176-1.332 9-6.03 9-11.622 0-1.042-.133-2.052-.382-3.016z" />
                </svg>
              </div>
              <div>
                <h3 class="text-base font-extrabold text-navy mb-1">Berita Terverifikasi & Beretika</h3>
                <p class="text-sm text-slatebody leading-relaxed">
                  Disusun berpedoman pada Kode Etik Jurnalistik dan UU No. 40 Tahun 1999 tentang Pers untuk menangkal hoaks lokal.
                </p>
              </div>
            </div>

            <!-- Poin 2 -->
            <div class="p-5 sm:p-6 rounded-3xl bg-ice/80 border border-slate-200/80 flex items-start gap-4">
              <div class="w-11 h-11 rounded-2xl bg-royal text-white flex items-center justify-center shrink-0">
                <svg class="w-6 h-6" fill="none" stroke="currentColor" stroke-width="2.2" viewBox="0 0 24 24">
                  <path stroke-linecap="round" stroke-linejoin="round" d="M12 18h.01M8 21h8a2 2 0 002-2V5a2 2 0 00-2-2H8a2 2 0 00-2 2v14a2 2 0 002 2z" />
                </svg>
              </div>
              <div>
                <h3 class="text-base font-extrabold text-navy mb-1">Kemasan Ringkas & Visual Mobile-First</h3>
                <p class="text-sm text-slatebody leading-relaxed">
                  Informasi lengkap yang terhubung dengan ringkasan visual di TikTok, Instagram, dan Saluran WhatsApp.
                </p>
              </div>
            </div>

            <!-- Poin 3 -->
            <div class="p-5 sm:p-6 rounded-3xl bg-ice/80 border border-slate-200/80 flex items-start gap-4">
              <div class="w-11 h-11 rounded-2xl bg-cyanbrand text-white flex items-center justify-center shrink-0">
                <svg class="w-6 h-6" fill="none" stroke="currentColor" stroke-width="2.2" viewBox="0 0 24 24">
                  <path stroke-linecap="round" stroke-linejoin="round" d="M17 8h2a2 2 0 012 2v6a2 2 0 01-2 2h-2v4l-4-4H9a1.994 1.994 0 01-1.414-.586m0 0L11 14h4a2 2 0 002-2V6a2 2 0 00-2-2H5a2 2 0 00-2 2v6a2 2 0 002 2h2v4l.586-.586z" />
                </svg>
              </div>
              <div>
                <h3 class="text-base font-extrabold text-navy mb-1">Ruang Partisipasi & Hak Jawab Warga</h3>
                <p class="text-sm text-slatebody leading-relaxed">
                  Membuka ruang laporan warga, klarifikasi informasi publik, serta hak jawab secara terbuka dan proporsional.
                </p>
              </div>
            </div>
          </div>

        </div>
      </div>
    </section>

    <!-- =====================================================================
         4. SECTION "WILAYAH LIPUTAN KAMI" (PURWASUKA) (#wilayah)
         ===================================================================== -->
    <section id="wilayah" class="py-16 sm:py-24 bg-ice border-y border-slate-200/70">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">

        <div class="max-w-3xl mx-auto text-center space-y-3 reveal">
          <span class="inline-block px-3.5 py-1.5 rounded-full bg-white text-navy border border-slate-200 text-xs font-heading font-extrabold tracking-widest uppercase">
            Cakupan Tiga Kabupaten
          </span>
          <h2 class="text-3xl sm:text-4xl font-extrabold text-navy tracking-tight">
            Wilayah Liputan Kami
          </h2>
          <p class="text-base text-slatebody leading-relaxed">
            Tiga titik utama segitiga informasi <strong class="text-navy">Purwasuka</strong>. Pilih wilayah untuk menyaring berita dan cerita terkini dari masing-masing kabupaten.
          </p>
        </div>

        <div class="mt-12 grid grid-cols-1 md:grid-cols-3 gap-7">

          <!-- KARTU WILAYAH 1: PURWAKARTA -->
          <div class="reveal group bg-white rounded-3xl overflow-hidden border border-slate-200/90 hover:border-cyanbrand/60 shadow-sm hover:shadow-card-hover transition-all duration-300 flex flex-col justify-between">
            <div>
              <!-- Ilustrasi SVG Editorial Taman Air Mancur Sri Baduga Situ Buleud -->
              <div class="relative h-48 bg-navy overflow-hidden">
                <svg class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500" viewBox="0 0 400 220" fill="none" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Ilustrasi Taman Air Mancur Sri Baduga Purwakarta">
                  <rect width="400" height="220" fill="#061524" />
                  <!-- Sorotan Cahaya Malam -->
                  <polygon points="200,130 90,10 155,10" fill="#00B4D8" fill-opacity="0.16" />
                  <polygon points="200,130 245,10 310,10" fill="#0D4F8B" fill-opacity="0.25" />
                  <polygon points="200,130 175,5 225,5" fill="#48CAE4" fill-opacity="0.22" />
                  <!-- Semburan Air Mancur -->
                  <path d="M200 142C200 95 200 55 200 32" stroke="#48CAE4" stroke-width="4" stroke-linecap="round" />
                  <path d="M185 142C175 100 158 68 140 50" stroke="#00B4D8" stroke-width="3" stroke-linecap="round" />
                  <path d="M215 142C225 100 242 68 260 50" stroke="#00B4D8" stroke-width="3" stroke-linecap="round" />
                  <path d="M170 144C152 112 125 88 98 76" stroke="#38BDF8" stroke-width="2.5" stroke-linecap="round" stroke-opacity="0.8" />
                  <path d="M230 144C248 112 275 88 302 76" stroke="#38BDF8" stroke-width="2.5" stroke-linecap="round" stroke-opacity="0.8" />
                  <path d="M155 146C130 124 95 110 65 104" stroke="#0EA5E9" stroke-width="2" stroke-linecap="round" stroke-opacity="0.65" />
                  <path d="M245 146C270 124 305 110 335 104" stroke="#0EA5E9" stroke-width="2" stroke-linecap="round" stroke-opacity="0.65" />
                  <!-- Siluet Patung Teratai Sri Baduga -->
                  <path d="M174 146L185 132L200 142L215 132L226 146H174Z" fill="#00B4D8" />
                  <circle cx="200" cy="112" r="7" fill="#E0F7FC" />
                  <path d="M189 133C189 124 194 120 200 120C206 120 211 124 211 133H189Z" fill="#E0F7FC" />
                  <!-- Permukaan Air Situ Buleud & Refleksi -->
                  <rect y="146" width="400" height="74" fill="#0A2239" />
                  <ellipse cx="200" cy="164" rx="135" ry="12" fill="#00B4D8" fill-opacity="0.22" />
                  <ellipse cx="200" cy="186" rx="95" ry="8" fill="#48CAE4" fill-opacity="0.18" />
                  <!-- Dermaga Tengah -->
                  <polygon points="184,220 193,152 207,152 216,220" fill="#061524" stroke="#1E3A5F" stroke-width="1.5" />
                </svg>
                <span class="absolute top-4 left-4 px-3 py-1 rounded-full bg-navy/85 backdrop-blur-sm border border-cyanbrand/40 text-cyanbrand text-xs font-heading font-extrabold">
                  WILAYAH 01
                </span>
              </div>

              <div class="p-6">
                <h3 class="text-xl font-extrabold text-navy mb-2">Purwakarta</h3>
                <p class="text-sm text-slatebody leading-relaxed">
                  Ikon Taman Air Mancur Sri Baduga Situ Buleud, pusat kegiatan budaya, destinasi wisata kota, serta simpul penghubung strategis Purwasuka.
                </p>
              </div>
            </div>

            <div class="px-6 pb-6">
              <button
                type="button"
                onclick="filterNewsByRegion('Purwakarta')"
                class="w-full inline-flex items-center justify-center gap-2 px-4 py-3 rounded-xl bg-ice hover:bg-navy text-navy hover:text-white font-heading text-xs sm:text-sm font-bold transition-colors cursor-pointer"
              >
                <span>Lihat Berita Purwakarta</span>
                <svg class="w-3.5 h-3.5" viewBox="0 0 16 16" fill="currentColor"><path d="M4 2.5L13 8L4 13.5V2.5Z"/></svg>
              </button>
            </div>
          </div>

          <!-- KARTU WILAYAH 2: SUBANG -->
          <div class="reveal group bg-white rounded-3xl overflow-hidden border border-slate-200/90 hover:border-cyanbrand/60 shadow-sm hover:shadow-card-hover transition-all duration-300 flex flex-col justify-between">
            <div>
              <!-- Ilustrasi SVG Editorial Kebun Teh Ciater & Pegunungan Subang -->
              <div class="relative h-48 bg-sky-100 overflow-hidden">
                <svg class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500" viewBox="0 0 400 220" fill="none" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Ilustrasi Kebun Teh dan Pegunungan Subang">
                  <defs>
                    <linearGradient id="subangSky" x1="0" y1="0" x2="0" y2="1">
                      <stop offset="0%" stop-color="#BAE6FD" />
                      <stop offset="100%" stop-color="#F0F9FF" />
                    </linearGradient>
                  </defs>
                  <rect width="400" height="220" fill="url(#subangSky)" />
                  <!-- Gunung Tangkuban Parahu / Pegunungan Selatan Subang -->
                  <path d="M0 120L95 55L170 92L255 46L345 88L400 72V160H0V120Z" fill="#1E4E68" fill-opacity="0.45" />
                  <path d="M40 135L145 72L230 112L320 68L400 105V175H40V135Z" fill="#0D4F8B" fill-opacity="0.55" />
                  <!-- Bukit Perkebunan Teh Terasering -->
                  <path d="M0 132C95 112 185 128 280 148C335 160 375 152 400 145V220H0V132Z" fill="#15803D" />
                  <path d="M0 154C110 138 210 162 400 142V220H0V154Z" fill="#166534" />
                  <path d="M0 176C130 164 255 182 400 168V220H0V176Z" fill="#14532D" />
                  <!-- Garis Alur Kebun Teh -->
                  <path d="M18 148C105 135 185 150 265 164" stroke="#4ADE80" stroke-width="2" stroke-opacity="0.45" stroke-dasharray="6 4" />
                  <path d="M140 166C230 156 315 162 385 155" stroke="#4ADE80" stroke-width="2" stroke-opacity="0.45" stroke-dasharray="6 4" />
                </svg>
                <span class="absolute top-4 left-4 px-3 py-1 rounded-full bg-navy/85 backdrop-blur-sm border border-cyanbrand/40 text-cyanbrand text-xs font-heading font-extrabold">
                  WILAYAH 02
                </span>
              </div>

              <div class="p-6">
                <h3 class="text-xl font-extrabold text-navy mb-2">Subang</h3>
                <p class="text-sm text-slatebody leading-relaxed">
                  Hamparan kebun teh Ciater, wisata alam Curug Cileat & Sari Ater, serta dinamika pertumbuhan kawasan industri dan kelestarian lingkungan.
                </p>
              </div>
            </div>

            <div class="px-6 pb-6">
              <button
                type="button"
                onclick="filterNewsByRegion('Subang')"
                class="w-full inline-flex items-center justify-center gap-2 px-4 py-3 rounded-xl bg-ice hover:bg-royal text-navy hover:text-white font-heading text-xs sm:text-sm font-bold transition-colors cursor-pointer"
              >
                <span>Lihat Berita Subang</span>
                <svg class="w-3.5 h-3.5" viewBox="0 0 16 16" fill="currentColor"><path d="M4 2.5L13 8L4 13.5V2.5Z"/></svg>
              </button>
            </div>
          </div>

          <!-- KARTU WILAYAH 3: KARAWANG -->
          <div class="reveal group bg-white rounded-3xl overflow-hidden border border-slate-200/90 hover:border-cyanbrand/60 shadow-sm hover:shadow-card-hover transition-all duration-300 flex flex-col justify-between">
            <div>
              <!-- Ilustrasi SVG Editorial Hamparan Sawah Lumbung Padi Karawang -->
              <div class="relative h-48 bg-amber-50 overflow-hidden">
                <svg class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500" viewBox="0 0 400 220" fill="none" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Ilustrasi Hamparan Sawah dan Kawasan Karawang">
                  <defs>
                    <linearGradient id="karawangSky" x1="0" y1="0" x2="0" y2="1">
                      <stop offset="0%" stop-color="#E0F2FE" />
                      <stop offset="100%" stop-color="#FEF3C7" />
                    </linearGradient>
                  </defs>
                  <rect width="400" height="220" fill="url(#karawangSky)" />
                  <!-- Matahari Pagi -->
                  <circle cx="315" cy="54" r="24" fill="#FDE68A" />
                  <!-- Siluet Kawasan & Permukiman di Cakrawala -->
                  <rect x="35" y="92" width="26" height="24" fill="#94A3B8" fill-opacity="0.45" />
                  <rect x="65" y="86" width="34" height="30" fill="#64748B" fill-opacity="0.45" />
                  <rect x="104" y="96" width="22" height="20" fill="#94A3B8" fill-opacity="0.45" />
                  <!-- Hamparan Petak Sawah Hijau -->
                  <rect y="114" width="400" height="106" fill="#22C55E" />
                  <polygon points="0,114 150,114 95,220 0,220" fill="#16A34A" />
                  <polygon points="150,114 275,114 315,220 95,220" fill="#15803D" />
                  <polygon points="275,114 400,114 400,220 315,220" fill="#22C55E" />
                  <!-- Pematang Sawah -->
                  <line x1="150" y1="114" x2="95" y2="220" stroke="#ECFCCB" stroke-width="3" />
                  <line x1="275" y1="114" x2="315" y2="220" stroke="#ECFCCB" stroke-width="3" />
                  <line x1="0" y1="158" x2="400" y2="164" stroke="#ECFCCB" stroke-width="2.5" />
                </svg>
                <span class="absolute top-4 left-4 px-3 py-1 rounded-full bg-navy/85 backdrop-blur-sm border border-cyanbrand/40 text-cyanbrand text-xs font-heading font-extrabold">
                  WILAYAH 03
                </span>
              </div>

              <div class="p-6">
                <h3 class="text-xl font-extrabold text-navy mb-2">Karawang</h3>
                <p class="text-sm text-slatebody leading-relaxed">
                  Lumbung padi Jawa Barat dengan hamparan sawah hijau, pusat industri strategis, inovasi mahasiswa kampus, dan ragam kuliner khas.
                </p>
              </div>
            </div>

            <div class="px-6 pb-6">
              <button
                type="button"
                onclick="filterNewsByRegion('Karawang')"
                class="w-full inline-flex items-center justify-center gap-2 px-4 py-3 rounded-xl bg-ice hover:bg-cyanbrand text-navy hover:text-white font-heading text-xs sm:text-sm font-bold transition-colors cursor-pointer"
              >
                <span>Lihat Berita Karawang</span>
                <svg class="w-3.5 h-3.5" viewBox="0 0 16 16" fill="currentColor"><path d="M4 2.5L13 8L4 13.5V2.5Z"/></svg>
              </button>
            </div>
          </div>

        </div>
      </div>
    </section>

    <!-- =====================================================================
         5. SECTION "APA YANG KAMI SAJIKAN?" (7 RUBRIK RESMI) (#rubrik)
         ===================================================================== -->
    <section id="rubrik" class="py-16 sm:py-24 bg-white">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">

        <div class="max-w-3xl mx-auto text-center space-y-3 reveal">
          <span class="inline-block px-3.5 py-1.5 rounded-full bg-ice text-royal text-xs font-heading font-extrabold tracking-widest uppercase">
            Tujuh Kanal Informasi
          </span>
          <h2 class="text-3xl sm:text-4xl font-extrabold text-navy tracking-tight">
            Apa yang Kami Sajikan?
          </h2>
          <p class="text-base text-slatebody leading-relaxed">
            Tujuh rubrik utama <strong class="text-navy">segitiga.id</strong> dirancang untuk menjawab kebutuhan informasi warga Purwasuka. Klik kartu rubrik untuk menyaring sajian berita di bawah.
          </p>
        </div>

        <!-- Grid 7 Kartu Rubrik Interaktif -->
        <div class="mt-12 grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-5">

          <!-- 1. Purwasuka Hari Ini -->
          <button type="button" onclick="selectRubrikFromCard('Purwasuka Hari Ini')" class="reveal text-left group p-6 rounded-3xl bg-ice/75 hover:bg-white border border-slate-200/80 hover:border-navy shadow-sm hover:shadow-card-hover transition-all duration-300 cursor-pointer">
            <div class="w-11 h-11 rounded-2xl bg-navy text-cyanbrand flex items-center justify-center mb-4 group-hover:scale-105 transition-transform">
              <svg class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="2.2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M19 20H5a2 2 0 01-2-2V6a2 2 0 012-2h10a2 2 0 012 2v1m2 13a2 2 0 01-2-2V7m2 13a2 2 0 002-2V9a2 2 0 00-2-2h-2"/></svg>
            </div>
            <h3 class="text-base font-extrabold text-navy mb-1.5">Purwasuka Hari Ini</h3>
            <p class="text-sm text-slatebody leading-relaxed">Informasi dan peristiwa terkini.</p>
          </button>

          <!-- 2. Purwasuka Pendidikan -->
          <button type="button" onclick="selectRubrikFromCard('Purwasuka Pendidikan')" class="reveal text-left group p-6 rounded-3xl bg-ice/75 hover:bg-white border border-slate-200/80 hover:border-royal shadow-sm hover:shadow-card-hover transition-all duration-300 cursor-pointer">
            <div class="w-11 h-11 rounded-2xl bg-royal text-white flex items-center justify-center mb-4 group-hover:scale-105 transition-transform">
              <svg class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="2.2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M12 14l9-5-9-5-9 5 9 5z"/><path stroke-linecap="round" stroke-linejoin="round" d="M12 14l6.16-3.422a12.083 12.083 0 01.665 6.479A11.952 11.952 0 0012 20.055a11.952 11.952 0 00-6.824-2.998 12.078 12.078 0 01.665-6.479L12 14z"/></svg>
            </div>
            <h3 class="text-base font-extrabold text-navy mb-1.5">Purwasuka Pendidikan</h3>
            <p class="text-sm text-slatebody leading-relaxed">Prestasi, kegiatan, dan perkembangan dunia pendidikan.</p>
          </button>

          <!-- 3. Purwasuka Budaya & Wisata -->
          <button type="button" onclick="selectRubrikFromCard('Purwasuka Budaya & Wisata')" class="reveal text-left group p-6 rounded-3xl bg-ice/75 hover:bg-white border border-slate-200/80 hover:border-cyanbrand shadow-sm hover:shadow-card-hover transition-all duration-300 cursor-pointer">
            <div class="w-11 h-11 rounded-2xl bg-cyanbrand text-white flex items-center justify-center mb-4 group-hover:scale-105 transition-transform">
              <svg class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="2.2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M3.055 11H5a2 2 0 012 2v1a2 2 0 002 2 2 2 0 012 2v2.945M8 3.935V5.5A2.5 2.5 0 0010.5 8h.5a2 2 0 012 2 2 2 0 104 0 2 2 0 012-2h1.064M15 20.488V18a2 2 0 012-2h3.064M21 12a9 9 0 11-18 0 9 9 0 0118 0z"/></svg>
            </div>
            <h3 class="text-base font-extrabold text-navy mb-1.5">Purwasuka Budaya & Wisata</h3>
            <p class="text-sm text-slatebody leading-relaxed">Event, kebudayaan, dan destinasi wisata.</p>
          </button>

          <!-- 4. Purwasuka Sosial -->
          <button type="button" onclick="selectRubrikFromCard('Purwasuka Sosial')" class="reveal text-left group p-6 rounded-3xl bg-ice/75 hover:bg-white border border-slate-200/80 hover:border-royal shadow-sm hover:shadow-card-hover transition-all duration-300 cursor-pointer">
            <div class="w-11 h-11 rounded-2xl bg-navy text-white flex items-center justify-center mb-4 group-hover:scale-105 transition-transform">
              <svg class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="2.2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M17 20h5v-2a3 3 0 00-5.356-1.857M17 20H7m10 0v-2c0-.656-.126-1.283-.356-1.857M7 20H2v-2a3 3 0 015.356-1.857M7 20v-2c0-.656.126-1.283.356-1.857m0 0a5.002 5.002 0 019.288 0M15 7a3 3 0 11-6 0 3 3 0 016 0z"/></svg>
            </div>
            <h3 class="text-base font-extrabold text-navy mb-1.5">Purwasuka Sosial</h3>
            <p class="text-sm text-slatebody leading-relaxed">Isu sosial dan kehidupan masyarakat.</p>
          </button>

          <!-- 5. Purwasuka Ekonomi -->
          <button type="button" onclick="selectRubrikFromCard('Purwasuka Ekonomi')" class="reveal text-left group p-6 rounded-3xl bg-ice/75 hover:bg-white border border-slate-200/80 hover:border-royal shadow-sm hover:shadow-card-hover transition-all duration-300 cursor-pointer">
            <div class="w-11 h-11 rounded-2xl bg-royal text-cyanbrand flex items-center justify-center mb-4 group-hover:scale-105 transition-transform">
              <svg class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="2.2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M13 7h8m0 0v8m0-8l-8 8-4-4-6 6"/></svg>
            </div>
            <h3 class="text-base font-extrabold text-navy mb-1.5">Purwasuka Ekonomi</h3>
            <p class="text-sm text-slatebody leading-relaxed">Informasi ekonomi, UMK, bisnis, dan ketenagakerjaan.</p>
          </button>

          <!-- 6. Purwasuka Rasa -->
          <button type="button" onclick="selectRubrikFromCard('Purwasuka Rasa')" class="reveal text-left group p-6 rounded-3xl bg-ice/75 hover:bg-white border border-slate-200/80 hover:border-cyanbrand shadow-sm hover:shadow-card-hover transition-all duration-300 cursor-pointer">
            <div class="w-11 h-11 rounded-2xl bg-cyanbrand/15 text-royal flex items-center justify-center mb-4 group-hover:scale-105 transition-transform">
              <svg class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="2.2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M12 8c-1.657 0-3 .895-3 2s1.343 2 3 2 3 .895 3 2-1.343 2-3 2m0-8c1.11 0 2.08.402 2.599 1M12 8V7m0 1v8m0 0v1m0-1c-1.11 0-2.08-.402-2.599-1M21 12a9 9 0 11-18 0 9 9 0 0118 0z"/></svg>
            </div>
            <h3 class="text-base font-extrabold text-navy mb-1.5">Purwasuka Rasa</h3>
            <p class="text-sm text-slatebody leading-relaxed">Kuliner dan rekomendasi tempat makan.</p>
          </button>

          <!-- 7. Purwasuka Fakta -->
          <button type="button" onclick="selectRubrikFromCard('Purwasuka Fakta')" class="reveal sm:col-span-2 lg:col-span-2 text-left group p-6 rounded-3xl bg-gradient-to-r from-navy to-royal text-white border border-navy shadow-sm hover:shadow-card-hover transition-all duration-300 cursor-pointer flex items-center justify-between gap-4">
            <div>
              <div class="inline-flex items-center gap-2 px-2.5 py-0.5 rounded-full bg-cyanbrand/20 text-cyanbrand text-[11px] font-heading font-extrabold uppercase tracking-wider mb-2">
                <span>Cek Fakta & Hak Jawab</span>
              </div>
              <h3 class="text-lg font-extrabold text-white mb-1">Purwasuka Fakta</h3>
              <p class="text-sm text-slate-200 leading-relaxed">Klarifikasi informasi, fakta, dan hak jawab.</p>
            </div>
            <div class="w-12 h-12 rounded-2xl bg-cyanbrand text-navy flex items-center justify-center shrink-0 group-hover:scale-105 transition-transform">
              <svg class="w-6 h-6" fill="none" stroke="currentColor" stroke-width="2.5" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M5 13l4 4L19 7"/></svg>
            </div>
          </button>

        </div>
      </div>
    </section>

    <!-- =====================================================================
         6. SECTION "BERITA PURWASUKA" (PORTAL BERITA 8 ARTIKEL LENGKAP) (#berita)
         ===================================================================== -->
    <section id="berita" class="py-16 sm:py-24 bg-[#F8FAFC] border-t border-slate-200/80">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">

        <!-- Header Portal Berita -->
        <div class="flex flex-col md:flex-row md:items-end justify-between gap-6 mb-8 reveal">
          <div>
            <span class="inline-block px-3.5 py-1.5 rounded-full bg-white text-royal border border-slate-200 text-xs font-heading font-extrabold tracking-widest uppercase mb-3">
              Sajian Berita Redaksi
            </span>
            <h2 class="text-3xl sm:text-4xl font-extrabold text-navy tracking-tight">
              Berita Purwasuka
            </h2>
            <p class="text-sm sm:text-base text-slatebody mt-1">
              Kumpulan liputan terkini, prestasi pendidikan, wisata, ekonomi, kuliner, dan klarifikasi fakta dari Purwakarta, Subang, dan Karawang.
            </p>
          </div>

          <!-- Kolom Pencarian & Filter Wilayah -->
          <div class="flex flex-col sm:flex-row items-stretch sm:items-center gap-3 w-full md:w-auto">
            <!-- Filter Wilayah -->
            <div class="relative">
              <select
                id="regionFilterSelect"
                aria-label="Filter Wilayah Berita"
                onchange="handleRegionSelect(this.value)"
                class="w-full sm:w-44 appearance-none px-4 py-3 pr-9 rounded-2xl bg-white border border-slate-200 text-sm font-heading font-bold text-navy focus:outline-none focus:border-cyanbrand cursor-pointer"
              >
                <option value="Semua">Semua Wilayah</option>
                <option value="Purwakarta">Purwakarta</option>
                <option value="Subang">Subang</option>
                <option value="Karawang">Karawang</option>
                <option value="Purwasuka">Lintas Purwasuka</option>
              </select>
              <svg class="w-4 h-4 text-slate-400 pointer-events-none absolute right-3.5 top-1/2 -translate-y-1/2" fill="none" stroke="currentColor" stroke-width="2.2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M19 9l-7 7-7-7"/></svg>
            </div>

            <!-- Kolom Pencarian -->
            <div class="relative flex-1 sm:w-64">
              <input
                id="newsSearchInput"
                type="search"
                placeholder="Cari judul atau topik berita..."
                oninput="handleSearchInput(this.value)"
                class="w-full pl-10 pr-4 py-3 rounded-2xl bg-white border border-slate-200 text-sm text-navy placeholder:text-slate-400 focus:outline-none focus:border-cyanbrand"
              />
              <svg class="w-4 h-4 text-slate-400 absolute left-3.5 top-1/2 -translate-y-1/2" fill="none" stroke="currentColor" stroke-width="2.2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M21 21l-6-6m2-5a7 7 0 11-14 0 7 7 0 0114 0z"/></svg>
            </div>
          </div>
        </div>

        <!-- Bar Filter Tab Rubrik -->
        <div class="flex items-center gap-2 overflow-x-auto no-scrollbar pb-3 mb-8" role="tablist" aria-label="Filter Rubrik Berita">
          <button type="button" data-rubrik="Semua" onclick="setRubrikFilter('Semua')" class="rubrik-tab shrink-0 px-4 py-2.5 rounded-xl text-xs sm:text-sm font-heading font-bold bg-navy text-white transition-all cursor-pointer">
            Semua Rubrik (8)
          </button>
          <button type="button" data-rubrik="Purwasuka Hari Ini" onclick="setRubrikFilter('Purwasuka Hari Ini')" class="rubrik-tab shrink-0 px-4 py-2.5 rounded-xl text-xs sm:text-sm font-heading font-bold bg-white text-slatebody border border-slate-200 hover:border-navy transition-all cursor-pointer">
            Purwasuka Hari Ini
          </button>
          <button type="button" data-rubrik="Purwasuka Pendidikan" onclick="setRubrikFilter('Purwasuka Pendidikan')" class="rubrik-tab shrink-0 px-4 py-2.5 rounded-xl text-xs sm:text-sm font-heading font-bold bg-white text-slatebody border border-slate-200 hover:border-navy transition-all cursor-pointer">
            Purwasuka Pendidikan
          </button>
          <button type="button" data-rubrik="Purwasuka Budaya & Wisata" onclick="setRubrikFilter('Purwasuka Budaya & Wisata')" class="rubrik-tab shrink-0 px-4 py-2.5 rounded-xl text-xs sm:text-sm font-heading font-bold bg-white text-slatebody border border-slate-200 hover:border-navy transition-all cursor-pointer">
            Purwasuka Budaya & Wisata
          </button>
          <button type="button" data-rubrik="Purwasuka Sosial" onclick="selectRubrikTab('Purwasuka Sosial')" class="rubrik-tab shrink-0 px-4 py-2.5 rounded-xl text-xs sm:text-sm font-heading font-bold bg-white text-slatebody border border-slate-200 hover:border-navy transition-all cursor-pointer">
            Purwasuka Sosial
          </button>
          <button type="button" data-rubrik="Purwasuka Ekonomi" onclick="setRubrikFilter('Purwasuka Ekonomi')" class="rubrik-tab shrink-0 px-4 py-2.5 rounded-xl text-xs sm:text-sm font-heading font-bold bg-white text-slatebody border border-slate-200 hover:border-navy transition-all cursor-pointer">
            Purwasuka Ekonomi
          </button>
          <button type="button" data-rubrik="Purwasuka Rasa" onclick="setRubrikFilter('Purwasuka Rasa')" class="rubrik-tab shrink-0 px-4 py-2.5 rounded-xl text-xs sm:text-sm font-heading font-bold bg-white text-slatebody border border-slate-200 hover:border-navy transition-all cursor-pointer">
            Purwasuka Rasa
          </button>
          <button type="button" data-rubrik="Purwasuka Fakta" onclick="setRubrikFilter('Purwasuka Fakta')" class="rubrik-tab shrink-0 px-4 py-2.5 rounded-xl text-xs sm:text-sm font-heading font-bold bg-white text-slatebody border border-slate-200 hover:border-navy transition-all cursor-pointer">
            Purwasuka Fakta
          </button>
        </div>

        <!-- Status Filter Aktif -->
        <div id="filterStatusBar" class="hidden mb-6 flex flex-wrap items-center justify-between gap-3 px-4 py-3 rounded-2xl bg-white border border-cyanbrand/40 text-xs sm:text-sm">
          <p id="filterStatusText" class="font-semibold text-navy"></p>
          <button type="button" onclick="resetAllFilters()" class="font-heading font-bold text-royal hover:text-cyanbrand underline cursor-pointer">
            Tampilkan Semua Berita
          </button>
        </div>

        <!-- Kontainer Berita Utama (Featured Headline) -->
        <div id="featuredNewsContainer" class="mb-8"></div>

        <!-- Kontainer Grid Kartu Berita -->
        <div id="newsGridContainer" class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-7"></div>

        <!-- State Kosong Jika Pencarian Tidak Ditemukan -->
        <div id="emptyNewsState" class="hidden text-center py-16 px-6 rounded-3xl bg-white border border-slate-200">
          <div class="w-14 h-14 rounded-2xl bg-ice text-royal flex items-center justify-center mx-auto mb-4">
            <svg class="w-7 h-7" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M9.172 16.172a4 4 0 015.656 0M9 10h.01M15 10h.01M21 12a9 9 0 11-18 0 9 9 0 0118 0z"/></svg>
          </div>
          <h3 class="text-lg font-extrabold text-navy mb-1">Berita Tidak Ditemukan</h3>
          <p class="text-sm text-slatebody mb-5">Tidak ada artikel yang cocok dengan kata kunci atau filter wilayah/rubrik yang Anda pilih.</p>
          <button type="button" onclick="resetAllFilters()" class="px-5 py-2.5 rounded-xl bg-navy text-white font-heading text-xs font-bold hover:bg-royal transition-colors cursor-pointer">
            Atur Ulang Filter
          </button>
        </div>

      </div>
    </section>

    <!-- =====================================================================
         7. SECTION "HUBUNGI KAMI" & 3 KANAL RESMI SEGITIGA.ID (#kontak)
         ===================================================================== -->
    <section id="kontak" class="py-16 sm:py-24 bg-white border-t border-slate-200/70">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">

        <div class="max-w-3xl mx-auto text-center space-y-3 reveal mb-12">
          <span class="inline-block px-3.5 py-1.5 rounded-full bg-ice text-royal text-xs font-heading font-extrabold tracking-widest uppercase">
            Layanan Warga & Kemitraan
          </span>
          <h2 class="text-3xl sm:text-4xl font-extrabold text-navy tracking-tight">
            Hubungi Kami
          </h2>
          <p class="text-base sm:text-lg text-slatebody leading-relaxed">
            Punya informasi, berita, kritik, saran, atau ingin bekerja sama dengan SEGITIGA? Hubungi tim redaksi kami melalui kontak berikut.
          </p>
        </div>

        <div class="grid grid-cols-1 lg:grid-cols-12 gap-8 items-start">

          <!-- Kolom Kiri: Contact Person Redaksi & 3 Saluran Resmi -->
          <div class="lg:col-span-5 space-y-6 reveal">

            <!-- Kartu Contact Person Redaksi SEGITIGA -->
            <div class="rounded-3xl bg-navy text-white p-6 sm:p-8 shadow-soft-navy relative overflow-hidden">
              <div class="pointer-events-none absolute -right-10 -bottom-10 w-44 h-44 opacity-10">
                <svg viewBox="0 0 200 200" fill="none"><polygon points="100,10 190,175 10,175" stroke="#00B4D8" stroke-width="16"/></svg>
              </div>

              <span class="inline-block px-3 py-1 rounded-full bg-cyanbrand/20 text-cyanbrand text-xs font-heading font-extrabold uppercase tracking-wider mb-3">
                Contact Person
              </span>
              <h3 class="text-2xl font-extrabold text-white mb-5">Redaksi SEGITIGA</h3>

              <div class="space-y-4 relative z-10">
                <!-- Nomor WhatsApp -->
                <div class="p-4 rounded-2xl bg-white/10 border border-white/15 flex items-center justify-between gap-3">
                  <div class="min-w-0">
                    <p class="text-xs text-slate-300 font-medium">Nomor WhatsApp</p>
                    <a href="https://wa.me/6281234567890" target="_blank" rel="noopener noreferrer" class="text-base sm:text-lg font-heading font-extrabold text-cyanbrand hover:underline">
                      081234567890
                    </a>
                  </div>
                  <div class="flex items-center gap-2 shrink-0">
                    <button type="button" onclick="copyText('081234567890', 'Nomor WhatsApp 081234567890 berhasil disalin!')" title="Salin Nomor WhatsApp" aria-label="Salin Nomor WhatsApp" class="p-2.5 rounded-xl bg-white/10 hover:bg-white/20 text-white transition-colors cursor-pointer">
                      <svg class="w-4 h-4" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M8 16H6a2 2 0 01-2-2V6a2 2 0 012-2h8a2 2 0 012 2v2m-6 12h8a2 2 0 002-2v-8a2 2 0 00-2-2h-8a2 2 0 00-2 2v8a2 2 0 002 2z"/></svg>
                    </button>
                    <a href="https://wa.me/6281234567890" target="_blank" rel="noopener noreferrer" class="px-3.5 py-2 rounded-xl bg-emerald-500 hover:bg-emerald-400 text-navy font-heading text-xs font-extrabold transition-colors">
                      Chat WA
                    </a>
                  </div>
                </div>

                <!-- Email Redaksi -->
                <div class="p-4 rounded-2xl bg-white/10 border border-white/15 flex items-center justify-between gap-3">
                  <div class="min-w-0">
                    <p class="text-xs text-slate-300 font-medium">Email Redaksi</p>
                    <a href="mailto:redaksi.segitiga@gmail.com" class="text-sm sm:text-base font-heading font-extrabold text-white hover:text-cyanbrand truncate block">
                      redaksi.segitiga@gmail.com
                    </a>
                  </div>
                  <div class="flex items-center gap-2 shrink-0">
                    <button type="button" onclick="copyText('redaksi.segitiga@gmail.com', 'Email redaksi.segitiga@gmail.com berhasil disalin!')" title="Salin Email Redaksi" aria-label="Salin Email Redaksi" class="p-2.5 rounded-xl bg-white/10 hover:bg-white/20 text-white transition-colors cursor-pointer">
                      <svg class="w-4 h-4" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M8 16H6a2 2 0 01-2-2V6a2 2 0 012-2h8a2 2 0 012 2v2m-6 12h8a2 2 0 002-2v-8a2 2 0 00-2-2h-8a2 2 0 00-2 2v8a2 2 0 002 2z"/></svg>
                    </button>
                    <a href="mailto:redaksi.segitiga@gmail.com" class="px-3.5 py-2 rounded-xl bg-cyanbrand hover:bg-cyanbrand-light text-navy font-heading text-xs font-extrabold transition-colors">
                      Email
                    </a>
                  </div>
                </div>
              </div>
            </div>

            <!-- Kartu 3 Saluran Resmi SEGITIGA.ID (HANYA 3) -->
            <div class="rounded-3xl bg-ice p-6 sm:p-7 border border-slate-200/90">
              <h4 class="text-base font-extrabold text-navy mb-1">3 Saluran Resmi SEGITIGA.ID</h4>
              <p class="text-xs text-slatebody mb-4">Ikuti pembaruan berita dan video singkat kami hanya melalui akun resmi berikut:</p>

              <div class="space-y-3">
                <!-- 1. TikTok -->
                <div class="flex items-center justify-between gap-3 p-3.5 rounded-2xl bg-white border border-slate-200/80">
                  <div class="flex items-center gap-3 min-w-0">
                    <span class="w-10 h-10 rounded-xl bg-navy text-cyanbrand flex items-center justify-center shrink-0">
                      <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24"><path d="M16.6 5.82A4.28 4.28 0 0 1 15.54 3h-3.09v12.4a2.59 2.59 0 0 1-2.59 2.5c-1.42 0-2.6-1.16-2.6-2.6 0-1.72 1.66-3.01 3.37-2.48V9.66c-3.45-.46-6.47 2.22-6.47 5.64 0 3.33 2.76 5.7 5.69 5.7 3.14 0 5.69-2.55 5.69-5.7V9.01a7.35 7.35 0 0 0 4.3 1.38V7.3s-1.88.09-3.24-1.48Z"/></svg>
                    </span>
                    <div class="truncate">
                      <p class="text-sm font-heading font-extrabold text-navy">TikTok</p>
                      <p class="text-xs text-slate-500 truncate">@redaksi.segitiga</p>
                    </div>
                  </div>
                  <div class="flex items-center gap-1.5 shrink-0">
                    <button type="button" onclick="copyText('https://www.tiktok.com/@redaksi.segitiga?_r=1&_t=ZS-9Bf5fEpCAP0', 'Tautan TikTok disalin!')" class="px-2.5 py-1.5 rounded-xl bg-ice hover:bg-slate-200/70 text-navy text-xs font-bold cursor-pointer">Salin</button>
                    <a href="https://www.tiktok.com/@redaksi.segitiga?_r=1&_t=ZS-9Bf5fEpCAP0" target="_blank" rel="noopener noreferrer" class="px-3.5 py-1.5 rounded-xl bg-navy hover:bg-royal text-white font-heading text-xs font-bold transition-colors">Buka</a>
                  </div>
                </div>

                <!-- 2. Instagram -->
                <div class="flex items-center justify-between gap-3 p-3.5 rounded-2xl bg-white border border-slate-200/80">
                  <div class="flex items-center gap-3 min-w-0">
                    <span class="w-10 h-10 rounded-xl bg-royal text-white flex items-center justify-center shrink-0">
                      <svg class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><rect x="2" y="2" width="20" height="20" rx="5"/><circle cx="12" cy="12" r="4"/><circle cx="17.5" cy="6.5" r="1" fill="currentColor" stroke="none"/></svg>
                    </span>
                    <div class="truncate">
                      <p class="text-sm font-heading font-extrabold text-navy">Instagram</p>
                      <p class="text-xs text-slate-500 truncate">@redaksi.segitiga</p>
                    </div>
                  </div>
                  <div class="flex items-center gap-1.5 shrink-0">
                    <button type="button" onclick="copyText('https://www.instagram.com/redaksi.segitiga?gwpx=MWx4eTQ1eG90bmoxdw==', 'Tautan Instagram disalin!')" class="px-2.5 py-1.5 rounded-xl bg-ice hover:bg-slate-200/70 text-navy text-xs font-bold cursor-pointer">Salin</button>
                    <a href="https://www.instagram.com/redaksi.segitiga?gwpx=MWx4eTQ1eG90bmoxdw==" target="_blank" rel="noopener noreferrer" class="px-3.5 py-1.5 rounded-xl bg-navy hover:bg-royal text-white font-heading text-xs font-bold transition-colors">Buka</a>
                  </div>
                </div>

                <!-- 3. Saluran WhatsApp -->
                <div class="flex items-center justify-between gap-3 p-3.5 rounded-2xl bg-white border border-slate-200/80">
                  <div class="flex items-center gap-3 min-w-0">
                    <span class="w-10 h-10 rounded-xl bg-cyanbrand text-white flex items-center justify-center shrink-0">
                      <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24"><path d="M12.04 2C6.58 2 2.13 6.45 2.13 11.91c0 1.75.46 3.45 1.32 4.95L2.05 22l5.25-1.38c1.45.79 3.08 1.21 4.74 1.21 5.46 0 9.91-4.45 9.91-9.91C21.95 6.45 17.5 2 12.04 2Zm5.82 14.01c-.24.68-1.41 1.3-1.96 1.38-.51.08-1.15.11-1.86-.11-.43-.14-.99-.32-1.7-.63-2.99-1.29-4.94-4.3-5.09-4.5-.15-.2-1.21-1.61-1.21-3.07 0-1.46.77-2.18 1.04-2.48.27-.3.59-.37.79-.37.2 0 .4 0 .57.01.18.01.43-.07.67.51.24.59.84 2.05.91 2.2.08.15.13.32.02.52-.1.2-.15.32-.3.5-.15.17-.31.38-.45.51-.15.15-.3.31-.13.61.17.3.77 1.27 1.65 2.05 1.13 1.01 2.09 1.32 2.39 1.47.3.15.47.12.65-.08.17-.2.74-.86.94-1.16.2-.3.4-.25.67-.15.27.1 1.73.82 2.03.97.3.15.5.22.57.34.07.12.07.7-.17 1.38Z"/></svg>
                    </span>
                    <div class="truncate">
                      <p class="text-sm font-heading font-extrabold text-navy">Saluran WhatsApp</p>
                      <p class="text-xs text-slate-500 truncate">segitiga.id Official Channel</p>
                    </div>
                  </div>
                  <div class="flex items-center gap-1.5 shrink-0">
                    <button type="button" onclick="copyText('https://whatsapp.com/channel/0029Vb9QOPJ3LdQQIEvpWi0K', 'Tautan Saluran WhatsApp disalin!')" class="px-2.5 py-1.5 rounded-xl bg-ice hover:bg-slate-200/70 text-navy text-xs font-bold cursor-pointer">Salin</button>
                    <a href="https://whatsapp.com/channel/0029Vb9QOPJ3LdQQIEvpWi0K" target="_blank" rel="noopener noreferrer" class="px-3.5 py-1.5 rounded-xl bg-navy hover:bg-royal text-white font-heading text-xs font-bold transition-colors">Gabung</a>
                  </div>
                </div>
              </div>
            </div>

          </div>

          <!-- Kolom Kanan: Form Interaktif Kirim Laporan Warga / Kerja Sama / Hak Jawab -->
          <div class="lg:col-span-7 reveal">
            <div class="rounded-3xl bg-ice/70 p-6 sm:p-9 border border-slate-200/90 shadow-sm">
              <div class="mb-6">
                <span class="text-xs font-heading font-extrabold tracking-widest text-royal uppercase">Formulir Meja Redaksi</span>
                <h3 class="text-2xl font-extrabold text-navy mt-1">
                  Kirim Laporan Warga, Kerja Sama, atau Hak Jawab
                </h3>
                <p class="text-sm text-slatebody mt-1">
                  Isi formulir di bawah ini untuk meneruskan pesan secara terstruktur langsung ke WhatsApp Redaksi (<strong class="text-navy">081234567890</strong>) atau Email (<strong class="text-navy">redaksi.segitiga@gmail.com</strong>).
                </p>
              </div>

              <form id="editorialContactForm" class="space-y-4" onsubmit="event.preventDefault(); sendEditorialMessage('wa');">
                <div class="grid grid-cols-1 sm:grid-cols-2 gap-4">
                  <!-- Kategori -->
                  <div>
                    <label for="contactCategory" class="block text-xs font-heading font-extrabold text-navy uppercase tracking-wider mb-1.5">
                      Kategori Pesan
                    </label>
                    <select id="contactCategory" class="w-full px-4 py-3 rounded-2xl bg-white border border-slate-200 text-sm font-semibold text-navy focus:outline-none focus:border-cyanbrand">
                      <option value="Laporan Warga">Laporan Warga</option>
                      <option value="Kerja Sama UMKM / Iklan">Kerja Sama UMKM / Iklan</option>
                      <option value="Kritik & Saran">Kritik & Saran</option>
                      <option value="Hak Jawab & Koreksi">Hak Jawab & Koreksi</option>
                    </select>
                  </div>

                  <!-- Wilayah -->
                  <div>
                    <label for="contactRegion" class="block text-xs font-heading font-extrabold text-navy uppercase tracking-wider mb-1.5">
                      Wilayah
                    </label>
                    <select id="contactRegion" class="w-full px-4 py-3 rounded-2xl bg-white border border-slate-200 text-sm font-semibold text-navy focus:outline-none focus:border-cyanbrand">
                      <option value="Purwakarta">Purwakarta</option>
                      <option value="Subang">Subang</option>
                      <option value="Karawang">Karawang</option>
                      <option value="Lintas Purwasuka">Lintas Purwasuka</option>
                    </select>
                  </div>
                </div>

                <!-- Nama Pengirim -->
                <div>
                  <label for="contactName" class="block text-xs font-heading font-extrabold text-navy uppercase tracking-wider mb-1.5">
                    Nama / Instansi / Komunitas
                  </label>
                  <input
                    id="contactName"
                    type="text"
                    required
                    placeholder="Contoh: Rizky Pratama / UMKM Kuliner Karawang"
                    class="w-full px-4 py-3 rounded-2xl bg-white border border-slate-200 text-sm text-navy placeholder:text-slate-400 focus:outline-none focus:border-cyanbrand"
                  />
                </div>

                <!-- Isi Pesan -->
                <div>
                  <label for="contactMessage" class="block text-xs font-heading font-extrabold text-navy uppercase tracking-wider mb-1.5">
                    Detail Informasi / Pesan
                  </label>
                  <textarea
                    id="contactMessage"
                    rows="4"
                    required
                    placeholder="Tuliskan kronologi informasi warga, rencana kerja sama, kritik/saran, atau keterangan hak jawab Anda..."
                    class="w-full px-4 py-3 rounded-2xl bg-white border border-slate-200 text-sm text-navy placeholder:text-slate-400 focus:outline-none focus:border-cyanbrand"
                  ></textarea>
                </div>

                <!-- Tombol Aksi Kirim -->
                <div class="pt-2 flex flex-col sm:flex-row gap-3">
                  <button
                    type="button"
                    onclick="sendEditorialMessage('wa')"
                    class="flex-1 inline-flex items-center justify-center gap-2.5 px-6 py-3.5 rounded-2xl bg-navy hover:bg-royal text-white font-heading text-sm font-bold shadow-sm transition-colors cursor-pointer"
                  >
                    <svg class="w-4 h-4 text-emerald-400" fill="currentColor" viewBox="0 0 24 24"><path d="M12.04 2C6.58 2 2.13 6.45 2.13 11.91c0 1.75.46 3.45 1.32 4.95L2.05 22l5.25-1.38c1.45.79 3.08 1.21 4.74 1.21 5.46 0 9.91-4.45 9.91-9.91C21.95 6.45 17.5 2 12.04 2Zm5.82 14.01c-.24.68-1.41 1.3-1.96 1.38-.51.08-1.15.11-1.86-.11-.43-.14-.99-.32-1.7-.63-2.99-1.29-4.94-4.3-5.09-4.5-.15-.2-1.21-1.61-1.21-3.07 0-1.46.77-2.18 1.04-2.48.27-.3.59-.37.79-.37.2 0 .4 0 .57.01.18.01.43-.07.67.51.24.59.84 2.05.91 2.2.08.15.13.32.02.52-.1.2-.15.32-.3.5-.15.17-.31.38-.45.51-.15.15-.3.31-.13.61.17.3.77 1.27 1.65 2.05 1.13 1.01 2.09 1.32 2.39 1.47.3.15.47.12.65-.08.17-.2.74-.86.94-1.16.2-.3.4-.25.67-.15.27.1 1.73.82 2.03.97.3.15.5.22.57.34.07.12.07.7-.17 1.38Z"/></svg>
                    <span>Kirim via WhatsApp Redaksi</span>
                  </button>

                  <button
                    type="button"
                    onclick="sendEditorialMessage('email')"
                    class="flex-1 inline-flex items-center justify-center gap-2.5 px-6 py-3.5 rounded-2xl bg-white hover:bg-ice text-navy border-2 border-navy/15 hover:border-cyanbrand font-heading text-sm font-bold transition-colors cursor-pointer"
                  >
                    <svg class="w-4 h-4 text-royal" fill="none" stroke="currentColor" stroke-width="2.2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"/></svg>
                    <span>Kirim via Email Redaksi</span>
                  </button>
                </div>
              </form>
            </div>
          </div>

        </div>
      </div>
    </section>
  </main>

  <!-- =====================================================================
       8. FOOTER EDITORIAL & BOX REDAKSI (PASAL 12 UU PERS)
       ===================================================================== -->
  <footer class="bg-navy-dark text-white pt-16 pb-10 border-t border-white/10">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">

      <div class="grid grid-cols-1 lg:grid-cols-12 gap-10 pb-12 border-b border-white/10">

        <!-- Kolom 1: Logo Versi Terang/Gelap & Tagline -->
        <div class="lg:col-span-4 space-y-4">
          <a href="#beranda" class="inline-flex items-center gap-3" aria-label="Beranda segitiga.id">
            <svg class="w-10 h-9" viewBox="0 0 220 200" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M104.2 17.5C106.8 13.1 113.2 13.1 115.8 17.5L196.4 157.2C199.0 161.7 195.8 167.3 190.6 167.3H29.4C24.2 167.3 21.0 161.7 23.6 157.2L104.2 17.5Z" fill="url(#segitigaLogoGrad)" />
              <path d="M62 146C51 134 49 112 58 93C55 113 62 131 76 140L62 146Z" fill="#FFFFFF" />
              <path d="M137 88C128 73 108 65 91 71C75 77 68 95 70 114C72 132 84 143 104 143C115 143 124 140 130 137C121 151 104 162 85 169H103C122 161 138 147 146 130C151 118 147 101 137 88Z" fill="#FFFFFF" />
              <path d="M101 92.5C101 89.8 104.0 88.2 106.3 89.6L127.5 102.6C129.7 103.9 129.7 107.1 127.5 108.4L106.3 121.4C104.0 122.8 101 121.2 101 118.5V92.5Z" fill="#00B4D8" />
              <path d="M97 135C121 121 146 93 169 55" stroke="#061524" stroke-width="14" stroke-linecap="round" />
              <path d="M97 135C121 121 146 93 169 55" stroke="#00B4D8" stroke-width="7.5" stroke-linecap="round" />
              <circle cx="172" cy="52" r="10.5" fill="#00B4D8" />
            </svg>

            <!-- Wordmark Putih & Cyan untuk Latar Gelap -->
            <svg class="h-7 w-auto" viewBox="0 0 245 48" fill="none" xmlns="http://www.w3.org/2000/svg">
              <text x="0" y="36" fill="#FFFFFF" font-family="'Plus Jakarta Sans', sans-serif" font-weight="800" font-size="36" letter-spacing="-1.2">segitiga</text>
              <polygon points="154,26 164,31.5 154,37" fill="#FFFFFF" />
              <rect x="171" y="16" width="7.2" height="20" rx="1.5" fill="#00B4D8" />
              <polygon points="171,4 181.5,9.5 171,15" fill="#00B4D8" />
              <text x="184" y="36" fill="#00B4D8" font-family="'Plus Jakarta Sans', sans-serif" font-weight="800" font-size="36" letter-spacing="-1">d</text>
            </svg>
          </a>

          <p class="text-sm font-heading font-bold text-cyanbrand">
            "Fakta untuk Warga"
          </p>
          <p class="text-sm text-slate-300 leading-relaxed">
            Media hyperlocal digital untuk wilayah Purwakarta, Subang, dan Karawang (Purwasuka). Menyajikan informasi aktual, ringkas, visual, dan terverifikasi.
          </p>

          <!-- 3 Saluran Resmi di Footer -->
          <div class="pt-2 flex flex-wrap items-center gap-2.5">
            <a href="https://www.tiktok.com/@redaksi.segitiga?_r=1&_t=ZS-9Bf5fEpCAP0" target="_blank" rel="noopener noreferrer" class="inline-flex items-center gap-2 px-3.5 py-2 rounded-xl bg-white/10 hover:bg-cyanbrand hover:text-navy text-xs font-heading font-bold transition-colors">
              <svg class="w-4 h-4" fill="currentColor" viewBox="0 0 24 24"><path d="M16.6 5.82A4.28 4.28 0 0 1 15.54 3h-3.09v12.4a2.59 2.59 0 0 1-2.59 2.5c-1.42 0-2.6-1.16-2.6-2.6 0-1.72 1.66-3.01 3.37-2.48V9.66c-3.45-.46-6.47 2.22-6.47 5.64 0 3.33 2.76 5.7 5.69 5.7 3.14 0 5.69-2.55 5.69-5.7V9.01a7.35 7.35 0 0 0 4.3 1.38V7.3s-1.88.09-3.24-1.48Z"/></svg>
              <span>TikTok</span>
            </a>
            <a href="https://www.instagram.com/redaksi.segitiga?gwpx=MWx4eTQ1eG90bmoxdw==" target="_blank" rel="noopener noreferrer" class="inline-flex items-center gap-2 px-3.5 py-2 rounded-xl bg-white/10 hover:bg-cyanbrand hover:text-navy text-xs font-heading font-bold transition-colors">
              <svg class="w-4 h-4" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><rect x="2" y="2" width="20" height="20" rx="5"/><circle cx="12" cy="12" r="4"/><circle cx="17.5" cy="6.5" r="1" fill="currentColor" stroke="none"/></svg>
              <span>Instagram</span>
            </a>
            <a href="https://whatsapp.com/channel/0029Vb9QOPJ3LdQQIEvpWi0K" target="_blank" rel="noopener noreferrer" class="inline-flex items-center gap-2 px-3.5 py-2 rounded-xl bg-white/10 hover:bg-cyanbrand hover:text-navy text-xs font-heading font-bold transition-colors">
              <svg class="w-4 h-4" fill="currentColor" viewBox="0 0 24 24"><path d="M12.04 2C6.58 2 2.13 6.45 2.13 11.91c0 1.75.46 3.45 1.32 4.95L2.05 22l5.25-1.38c1.45.79 3.08 1.21 4.74 1.21 5.46 0 9.91-4.45 9.91-9.91C21.95 6.45 17.5 2 12.04 2Zm5.82 14.01c-.24.68-1.41 1.3-1.96 1.38-.51.08-1.15.11-1.86-.11-.43-.14-.99-.32-1.7-.63-2.99-1.29-4.94-4.3-5.09-4.5-.15-.2-1.21-1.61-1.21-3.07 0-1.46.77-2.18 1.04-2.48.27-.3.59-.37.79-.37.2 0 .4 0 .57.01.18.01.43-.07.67.51.24.59.84 2.05.91 2.2.08.15.13.32.02.52-.1.2-.15.32-.3.5-.15.17-.31.38-.45.51-.15.15-.3.31-.13.61.17.3.77 1.27 1.65 2.05 1.13 1.01 2.09 1.32 2.39 1.47.3.15.47.12.65-.08.17-.2.74-.86.94-1.16.2-.3.4-.25.67-.15.27.1 1.73.82 2.03.97.3.15.5.22.57.34.07.12.07.7-.17 1.38Z"/></svg>
              <span>Saluran WhatsApp</span>
            </a>
          </div>
        </div>

        <!-- Kolom 2: Navigasi Cepat -->
        <div class="lg:col-span-3 space-y-3">
          <h4 class="text-xs font-heading font-extrabold tracking-widest text-cyanbrand uppercase">Navigasi Cepat</h4>
          <ul class="space-y-2.5 text-sm text-slate-300 font-medium">
            <li><a href="#beranda" class="hover:text-white transition-colors">Beranda</a></li>
            <li><a href="#tentang" class="hover:text-white transition-colors">Tentang SEGITIGA</a></li>
            <li><a href="#wilayah" class="hover:text-white transition-colors">Wilayah Purwasuka</a></li>
            <li><a href="#rubrik" class="hover:text-white transition-colors">7 Rubrik Informasi</a></li>
            <li><a href="#berita" class="hover:text-white transition-colors">Berita Purwasuka</a></li>
            <li><a href="#kontak" class="hover:text-white transition-colors">Hubungi Redaksi</a></li>
          </ul>
        </div>

        <!-- Kolom 3: Box Redaksi (Pasal 12 UU No. 40 Tahun 1999 tentang Pers) -->
        <div class="lg:col-span-5">
          <div class="rounded-2xl bg-white/5 border border-white/10 p-5 sm:p-6 space-y-3">
            <div class="flex items-center justify-between gap-2">
              <h4 class="text-xs font-heading font-extrabold tracking-widest text-cyanbrand uppercase">Box Redaksi (Pasal 12 UU Pers)</h4>
              <span class="text-[11px] text-slate-400">PT Segitiga Media Digital</span>
            </div>

            <dl class="grid grid-cols-1 sm:grid-cols-2 gap-x-4 gap-y-2.5 text-xs">
              <div>
                <dt class="text-slate-400">Direktur / Penanggung Jawab</dt>
                <dd class="font-heading font-bold text-white mt-0.5">Jalu Ageng Sajiwo</dd>
              </div>
              <div>
                <dt class="text-slate-400">Pemimpin Redaksi</dt>
                <dd class="font-heading font-bold text-white mt-0.5">Nabila Azzahro</dd>
              </div>
              <div>
                <dt class="text-slate-400">Redaktur Pelaksana / Editor</dt>
                <dd class="font-heading font-bold text-white mt-0.5">Eric Fernando</dd>
              </div>
              <div>
                <dt class="text-slate-400">Pemimpin Usaha</dt>
                <dd class="font-heading font-bold text-white mt-0.5">Mufida Istiqomah</dd>
              </div>
              <div>
                <dt class="text-slate-400">Tim Teknologi / CMS</dt>
                <dd class="font-heading font-bold text-white mt-0.5">Jenny Pasya</dd>
              </div>
              <div>
                <dt class="text-slate-400">Kontak Redaksi</dt>
                <dd class="font-heading font-bold text-cyanbrand mt-0.5">081234567890 • redaksi.segitiga@gmail.com</dd>
              </div>
            </dl>

            <p class="text-[11px] text-slate-400 leading-relaxed pt-2 border-t border-white/10">
              Dalam menjalankan tugas jurnalistik, redaksi segitiga.id berpedoman pada Undang-Undang Nomor 40 Tahun 1999 tentang Pers, Kode Etik Jurnalistik, dan Pedoman Pemberitaan Media Siber Dewan Pers.
            </p>
          </div>
        </div>

      </div>

      <div class="pt-7 flex flex-col sm:flex-row items-center justify-between gap-3 text-xs text-slate-400">
        <p>© 2026 segitiga.id — PT Segitiga Media Digital. Hak Cipta Dilindungi.</p>
        <p class="text-slate-300 font-medium">Purwakarta • Subang • Karawang (Purwasuka)</p>
      </div>
    </div>
  </footer>

  <!-- =====================================================================
       MODAL 1: 3 SALURAN RESMI SEGITIGA.ID (TIKTOK, INSTAGRAM, SALURAN WHATSAPP)
       ===================================================================== -->
  <div id="socialModal" class="fixed inset-0 z-50 hidden items-center justify-center p-4 bg-navy/65 backdrop-blur-sm" role="dialog" aria-modal="true" aria-labelledby="socialModalTitle">
    <div class="bg-white rounded-3xl max-w-lg w-full p-6 sm:p-8 shadow-2xl border border-slate-200 relative">
      <button
        type="button"
        onclick="closeSocialModal()"
        aria-label="Tutup Jendela Saluran"
        class="absolute top-5 right-5 p-2 rounded-xl text-slate-400 hover:text-navy hover:bg-ice transition-colors cursor-pointer"
      >
        <svg class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="2.2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12"/></svg>
      </button>

      <div class="flex items-center gap-2 mb-2">
        <span class="w-2.5 h-2.5 rounded-full bg-cyanbrand"></span>
        <span class="text-xs font-heading font-extrabold tracking-widest text-royal uppercase">Saluran Resmi</span>
      </div>
      <h3 id="socialModalTitle" class="text-2xl font-extrabold text-navy mb-1.5">
        Ikuti <span class="text-royal">segitiga</span><span class="text-cyanbrand">.id</span>
      </h3>
      <p class="text-sm text-slatebody mb-6">
        Dapatkan rangkuman informasi harian Purwakarta, Subang, dan Karawang melalui 3 saluran resmi kami:
      </p>

      <div class="space-y-3">
        <!-- 1. TikTok -->
        <div class="flex items-center justify-between gap-3 p-3.5 rounded-2xl bg-ice/80 hover:bg-ice border border-slate-200/80 transition-colors">
          <div class="flex items-center gap-3.5 min-w-0">
            <div class="w-11 h-11 rounded-xl bg-navy text-cyanbrand flex items-center justify-center shrink-0">
              <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24"><path d="M16.6 5.82A4.28 4.28 0 0 1 15.54 3h-3.09v12.4a2.59 2.59 0 0 1-2.59 2.5c-1.42 0-2.6-1.16-2.6-2.6 0-1.72 1.66-3.01 3.37-2.48V9.66c-3.45-.46-6.47 2.22-6.47 5.64 0 3.33 2.76 5.7 5.69 5.7 3.14 0 5.69-2.55 5.69-5.7V9.01a7.35 7.35 0 0 0 4.3 1.38V7.3s-1.88.09-3.24-1.48Z"/></svg>
            </div>
            <div class="truncate">
              <p class="text-sm font-heading font-extrabold text-navy">TikTok</p>
              <p class="text-xs text-slate-500 truncate">@redaksi.segitiga</p>
            </div>
          </div>
          <div class="flex items-center gap-2 shrink-0">
            <button type="button" onclick="copyText('https://www.tiktok.com/@redaksi.segitiga?_r=1&_t=ZS-9Bf5fEpCAP0', 'Tautan TikTok @redaksi.segitiga disalin!')" class="px-3 py-1.5 rounded-xl bg-white border border-slate-200 hover:border-cyanbrand text-xs font-bold text-navy cursor-pointer">Salin</button>
            <a href="https://www.tiktok.com/@redaksi.segitiga?_r=1&_t=ZS-9Bf5fEpCAP0" target="_blank" rel="noopener noreferrer" class="px-3.5 py-1.5 rounded-xl bg-navy hover:bg-royal text-white font-heading text-xs font-bold transition-colors">Buka</a>
          </div>
        </div>

        <!-- 2. Instagram -->
        <div class="flex items-center justify-between gap-3 p-3.5 rounded-2xl bg-ice/80 hover:bg-ice border border-slate-200/80 transition-colors">
          <div class="flex items-center gap-3.5 min-w-0">
            <div class="w-11 h-11 rounded-xl bg-royal text-white flex items-center justify-center shrink-0">
              <svg class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><rect x="2" y="2" width="20" height="20" rx="5"/><circle cx="12" cy="12" r="4"/><circle cx="17.5" cy="6.5" r="1" fill="currentColor" stroke="none"/></svg>
            </div>
            <div class="truncate">
              <p class="text-sm font-heading font-extrabold text-navy">Instagram</p>
              <p class="text-xs text-slate-500 truncate">@redaksi.segitiga</p>
            </div>
          </div>
          <div class="flex items-center gap-2 shrink-0">
            <button type="button" onclick="copyText('https://www.instagram.com/redaksi.segitiga?gwpx=MWx4eTQ1eG90bmoxdw==', 'Tautan Instagram @redaksi.segitiga disalin!')" class="px-3 py-1.5 rounded-xl bg-white border border-slate-200 hover:border-cyanbrand text-xs font-bold text-navy cursor-pointer">Salin</button>
            <a href="https://www.instagram.com/redaksi.segitiga?gwpx=MWx4eTQ1eG90bmoxdw==" target="_blank" rel="noopener noreferrer" class="px-3.5 py-1.5 rounded-xl bg-navy hover:bg-royal text-white font-heading text-xs font-bold transition-colors">Buka</a>
          </div>
        </div>

        <!-- 3. Saluran WhatsApp -->
        <div class="flex items-center justify-between gap-3 p-3.5 rounded-2xl bg-ice/80 hover:bg-ice border border-slate-200/80 transition-colors">
          <div class="flex items-center gap-3.5 min-w-0">
            <div class="w-11 h-11 rounded-xl bg-cyanbrand text-white flex items-center justify-center shrink-0">
              <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24"><path d="M12.04 2C6.58 2 2.13 6.45 2.13 11.91c0 1.75.46 3.45 1.32 4.95L2.05 22l5.25-1.38c1.45.79 3.08 1.21 4.74 1.21 5.46 0 9.91-4.45 9.91-9.91C21.95 6.45 17.5 2 12.04 2Zm5.82 14.01c-.24.68-1.41 1.3-1.96 1.38-.51.08-1.15.11-1.86-.11-.43-.14-.99-.32-1.7-.63-2.99-1.29-4.94-4.3-5.09-4.5-.15-.2-1.21-1.61-1.21-3.07 0-1.46.77-2.18 1.04-2.48.27-.3.59-.37.79-.37.2 0 .4 0 .57.01.18.01.43-.07.67.51.24.59.84 2.05.91 2.2.08.15.13.32.02.52-.1.2-.15.32-.3.5-.15.17-.31.38-.45.51-.15.15-.3.31-.13.61.17.3.77 1.27 1.65 2.05 1.13 1.01 2.09 1.32 2.39 1.47.3.15.47.12.65-.08.17-.2.74-.86.94-1.16.2-.3.4-.25.67-.15.27.1 1.73.82 2.03.97.3.15.5.22.57.34.07.12.07.7-.17 1.38Z"/></svg>
            </div>
            <div class="truncate">
              <p class="text-sm font-heading font-extrabold text-navy">Saluran WhatsApp</p>
              <p class="text-xs text-slate-500 truncate">segitiga.id Official Channel</p>
            </div>
          </div>
          <div class="flex items-center gap-2 shrink-0">
            <button type="button" onclick="copyText('https://whatsapp.com/channel/0029Vb9QOPJ3LdQQIEvpWi0K', 'Tautan Saluran WhatsApp disalin!')" class="px-3 py-1.5 rounded-xl bg-white border border-slate-200 hover:border-cyanbrand text-xs font-bold text-navy cursor-pointer">Salin</button>
            <a href="https://whatsapp.com/channel/0029Vb9QOPJ3LdQQIEvpWi0K" target="_blank" rel="noopener noreferrer" class="px-3.5 py-1.5 rounded-xl bg-navy hover:bg-royal text-white font-heading text-xs font-bold transition-colors">Gabung</a>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- =====================================================================
       MODAL 2: PEMBACA ARTIKEL LENGKAP (ARTICLE READER MODAL)
       ===================================================================== -->
  <div id="articleModal" class="fixed inset-0 z-50 hidden items-center justify-center p-3 sm:p-6 bg-navy/70 backdrop-blur-sm" role="dialog" aria-modal="true" aria-labelledby="articleModalHeading">
    <div class="bg-white rounded-3xl max-w-3xl w-full shadow-2xl border border-slate-200 overflow-hidden flex flex-col max-h-[92vh]">

      <!-- Top Bar Modal Artikel -->
      <div class="px-5 sm:px-8 py-4 bg-ice border-b border-slate-200/80 flex items-center justify-between gap-3 shrink-0">
        <div class="flex items-center gap-2 min-w-0">
          <span id="modalArticleRubrik" class="px-3 py-1 rounded-full bg-navy text-cyanbrand text-xs font-heading font-extrabold truncate"></span>
          <span id="modalArticleRegion" class="px-2.5 py-1 rounded-full bg-white border border-slate-200 text-navy text-xs font-heading font-bold"></span>
        </div>

        <div class="flex items-center gap-2 shrink-0">
          <button
            id="modalCopyArticleBtn"
            type="button"
            class="inline-flex items-center gap-1.5 px-3 py-1.5 rounded-xl bg-white hover:bg-navy text-navy hover:text-white border border-slate-200 text-xs font-heading font-bold transition-colors cursor-pointer"
          >
            <svg class="w-3.5 h-3.5" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M8 16H6a2 2 0 01-2-2V6a2 2 0 012-2h8a2 2 0 012 2v2m-6 12h8a2 2 0 002-2v-8a2 2 0 00-2-2h-8a2 2 0 00-2 2v8a2 2 0 002 2z"/></svg>
            <span>Salin Berita</span>
          </button>

          <button
            type="button"
            onclick="closeArticleModal()"
            aria-label="Tutup Artikel"
            class="p-2 rounded-xl bg-white hover:bg-slate-200/70 text-navy border border-slate-200 transition-colors cursor-pointer"
          >
            <svg class="w-5 h-5" fill="none" stroke="currentColor" stroke-width="2.2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M6 18L18 6M6 6l12 12"/></svg>
          </button>
        </div>
      </div>

      <!-- Konten Artikel Scrollable -->
      <div id="articleModalScrollArea" class="px-5 sm:px-9 py-6 sm:py-8 overflow-y-auto space-y-6">
        <div class="space-y-3">
          <div class="flex flex-wrap items-center gap-2 text-xs text-slate-500 font-medium">
            <span id="modalArticleDateline" class="font-bold text-royal"></span>
            <span>•</span>
            <span id="modalArticleReadTime"></span>
            <span>•</span>
            <span>Redaksi segitiga.id</span>
          </div>
          <h2 id="articleModalHeading" class="text-2xl sm:text-3xl font-extrabold text-navy leading-snug"></h2>
        </div>

        <!-- Ilustrasi SVG Editorial Artikel -->
        <figure class="rounded-2xl overflow-hidden border border-slate-200/90 bg-ice">
          <div id="modalArticleIllustration" class="w-full"></div>
          <figcaption id="modalArticleCaption" class="px-4 py-2.5 text-xs text-slate-500 italic bg-slate-50 border-t border-slate-200/70 text-center"></figcaption>
        </figure>

        <!-- Isi Teks Lengkap 100% Utuh -->
        <div id="modalArticleBody" class="space-y-4 text-base text-slatebody leading-[1.8]"></div>

        <!-- Kotak Ajak Ikuti 3 Saluran Resmi di Akhir Artikel -->
        <div class="mt-8 p-5 rounded-2xl bg-ice border border-cyanbrand/30 flex flex-col sm:flex-row sm:items-center justify-between gap-4">
          <div>
            <p class="text-xs font-heading font-extrabold text-royal uppercase tracking-wider">Fakta untuk Warga Purwasuka</p>
            <p class="text-sm font-bold text-navy mt-0.5">Ikuti pembaruan berita segitiga.id di saluran resmi kami:</p>
          </div>
          <div class="flex flex-wrap items-center gap-2 shrink-0">
            <a href="https://www.tiktok.com/@redaksi.segitiga?_r=1&_t=ZS-9Bf5fEpCAP0" target="_blank" rel="noopener noreferrer" class="px-3 py-2 rounded-xl bg-navy text-white text-xs font-heading font-bold hover:bg-royal transition-colors">TikTok</a>
            <a href="https://www.instagram.com/redaksi.segitiga?gwpx=MWx4eTQ1eG90bmoxdw==" target="_blank" rel="noopener noreferrer" class="px-3 py-2 rounded-xl bg-royal text-white text-xs font-heading font-bold hover:bg-navy transition-colors">Instagram</a>
            <a href="https://whatsapp.com/channel/0029Vb9QOPJ3LdQQIEvpWi0K" target="_blank" rel="noopener noreferrer" class="px-3 py-2 rounded-xl bg-cyanbrand text-navy text-xs font-heading font-extrabold hover:opacity-90 transition-opacity">Saluran WA</a>
          </div>
        </div>
      </div>

      <!-- Footer Navigasi Antar-Berita -->
      <div class="px-5 sm:px-8 py-3.5 bg-slate-50 border-t border-slate-200/80 flex items-center justify-between gap-3 shrink-0">
        <button id="prevArticleBtn" type="button" class="inline-flex items-center gap-1.5 text-xs sm:text-sm font-heading font-bold text-navy hover:text-royal cursor-pointer">
          <svg class="w-4 h-4" fill="none" stroke="currentColor" stroke-width="2.2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M15 19l-7-7 7-7"/></svg>
          <span>Berita Sebelumnya</span>
        </button>
        <button id="nextArticleBtn" type="button" class="inline-flex items-center gap-1.5 text-xs sm:text-sm font-heading font-bold text-navy hover:text-royal cursor-pointer">
          <span>Berita Berikutnya</span>
          <svg class="w-4 h-4" fill="none" stroke="currentColor" stroke-width="2.2" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" d="M9 5l7 7-7 7"/></svg>
        </button>
      </div>
    </div>
  </div>

  <!-- =====================================================================
       TOAST NOTIFIKASI HALUS (Pengganti alert())
       ===================================================================== -->
  <div id="toastNotification" class="fixed bottom-6 right-6 z-50 pointer-events-none opacity-0 translate-y-3 transition-all duration-300">
    <div class="flex items-center gap-3 px-4 py-3 rounded-2xl bg-navy text-white text-sm font-semibold shadow-xl border border-cyanbrand/35">
      <span class="w-2.5 h-2.5 rounded-full bg-cyanbrand"></span>
      <span id="toastMessage">Berhasil disalin!</span>
    </div>
  </div>

  <!-- =====================================================================
       JAVASCRIPT DATA BERITA LENGKAP & INTERAKTIVITAS
       ===================================================================== -->
  <script>
    // =========================================================================
    // 1. ILUSTRASI SVG EDITORIAL TEMATIK UNTUK MASING-MASING BERITA
    // =========================================================================
    function getArticleIllustrationSVG(key, isLarge = false) {
      const heightClass = isLarge ? 'h-64 sm:h-80' : 'h-48';

      const svgs = {
        jalan: `
          <svg class="w-full ${heightClass} object-cover" viewBox="0 0 640 320" fill="none" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Ilustrasi Perbaikan Jalan Penghubung Purwakarta-Subang">
            <rect width="640" height="320" fill="#E0F2FE"/>
            <circle cx="530" cy="64" r="32" fill="#FEF08A"/>
            <!-- Pepohonan Latar -->
            <circle cx="80" cy="145" r="45" fill="#15803D"/>
            <circle cx="135" cy="152" r="38" fill="#166534"/>
            <circle cx="545" cy="148" r="46" fill="#15803D"/>
            <circle cx="595" cy="155" r="36" fill="#166534"/>
            <!-- Gapura Perbatasan Purwakarta - Subang -->
            <rect x="155" y="65" width="12" height="125" fill="#475569"/>
            <rect x="473" y="65" width="12" height="125" fill="#475569"/>
            <path d="M150 65Q235 35 320 65Q405 35 490 65V96H150V65Z" fill="#0A2239" stroke="#00B4D8" stroke-width="2.5"/>
            <text x="235" y="83" text-anchor="middle" fill="#FFFFFF" font-family="'Plus Jakarta Sans', sans-serif" font-weight="800" font-size="11">KABUPATEN SUBANG</text>
            <text x="405" y="83" text-anchor="middle" fill="#48CAE4" font-family="'Plus Jakarta Sans', sans-serif" font-weight="800" font-size="11">BATAS PURWAKARTA</text>
            <!-- Badan Jalan Aspal -->
            <polygon points="0,320 140,185 500,185 640,320" fill="#334155"/>
            <polygon points="220,320 265,185 375,185 420,320" fill="#475569"/>
            <!-- Area Perbaikan & Pengaspalan Baru -->
            <polygon points="245,305 275,215 350,215 375,305" fill="#0F172A"/>
            <!-- Alat Berat / Road Roller Kuning -->
            <rect x="295" y="182" width="52" height="32" rx="6" fill="#F59E0B"/>
            <rect x="305" y="166" width="28" height="18" rx="3" fill="#0A2239"/>
            <circle cx="304" cy="216" r="13" fill="#1E293B" stroke="#94A3B8" stroke-width="3"/>
            <circle cx="340" cy="216" r="13" fill="#1E293B" stroke="#94A3B8" stroke-width="3"/>
            <!-- Kerucut Pembatas Oranye (Traffic Cones) -->
            <polygon points="180,260 190,232 200,260" fill="#F97316"/>
            <polygon points="210,225 218,204 226,225" fill="#F97316"/>
            <polygon points="445,260 455,232 465,260" fill="#F97316"/>
          </svg>
        `,
        inovasi: `
          <svg class="w-full ${heightClass} object-cover" viewBox="0 0 640 320" fill="none" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Ilustrasi Inovasi Mahasiswa Karawang Pengolahan Sampah Organik Menjadi Biogas">
            <rect width="640" height="320" fill="#F0F9FF"/>
            <!-- Banner Pameran Inovasi -->
            <rect x="70" y="28" width="500" height="195" rx="18" fill="#FFFFFF" stroke="#CBD5E1" stroke-width="2"/>
            <rect x="70" y="28" width="500" height="46" rx="18" fill="#0A2239"/>
            <text x="320" y="56" text-anchor="middle" fill="#FFFFFF" font-family="'Plus Jakarta Sans', sans-serif" font-weight="800" font-size="14">INOVASI PENGOLAHAN SAMPAH ORGANIK MENJADI BIOGAS</text>
            <!-- Diagram Proses di Poster -->
            <rect x="105" y="95" width="110" height="90" rx="14" fill="#DCFCE7"/>
            <circle cx="160" cy="132" r="20" fill="#16A34A"/>
            <text x="160" y="170" text-anchor="middle" fill="#166534" font-family="'Plus Jakarta Sans', sans-serif" font-weight="800" font-size="11">Sampah Organik</text>
            <path d="M225 140H265" stroke="#00B4D8" stroke-width="4" stroke-linecap="round"/>
            <polygon points="262,133 275,140 262,147" fill="#00B4D8"/>
            <!-- Tabung Reaktor Biogas -->
            <rect x="280" y="90" width="85" height="100" rx="16" fill="#0D4F8B"/>
            <rect x="298" y="112" width="49" height="24" rx="6" fill="#00B4D8"/>
            <text x="322" y="128" text-anchor="middle" fill="#0A2239" font-family="'Plus Jakarta Sans', sans-serif" font-weight="800" font-size="10">BIOGAS</text>
            <text x="322" y="172" text-anchor="middle" fill="#FFFFFF" font-family="'Plus Jakarta Sans', sans-serif" font-weight="700" font-size="10">Fermentasi</text>
            <path d="M375 140H415" stroke="#00B4D8" stroke-width="4" stroke-linecap="round"/>
            <polygon points="412,133 425,140 412,147" fill="#00B4D8"/>
            <!-- Piagam Juara 1 -->
            <rect x="430" y="95" width="115" height="90" rx="14" fill="#FEF3C7" stroke="#F59E0B" stroke-width="2"/>
            <text x="487" y="132" text-anchor="middle" fill="#0A2239" font-family="'Plus Jakarta Sans', sans-serif" font-weight="800" font-size="15">JUARA 1</text>
            <text x="487" y="152" text-anchor="middle" fill="#0D4F8B" font-family="'Inter', sans-serif" font-weight="700" font-size="10">Inovasi Nasional 2026</text>
            <!-- Meja Display -->
            <rect x="40" y="225" width="560" height="95" rx="12" fill="#0A2239"/>
            <text x="320" y="275" text-anchor="middle" fill="#48CAE4" font-family="'Plus Jakarta Sans', sans-serif" font-weight="800" font-size="14">TIM MAHASISWA KARAWANG • ENERGI ALTERNATIF RAMAH LINGKUNGAN</text>
          </svg>
        `,
        konser: `
          <svg class="w-full ${heightClass} object-cover" viewBox="0 0 640 320" fill="none" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Ilustrasi Konser Nostalgia Purwakarta 2026">
            <rect width="640" height="320" fill="#061524"/>
            <!-- Sorotan Lampu Panggung -->
            <polygon points="180,95 60,0 130,0" fill="#00B4D8" fill-opacity="0.22"/>
            <polygon points="320,95 250,0 390,0" fill="#38BDF8" fill-opacity="0.25"/>
            <polygon points="460,95 510,0 580,0" fill="#0D4F8B" fill-opacity="0.35"/>
            <!-- Struktur Panggung Utama -->
            <rect x="130" y="80" width="380" height="130" rx="12" fill="#0A2239" stroke="#00B4D8" stroke-width="2.5"/>
            <rect x="155" y="100" width="330" height="75" rx="8" fill="#0D4F8B"/>
            <text x="320" y="132" text-anchor="middle" fill="#FFFFFF" font-family="'Plus Jakarta Sans', sans-serif" font-weight="800" font-size="18">NOSTALGIA MUSIK INDONESIA 2026</text>
            <text x="320" y="156" text-anchor="middle" fill="#48CAE4" font-family="'Plus Jakarta Sans', sans-serif" font-weight="700" font-size="12">LAPANGAN PURNAWARMAN • PURWAKARTA</text>
            <!-- Siluet Penonton -->
            <path d="M0 245Q80 220 160 245T320 245T480 245T640 245V320H0V245Z" fill="#0A2239"/>
            <path d="M0 270Q110 248 220 270T440 270T640 265V320H0V270Z" fill="#020617"/>
            <!-- Titik Cahaya Penonton -->
            <circle cx="120" cy="252" r="3" fill="#48CAE4"/>
            <circle cx="235" cy="246" r="3.5" fill="#FDE047"/>
            <circle cx="340" cy="250" r="3" fill="#00B4D8"/>
            <circle cx="475" cy="245" r="3.5" fill="#FDE047"/>
          </svg>
        `,
        wisata: `
          <svg class="w-full ${heightClass} object-cover" viewBox="0 0 640 320" fill="none" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Ilustrasi 5 Destinasi Wisata Purwasuka">
            <rect width="640" height="320" fill="#E0F7FC"/>
            <!-- 3 Panel Kolase Purwakarta - Subang - Karawang -->
            <!-- Panel 1: Purwakarta -->
            <rect x="24" y="28" width="186" height="264" rx="18" fill="#0A2239"/>
            <path d="M117 175C117 120 117 85 117 65" stroke="#00B4D8" stroke-width="4" stroke-linecap="round"/>
            <path d="M100 175C85 130 68 105 52 90" stroke="#48CAE4" stroke-width="3" stroke-linecap="round"/>
            <path d="M134 175C149 130 166 105 182 90" stroke="#48CAE4" stroke-width="3" stroke-linecap="round"/>
            <ellipse cx="117" cy="186" rx="68" ry="12" fill="#00B4D8" fill-opacity="0.3"/>
            <text x="117" y="236" text-anchor="middle" fill="#FFFFFF" font-family="'Plus Jakarta Sans', sans-serif" font-weight="800" font-size="13">SRI BADUGA</text>
            <text x="117" y="256" text-anchor="middle" fill="#48CAE4" font-family="'Inter', sans-serif" font-weight="600" font-size="11">Purwakarta</text>

            <!-- Panel 2: Subang -->
            <rect x="227" y="28" width="186" height="264" rx="18" fill="#0D4F8B"/>
            <path d="M227 165L290 95L345 135L385 88L413 125V205H227V165Z" fill="#15803D"/>
            <path d="M312 108C312 140 315 170 315 198" stroke="#E0F7FC" stroke-width="6" stroke-linecap="round"/>
            <text x="320" y="236" text-anchor="middle" fill="#FFFFFF" font-family="'Plus Jakarta Sans', sans-serif" font-weight="800" font-size="13">CILEAT & SARI ATER</text>
            <text x="320" y="256" text-anchor="middle" fill="#BAE6FD" font-family="'Inter', sans-serif" font-weight="600" font-size="11">Subang</text>

            <!-- Panel 3: Karawang -->
            <rect x="430" y="28" width="186" height="264" rx="18" fill="#0369A1"/>
            <circle cx="565" cy="78" r="18" fill="#FDE047"/>
            <rect x="430" y="145" width="186" height="58" fill="#0284C7"/>
            <polygon points="495,203 515,148 531,148 551,203" fill="#0A2239"/>
            <text x="523" y="236" text-anchor="middle" fill="#FFFFFF" font-family="'Plus Jakarta Sans', sans-serif" font-weight="800" font-size="13">PAKIS & CIGENTIS</text>
            <text x="523" y="256" text-anchor="middle" fill="#E0F7FC" font-family="'Inter', sans-serif" font-weight="600" font-size="11">Karawang</text>
          </svg>
        `,
        lingkungan: `
          <svg class="w-full ${heightClass} object-cover" viewBox="0 0 640 320" fill="none" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Ilustrasi Keluhan Pencemaran Saluran Air Kawasan Industri Subang">
            <rect width="640" height="320" fill="#F1F5F9"/>
            <!-- Bangunan Kawasan Industri -->
            <rect x="65" y="75" width="165" height="105" rx="6" fill="#475569"/>
            <rect x="230" y="105" width="145" height="75" fill="#64748B"/>
            <rect x="180" y="38" width="18" height="42" fill="#334155"/>
            <rect x="208" y="48" width="16" height="32" fill="#334155"/>
            <circle cx="192" cy="26" r="12" fill="#CBD5E1"/>
            <circle cx="212" cy="18" r="15" fill="#E2E8F0"/>
            <!-- Tepi Sungai Hijau -->
            <rect y="175" width="640" height="145" fill="#166534"/>
            <!-- Aliran Sungai & Perubahan Warna/Busa -->
            <polygon points="240,175 340,175 495,320 145,320" fill="#0D4F8B"/>
            <path d="M275 190C295 215 250 245 310 275C355 295 390 305 435 318" stroke="#FFFFFF" stroke-width="14" stroke-linecap="round" stroke-opacity="0.78"/>
            <!-- Badge Perhatian Lingkungan -->
            <rect x="415" y="56" width="175" height="78" rx="16" fill="#FFFFFF" stroke="#CBD5E1" stroke-width="2"/>
            <text x="502" y="88" text-anchor="middle" fill="#0A2239" font-family="'Plus Jakarta Sans', sans-serif" font-weight="800" font-size="12">PENGAWASAN IPAL</text>
            <text x="502" y="108" text-anchor="middle" fill="#0D4F8B" font-family="'Inter', sans-serif" font-weight="600" font-size="11">Kabupaten Subang</text>
          </svg>
        `,
        umk: `
          <svg class="w-full ${heightClass} object-cover" viewBox="0 0 640 320" fill="none" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Ilustrasi Proyeksi Kenaikan UMK Purwakarta Subang Karawang 2027">
            <rect width="640" height="320" fill="#0A2239"/>
            <text x="44" y="48" fill="#48CAE4" font-family="'Plus Jakarta Sans', sans-serif" font-weight="800" font-size="13">SIMULASI PROYEKSI UMK PURWASUKA 2027</text>
            <text x="44" y="72" fill="#FFFFFF" font-family="'Plus Jakarta Sans', sans-serif" font-weight="800" font-size="20">Perbandingan Nominal Tiga Kabupaten</text>

            <!-- Grafik Batang 1: Subang -->
            <rect x="65" y="160" width="135" height="105" rx="14" fill="#0D4F8B"/>
            <text x="132" y="148" text-anchor="middle" fill="#48CAE4" font-family="'Plus Jakarta Sans', sans-serif" font-weight="800" font-size="14">Rp3.925.000</text>
            <text x="132" y="212" text-anchor="middle" fill="#FFFFFF" font-family="'Plus Jakarta Sans', sans-serif" font-weight="800" font-size="14">SUBANG</text>
            <text x="132" y="232" text-anchor="middle" fill="#BAE6FD" font-family="'Inter', sans-serif" font-size="11">2026: Rp3.737.482</text>

            <!-- Grafik Batang 2: Purwakarta -->
            <rect x="252" y="132" width="135" height="133" rx="14" fill="#1767B0"/>
            <text x="319" y="120" text-anchor="middle" fill="#48CAE4" font-family="'Plus Jakarta Sans', sans-serif" font-weight="800" font-size="14">Rp5.305.000</text>
            <text x="319" y="198" text-anchor="middle" fill="#FFFFFF" font-family="'Plus Jakarta Sans', sans-serif" font-weight="800" font-size="14">PURWAKARTA</text>
            <text x="319" y="218" text-anchor="middle" fill="#BAE6FD" font-family="'Inter', sans-serif" font-size="11">2026: Rp5.052.856</text>

            <!-- Grafik Batang 3: Karawang -->
            <rect x="440" y="105" width="135" height="160" rx="14" fill="#00B4D8"/>
            <text x="507" y="93" text-anchor="middle" fill="#FFFFFF" font-family="'Plus Jakarta Sans', sans-serif" font-weight="800" font-size="14">Rp6.180.000</text>
            <text x="507" y="185" text-anchor="middle" fill="#0A2239" font-family="'Plus Jakarta Sans', sans-serif" font-weight="800" font-size="14">KARAWANG</text>
            <text x="507" y="205" text-anchor="middle" fill="#061524" font-family="'Inter', sans-serif" font-weight="600" font-size="11">2026: Rp5.886.853</text>
          </svg>
        `,
        kuliner: `
          <svg class="w-full ${heightClass} object-cover" viewBox="0 0 640 320" fill="none" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Ilustrasi 3 Kuliner Khas Karawang">
            <rect width="640" height="320" fill="#FFFBEB"/>
            <!-- 3 Sajian Kuliner Khas Karawang -->
            <!-- 1. Pepes Jambal Walahar -->
            <rect x="28" y="34" width="182" height="252" rx="20" fill="#FFFFFF" stroke="#FDE68A" stroke-width="2"/>
            <ellipse cx="119" cy="128" rx="64" ry="30" transform="rotate(-14 119 128)" fill="#15803D"/>
            <path d="M68 138L168 112" stroke="#FEF08A" stroke-width="4" stroke-dasharray="6 4"/>
            <text x="119" y="206" text-anchor="middle" fill="#0A2239" font-family="'Plus Jakarta Sans', sans-serif" font-weight="800" font-size="13">Pepes Jambal</text>
            <text x="119" y="226" text-anchor="middle" fill="#0D4F8B" font-family="'Inter', sans-serif" font-weight="600" font-size="11">Khas Walahar</text>

            <!-- 2. Soto Tangkar Karawang -->
            <rect x="229" y="34" width="182" height="252" rx="20" fill="#FFFFFF" stroke="#FDE68A" stroke-width="2"/>
            <circle cx="320" cy="126" r="46" fill="#0A2239"/>
            <circle cx="320" cy="126" r="38" fill="#D97706"/>
            <circle cx="308" cy="118" r="8" fill="#78350F"/>
            <circle cx="332" cy="132" r="9" fill="#78350F"/>
            <circle cx="334" cy="114" r="9" fill="#BEF264"/>
            <text x="320" y="206" text-anchor="middle" fill="#0A2239" font-family="'Plus Jakarta Sans', sans-serif" font-weight="800" font-size="13">Soto Tangkar</text>
            <text x="320" y="226" text-anchor="middle" fill="#0D4F8B" font-family="'Inter', sans-serif" font-weight="600" font-size="11">Kuah Rempah Karawang</text>

            <!-- 3. Serabi Hijau -->
            <rect x="430" y="34" width="182" height="252" rx="20" fill="#FFFFFF" stroke="#FDE68A" stroke-width="2"/>
            <circle cx="505" cy="130" r="26" fill="#22C55E"/>
            <circle cx="536" cy="122" r="26" fill="#4ADE80"/>
            <circle cx="520" cy="144" r="24" fill="#16A34A"/>
            <ellipse cx="520" cy="140" rx="26" ry="12" fill="#D97706" fill-opacity="0.75"/>
            <text x="521" y="206" text-anchor="middle" fill="#0A2239" font-family="'Plus Jakarta Sans', sans-serif" font-weight="800" font-size="13">Serabi Hijau</text>
            <text x="521" y="226" text-anchor="middle" fill="#0D4F8B" font-family="'Inter', sans-serif" font-weight="600" font-size="11">Aroma Pandan & Kinca</text>
          </svg>
        `,
        klarifikasi: `
          <svg class="w-full ${heightClass} object-cover" viewBox="0 0 640 320" fill="none" xmlns="http://www.w3.org/2000/svg" role="img" aria-label="Ilustrasi Klarifikasi Kebakaran Toko Bahtera Jaya Subang">
            <rect width="640" height="320" fill="#0A2239"/>
            <!-- Panel Cek Fakta & Klarifikasi Resmi -->
            <rect x="52" y="38" width="536" height="244" rx="22" fill="#133557" stroke="#00B4D8" stroke-width="2"/>
            <rect x="82" y="64" width="175" height="30" rx="15" fill="#00B4D8"/>
            <text x="169" y="83" text-anchor="middle" fill="#0A2239" font-family="'Plus Jakarta Sans', sans-serif" font-weight="800" font-size="12">KLARIFIKASI & HAK JAWAB</text>

            <text x="82" y="130" fill="#FFFFFF" font-family="'Plus Jakarta Sans', sans-serif" font-weight="800" font-size="20">Keterangan Resmi Toko Bahtera Jaya</text>
            <text x="82" y="158" fill="#BAE6FD" font-family="'Inter', sans-serif" font-size="13">Meluruskan informasi penyebab kebakaran di Kabupaten Subang:</text>

            <rect x="82" y="180" width="476" height="72" rx="14" fill="#0A2239"/>
            <circle cx="114" cy="216" r="14" fill="#00B4D8"/>
            <path d="M108 216L112 220L121 211" stroke="#0A2239" stroke-width="3" stroke-linecap="round" stroke-linejoin="round"/>
            <text x="142" y="211" fill="#FFFFFF" font-family="'Plus Jakarta Sans', sans-serif" font-weight="700" font-size="13">Sumber api berasal dari kelalaian internal karyawan toko,</text>
            <text x="142" y="231" fill="#48CAE4" font-family="'Inter', sans-serif" font-weight="600" font-size="12">bukan dari aktivitas pembakaran sampah oleh warga sekitar.</text>
          </svg>
        `
      };

      return svgs[key] || svgs.jalan;
    }

    // =========================================================================
    // 2. DATA LENGKAP 8 ARTIKEL BERITA PURWASUKA (100% UTUH SESUAI DOKUMEN)
    // =========================================================================
    const articlesData = [
      {
        id: 1,
        featured: true,
        rubrik: 'Purwasuka Hari Ini',
        wilayah: 'Purwakarta',
        dateline: 'PURWAKARTA, segitiga.id',
        readTime: '3 Menit Baca',
        illustrationKey: 'jalan',
        caption: 'Gambar hanya sebagai ilustrasi',
        title: 'SETELAH BERTAHUN-TAHUN DIKELUHKAN WARGA, JALAN PENGHUBUNG PURWAKARTA-SUBANG AKHIRNYA MULAI DIPERBAIKI',
        excerpt: 'Kabar baik akhirnya datang bagi masyarakat yang tinggal di wilayah perbatasan Kabupaten Purwakarta dan Kabupaten Subang. Setelah bertahun-tahun mengalami kerusakan dan menjadi keluhan warga, jalan penghubung kedua kabupaten tersebut kini mulai mendapatkan perbaikan.',
        paragraphs: [
          'PURWAKARTA, segitiga.id - Kabar baik akhirnya datang bagi masyarakat yang tinggal di wilayah perbatasan Kabupaten Purwakarta dan Kabupaten Subang. Setelah bertahun-tahun mengalami kerusakan dan menjadi keluhan warga, jalan penghubung kedua kabupaten tersebut kini mulai mendapatkan perbaikan. Jalan yang selama ini menjadi salah satu akses utama mobilitas masyarakat tersebut sebelumnya mengalami kerusakan cukup parah, mulai dari permukaan aspal yang mengelupas, lubang di sejumlah titik, hingga kondisi jalan yang tidak rata. Kerusakan tersebut telah berlangsung cukup lama dan dinilai mengganggu aktivitas masyarakat yang setiap hari melintasi jalur tersebut.',
          'Kondisi jalan yang rusak selama ini menjadi persoalan bagi pengendara, khususnya pengguna sepeda motor dan kendaraan pengangkut barang. Saat musim hujan, sejumlah lubang jalan kerap tertutup genangan air sehingga sulit terlihat oleh pengendara. Situasi tersebut meningkatkan risiko kecelakaan dan membuat perjalanan menjadi lebih lambat. Tidak sedikit warga yang mengaku harus mengurangi kecepatan kendaraan atau mencari jalur alternatif untuk menghindari bagian jalan yang mengalami kerusakan paling parah. Padahal, jalan tersebut memiliki peran penting sebagai penghubung aktivitas ekonomi, pendidikan, dan sosial masyarakat dari kedua kabupaten.',
          'Salah seorang warga yang setiap hari melintasi jalur tersebut mengungkapkan rasa syukurnya setelah melihat aktivitas perbaikan mulai dilakukan. Menurutnya, masyarakat sudah cukup lama menantikan perhatian pemerintah terhadap kondisi jalan tersebut. "Kami sudah bertahun-tahun melewati jalan yang rusak seperti ini. Apalagi kalau hujan, lubangnya tertutup air dan sangat membahayakan pengendara. Kami berharap perbaikan kali ini benar-benar selesai dan tidak hanya dilakukan sementara," ungkapnya. Warga lainnya juga berharap proses pengerjaan dapat dilakukan secara menyeluruh, terutama pada titik-titik yang mengalami kerusakan cukup berat.',
          'Dalam pelaksanaannya, perbaikan jalan dilakukan secara bertahap dengan mencakup penambalan lubang, pengaspalan ulang, serta pemerataan permukaan jalan di sejumlah titik yang mengalami kerusakan. Pekerjaan tersebut diharapkan dapat meningkatkan kenyamanan dan keselamatan pengguna jalan. Masyarakat juga meminta agar pihak terkait melakukan pengawasan terhadap kualitas pengerjaan sehingga hasil perbaikan dapat bertahan dalam jangka panjang. Selain itu, pemeliharaan secara berkala dinilai penting untuk mencegah kerusakan serupa kembali terjadi, mengingat jalur tersebut memiliki intensitas penggunaan yang cukup tinggi setiap harinya.',
          'Dimulainya perbaikan jalan ini menjadi harapan baru bagi masyarakat di perbatasan Purwakarta dan Subang. Warga berharap akses transportasi yang lebih baik dapat memperlancar perjalanan, mendukung kegiatan perdagangan, serta memudahkan masyarakat dalam menjalankan aktivitas sehari-hari. Mereka juga berharap pemerintah dapat memberikan perhatian lebih terhadap infrastruktur di wilayah perbatasan yang selama ini menjadi jalur penting penghubung antardaerah. Dengan adanya perbaikan tersebut, masyarakat kini menantikan penyelesaian pengerjaan hingga seluruh ruas jalan dapat kembali digunakan dengan aman dan nyaman.'
        ]
      },
      {
        id: 2,
        featured: false,
        rubrik: 'Purwasuka Pendidikan',
        wilayah: 'Karawang',
        dateline: 'KARAWANG, segitiga.id',
        readTime: '3 Menit Baca',
        illustrationKey: 'inovasi',
        caption: 'Gambar hanya ilustrasi',
        title: 'MAHASISWA ASAL KARAWANG RAIH PRESTASI NASIONAL, KEMBANGKAN INOVASI PENGOLAHAN SAMPAH MENJADI ENERGI ALTERNATIF',
        excerpt: 'Prestasi membanggakan kembali ditorehkan oleh mahasiswa asal Kabupaten Karawang, Jawa Barat. Sekelompok mahasiswa berhasil meraih juara pertama dalam ajang Kompetisi Inovasi Mahasiswa Nasional 2026 melalui pengembangan teknologi pengolahan sampah organik menjadi energi alternatif.',
        paragraphs: [
          'KARAWANG, segitiga.id - Prestasi membanggakan kembali ditorehkan oleh mahasiswa asal Kabupaten Karawang, Jawa Barat. Sekelompok mahasiswa dari Universitas Teknologi Karawang (nama perguruan tinggi fiktif) berhasil meraih juara pertama dalam ajang Kompetisi Inovasi Mahasiswa Nasional 2026 melalui pengembangan teknologi pengolahan sampah organik menjadi energi alternatif. Kompetisi tersebut diikuti oleh puluhan perguruan tinggi dari berbagai daerah di Indonesia. Inovasi yang mereka hadirkan dinilai memiliki potensi untuk membantu mengatasi permasalahan sampah sekaligus memberikan solusi terhadap kebutuhan energi alternatif yang lebih ramah lingkungan.',
          'Tim mahasiswa yang terdiri atas tiga orang tersebut mengembangkan sebuah alat pengolah sampah organik yang mampu menghasilkan biogas melalui proses fermentasi. Bahan baku yang digunakan berasal dari sampah rumah tangga, seperti sisa sayuran, kulit buah, dan limbah makanan yang selama ini sering kali berakhir di tempat pembuangan akhir. Melalui penelitian dan pengembangan selama kurang lebih enam bulan, mereka berhasil menciptakan prototipe alat yang dapat mengubah sampah organik menjadi sumber energi yang berpotensi dimanfaatkan untuk kebutuhan memasak dalam skala rumah tangga. Inovasi tersebut juga dirancang menggunakan bahan dan komponen yang relatif mudah ditemukan sehingga diharapkan dapat dikembangkan lebih lanjut oleh masyarakat.',
          'Ketua tim inovasi, Andika Pratama (nama fiktif), menjelaskan bahwa gagasan tersebut berawal dari keprihatinannya terhadap persoalan sampah di lingkungan tempat tinggalnya. Menurutnya, sampah organik masih sering dianggap sebagai limbah yang tidak memiliki nilai guna, padahal apabila dikelola dengan tepat dapat menghasilkan manfaat bagi masyarakat. "Kami melihat bahwa persoalan sampah masih menjadi tantangan di lingkungan sekitar. Dari situ kami mencoba mencari solusi sederhana agar sampah yang sebelumnya tidak dimanfaatkan bisa diolah menjadi sesuatu yang bernilai, salah satunya sebagai sumber energi alternatif," ungkap Andika. Ia juga menjelaskan bahwa proses pengembangan alat tersebut tidak selalu berjalan mudah karena tim harus melakukan beberapa kali percobaan untuk mendapatkan hasil fermentasi yang optimal.',
          'Keberhasilan tersebut mendapatkan apresiasi dari pihak kampus yang menilai bahwa prestasi mahasiswa tidak hanya diukur melalui pencapaian akademik, tetapi juga melalui kemampuan menghasilkan gagasan dan inovasi yang bermanfaat bagi masyarakat. Pihak universitas berharap penghargaan yang diraih dapat menjadi motivasi bagi mahasiswa lainnya untuk terus mengembangkan kreativitas, melakukan penelitian, serta berani mengikuti kompetisi di tingkat nasional maupun internasional. Selain itu, kampus berencana memberikan pendampingan lanjutan agar hasil penelitian tersebut dapat disempurnakan dan memiliki peluang untuk diterapkan dalam kehidupan masyarakat. Inovasi tersebut juga diharapkan dapat menjadi salah satu bentuk kontribusi perguruan tinggi dalam mendukung pengelolaan lingkungan yang lebih berkelanjutan.'
        ]
      },
      {
        id: 3,
        featured: false,
        rubrik: 'Purwasuka Budaya & Wisata',
        wilayah: 'Purwakarta',
        dateline: 'PURWAKARTA, segitiga.id',
        readTime: '3 Menit Baca',
        illustrationKey: 'konser',
        caption: 'Gambar hanya ilustrasi',
        title: 'KONSER NOSTALGIA PURWAKARTA 2026, SIAP HADIRKAN DEWA 19 HINGGA SHEILA ON 7',
        excerpt: 'Kabupaten Purwakarta dikabarkan akan menjadi tuan rumah sebuah konser musik bertajuk "Nostalgia Musik Indonesia 2026" pada Sabtu, 19 Desember 2026 di Lapangan Purnawarman, menghadirkan Dewa 19, Sheila On 7, Ungu, D\'Masiv, dan Nidji.',
        paragraphs: [
          'PURWAKARTA, segitiga.id - Kabar gembira bagi para pencinta musik Indonesia, khususnya generasi yang tumbuh bersama lagu-lagu populer era 1990-an hingga 2000-an. Kabupaten Purwakarta dikabarkan akan menjadi tuan rumah sebuah konser musik bertajuk "Nostalgia Musik Indonesia 2026" yang siap menghadirkan sejumlah grup musik legendaris Tanah Air. Konser tersebut direncanakan berlangsung pada Sabtu, 19 Desember 2026, bertempat di Lapangan Purnawarman, Purwakarta. Acara ini dipersiapkan sebagai salah satu hiburan akhir tahun yang mengusung konsep nostalgia dengan menghadirkan lagu-lagu yang pernah menjadi bagian dari perjalanan musik masyarakat Indonesia.',
          'Sejumlah musisi dan grup band yang dijadwalkan tampil dalam konser tersebut antara lain Dewa 19, Sheila On 7, Ungu, D\'Masiv, dan Nidji. Kehadiran nama-nama besar tersebut diperkirakan akan menarik perhatian para penggemar musik dari berbagai kalangan usia, mulai dari generasi milenial hingga generasi muda. Penonton nantinya akan diajak bernostalgia melalui berbagai lagu populer yang masih sering didengarkan hingga saat ini. Konsep pertunjukan dirancang dengan menghadirkan suasana konser terbuka yang dilengkapi tata panggung, pencahayaan, dan sistem suara untuk memberikan pengalaman hiburan yang menarik bagi para pengunjung.',
          'Selain pertunjukan musik, penyelenggara juga menyiapkan sejumlah kegiatan pendukung untuk memeriahkan acara. Pengunjung dapat menikmati area kuliner yang menghadirkan berbagai makanan khas Purwakarta, bazar produk UMKM lokal, serta stan komunitas kreatif. Kehadiran berbagai kegiatan tersebut diharapkan dapat memberikan kesempatan kepada pelaku usaha lokal untuk memperkenalkan produk mereka kepada pengunjung yang datang dari luar daerah. Konser ini juga diharapkan mampu meningkatkan aktivitas ekonomi masyarakat, khususnya para pedagang makanan, pelaku usaha kecil, dan penyedia jasa di sekitar lokasi kegiatan.',
          'Penyelenggara kegiatan dalam keterangan fiktifnya menyampaikan bahwa konser ini tidak hanya bertujuan menghadirkan hiburan, tetapi juga menjadi wadah untuk mempertemukan masyarakat melalui musik. Menurut pihak penyelenggara, lagu-lagu dari grup musik yang dihadirkan memiliki kenangan tersendiri bagi banyak orang sehingga konsep nostalgia dipilih sebagai tema utama acara. Konser direncanakan mulai berlangsung pukul 16.00 WIB hingga selesai. Masyarakat yang berminat menghadiri kegiatan tersebut diimbau untuk memperhatikan informasi mengenai harga tiket, kategori penonton, akses masuk, serta ketentuan acara melalui kanal resmi penyelenggara.',
          'Melalui penyelenggaraan Konser Nostalgia Musik Indonesia 2026, Purwakarta diharapkan dapat menjadi salah satu tujuan hiburan masyarakat menjelang pergantian tahun. Kehadiran konser berskala besar ini juga diharapkan mampu memperkenalkan potensi daerah sekaligus mendorong pertumbuhan sektor hiburan dan ekonomi kreatif. Bagi masyarakat yang ingin menikmati kembali lagu-lagu penuh kenangan bersama teman maupun keluarga, acara ini tentu menjadi salah satu agenda yang menarik untuk dinantikan. Jadi, siapkan diri untuk bernyanyi bersama dan menikmati malam penuh nostalgia bersama musisi favorit di Purwakarta.'
        ]
      },
      {
        id: 4,
        featured: false,
        rubrik: 'Purwasuka Budaya & Wisata',
        wilayah: 'Purwasuka',
        dateline: 'PURWASUKA, segitiga.id',
        readTime: '3 Menit Baca',
        illustrationKey: 'wisata',
        caption: 'Rekomendasi 5 destinasi wisata akhir pekan di Purwakarta, Subang, dan Karawang.',
        title: 'BINGUNG MENGHABISKAN AKHIR PEKAN? INI 5 DESTINASI WISATA MENARIK DI PURWASUKA YANG WAJIB DIKUNJUNGI',
        excerpt: 'Bagi masyarakat yang tinggal di wilayah Purwakarta, Subang, dan Karawang, terdapat berbagai destinasi wisata menarik mulai dari Taman Air Mancur Sri Baduga, Curug Cileat, Pantai Tanjung Pakis, Sari Ater, hingga Curug Cigentis.',
        paragraphs: [
          'PURWASUKA - Akhir pekan menjadi waktu yang tepat untuk beristirahat sejenak dari rutinitas pekerjaan maupun aktivitas sehari-hari. Bagi masyarakat yang tinggal di wilayah Purwakarta, Subang, dan Karawang, terdapat berbagai destinasi wisata menarik yang dapat menjadi pilihan untuk menghabiskan waktu bersama keluarga maupun teman. Ketiga kabupaten tersebut memiliki daya tarik wisata yang beragam, mulai dari wisata alam, pantai, pemandian air panas, hingga taman rekreasi. Tidak perlu melakukan perjalanan terlalu jauh, masyarakat dapat menikmati berbagai pengalaman liburan menarik di wilayah Purwasuka.',
          'Berikut lima tempat wisata yang bisa masuk dalam daftar kunjungan akhir pekan:'
        ],
        listItems: [
          {
            title: '1. Taman Air Mancur Sri Baduga, Purwakarta',
            desc: 'Terletak di kawasan Situ Buleud, tempat ini menjadi salah satu ikon wisata Purwakarta. Pengunjung dapat menikmati suasana taman kota, bersantai, dan berfoto bersama keluarga. Pertunjukan air mancur dapat dinikmati apabila sedang dijadwalkan.'
          },
          {
            title: '2. Curug Cileat, Subang',
            desc: 'Bagi pencinta alam, Curug Cileat bisa menjadi pilihan menarik. Air terjun yang dikelilingi pepohonan hijau ini menawarkan suasana sejuk dan pemandangan alam yang menyegarkan.'
          },
          {
            title: '3. Pantai Tanjung Pakis, Karawang',
            desc: 'Ingin menikmati suasana pantai? Tanjung Pakis bisa menjadi pilihan. Pengunjung dapat menikmati pemandangan laut, bermain pasir, hingga mencicipi berbagai hidangan laut yang dijual oleh masyarakat sekitar.'
          },
          {
            title: '4. Sari Ater, Subang',
            desc: 'Pemandian air panas alami di kawasan Ciater ini cocok bagi pengunjung yang ingin bersantai. Suasana pegunungan yang sejuk menjadi daya tarik tersendiri bagi wisatawan.'
          },
          {
            title: '5. Curug Cigentis, Karawang',
            desc: 'Terletak di kawasan pegunungan Karawang, Curug Cigentis menawarkan pemandangan air terjun yang dikelilingi alam hijau. Destinasi ini cocok bagi pengunjung yang ingin menikmati suasana alam dan berpetualang.'
          }
        ],
        closingParagraphs: [
          'Kelima destinasi tersebut bisa menjadi alternatif liburan tanpa harus bepergian terlalu jauh. Pastikan untuk memeriksa kondisi cuaca, akses jalan, tarif masuk, dan jam operasional sebelum berkunjung.'
        ]
      },
      {
        id: 5,
        featured: false,
        rubrik: 'Purwasuka Sosial',
        wilayah: 'Subang',
        dateline: 'SUBANG, segitiga.id',
        readTime: '3 Menit Baca',
        illustrationKey: 'lingkungan',
        caption: 'Gambar hanya sebagai ilustrasi',
        title: 'WARGA KELUHKAN PENCEMARAN LINGKUNGAN SETELAH BERDIRINYA PABRIK BARU DI SUBANG, PEMERINTAH DIMINTA TURUN TANGAN',
        excerpt: 'Kehadiran sebuah perusahaan industri baru di salah satu kawasan Kabupaten Subang mulai menuai keluhan dari masyarakat sekitar terkait perubahan warna dan bau pada saluran air di dekat permukiman warga.',
        paragraphs: [
          'SUBANG, segitiga.id - Kehadiran sebuah perusahaan industri baru di salah satu kawasan Kabupaten Subang mulai menuai keluhan dari masyarakat sekitar. Sejumlah warga mengaku mengalami perubahan kondisi lingkungan sejak aktivitas operasional perusahaan tersebut berlangsung. Keluhan terutama berkaitan dengan kondisi saluran air yang berada tidak jauh dari kawasan permukiman. Warga menduga adanya pembuangan air limbah industri yang belum dikelola secara optimal sehingga menimbulkan perubahan warna dan bau pada aliran air di sekitar tempat tinggal mereka. Kondisi tersebut memunculkan kekhawatiran masyarakat terhadap kualitas lingkungan dan dampaknya bagi kehidupan sehari-hari.',
          'Selain perubahan kondisi saluran air, beberapa warga juga mengeluhkan munculnya bau tidak sedap pada waktu-waktu tertentu, terutama ketika aktivitas produksi perusahaan sedang berlangsung. Masyarakat khawatir apabila kondisi tersebut terus dibiarkan, dampaknya dapat semakin meluas dan mengganggu kenyamanan lingkungan permukiman. Salah seorang warga setempat, Dedi (nama samaran), mengatakan bahwa kondisi lingkungan sebelumnya relatif baik sebelum aktivitas industri mulai berjalan. Ia menjelaskan bahwa masyarakat sebenarnya mendukung pembangunan industri karena dapat membuka kesempatan kerja bagi penduduk sekitar, tetapi perusahaan tetap harus memperhatikan dampak lingkungan yang ditimbulkan dari kegiatan operasionalnya.',
          '"Kami tidak menolak adanya pembangunan pabrik karena tentu bisa membuka lapangan pekerjaan bagi masyarakat. Namun, kami juga berharap perusahaan memperhatikan kondisi lingkungan dan warga yang tinggal di sekitarnya. Jangan sampai masyarakat justru harus menanggung dampak buruk dari aktivitas industri tersebut," ungkapnya. Warga berharap perusahaan segera melakukan evaluasi terhadap sistem pengelolaan limbah, termasuk memastikan ketersediaan instalasi pengolahan air limbah atau IPAL yang sesuai dengan ketentuan. Mereka juga meminta agar saluran pembuangan tidak langsung dialirkan ke lingkungan permukiman tanpa melalui proses pengolahan yang memadai.',
          'Menanggapi keluhan tersebut, masyarakat meminta pemerintah daerah melalui instansi terkait segera melakukan pemeriksaan terhadap aktivitas perusahaan. Pemeriksaan diharapkan mencakup sistem pengelolaan limbah, kondisi saluran pembuangan, serta pengujian kualitas air di sekitar kawasan industri. Langkah tersebut dinilai penting untuk memastikan apakah dugaan pencemaran lingkungan benar-benar terjadi dan mengetahui penyebab perubahan kondisi air yang dikeluhkan warga. Selain itu, masyarakat berharap pemerintah dapat memfasilitasi komunikasi antara pihak perusahaan dan warga agar persoalan tersebut dapat diselesaikan secara terbuka tanpa menimbulkan konflik berkepanjangan.',
          'Masyarakat berharap keberadaan industri di Kabupaten Subang dapat memberikan manfaat ekonomi tanpa mengabaikan kelestarian lingkungan. Pembukaan lapangan pekerjaan dan peningkatan investasi memang menjadi salah satu faktor penting dalam perkembangan daerah, tetapi pengelolaan lingkungan harus tetap menjadi tanggung jawab perusahaan. Warga meminta adanya pengawasan secara berkala agar aktivitas produksi tidak menimbulkan dampak negatif bagi lingkungan permukiman. Dengan adanya perhatian dari pemerintah dan tanggung jawab perusahaan, masyarakat berharap pembangunan industri dapat berjalan berdampingan dengan kehidupan warga serta tetap menjaga kualitas lingkungan untuk generasi mendatang.'
        ]
      },
      {
        id: 6,
        featured: false,
        rubrik: 'Purwasuka Ekonomi',
        wilayah: 'Purwasuka',
        dateline: 'PURWASUKA, segitiga.id',
        readTime: '3 Menit Baca',
        illustrationKey: 'umk',
        caption: 'Gambar hanya sebagai ilustrasi',
        title: 'KABAR BAIK BAGI PEKERJA! UMK PURWAKARTA, SUBANG, DAN KARAWANG DIPROYEKSIKAN NAIK PADA 2027',
        excerpt: 'Dalam simulasi pemberitaan ini, UMK Purwakarta, Subang, dan Karawang diproyeksikan mengalami kenaikan pada tahun 2027 dengan Karawang tetap menempati nominal tertinggi di kawasan Purwasuka.',
        paragraphs: [
          'PURWASUKA, segitiga.id - Kabar mengenai kenaikan Upah Minimum Kabupaten (UMK) menjadi perhatian para pekerja di wilayah Purwakarta, Subang, dan Karawang. Dalam simulasi pemberitaan ini, ketiga daerah tersebut diproyeksikan mengalami kenaikan upah minimum pada tahun 2027. Informasi tersebut menjadi salah satu isu yang banyak diperhatikan masyarakat, khususnya para pekerja sektor industri dan manufaktur yang mendominasi sejumlah kawasan di wilayah Purwasuka. Kenaikan upah minimum diharapkan dapat membantu pekerja dalam memenuhi kebutuhan hidup sehari-hari, terutama di tengah perubahan harga berbagai kebutuhan pokok yang terus menjadi perhatian masyarakat.',
          'Berdasarkan data simulasi yang disusun untuk pemberitaan ini, Kabupaten Purwakarta yang sebelumnya memiliki UMK sebesar Rp5.052.856 pada tahun 2026 diproyeksikan meningkat menjadi Rp5.305.000 pada tahun 2027. Sementara itu, Kabupaten Subang yang memiliki UMK sebesar Rp3.737.482 pada tahun 2026 diproyeksikan mengalami kenaikan menjadi Rp3.925.000. Adapun Kabupaten Karawang yang sebelumnya memiliki UMK sebesar Rp5.886.853 diproyeksikan meningkat menjadi Rp6.180.000 pada tahun 2027. Angka tersebut merupakan ilustrasi kenaikan upah di ketiga wilayah dan belum merupakan ketetapan resmi pemerintah.'
        ],
        umkTable: [
          { daerah: 'Kabupaten Purwakarta', umk2026: 'Rp5.052.856', proyeksi2027: 'Rp5.305.000' },
          { daerah: 'Kabupaten Subang', umk2026: 'Rp3.737.482', proyeksi2027: 'Rp3.925.000' },
          { daerah: 'Kabupaten Karawang', umk2026: 'Rp5.886.853', proyeksi2027: 'Rp6.180.000' }
        ],
        closingParagraphs: [
          'Dari ketiga kabupaten tersebut, Karawang masih menempati posisi dengan nominal UMK tertinggi berdasarkan angka simulasi yang digunakan. Kondisi ini tidak terlepas dari besarnya aktivitas industri dan manufaktur yang berkembang di wilayah tersebut. Sementara itu, Purwakarta juga memiliki sejumlah kawasan industri yang menyerap tenaga kerja dalam jumlah besar. Kabupaten Subang pun terus mengembangkan sektor industri dan investasi untuk mendorong pertumbuhan ekonomi daerah. Perbedaan nominal upah minimum di masing-masing kabupaten menunjukkan adanya variasi kondisi ekonomi, struktur industri, serta karakteristik ketenagakerjaan di setiap wilayah.',
          'Bagi para pekerja, kenaikan UMK diharapkan dapat meningkatkan daya beli dan membantu memenuhi kebutuhan rumah tangga. Namun, penyesuaian upah juga menjadi perhatian bagi para pelaku usaha karena dapat memengaruhi perencanaan biaya operasional perusahaan. Oleh karena itu, kebijakan pengupahan perlu mempertimbangkan kondisi ekonomi, produktivitas tenaga kerja, serta kemampuan dunia usaha. Pemerintah juga diharapkan dapat memastikan bahwa perusahaan menjalankan ketentuan pengupahan sesuai dengan peraturan yang berlaku sehingga hak pekerja tetap terlindungi.',
          'Masyarakat, khususnya para pekerja di wilayah Purwasuka, diimbau untuk menunggu pengumuman resmi pemerintah mengenai penetapan UMK tahun 2027. Informasi mengenai besaran upah minimum perlu diperoleh melalui sumber resmi agar tidak menimbulkan kesalahpahaman. Terlepas dari proyeksi kenaikan tersebut, para pekerja berharap kebijakan pengupahan dapat memberikan kesejahteraan yang lebih baik sekaligus mendukung hubungan industrial yang sehat. Dengan keseimbangan antara perlindungan tenaga kerja dan keberlangsungan usaha, pertumbuhan ekonomi di Purwakarta, Subang, dan Karawang diharapkan dapat berjalan secara berkelanjutan.'
        ]
      },
      {
        id: 7,
        featured: false,
        rubrik: 'Purwasuka Rasa',
        wilayah: 'Karawang',
        dateline: 'KARAWANG, segitiga.id',
        readTime: '2 Menit Baca',
        illustrationKey: 'kuliner',
        caption: 'Rekomendasi 3 sajian kuliner khas Kabupaten Karawang.',
        title: 'KANGEN KULINER KARAWANG? INI 3 MAKANAN KHAS DAN REKOMENDASI TEMPAT YANG WAJIB MASUK DAFTAR KUNJUNGANMU!',
        excerpt: 'Berbicara tentang Karawang, bukan hanya kawasan industri dan hamparan persawahan yang menjadi daya tariknya. Kabupaten ini juga memiliki Pepes Jambal Walahar, Soto Tangkar Karawang, dan Serabi Hijau.',
        paragraphs: [
          'KARAWANG, segitiga.id - Berbicara tentang Karawang, bukan hanya kawasan industri dan hamparan persawahan yang menjadi daya tariknya. Kabupaten ini juga memiliki beragam kuliner khas yang sayang untuk dilewatkan.',
          'Bagi kamu yang sedang berkunjung atau ingin bernostalgia dengan cita rasa makanan khas Karawang, berikut tiga rekomendasi kuliner yang bisa dicoba:'
        ],
        listItems: [
          {
            title: '1. Pepes Jambal Walahar',
            desc: 'Kalau berkunjung ke Karawang, rasanya belum lengkap tanpa mencicipi pepes jambal khas Walahar. Olahan ikan yang dibumbui rempah-rempah dan dibungkus daun pisang ini memiliki cita rasa gurih dan khas. Kawasan Walahar juga dikenal sebagai salah satu tujuan wisata kuliner yang cukup populer di Karawang.'
          },
          {
            title: '2. Soto Tangkar Karawang',
            desc: 'Bagi pencinta makanan berkuah, Soto Tangkar bisa menjadi pilihan. Hidangan ini menggunakan daging sapi dan kuah berbumbu rempah yang kaya rasa. Cocok dinikmati saat makan siang bersama keluarga.'
          },
          {
            title: '3. Serabi Hijau',
            desc: 'Ingin mencari camilan tradisional? Serabi hijau bisa menjadi pilihan. Teksturnya lembut dengan aroma pandan dan cita rasa manis yang cocok dinikmati sebagai teman bersantai.'
          }
        ],
        closingParagraphs: [
          'Ketiga kuliner tersebut dapat menjadi pilihan untuk mengenal lebih dekat kekayaan cita rasa daerah Karawang.',
          'Jadi, kalau akhir pekan ini kamu berkunjung ke Karawang, jangan lupa masukkan wisata kuliner ke dalam agenda perjalananmu!'
        ]
      },
      {
        id: 8,
        featured: false,
        rubrik: 'Purwasuka Fakta',
        wilayah: 'Subang',
        dateline: 'SUBANG, segitiga.id',
        readTime: '3 Menit Baca',
        illustrationKey: 'klarifikasi',
        caption: 'Gambar hanya sebagai ilustrasi',
        title: 'KLARIFIKASI KEBAKARAN TOKO BAHTERA JAYA, PIMPINAN TOKO TEGASKAN SUMBER API BERASAL DARI KELALAIAN INTERNAL',
        excerpt: 'Pimpinan Toko Bahtera Jaya memberikan klarifikasi resmi meluruskan isu yang beredar di masyarakat: sumber api berasal dari kelalaian internal karyawan toko, bukan pembakaran sampah oleh warga sekitar.',
        paragraphs: [
          'SUBANG, segitiga.id - Pimpinan Toko Bahtera Jaya akhirnya memberikan klarifikasi terkait peristiwa kebakaran hebat yang sebelumnya menghanguskan sebagian besar bangunan toko tersebut. Klarifikasi ini disampaikan menyusul beredarnya informasi di tengah masyarakat yang menyebutkan bahwa kebakaran diduga berasal dari aktivitas pembakaran sampah oleh warga di sekitar lokasi. Informasi tersebut sempat menjadi perbincangan masyarakat dan menimbulkan kesalahpahaman terhadap warga yang tinggal di sekitar toko. Melalui keterangan resminya, pihak manajemen ingin meluruskan informasi yang berkembang agar masyarakat memperoleh penjelasan mengenai penyebab kebakaran berdasarkan hasil pemeriksaan internal.',
          'Dalam keterangannya, pimpinan Toko Bahtera Jaya menjelaskan bahwa berdasarkan pemeriksaan internal, sumber api justru diduga berasal dari kelalaian salah satu karyawan toko. Sebelum kejadian, terdapat aktivitas yang dilakukan oleh karyawan di area belakang bangunan. Namun, setelah aktivitas tersebut selesai, sumber api diduga tidak dipastikan benar-benar padam. Kondisi tersebut kemudian menyebabkan api membesar dan merambat ke bagian bangunan lainnya hingga menimbulkan kebakaran yang cukup parah. Peristiwa tersebut mengakibatkan sejumlah bagian bangunan mengalami kerusakan dan menimbulkan kerugian material bagi pihak toko.',
          '"Kami ingin meluruskan informasi yang berkembang di masyarakat. Berdasarkan hasil pemeriksaan internal kami, sumber api berasal dari kelalaian karyawan kami sendiri, bukan dari aktivitas pembakaran sampah oleh warga sekitar. Kami menyampaikan klarifikasi ini agar tidak ada lagi kesalahpahaman yang merugikan masyarakat," ungkap pimpinan Toko Bahtera Jaya dalam keterangan tertulisnya. Ia juga menyampaikan permohonan maaf kepada warga sekitar apabila informasi yang sebelumnya beredar telah menimbulkan keresahan atau membuat masyarakat merasa disalahkan atas kejadian tersebut. Pihak manajemen menegaskan bahwa warga sekitar tidak seharusnya menjadi sasaran tuduhan tanpa adanya bukti yang jelas.',
          'Sebagai bentuk tanggung jawab, pihak manajemen berkomitmen untuk melakukan evaluasi terhadap prosedur keselamatan kerja di lingkungan toko. Beberapa langkah yang akan dilakukan meliputi peningkatan pengawasan terhadap aktivitas karyawan, pemeriksaan rutin terhadap area yang berpotensi menimbulkan kebakaran, serta penyediaan fasilitas pencegahan dan penanganan kebakaran yang lebih memadai. Pimpinan toko juga menegaskan pentingnya memberikan pemahaman kepada seluruh karyawan mengenai prosedur keselamatan kerja agar kejadian serupa tidak kembali terulang. Evaluasi tersebut diharapkan dapat meningkatkan keamanan bangunan sekaligus memberikan rasa nyaman bagi masyarakat yang berada di sekitar lokasi usaha.',
          'Melalui klarifikasi tersebut, pihak Toko Bahtera Jaya berharap informasi yang sebelumnya berkembang dapat diluruskan dan tidak lagi menimbulkan kesalahpahaman di tengah masyarakat. Peristiwa ini menjadi pengingat bahwa penyebaran informasi mengenai suatu kejadian perlu didasarkan pada fakta dan keterangan yang dapat dipertanggungjawabkan. Masyarakat juga diimbau untuk tidak langsung mempercayai atau menyebarkan informasi yang belum terverifikasi, terutama apabila informasi tersebut menyangkut nama baik seseorang atau kelompok tertentu. SEGITIGA mengajak seluruh masyarakat untuk lebih bijak dalam menerima informasi serta memberikan ruang bagi pihak terkait untuk menyampaikan klarifikasi demi terciptanya lingkungan informasi yang sehat dan bertanggung jawab.'
        ]
      }
    ];

    // =========================================================================
    // 3. STATE FILTER & RENDER PORTAL BERITA
    // =========================================================================
    let activeRubrik = 'Semua';
    let activeRegion = 'Semua';
    let searchQuery = '';
    let currentOpenedArticleId = 1;

    function getRubrikBadgeStyle(rubrik) {
      const map = {
        'Purwasuka Hari Ini': 'bg-navy text-cyanbrand',
        'Purwasuka Pendidikan': 'bg-royal text-white',
        'Purwasuka Budaya & Wisata': 'bg-cyanbrand/20 text-navy',
        'Purwasuka Sosial': 'bg-slate-800 text-white',
        'Purwasuka Ekonomi': 'bg-sky-100 text-royal',
        'Purwasuka Rasa': 'bg-amber-100 text-amber-900',
        'Purwasuka Fakta': 'bg-emerald-100 text-emerald-900'
      };
      return map[rubrik] || 'bg-navy text-white';
    }

    function renderNewsSection() {
      const featuredContainer = document.getElementById('featuredNewsContainer');
      const gridContainer = document.getElementById('newsGridContainer');
      const emptyState = document.getElementById('emptyNewsState');
      const statusBar = document.getElementById('filterStatusBar');
      const statusText = document.getElementById('filterStatusText');

      const q = searchQuery.trim().toLowerCase();

      const filtered = articlesData.filter((art) => {
        const matchRubrik = activeRubrik === 'Semua' || art.rubrik === activeRubrik;
        const matchRegion =
          activeRegion === 'Semua' ||
          art.wilayah === activeRegion ||
          (activeRegion !== 'Purwasuka' && art.wilayah === 'Purwasuka');
        const fullText = [
          art.title,
          art.excerpt,
          art.rubrik,
          art.wilayah,
          ...art.paragraphs,
          ...(art.listItems ? art.listItems.map((i) => i.title + ' ' + i.desc) : []),
          ...(art.closingParagraphs || [])
        ].join(' ').toLowerCase();
        const matchQuery = !q || fullText.includes(q);
        return matchRubrik && matchRegion && matchQuery;
      });

      // Tampilkan status bar jika ada filter aktif
      const hasActiveFilter = activeRubrik !== 'Semua' || activeRegion !== 'Semua' || q !== '';
      if (hasActiveFilter) {
        statusBar.classList.remove('hidden');
        statusText.textContent = `Menampilkan ${filtered.length} berita (Rubrik: ${activeRubrik} • Wilayah: ${activeRegion}${q ? ` • Kata kunci: "${searchQuery}"` : ''})`;
      } else {
        statusBar.classList.add('hidden');
      }

      if (filtered.length === 0) {
        featuredContainer.innerHTML = '';
        gridContainer.innerHTML = '';
        emptyState.classList.remove('hidden');
        return;
      }

      emptyState.classList.add('hidden');

      // Artikel pertama sebagai Berita Utama (Featured Headline)
      const leadArticle = filtered[0];
      const remainingArticles = filtered.slice(1);

      featuredContainer.innerHTML = `
        <article onclick="openArticleModal(${leadArticle.id})" class="group bg-white rounded-[2rem] overflow-hidden border border-slate-200/90 hover:border-cyanbrand/60 shadow-soft-navy hover:shadow-card-hover transition-all duration-300 cursor-pointer">
          <div class="grid grid-cols-1 lg:grid-cols-12 items-stretch">
            <div class="lg:col-span-6 relative bg-ice overflow-hidden">
              ${getArticleIllustrationSVG(leadArticle.illustrationKey, true)}
              <span class="absolute top-4 left-4 px-3.5 py-1.5 rounded-full bg-navy/90 backdrop-blur-sm text-cyanbrand text-xs font-heading font-extrabold uppercase tracking-wider">
                Sorotan Utama
              </span>
              <span class="absolute bottom-3 right-3 px-2.5 py-1 rounded-lg bg-navy/75 text-white/90 text-[11px] italic">
                ${leadArticle.caption}
              </span>
            </div>

            <div class="lg:col-span-6 p-6 sm:p-9 flex flex-col justify-between space-y-5">
              <div class="space-y-3.5">
                <div class="flex flex-wrap items-center gap-2">
                  <span class="px-3 py-1 rounded-full text-xs font-heading font-extrabold ${getRubrikBadgeStyle(leadArticle.rubrik)}">
                    ${leadArticle.rubrik}
                  </span>
                  <span class="px-3 py-1 rounded-full bg-ice border border-slate-200 text-navy text-xs font-heading font-bold">
                    ${leadArticle.wilayah}
                  </span>
                  <span class="text-xs text-slate-400 font-medium">• ${leadArticle.readTime}</span>
                </div>

                <h3 class="text-xl sm:text-2xl lg:text-[1.65rem] font-extrabold text-navy group-hover:text-royal leading-snug transition-colors">
                  ${leadArticle.title}
                </h3>

                <p class="text-sm sm:text-base text-slatebody leading-relaxed line-clamp-4">
                  ${leadArticle.excerpt}
                </p>
              </div>

              <div class="pt-4 border-t border-slate-100 flex items-center justify-between gap-3">
                <span class="text-xs font-semibold text-slate-500">${leadArticle.dateline}</span>
                <span class="inline-flex items-center gap-2 px-4 py-2.5 rounded-xl bg-navy group-hover:bg-cyanbrand text-white group-hover:text-navy font-heading text-xs sm:text-sm font-bold transition-colors">
                  <span>Baca Selengkapnya</span>
                  <svg class="w-3.5 h-3.5" viewBox="0 0 16 16" fill="currentColor"><path d="M4 2.5L13 8L4 13.5V2.5Z"/></svg>
                </span>
              </div>
            </div>
          </div>
        </article>
      `;

      // Render sisa artikel dalam grid 3 kolom
      gridContainer.innerHTML = remainingArticles.map((art) => `
        <article onclick="openArticleModal(${art.id})" class="group bg-white rounded-3xl overflow-hidden border border-slate-200/90 hover:border-cyanbrand/60 shadow-sm hover:shadow-card-hover transition-all duration-300 flex flex-col justify-between cursor-pointer">
          <div>
            <div class="relative bg-ice overflow-hidden">
              ${getArticleIllustrationSVG(art.illustrationKey, false)}
              <span class="absolute bottom-2.5 right-2.5 px-2 py-0.5 rounded-md bg-navy/75 text-white/90 text-[10px] italic">
                ${art.caption}
              </span>
            </div>

            <div class="p-6 space-y-3">
              <div class="flex flex-wrap items-center gap-2">
                <span class="px-2.5 py-1 rounded-full text-[11px] font-heading font-extrabold ${getRubrikBadgeStyle(art.rubrik)}">
                  ${art.rubrik}
                </span>
                <span class="px-2.5 py-1 rounded-full bg-ice border border-slate-200 text-navy text-[11px] font-heading font-bold">
                  ${art.wilayah}
                </span>
              </div>

              <h3 class="text-base sm:text-lg font-extrabold text-navy group-hover:text-royal leading-snug transition-colors line-clamp-3">
                ${art.title}
              </h3>

              <p class="text-sm text-slatebody leading-relaxed line-clamp-3">
                ${art.excerpt}
              </p>
            </div>
          </div>

          <div class="px-6 pb-6 pt-3 border-t border-slate-100 flex items-center justify-between gap-2">
            <span class="text-xs text-slate-400 font-medium">${art.readTime}</span>
            <span class="inline-flex items-center gap-1.5 text-xs font-heading font-extrabold text-royal group-hover:text-cyanbrand transition-colors">
              <span>Baca Selengkapnya</span>
              <svg class="w-3.5 h-3.5" viewBox="0 0 16 16" fill="currentColor"><path d="M4 2.5L13 8L4 13.5V2.5Z"/></svg>
            </span>
          </div>
        </article>
      `).join('');
    }

    function updateRubrikTabsUI() {
      document.querySelectorAll('.rubrik-tab').forEach((btn) => {
        const isTarget = btn.dataset.rubrik === activeRubrik;
        if (isTarget) {
          btn.className = 'rubrik-tab shrink-0 px-4 py-2.5 rounded-xl text-xs sm:text-sm font-heading font-bold bg-navy text-white transition-all cursor-pointer';
        } else {
          btn.className = 'rubrik-tab shrink-0 px-4 py-2.5 rounded-xl text-xs sm:text-sm font-heading font-bold bg-white text-slatebody border border-slate-200 hover:border-navy transition-all cursor-pointer';
        }
      });
    }

    function setRubrikFilter(rubrik) {
      activeRubrik = rubrik;
      updateRubrikTabsUI();
      renderNewsSection();
    }

    function selectRubrikTab(rubrik) {
      setRubrikFilter(rubrik);
    }

    function selectRubrikFromCard(rubrik) {
      setRubrikFilter(rubrik);
      document.getElementById('berita').scrollIntoView({ behavior: 'smooth' });
    }

    function filterNewsByRegion(region) {
      activeRegion = region;
      document.getElementById('regionFilterSelect').value = region;
      renderNewsSection();
      document.getElementById('berita').scrollIntoView({ behavior: 'smooth' });
    }

    function handleRegionSelect(region) {
      activeRegion = region;
      renderNewsSection();
    }

    function handleSearchInput(val) {
      searchQuery = val;
      renderNewsSection();
    }

    function resetAllFilters() {
      activeRubrik = 'Semua';
      activeRegion = 'Semua';
      searchQuery = '';
      document.getElementById('regionFilterSelect').value = 'Semua';
      document.getElementById('newsSearchInput').value = '';
      updateRubrikTabsUI();
      renderNewsSection();
    }

    // =========================================================================
    // 4. MODAL PEMBACA ARTIKEL LENGKAP (100% TEKS UTUH)
    // =========================================================================
    const articleModal = document.getElementById('articleModal');

    function openArticleModal(articleId) {
      const idx = articlesData.findIndex((a) => a.id === articleId);
      if (idx === -1) return;

      currentOpenedArticleId = articleId;
      const art = articlesData[idx];

      document.getElementById('modalArticleRubrik').textContent = art.rubrik;
      document.getElementById('modalArticleRegion').textContent = art.wilayah;
      document.getElementById('modalArticleDateline').textContent = art.dateline;
      document.getElementById('modalArticleReadTime').textContent = art.readTime;
      document.getElementById('articleModalHeading').textContent = art.title;
      document.getElementById('modalArticleIllustration').innerHTML = getArticleIllustrationSVG(art.illustrationKey, true);
      document.getElementById('modalArticleCaption').textContent = art.caption;

      // Susun isi lengkap 100% utuh
      let bodyHtml = art.paragraphs.map((p) => `<p>${p}</p>`).join('');

      // Jika artikel memiliki daftar bernomor (Artikel 4 Wisata & Artikel 7 Kuliner)
      if (art.listItems && art.listItems.length > 0) {
        const listHtml = art.listItems.map((item) => `
          <div class="p-4 sm:p-5 rounded-2xl bg-ice border border-slate-200/80">
            <h4 class="text-base font-extrabold text-navy mb-1.5">${item.title}</h4>
            <p class="text-sm sm:text-base text-slatebody leading-relaxed">${item.desc}</p>
          </div>
        `).join('');
        bodyHtml += `<div class="space-y-3 my-4">${listHtml}</div>`;
      }

      // Jika artikel memiliki tabel komparasi UMK (Artikel 6 UMK 2027)
      if (art.umkTable && art.umkTable.length > 0) {
        const rowsHtml = art.umkTable.map((row) => `
          <tr class="border-t border-slate-200">
            <td class="px-4 py-3 font-heading font-bold text-navy">${row.daerah}</td>
            <td class="px-4 py-3 text-slatebody">${row.umk2026}</td>
            <td class="px-4 py-3 font-heading font-extrabold text-royal">${row.proyeksi2027}</td>
          </tr>
        `).join('');

        bodyHtml += `
          <div class="my-5 rounded-2xl overflow-hidden border border-slate-200">
            <div class="px-4 py-2.5 bg-navy text-white text-xs font-heading font-extrabold uppercase tracking-wider">
              Tabel Simulasi Komparasi UMK 2026 vs Proyeksi 2027
            </div>
            <div class="overflow-x-auto">
              <table class="w-full text-left text-xs sm:text-sm">
                <thead class="bg-ice text-navy font-heading font-bold">
                  <tr>
                    <th class="px-4 py-3">Kabupaten</th>
                    <th class="px-4 py-3">UMK 2026</th>
                    <th class="px-4 py-3">Proyeksi 2027</th>
                  </tr>
                </thead>
                <tbody class="bg-white">
                  ${rowsHtml}
                </tbody>
              </table>
            </div>
          </div>
        `;
      }

      if (art.closingParagraphs && art.closingParagraphs.length > 0) {
        bodyHtml += art.closingParagraphs.map((p) => `<p>${p}</p>`).join('');
      }

      document.getElementById('modalArticleBody').innerHTML = bodyHtml;

      // Tombol salin ringkasan berita
      document.getElementById('modalCopyArticleBtn').onclick = () => {
        const shareText = `${art.title}\n(${art.rubrik} - ${art.wilayah})\n\n${art.excerpt}\n\nBaca selengkapnya di segitiga.id — Fakta untuk Warga`;
        copyText(shareText, 'Judul & ringkasan berita berhasil disalin!');
      };

      // Navigasi sebelumnya / berikutnya
      const prevIdx = (idx - 1 + articlesData.length) % articlesData.length;
      const nextIdx = (idx + 1) % articlesData.length;
      document.getElementById('prevArticleBtn').onclick = () => openArticleModal(articlesData[prevIdx].id);
      document.getElementById('nextArticleBtn').onclick = () => openArticleModal(articlesData[nextIdx].id);

      articleModal.classList.remove('hidden');
      articleModal.classList.add('flex');
      document.getElementById('articleModalScrollArea').scrollTop = 0;
      document.body.style.overflow = 'hidden';
    }

    function closeArticleModal() {
      articleModal.classList.add('hidden');
      articleModal.classList.remove('flex');
      document.body.style.overflow = '';
    }

    // =========================================================================
    // 5. INTERAKSI PILAR FILOSOFI LOGO
    // =========================================================================
    const philosophyData = {
      1: {
        title: 'Sisi 01 — Fakta & Kredibilitas',
        badge: '#0A2239',
        desc: 'Fondasi berita berdiri di atas verifikasi sumber primer, akurasi data, serta kepatuhan pada Kode Etik Jurnalistik.'
      },
      2: {
        title: 'Sisi 02 — Perspektif & Kedalaman',
        badge: '#0D4F8B',
        desc: 'Menghadirkan gambaran utuh dan berimbang dari Purwakarta, Subang, dan Karawang agar warga memahami konteks peristiwa.'
      },
      3: {
        title: 'Sisi 03 — Ekspresi & Konektivitas Digital',
        badge: '#00B4D8',
        desc: 'Ikon Play dan titik sinyal melambangkan penyampaian informasi yang hidup dan terhubung melalui TikTok, Instagram, dan Saluran WhatsApp.'
      }
    };

    function selectPhilosophy(side) {
      document.querySelectorAll('.philosophy-tab').forEach((btn) => {
        btn.classList.toggle('active', Number(btn.dataset.side) === side);
      });

      [1, 2, 3].forEach((idx) => {
        const el = document.getElementById(`highlightSide${idx}`);
        if (el) {
          el.classList.toggle('opacity-100', idx === side);
          el.classList.toggle('opacity-40', idx !== side);
        }
      });

      const info = philosophyData[side];
      document.getElementById('detailTitle').textContent = info.title;
      const badgeEl = document.getElementById('detailColorBadge');
      badgeEl.textContent = info.badge;
      badgeEl.style.backgroundColor = info.badge;
      document.getElementById('detailDesc').textContent = info.desc;
    }

    // =========================================================================
    // 6. FORM KIRIM LAPORAN WARGA / KERJA SAMA / HAK JAWAB
    // =========================================================================
    function sendEditorialMessage(channel) {
      const category = document.getElementById('contactCategory').value;
      const region = document.getElementById('contactRegion').value;
      const name = document.getElementById('contactName').value.trim();
      const message = document.getElementById('contactMessage').value.trim();

      if (!name || !message) {
        showToast('Mohon lengkapi nama dan isi pesan Anda terlebih dahulu.');
        return;
      }

      const formattedText =
        `Halo Redaksi SEGITIGA,\n\n` +
        `Kategori: ${category}\n` +
        `Wilayah: ${region}\n` +
        `Pengirim: ${name}\n\n` +
        `Pesan:\n${message}`;

      if (channel === 'wa') {
        const waUrl = `https://wa.me/6281234567890?text=${encodeURIComponent(formattedText)}`;
        window.open(waUrl, '_blank', 'noopener,noreferrer');
        showToast('Membuka WhatsApp Redaksi SEGITIGA...');
      } else {
        const subject = `[${category} - ${region}] dari ${name}`;
        const mailUrl = `mailto:redaksi.segitiga@gmail.com?subject=${encodeURIComponent(subject)}&body=${encodeURIComponent(formattedText)}`;
        window.location.href = mailUrl;
        showToast('Membuka aplikasi email menuju redaksi.segitiga@gmail.com...');
      }
    }

    // =========================================================================
    // 7. MODAL SALURAN RESMI, MENU MOBILE, CLIPBOARD & SCROLL REVEAL
    // =========================================================================
    const socialModal = document.getElementById('socialModal');

    function openSocialModal() {
      socialModal.classList.remove('hidden');
      socialModal.classList.add('flex');
      document.body.style.overflow = 'hidden';
    }

    function closeSocialModal() {
      socialModal.classList.add('hidden');
      socialModal.classList.remove('flex');
      document.body.style.overflow = '';
    }

    [socialModal, articleModal].forEach((modal) => {
      modal.addEventListener('click', (e) => {
        if (e.target === modal) {
          closeSocialModal();
          closeArticleModal();
        }
      });
    });

    document.addEventListener('keydown', (e) => {
      if (e.key === 'Escape') {
        closeSocialModal();
        closeArticleModal();
      }
    });

    // Toggle Menu Mobile
    const mobileMenuBtn = document.getElementById('mobileMenuBtn');
    const mobileMenu = document.getElementById('mobileMenu');
    const hamburgerIcon = document.getElementById('hamburgerIcon');
    const closeIcon = document.getElementById('closeIcon');

    mobileMenuBtn.addEventListener('click', () => {
      const isHidden = mobileMenu.classList.contains('hidden');
      mobileMenu.classList.toggle('hidden');
      hamburgerIcon.classList.toggle('hidden', !isHidden);
      closeIcon.classList.toggle('hidden', isHidden);
      mobileMenuBtn.setAttribute('aria-expanded', String(isHidden));
    });

    document.querySelectorAll('.mobile-nav-link').forEach((link) => {
      link.addEventListener('click', () => {
        mobileMenu.classList.add('hidden');
        hamburgerIcon.classList.remove('hidden');
        closeIcon.classList.add('hidden');
        mobileMenuBtn.setAttribute('aria-expanded', 'false');
      });
    });

    // Salin ke Clipboard + Toast
    let toastTimeout;
    function showToast(message) {
      const toast = document.getElementById('toastNotification');
      const toastMsg = document.getElementById('toastMessage');
      toastMsg.textContent = message;

      toast.classList.remove('opacity-0', 'translate-y-3');
      toast.classList.add('opacity-100', 'translate-y-0');

      clearTimeout(toastTimeout);
      toastTimeout = setTimeout(() => {
        toast.classList.add('opacity-0', 'translate-y-3');
        toast.classList.remove('opacity-100', 'translate-y-0');
      }, 2800);
    }

    function copyText(text, customMessage) {
      const tempInput = document.createElement('textarea');
      tempInput.value = text;
      tempInput.setAttribute('readonly', '');
      tempInput.style.position = 'fixed';
      tempInput.style.opacity = '0';
      document.body.appendChild(tempInput);
      tempInput.select();

      try {
        document.execCommand('copy');
        showToast(customMessage || 'Berhasil disalin!');
      } catch (err) {
        showToast('Silakan salin manual: ' + text);
      } finally {
        document.body.removeChild(tempInput);
      }
    }

    // Inisialisasi saat halaman dimuat
    document.addEventListener('DOMContentLoaded', () => {
      renderNewsSection();

      const revealElements = document.querySelectorAll('.reveal');
      if ('IntersectionObserver' in window) {
        const observer = new IntersectionObserver(
          (entries, obs) => {
            entries.forEach((entry) => {
              if (entry.isIntersecting) {
                entry.target.classList.add('is-visible');
                obs.unobserve(entry.target);
              }
            });
          },
          { threshold: 0.1, rootMargin: '0px 0px -25px 0px' }
        );
        revealElements.forEach((el) => observer.observe(el));
      } else {
        revealElements.forEach((el) => el.classList.add('is-visible'));
      }
    });
  </script>
</body>
</html>
