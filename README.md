<!doctype html>

<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>SmartNewsk — Latest News & Analysis</title>
  <meta name="description" content="SmartNewsk: local & global news, trending stories, opinion and analysis." />
  <meta name="theme-color" content="#0f172a" />  <!--
    SmartNewsk - Single-file starter site (index.html)
    -------------------------------------------------
    How to use:
      1) Save this file as `index.html` and upload to a static host (GitHub Pages, Netlify, Vercel, Surge)
      2) Replace sample articles with your own content under <main id="articles">.
      3) To monetize with AdSense: sign up for Google AdSense and paste the AdSense <script> into the
         <head> as instructed by Google. Replace the placeholder <ins class="adsbygoogle"> element below
         with the ad unit code Google gives you.
      4) Customize branding (logo, colors) by editing the CSS variables below.

    Files you may want to add alongside this one:
      - /assets/logo.png (site logo)
      - /assets/hero.jpg (hero image)
      - /css/custom.css (if you split styles)
      - /rss.xml (for feeds)
  -->  <style>
    :root{
      --bg:#0b1220; --card:#0f172a; --muted:#94a3b8; --accent:#06b6d4; --glass: rgba(255,255,255,0.03);
      --maxw:1100px;
      font-family: Inter, system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial;
    }
    *{box-sizing:border-box}
    body{margin:0;background:linear-gradient(180deg,var(--bg),#071021);color:#e6eef6;line-height:1.45}
    header{background:linear-gradient(90deg,rgba(6,182,212,0.06),transparent);backdrop-filter:blur(4px);border-bottom:1px solid rgba(255,255,255,0.03)}
    .wrap{max-width:var(--maxw);margin:0 auto;padding:20px}
    .brand{display:flex;gap:14px;align-items:center}
    .logo{width:44px;height:44px;border-radius:8px;background:linear-gradient(135deg,var(--accent),#7c3aed);display:flex;align-items:center;justify-content:center;font-weight:700}
    .site-title{font-size:20px;margin:0}
    .site-sub{color:var(--muted);font-size:13px;margin-top:2px}

    nav{display:flex;gap:12px;align-items:center;margin-left:auto}
    .nav a{color:var(--muted);text-decoration:none;font-size:14px;padding:6px 8px;border-radius:6px}
    .nav a:hover{color:#fff;background:rgba(255,255,255,0.02)}

    .hero{display:grid;grid-template-columns:1fr 320px;gap:18px;margin-top:20px}
    .hero-card{background:var(--card);padding:18px;border-radius:12px;box-shadow:0 6px 18px rgba(2,6,23,0.6)}
    .hero h1{margin:0;font-size:28px}
    .meta{color:var(--muted);font-size:13px;margin-top:8px}
    .search{margin-top:12px}
    .search input{width:100%;padding:10px;border-radius:10px;border:1px solid rgba(255,255,255,0.03);background:var(--glass);color:inherit}

    main{display:grid;grid-template-columns:1fr 320px;gap:18px;margin-top:18px}
    .article{background:var(--card);padding:16px;border-radius:12px;border:1px solid rgba(255,255,255,0.02)}
    .article h2{margin:0 0 8px 0;font-size:18px}
    .article p{color:var(--muted);margin:0 0 12px 0}
    .read-more{display:inline-block;padding:8px 12px;border-radius:8px;background:rgba(255,255,255,0.02);text-decoration:none;color:#fff;font-size:13px}

    .sidebar .card{background:var(--card);padding:12px;border-radius:10px;margin-bottom:12px}
    .tag{display:inline-block;background:rgba(255,255,255,0.03);padding:6px 10px;border-radius:999px;font-size:13px;margin-right:6px;color:var(--muted)}

    footer{padding:24px 0;color:var(--muted);font-size:13px;margin-top:32px}

    @media (max-width:900px){
      .hero, main{grid-template-columns:1fr;}
      .hero{grid-template-columns:1fr}
    }
  </style>  <!-- Structured data for a news site (sample) -->  <script type="application/ld+json">
  {
    "@context":"https://schema.org",
    "@type":"NewsMediaOrganization",
    "name":"SmartNewsk",
    "url":"https://your-site.example",
    "logo":{
      "@type":"ImageObject",
      "url":"https://your-site.example/assets/logo.png"
    }
  }
  </script></head>
<body>
  <header>
    <div class="wrap" style="display:flex;align-items:center">
      <div class="brand">
        <div class="logo">SN</div>
        <div>
          <h1 class="site-title">SmartNewsk</h1>
          <div class="site-sub">Local & Global — Breaking news, analysis & opinion</div>
        </div>
      </div><nav class="nav" aria-label="Main navigation">
    <a href="#">Home</a>
    <a href="#world">World</a>
    <a href="#local">Local</a>
    <a href="#business">Business</a>
    <a href="#opinion">Opinion</a>
    <a href="#about">About</a>
  </nav>
</div>

  </header>  <div class="wrap">
    <section class="hero">
      <div class="hero-card">
        <h1>Kenya reacts as major court ruling shocks citizens</h1>
        <div class="meta">By SmartNewsk Reporter • Sep 18, 2025</div>
        <p style="margin-top:12px;color:var(--muted)">Quick summary of the top story with a short lead paragraph. Replace with your real story text. Keep intros short and punchy for mobile readers.</p>
        <div style="margin-top:12px"><a class="read-more" href="#">Read full story</a></div>
      </div><aside class="hero-card" style="display:flex;flex-direction:column;gap:10px">
    <div>
      <strong>Trending</strong>
      <div style="margin-top:8px;color:var(--muted)">Irene Jerotich case • Election analysis • Tech layoffs</div>
    </div>

    <div>
      <strong>Search</strong>
      <div class="search"><input placeholder="Search SmartNewsk" aria-label="Search"/></div>
    </div>

    <div>
      <strong>Newsletter</strong>
      <p style="color:var(--muted);margin:6px 0 8px 0">Get the top stories in your inbox.</p>
      <form onsubmit="event.preventDefault();alert('Thanks! Paste real signup code to connect to your email provider.')">
        <input placeholder="your@email.com" style="width:100%;padding:10px;border-radius:8px;border:1px solid rgba(255,255,255,0.03);background:var(--glass)" />
        <div style="margin-top:8px"><button style="width:100%;padding:10px;border-radius:8px;background:linear-gradient(90deg,var(--accent),#7c3aed);border:none;color:#021024">Subscribe</button></div>
      </form>
    </div>
  </aside>
</section>

<main>
  <div id="articles">
    <!-- Sample article cards - replace these with your real posts -->
    <article class="article">
      <h2>Local leaders demand faster response after flooding</h2>
      <div class="meta">By Staff • Sep 17, 2025</div>
      <p>Heavy rains caused flooding across several counties. Residents say the response from authorities has been slow.</p>
      <a class="read-more" href="#">Read more</a>
    </article>

    <article class="article" style="margin-top:12px">
      <h2>Business: Startups raise $10M in Series A round</h2>
      <div class="meta">By Business Desk • Sep 16, 2025</div>
      <p>A local fintech startup closed a Series A round as investors show renewed interest in African tech.</p>
      <a class="read-more" href="#">Read more</a>
    </article>

    <article class="article" style="margin-top:12px">
      <h2>Opinion: What our election results mean for the economy</h2>
      <div class="meta">By Opinion • Sep 15, 2025</div>
      <p>Analysis of the incoming economic policies and what they could mean for small businesses.</p>
      <a class="read-more" href="#">Read more</a>
    </article>

    <!-- Pagination (static placeholder) -->
    <div style="margin-top:16px;display:flex;gap:8px">
      <button disabled style="padding:8px 12px;border-radius:8px;background:rgba(255,255,255,0.02);border:none;color:var(--muted)">Previous</button>
      <button style="padding:8px 12px;border-radius:8px;background:linear-gradient(90deg,var(--accent),#7c3aed);border:none;color:#021024">Next</button>
    </div>

  </div>

  <aside class="sidebar">
    <div class="card">
      <h3>Top tags</h3>
      <div style="margin-top:8px">
        <span class="tag">Politics</span>
        <span class="tag">Business</span>
        <span class="tag">Crime</span>
        <span class="tag">Sports</span>
      </div>
    </div>

    <div class="card">
      <h3>Advertisement</h3>
      <p style="color:var(--muted);font-size:13px">Replace this block with your AdSense ad unit. Example placeholder below.</p>

      <!-- AdSense placeholder: replace with the exact code Google gives you -->
      <div style="background:rgba(255,255,255,0.02);padding:12px;border-radius:10px;text-align:center;color:var(--muted)">
        AD SPACE (paste AdSense code here)
      </div>

    </div>

    <div class="card">
      <h3>About SmartNewsk</h3>
      <p style="color:var(--muted);font-size:13px">SmartNewsk is an independent news site focused on fast, fair reporting. Contact: editor@smartnewsk.example</p>
    </div>
  </aside>
</main>

<footer>
  <div style="max-width:var(--maxw);margin:0 auto;display:flex;justify-content:space-between;align-items:center">
    <div>
      <strong>SmartNewsk</strong>
      <div style="color:var(--muted);margin-top:6px">© SmartNewsk 2025 • All rights reserved</div>
    </div>
    <div style="color:var(--muted);font-size:13px">Terms • Privacy • Contact</div>
  </div>
</footer>

  </div>  <script>
    // Small client-side helpers (search stub, dynamic time)
    document.querySelectorAll('.read-more').forEach(btn=>btn.addEventListener('click',e=>{e.preventDefault();alert('This is a demo. Replace links with real article pages.') }))

    // Example: detect mobile and show small UA info (optional)
    if(/Mobi|Android/i.test(navigator.userAgent)){
      console.log('Mobile visitor');
    }
  </script></body>
</html>
