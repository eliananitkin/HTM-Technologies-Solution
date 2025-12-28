# HTM-Technologies-Solution
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>HTM Technology Solution Inc. | Technology Consulting in Greater Washington, DC</title>
  <meta name="description" content="HTM Technology Solution Inc. provides technology consulting, digital solutions, and local IT services across the Greater Washington, DC area." />
  <meta name="theme-color" content="#1E3A8A" />

  <!-- Open Graph -->
  <meta property="og:title" content="HTM Technology Solution Inc." />
  <meta property="og:description" content="Technology consulting and digital solutions in Greater Washington, DC." />
  <meta property="og:type" content="website" />

  <style>
    :root{
      /* Cream + Blue palette */
      --cream: #F7F2E8;
      --cream-2:#EFE7D7;
      --blue:#1E3A8A;
      --blue-2:#274AA6;
      --ink:#0F172A;
      --muted:#475569;
      --card:#FFFFFF;
      --ring: rgba(30,58,138,.18);
      --shadow: 0 10px 30px rgba(15, 23, 42, .10);
      --radius: 18px;
      --max: 1120px;
      --font: ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial, "Apple Color Emoji","Segoe UI Emoji";
    }
    *{box-sizing:border-box}
    html,body{margin:0;padding:0}
    body{
      font-family: var(--font);
      color: var(--ink);
      background: radial-gradient(1200px 600px at 20% 0%, var(--cream-2) 0%, var(--cream) 55%, #fff 100%);
      line-height:1.55;
    }
    a{color:inherit;text-decoration:none}
    .wrap{max-width:var(--max); margin:0 auto; padding:0 20px}
    .nav{
      position: sticky; top: 0; z-index: 50;
      backdrop-filter: blur(10px);
      background: rgba(247,242,232,.78);
      border-bottom: 1px solid rgba(15,23,42,.06);
    }
    .nav-inner{
      display:flex; align-items:center; justify-content:space-between;
      padding: 14px 0;
      gap: 14px;
    }
    .brand{
      display:flex; align-items:center; gap:10px; font-weight:800;
      letter-spacing:.2px;
    }
    .logo{
      width:36px; height:36px; border-radius:12px;
      background: linear-gradient(135deg, var(--blue), var(--blue-2));
      box-shadow: 0 8px 20px rgba(30,58,138,.25);
      position:relative;
    }
    .logo:after{
      content:"";
      position:absolute; inset:9px;
      border-radius:10px;
      background: rgba(247,242,232,.9);
      transform: rotate(12deg);
    }
    .nav-links{
      display:flex; align-items:center; gap:18px;
      font-weight:600;
      color: var(--muted);
    }
    .nav-links a:hover{color: var(--ink)}
    .cta{
      display:inline-flex; align-items:center; justify-content:center;
      padding: 10px 14px;
      border-radius: 999px;
      background: var(--blue);
      color: #fff;
      font-weight:700;
      box-shadow: 0 10px 22px rgba(30,58,138,.20);
      border: 1px solid rgba(255,255,255,.18);
    }
    .cta:hover{background: var(--blue-2)}
    .menu-btn{display:none}
    @media (max-width: 860px){
      .nav-links{display:none}
      .menu-btn{
        display:inline-flex; gap:8px; align-items:center;
        padding:10px 12px; border-radius:999px;
        border:1px solid rgba(15,23,42,.10);
        background:#fff;
        font-weight:700;
      }
      .mobile{
        display:none;
        padding: 12px 0 18px;
      }
      .mobile a{
        display:block;
        padding:10px 0;
        color: var(--muted);
        font-weight:650;
      }
      .mobile a:hover{color: var(--ink)}
      .mobile.show{display:block}
    }

    /* Hero */
    .hero{padding: 56px 0 24px}
    .hero-grid{
      display:grid; grid-template-columns: 1.2fr .8fr; gap: 28px;
      align-items:stretch;
    }
    @media (max-width: 980px){ .hero-grid{grid-template-columns:1fr} }
    .pill{
      display:inline-flex; gap:10px; align-items:center;
      padding: 8px 12px;
      border-radius:999px;
      border:1px solid rgba(15,23,42,.10);
      background: rgba(255,255,255,.7);
      color: var(--muted);
      font-weight:650;
      width: fit-content;
    }
    .dot{
      width:10px; height:10px; border-radius:999px;
      background: var(--blue);
      box-shadow: 0 0 0 6px var(--ring);
    }
    h1{
      font-size: clamp(34px, 5vw, 54px);
      line-height: 1.05;
      margin: 14px 0 12px;
      letter-spacing:-.6px;
    }
    .lead{
      font-size: 18px;
      color: var(--muted);
      max-width: 58ch;
      margin: 0 0 18px;
    }
    .hero-actions{display:flex; gap:12px; flex-wrap:wrap; margin-top: 18px}
    .secondary{
      display:inline-flex; align-items:center; justify-content:center;
      padding:10px 14px;
      border-radius:999px;
      background:#fff;
      border:1px solid rgba(15,23,42,.12);
      font-weight:750;
    }
    .secondary:hover{border-color: rgba(30,58,138,.30)}
    .trust{
      display:flex; gap:14px; flex-wrap:wrap;
      margin-top: 22px;
      color: var(--muted);
      font-weight:650;
      font-size: 14px;
    }
    .trust span{
      display:inline-flex; gap:8px; align-items:center;
      padding: 8px 10px;
      border-radius: 999px;
      background: rgba(255,255,255,.65);
      border: 1px solid rgba(15,23,42,.08);
    }

    .card{
      background: rgba(255,255,255,.85);
      border: 1px solid rgba(15,23,42,.08);
      border-radius: var(--radius);
      box-shadow: var(--shadow);
    }
    .hero-card{
      padding: 18px;
      display:flex; flex-direction:column; gap:14px;
    }
    .mini{
      border-radius: 14px;
      padding: 14px;
      border: 1px solid rgba(15,23,42,.08);
      background: linear-gradient(180deg, #fff, rgba(255,255,255,.82));
    }
    .mini h3{margin:0 0 6px; font-size: 14px; color: var(--muted); letter-spacing:.2px; text-transform: uppercase}
    .mini p{margin:0; font-weight:750}
    .divider{height:1px; background: rgba(15,23,42,.08); margin: 10px 0}

    /* Sections */
    section{padding: 44px 0}
    .section-head{
      display:flex; justify-content:space-between; align-items:flex-end; gap:20px;
      margin-bottom: 18px;
    }
    .section-head h2{
      font-size: 28px; margin:0;
      letter-spacing:-.3px;
    }
    .section-head p{margin:0; color: var(--muted); max-width: 66ch}
    .grid3{display:grid; grid-template-columns: repeat(3, 1fr); gap: 16px}
    @media (max-width: 980px){ .grid3{grid-template-columns:1fr} }
    .service{
      padding: 18px;
      position:relative;
      overflow:hidden;
    }
    .service:before{
      content:"";
      position:absolute; inset:-80px -80px auto auto;
      width:180px; height:180px;
      background: radial-gradient(circle at 30% 30%, rgba(30,58,138,.25), transparent 60%);
      transform: rotate(15deg);
    }
    .badge{
      display:inline-flex; align-items:center;
      font-size:12px;
      font-weight:800;
      color: var(--blue);
      background: rgba(30,58,138,.10);
      border: 1px solid rgba(30,58,138,.20);
      padding: 6px 10px;
      border-radius:999px;
      margin-bottom:10px;
    }
    .service h3{margin: 0 0 6px; font-size: 18px}
    .service p{margin:0; color: var(--muted)}
    .list{
      margin: 12px 0 0; padding: 0 0 0 18px; color: var(--muted)
    }
    .list li{margin: 6px 0}

    /* About */
    .about{
      display:grid; grid-template-columns: 1fr 1fr; gap:16px;
      align-items:stretch;
    }
    @media (max-width: 980px){ .about{grid-template-columns:1fr} }
    .about .card{padding: 18px}
    .kpi{
      display:grid; grid-template-columns: repeat(3, 1fr); gap: 12px; margin-top: 12px
    }
    @media (max-width: 540px){ .kpi{grid-template-columns:1fr} }
    .kpi .mini p{font-size: 16px}
    .kpi .mini small{display:block; margin-top:6px; color: var(--muted); font-weight:650}

    /* Contact */
    .contact{
      display:grid; grid-template-columns: 1.1fr .9fr; gap:16px;
    }
    @media (max-width: 980px){ .contact{grid-template-columns:1fr} }
    form{display:grid; gap:10px}
    label{font-size: 13px; font-weight:800; color: var(--muted)}
    input, textarea{
      width:100%;
      padding: 12px 12px;
      border-radius: 12px;
      border: 1px solid rgba(15,23,42,.14);
      background: rgba(255,255,255,.9);
      font: inherit;
      outline: none;
    }
    input:focus, textarea:focus{border-color: rgba(30,58,138,.45); box-shadow: 0 0 0 6px var(--ring)}
    textarea{min-height: 120px; resize: vertical}
    .btn{
      cursor:pointer;
      border:none;
      border-radius: 999px;
      padding: 12px 14px;
      font-weight:850;
      background: var(--blue);
      color:#fff;
    }
    .btn:hover{background: var(--blue-2)}
    .note{color: var(--muted); font-size: 13px; margin: 6px 0 0}

    footer{
      padding: 26px 0 40px;
      color: var(--muted);
      font-size: 13px;
    }
    .footer-inner{
      display:flex; justify-content:space-between; align-items:center; gap:14px; flex-wrap:wrap;
      border-top: 1px solid rgba(15,23,42,.08);
      padding-top: 18px;
    }
    .tiny-links{display:flex; gap:14px; flex-wrap:wrap}
  </style>
</head>

<body>
  <!-- Nav -->
  <div class="nav">
    <div class="wrap">
      <div class="nav-inner">
        <a class="brand" href="#top" aria-label="HTM Technology Solution Inc. home">
          <span class="logo" aria-hidden="true"></span>
          <span>HTM Technology Solution Inc.</span>
        </a>

        <nav class="nav-links" aria-label="Primary navigation">
          <a href="#services">Services</a>
          <a href="#process">Process</a>
          <a href="#about">About</a>
          <a href="#contact">Contact</a>
        </nav>

        <button class="menu-btn" id="menuBtn" aria-expanded="false" aria-controls="mobileNav">
          Menu
        </button>

        <a class="cta" href="#contact">Request a consult</a>
      </div>

      <div class="mobile" id="mobileNav" aria-label="Mobile navigation">
        <a href="#services">Services</a>
        <a href="#process">Process</a>
        <a href="#about">About</a>
        <a href="#contact">Contact</a>
      </div>
    </div>
  </div>

  <!-- Hero -->
  <header class="hero" id="top">
    <div class="wrap">
      <div class="hero-grid">
        <div>
          <div class="pill"><span class="dot" aria-hidden="true"></span> Greater Washington, DC • Local Technology Consulting</div>
          <h1>Technology consulting that turns ideas into working systems.</h1>
          <p class="lead">
            HTM Technology Solution Inc. helps organizations modernize their digital presence, streamline operations,
            and launch reliable web and marketing infrastructure. Local support across the Greater Washington, DC area.
          </p>

          <div class="hero-actions">
            <a class="cta" href="#contact">Get a quote</a>
            <a class="secondary" href="#services">Explore services</a>
          </div>

          <div class="trust" aria-label="Trust indicators">
            <span>Fast turnaround</span>
            <span>Clear deliverables</span>
            <span>Training + documentation included</span>
          </div>
        </div>

        <aside class="card hero-card" aria-label="Highlights">
          <div class="mini">
            <h3>Primary services</h3>
            <p>Technology Consulting + Digital Delivery</p>
          </div>
          <div class="mini">
            <h3>Local service area</h3>
            <p>Washington, DC • MD • Northern VA</p>
          </div>
          <div class="divider"></div>
          <div class="mini">
            <h3>Typical engagement</h3>
            <p>4 to 6 weeks • defined scope • fixed deliverables</p>
          </div>
        </aside>
      </div>
    </div>
  </header>

  <!-- Services -->
  <section id="services">
    <div class="wrap">
      <div class="section-head">
        <div>
          <h2>Services</h2>
          <p>End-to-end support for web, brand, and marketing foundations — built to be easy to maintain.</p>
        </div>
      </div>

      <div class="grid3">
        <div class="card service">
          <div class="badge">Consulting</div>
          <h3>Technology Strategy</h3>
          <p>Align your goals, tools, and roadmap so execution is fast and measurable.</p>
          <ul class="list">
            <li>Discovery + requirements</li>
            <li>System recommendations</li>
            <li>Implementation plan</li>
          </ul>
        </div>

        <div class="card service">
          <div class="badge">Digital delivery</div>
          <h3>Website Development</h3>
          <p>Modern, responsive websites designed for credibility, speed, and conversions.</p>
          <ul class="list">
            <li>Landing pages + multi-section sites</li>
            <li>SEO basics + performance</li>
            <li>Mobile-first UX</li>
          </ul>
        </div>

        <div class="card service">
          <div class="badge">Marketing foundation</div>
          <h3>Branding + Analytics</h3>
          <p>Visual identity support plus tracking so you know what’s working.</p>
          <ul class="list">
            <li>Brand guidelines (colors, fonts, logo usage)</li>
            <li>Google Analytics + event tracking</li>
            <li>Ads setup support (when needed)</li>
          </ul>
        </div>
      </div>
    </div>
  </section>

  <!-- Process -->
  <section id="process">
    <div class="wrap">
      <div class="section-head">
        <div>
          <h2>How we work</h2>
          <p>A simple process designed for clarity: you’ll always know what’s next, what’s included, and what “done” means.</p>
        </div>
      </div>

      <div class="grid3">
        <div class="card service">
          <div class="badge">Step 1</div>
          <h3>Discovery</h3>
          <p>We define goals, audience, services, and success metrics.</p>
          <ul class="list">
            <li>Stakeholder interview</li>
            <li>Competitive scan</li>
            <li>Site map + messaging</li>
          </ul>
        </div>

        <div class="card service">
          <div class="badge">Step 2</div>
          <h3>Build</h3>
          <p>Design + development with quick feedback cycles.</p>
          <ul class="list">
            <li>Visual direction</li>
            <li>Web build + revisions</li>
            <li>Analytics + forms</li>
          </ul>
        </div>

        <div class="card service">
          <div class="badge">Step 3</div>
          <h3>Launch + Train</h3>
          <p>Go live with documentation so your team can maintain everything confidently.</p>
          <ul class="list">
            <li>Launch checklist</li>
            <li>Admin training</li>
            <li>Hand-off docs</li>
          </ul>
        </div>
      </div>
    </div>
  </section>

  <!-- About -->
  <section id="about">
    <div class="wrap">
      <div class="section-head">
        <div>
          <h2>About HTM</h2>
          <p>We support businesses and organizations with practical, results-driven technology consulting and digital execution.</p>
        </div>
      </div>

      <div class="about">
        <div class="card">
          <h3 style="margin:0 0 8px;">Local, reliable, and outcomes-focused</h3>
          <p style="margin:0; color: var(--muted);">
            HTM Technology Solution Inc. serves clients across the Greater Washington, DC area.
            Whether you need a modern website, a clear digital marketing foundation, or a tech strategy that actually gets implemented,
            we deliver with defined scope and clean documentation.
          </p>

          <div class="kpi">
            <div class="mini">
              <h3>Region</h3>
              <p>Greater DC</p>
              <small>Washington, DC • MD • Northern VA</small>
            </div>
            <div class="mini">
              <h3>Focus</h3>
              <p>Tech consulting</p>
              <small>Strategy + execution</small>
            </div>
            <div class="mini">
              <h3>Delivery</h3>
              <p>Practical builds</p>
              <small>Web + analytics + training</small>
            </div>
          </div>
        </div>

        <div class="card" style="padding:18px;">
          <h3 style="margin:0 0 8px;">Core capabilities</h3>
          <ul class="list" style="margin-top:10px;">
            <li>Website development and performance optimization</li>
            <li>Branding support and visual identity systems</li>
            <li>Social media + platform setup</li>
            <li>Digital marketing strategy + campaign foundations</li>
            <li>Analytics implementation and reporting basics</li>
            <li>Training materials and documentation for handoff</li>
          </ul>
          <p class="note">Want a version of this site with multiple pages (Home / Services / About / Contact)? That’s easy to convert.</p>
        </div>
      </div>
    </div>
  </section>

  <!-- Contact -->
  <section id="contact">
    <div class="wrap">
      <div class="section-head">
        <div>
          <h2>Contact</h2>
          <p>Tell us what you’re building. We’ll respond with next steps and a clear plan.</p>
        </div>
      </div>

      <div class="contact">
        <div class="card" style="padding:18px;">
          <form id="contactForm">
            <div>
              <label for="name">Name</label>
              <input id="name" name="name" autocomplete="name" placeholder="Your name" required />
            </div>
            <div>
              <label for="email">Email</label>
              <input id="email" name="email" type="email" autocomplete="email" placeholder="you@email.com" required />
            </div>
            <div>
              <label for="company">Company (optional)</label>
              <input id="company" name="company" autocomplete="organization" placeholder="Company name" />
            </div>
            <div>
              <label for="message">What do you need help with?</label>
              <textarea id="message" name="message" placeholder="Briefly describe your project, timeline, and goals." required></textarea>
            </div>
            <button class="btn" type="submit">Send message</button>
            <p class="note" id="formNote">
              This demo form opens your email client. To collect submissions automatically, connect Formspree or a Google Form endpoint.
            </p>
          </form>
        </div>

        <div class="card" style="padding:18px;">
          <h3 style="margin:0 0 10px;">Service area</h3>
          <p style="margin:0; color: var(--muted);">
            Greater Washington, DC region (Washington, DC • Maryland • Northern Virginia).
          </p>

          <div class="divider"></div>

          <h3 style="margin:0 0 10px;">Business info</h3>
          <p style="margin:0; color: var(--muted);">
            HTM Technology Solution Inc.<br/>
            Technology Consulting
          </p>

          <div class="divider"></div>

          <h3 style="margin:0 0 10px;">Quick links</h3>
          <p style="margin:0; color: var(--muted);">
            <a href="#services"><strong>Services</strong></a> •
            <a href="#process"><strong>Process</strong></a> •
            <a href="#about"><strong>About</strong></a>
          </p>
        </div>
      </div>
    </div>
  </section>

  <footer>
    <div class="wrap">
      <div class="footer-inner">
        <div>
          <strong>HTM Technology Solution Inc.</strong><br/>
          <span>Technology Consulting • Greater Washington, DC</span>
        </div>
        <div class="tiny-links">
          <a href="#top">Back to top</a>
          <a href="#contact">Contact</a>
        </div>
        <div>© <span id="year"></span> HTM Technology Solution Inc.</div>
      </div>
    </div>
  </footer>

  <script>
    // Mobile menu
    const menuBtn = document.getElementById('menuBtn');
    const mobileNav = document.getElementById('mobileNav');
    if (menuBtn && mobileNav) {
      menuBtn.addEventListener('click', () => {
        const isOpen = mobileNav.classList.toggle('show');
        menuBtn.setAttribute('aria-expanded', String(isOpen));
      });
      mobileNav.querySelectorAll('a').forEach(a => {
        a.addEventListener('click', () => {
          mobileNav.classList.remove('show');
          menuBtn.setAttribute('aria-expanded', 'false');
        });
      });
    }

    // Footer year
    document.getElementById('year').textContent = new Date().getFullYear();

    // Contact form: opens email client with prefilled message
    const form = document.getElementById('contactForm');
    form.addEventListener('submit', (e) => {
      e.preventDefault();

      const name = document.getElementById('name').value.trim();
      const email = document.getElementById('email').value.trim();
      const company = document.getElementById('company').value.trim();
      const message = document.getElementById('message').value.trim();

      // TODO: Replace with your business email:
      const toEmail = "info@htmtechsolutions.com";

      const subject = encodeURIComponent(`Website inquiry from ${name}${company ? " (" + company + ")" : ""}`);
      const body = encodeURIComponent(
        `Name: ${name}\n` +
        `Email: ${email}\n` +
        `Company: ${company || "N/A"}\n\n` +
        `Message:\n${message}\n\n` +
        `Service Area: Greater Washington, DC`
      );

      window.location.href = `mailto:${toEmail}?subject=${subject}&body=${body}`;
    });
  </script>
</body>
</html>
