# judemotors<!--
  File: index.html
  For: Jude Anthony Motors ("Reliable cars")

  Instructions:
  1) To enable contact form submissions without a backend — sign up at https://formspree.io (free tier available), create a form, then replace FORM_ID below (FORM_ID -> your real form id) in the form's action attribute.
     Example: <form action="https://formspree.io/f/mnqwerty" method="POST">

  2) To deploy for free: create a GitHub repository, add this file as index.html in the repo root, then enable GitHub Pages in repository settings and choose main branch / root. Your site will be live at https://<your-username>.github.io/<repo-name>/ or at the repo root if you choose user pages.

  3) Quick edits: replace the placeholder phone, email, location, and inventory items with your real info. Replace the hero/car image with your own photo.

  4) If you want me to deploy it for you (I can provide step-by-step commands), tell me your preference and I will give exact commands.
-->

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width,initial-scale=1">
  <title>Jude Anthony Motors — Reliable cars</title>
  <meta name="description" content="Jude Anthony Motors — Reliable cars. Used car sales, repairs, spare parts and vehicle servicing." />
  <style>
    :root{ --bg:#0f1720; --card:#0b1220; --muted:#aeb7c1; --accent:#d32f2f; --glass: rgba(255,255,255,0.03); --radius:12px; font-family: Inter, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial; }
    *{box-sizing:border-box}
    body{ margin:0; background: linear-gradient(180deg,#071018 0%, #0f1720 100%); color:#e6eef6; -webkit-font-smoothing:antialiased; -moz-osx-font-smoothing:grayscale; line-height:1.5; }
    header{ display:flex; align-items:center; justify-content:space-between; padding:1rem 1.5rem; backdrop-filter: blur(6px); background: linear-gradient(90deg, rgba(255,255,255,0.02), rgba(255,255,255,0.00)); border-bottom:1px solid rgba(255,255,255,0.03); position:sticky; top:0; z-index:40; }
    .brand{ display:flex; gap:.9rem; align-items:center; }
    .logo{ width:48px;height:48px;border-radius:10px;background:var(--accent); display:flex;align-items:center;justify-content:center;font-weight:700; color:#fff;font-size:18px;box-shadow:0 6px 18px rgba(211,47,47,0.15); }
    nav a{ color:var(--muted); text-decoration:none; margin-left:1rem; font-weight:600; }
    nav a:hover{ color:#fff }
    .container{ max-width:1100px; margin:2rem auto; padding:0 1rem }
    .hero{ display:grid; grid-template-columns: 1fr 420px; gap:1.5rem; align-items:center; margin-top:1rem; }
    .hero-card{ background: linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01)); padding:2.2rem; border-radius:var(--radius); box-shadow: 0 8px 30px rgba(2,6,23,0.6); }
    .kicker{ color:var(--muted); font-weight:700; letter-spacing:.06em; font-size:.85rem }
    h1{ margin:.35rem 0 0; font-size:2rem }
    p.lead{ color:var(--muted); margin:1rem 0 1.4rem }
    .cta-row{ display:flex; gap:.8rem; align-items:center }
    .btn{ padding:.85rem 1.05rem; border-radius:10px; border:0; font-weight:700; cursor:pointer; background:var(--accent); color:#fff; box-shadow:0 10px 30px rgba(211,47,47,0.18) }
    .btn.ghost{ background:transparent; border:1px solid rgba(255,255,255,0.06); color:var(--muted) }
    .stats{ display:flex; gap:1rem; margin-top:1.3rem }
    .stat{ background:var(--glass); padding:.8rem; border-radius:10px; flex:1; text-align:center }
    .stat strong{ display:block; font-size:1.25rem }
    .car-card{ border-radius:var(--radius); overflow:hidden; height:100%; background: linear-gradient(180deg,#081018,#0b1520); display:flex; flex-direction:column; align-items:center; justify-content:center; padding:1rem; position:relative }
    .car-card img{ max-width:100%; border-radius:8px; display:block }
    section{ margin-top:2.2rem }
    .cards{ display:grid; grid-template-columns:repeat(auto-fit,minmax(220px,1fr)); gap:1rem }
    .card{ background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01)); padding:1.2rem; border-radius:12px; border:1px solid rgba(255,255,255,0.03) }
    .card h3{ margin:0 0 .5rem }
    .contact-grid{ display:grid; grid-template-columns:1fr 320px; gap:1rem; align-items:start }
    .contact-card{ padding:1rem; border-radius:12px; background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01)); border:1px solid rgba(255,255,255,0.03) }
    form input, form textarea{ width:100%; padding:.7rem; border-radius:8px; border:1px solid rgba(255,255,255,0.06); background:transparent; color:inherit; margin:8px 0 }
    form button{ width:100%; padding:.8rem; border-radius:10px; border:0; background:var(--accent); color:#fff; font-weight:700; margin-top:.5rem }
    footer{ margin-top:2.5rem; padding:1.2rem 0; color:var(--muted); text-align:center; border-top:1px solid rgba(255,255,255,0.02) }
    @media (max-width:900px){ .hero{ grid-template-columns:1fr; text-align:center } .contact-grid{ grid-template-columns:1fr } .car-card{ order:-1 } header{ padding:.75rem 1rem } }
  </style>
</head>
<body>
  <header>
    <div class="brand">
      <div class="logo">JAM</div>
      <div>
        <div style="font-weight:800">Jude Anthony Motors</div>
        <div style="font-size:.8rem;color:var(--muted);margin-top:2px">Reliable cars</div>
      </div>
    </div>
    <nav>
      <a href="#about">About</a>
      <a href="#services">Services</a>
      <a href="#inventory">Inventory</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <main class="container">
    <div class="hero">
      <div class="hero-card">
        <div class="kicker">Trusted since 2023</div>
        <h1>Jude Anthony Motors — Reliable cars</h1>
        <p class="lead">Quality used vehicles, honest servicing, and affordable parts. We make buying and maintaining your car straightforward — no nonsense, no surprises.</p>

        <div class="cta-row">
          <button class="btn" onclick="window.location='#inventory'">Browse Inventory</button>
          <button class="btn ghost" onclick="document.getElementById('contact-form').scrollIntoView({behavior:'smooth'})">Book a Service</button>
        </div>

        <div class="stats" aria-hidden="true">
          <div class="stat"><strong>150+</strong> Vehicles sold</div>
          <div class="stat"><strong>5 yrs</strong> Average experience</div>
          <div class="stat"><strong>30+</strong> Serviced weekly</div>
        </div>
      </div>

      <div class="car-card" aria-hidden="true">
        <!-- replace image src with your photo -->
        <img src="https://images.unsplash.com/photo-1542367597-08a9b6a6b0d9?auto=format&fit=crop&w=1200&q=60" alt="Featured car" />
      </div>
    </div>

    <!-- ABOUT -->
    <section id="about">
      <div class="card">
        <h2>About Jude Anthony Motors</h2>
        <p style="color:var(--muted)">Jude Anthony Motors sells reliable pre-owned cars and provides mechanical servicing and spare parts. We focus on transparency — full vehicle history, visible inspections, and fair pricing. Our goal: keep you on the road without headaches.</p>
      </div>
    </section>

    <!-- SERVICES / inventory -->
    <section id="services">
      <h2>What we do</h2>
      <div class="cards" style="margin-top:1rem">
        <div class="card">
          <h3>Used Car Sales</h3>
          <p>Curated selection of inspected, roadworthy vehicles. Financing options available on approved applications.</p>
        </div>
        <div class="card">
          <h3>Servicing & Repairs</h3>
          <p>Routine maintenance, diagnostics, and mechanical repairs done by experienced technicians — honest estimates before we start work.</p>
        </div>
        <div class="card">
          <h3>Spare Parts</h3>
          <p>Common parts and consumables in stock. We can order harder-to-find parts quickly for most popular brands.</p>
        </div>
        <div class="card">
          <h3>Trade-ins & Valuations</h3>
          <p>Fair trade-in offers after inspection. We buy good-condition vehicles outright as well.</p>
        </div>
      </div>
    </section>

    <section id="inventory">
      <h2>Featured Inventory</h2>
      <div class="cards" style="margin-top:1rem">
        <div class="card"><h3>Toyota Corolla — 2016</h3><p>130,000 km, full service history, clean interior. Price: negotiable.</p></div>
        <div class="card"><h3>Nissan X-Trail — 2015</h3><p>Alloy wheels, recent brakes, good family SUV. Price: negotiable.</p></div>
        <div class="card"><h3>Honda Fit — 2017</h3><p>Fuel-efficient, city car, low mileage. Price: negotiable.</p></div>
      </div>
    </section>

    <!-- CONTACT -->
    <section id="contact" style="margin-bottom:2rem">
      <h2>Contact & Bookings</h2>
      <div class="contact-grid" style="margin-top:1rem">
        <div class="contact-card">
          <!-- Replace FORM_ID with your Formspree form id to receive real submissions -->
          <form id="contact-form" action="https://formspree.io/f/FORM_ID" method="POST">
            <label style="font-weight:700">Name</label>
            <input name="name" id="name" placeholder="Your name" required />
            <label style="font-weight:700">Email</label>
            <input name="email" id="email" type="email" placeholder="you@example.com" required />
            <label style="font-weight:700">Message</label>
            <textarea name="message" id="message" rows="5" placeholder="Tell us about the car or service you need" required></textarea>
            <button type="submit">Send message</button>
            <p style="font-size:.85rem;color:var(--muted);margin-top:.5rem">Tip: if you don't set up Formspree the form will still submit but will return an error. For a quick fallback the form also opens your email client (see script below).</p>
          </form>
          <div style="margin-top:.6rem">
            <button class="btn ghost" id="email-fallback">Open email client (fallback)</button>
          </div>
        </div>

        <aside class="contact-card">
          <h3>Contact Info</h3>
          <p style="color:var(--muted)">Replace these placeholders with your real contact details.</p>
          <p><strong>Phone:</strong> +256 7XX XXX XXX</p>
          <p><strong>Email:</strong> info@judeanthonymotors.com</p>
          <p><strong>Location:</strong> Mbale, Uganda</p>
          <div style="margin-top:1rem">
            <a href="#inventory" class="btn">View Inventory</a>
          </div>
        </aside>
      </div>
    </section>

    <footer>
      <div style="max-width:900px;margin:0 auto">
        <div style="display:flex;justify-content:space-between;align-items:center;gap:1rem;flex-wrap:wrap">
          <div style="font-weight:700">Jude Anthony Motors</div>
          <div style="color:var(--muted)">© <span id="year"></span> Jude Anthony Motors. All rights reserved.</div>
        </div>
      </div>
    </footer>
  </main>

  <script>
    document.getElementById('year').textContent = new Date().getFullYear();

    // fallback: open user's email client if Formspree isn't configured
    document.getElementById('email-fallback').addEventListener('click', function(){
      const name = document.getElementById('name').value.trim();
      const email = document.getElementById('email').value.trim();
      const message = document.getElementById('message').value.trim();
      const subject = encodeURIComponent('Contact from website: ' + (name || 'Visitor'));
      const body = encodeURIComponent('From: ' + (name || 'Visitor') + ' (' + (email || 'no-email') + ')%0D%0A%0D%0A' + (message || '(no message)'));
      window.location.href = 'mailto:info@judeanthonymotors.com?subject=' + subject + '&body=' + body;
    });

    // Optional: intercept Formspree errors and fallback to mailto automatically
    (function(){
      const form = document.getElementById('contact-form');
      form.addEventListener('submit', function(e){
        // Let form submit to Formspree normally. After submit the browser navigates.
        // If you want AJAX submission and nicer UX, tell me and I will add it.
      });
    })();
  </script>
</body>
</html>
