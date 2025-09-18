<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Campus Turn Up Party — 4th Edition</title>
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <header class="site-header">
    <div class="container header-inner">
      <div class="brand">
        <h1>Campus Turn Up Party</h1>
        <p class="slogan">All Universities, One Party</p>
      </div>
      <nav class="main-nav" id="mainNav">
        <a href="#upcoming">Upcoming</a>
        <a href="#past">Past</a>
        <a href="#tickets">Tickets</a>
        <a href="#contact">Contact</a>
      </nav>
      <button class="hamburger" id="hamburger" aria-label="menu">☰</button>
    </div>
  </header>

  <main>
    <section class="hero">
      <div class="hero-inner container">
        <h2>🔥 4th Edition — February 2026 🔥</h2>
        <p class="lead">Don’t miss a night of music, unity and vibes — The Round Table Lounge</p>
        <div class="cta-row">
          <a class="btn primary" href="#tickets">Book Ticket</a>
          <a class="btn outline" href="#past">Past Highlights</a>
        </div>

        <div class="countdown" id="countdown" aria-live="polite">
          <div><span id="days">--</span><small>Days</small></div>
          <div><span id="hours">--</span><small>Hours</small></div>
          <div><span id="minutes">--</span><small>Minutes</small></div>
          <div><span id="seconds">--</span><small>Seconds</small></div>
        </div>
      </div>
    </section>

    <section id="upcoming" class="section container">
      <h3>Upcoming Event</h3>
      <p class="muted">Edition: <strong>4th Edition</strong> — Date: <strong>February 2026</strong></p>
      <div class="grid-2">
        <div class="card">
          <h4>Event Details</h4>
          <ul>
            <li><strong>Venue:</strong> The Round Table Lounge (Opposite Shell Petrol Station)</li>
            <li><strong>Ticket Price:</strong> 15,000 UGX (includes a free drink)</li>
            <li><strong>Time:</strong> Doors open 7:00 PM</li>
          </ul>
        </div>
        <div class="card">
          <h4>Quick Links</h4>
          <p><a class="link" href="https://wa.me/256700000000" target="_blank" rel="noopener">Join WhatsApp Group</a></p>
          <p><a class="link" href="mailto:info@campusturnup.com">Email Organizers</a></p>
        </div>
      </div>
    </section>

    <section id="tickets" class="section pale">
      <div class="container">
        <h3>Get Tickets</h3>
        <p class="muted">Fill the form and book via WhatsApp or Email.</p>

        <form id="bookingForm" class="ticket-form">
          <input type="text" id="name" placeholder="Your Name" required />
          <input type="email" id="email" placeholder="Your Email" required />
          <input type="tel" id="whatsapp" placeholder="WhatsApp Number (eg. +2567...)" required />
          <select id="qty" required>
            <option value="">Number of Tickets</option>
            <option value="1">1</option>
            <option value="2">2</option>
            <option value="3">3</option>
            <option value="4">4</option>
          </select>

          <div class="form-actions">
            <button class="btn primary" type="submit">Book via WhatsApp</button>
            <button class="btn outline" type="button" id="emailBtn">Send Email</button>
          </div>
        </form>
        <p class="muted small">Tip: replace the placeholder contact number inside the site with your real WhatsApp number.</p>
      </div>
    </section>

    <section id="past" class="section container">
      <h3>Past Editions</h3>
      <p class="muted">Highlights from previous Campus Turn Up Parties</p>

      <div class="cards">
        <article class="past-card">
          <img src="https://images.unsplash.com/photo-1506157786151-b8491531f063?auto=format&fit=crop&w=1000&q=60" alt="Past event 1">
          <div class="card-body">
            <h4>3rd Edition</h4>
            <p>Music, battles and unforgettable energy — campus legends performed.</p>
          </div>
        </article>

        <article class="past-card">
          <img src="https://images.unsplash.com/photo-1515165562835-cb0d4b3a6f3e?auto=format&fit=crop&w=1000&q=60" alt="Past event 2">
          <div class="card-body">
            <h4>2nd Edition</h4>
            <p>Student competitions, dance-offs and great food stalls.</p>
          </div>
        </article>

        <article class="past-card">
          <img src="https://images.unsplash.com/photo-1531058020387-3be344556be6?auto=format&fit=crop&w=1000&q=60" alt="Past event 3">
          <div class="card-body">
            <h4>1st Edition</h4>
            <p>The launch that started it all — unity, music and massive turnout.</p>
          </div>
        </article>
      </div>
    </section>

    <section id="contact" class="section dark">
      <div class="container">
        <h3>Contact</h3>
        <p>Email: <a href="mailto:info@campusturnup.com" class="link">info@campusturnup.com</a></p>
        <p>WhatsApp: <a class="link" href="https://wa.me/256700000000" target="_blank" rel="noopener">+256 700 000000</a></p>
        <div class="socials">
          <a class="link" href="#" target="_blank" rel="noopener">Telegram</a> •
          <a class="link" href="#" target="_blank" rel="noopener">TikTok</a> •
          <a class="link" href="#" target="_blank" rel="noopener">Instagram</a>
        </div>
      </div>
    </section>
  </main>

  <footer class="site-footer">
    <div class="container">
      <p>© <span id="year"></span> Campus Turn Up Party — All Universities, One Party</p>
    </div>
  </footer>

  <script src="script.js"></script>
</body>
</html>
:root{
  --bg:#0f0f10; --card:#151516; --accent:#f1c40f; --muted:#bdbdbd; --text:#ffffff;
  --container:1100px;
}
*{box-sizing:border-box}
html,body{height:100%}
body{
  margin:0; font-family:Inter, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
  background:var(--bg); color:var(--text); -webkit-font-smoothing:antialiased;
}
.container{max-width:var(--container); margin:0 auto; padding:0 18px}
.site-header{background:#000; border-bottom:1px solid rgba(255,255,255,0.03)}
.header-inner{display:flex; align-items:center; justify-content:space-between; padding:14px 0}
.brand h1{margin:0; font-size:1.1rem; color:var(--accent)}
.brand .slogan{margin:2px 0 0; font-size:0.8rem; color:var(--muted)}
.main-nav a{color:var(--text); text-decoration:none; margin-left:18px; font-weight:600}
.hamburger{display:none; background:transparent; color:var(--text); border:0; font-size:22px}

/* Hero */
.hero{background-image:linear-gradient(180deg, rgba(0,0,0,0.35), rgba(0,0,0,0.6)), url('https://images.unsplash.com/photo-1506157786151-b8491531f063?auto=format&fit=crop&w=1600&q=60'); background-size:cover; background-position:center; padding:70px 0; text-align:center}
.hero-inner h2{font-size:2.2rem; margin:0 0 8px}
.lead{color:var(--muted); margin-bottom:18px}
.btn{display:inline-block; padding:12px 18px; border-radius:8px; text-decoration:none; font-weight:700}
.btn.primary{background:var(--accent); color:#000}
.btn.outline{background:transparent; border:2px solid rgba(255,255,255,0.06); color:var(--text)}

/* Countdown */
.countdown{display:flex; justify-content:center; gap:22px; margin-top:20px}
.countdown div{background:rgba(255,255,255,0.06); padding:10px 16px; border-radius:8px; min-width:70px}
.countdown span{display:block; font-size:1.2rem; font-weight:700; text-align:center}
.countdown small{display:block; text-align:center; color:var(--muted)}

/* Sections */
.section{padding:38px 0}
.section.pale{background:#0b0b0b}
.section .muted{color:var(--muted)}

/* Cards & grid */
.grid-2{display:grid; grid-template-columns:1fr 1fr; gap:18px; margin-top:14px}
.card{background:var(--card); padding:18px; border-radius:10px; text-align:left}
.cards{display:grid; grid-template-columns:repeat(3,1fr); gap:18px; margin-top:14px}
.past-card{background:#111; border-radius:10px; overflow:hidden; box-shadow:0 6px 18px rgba(0,0,0,0.6)}
.past-card img{width:100%; height:160px; object-fit:cover; display:block}
.card-body{padding:12px}

/* Ticket form */
.ticket-form{max-width:480px; margin:12px auto 0; display:flex; flex-direction:column; gap:12px}
.ticket-form input, .ticket-form select{padding:12px; border-radius:8px; border:0}
.form-actions{display:flex; gap:12px; margin-top:6px}
.small{font-size:0.85rem; color:var(--muted)}

/* Footer */
.site-footer{border-top:1px solid rgba(255,255,255,0.03); padding:18px 0; text-align:center; color:var(--muted)}

/* Responsive */
@media(max-width:900px){
  .cards{grid-template-columns:1fr}
  .grid-2{grid-template-columns:1fr}
}
@media(max-width:700px){
  .main-nav{display:none}
  .hamburger{display:inline-block}
  .hero-inner h2{font-size:1.6rem}
  .countdown{gap:10px}
}

