<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>For Anamika Islam Mim</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@400;500;600;700&family=Inter:wght@300;400;500;600&display=swap" rel="stylesheet">
  <style>
    :root {
      --bg-1: #fff8fb;
      --bg-2: #fdf3f7;
      --card: rgba(255,255,255,0.45);
      --text: #4b2e39;
      --muted: #7a5b66;
      --gold: #d4af7f;
      --rose: #d98ea3;
      --deep-rose: #b96b83;
      --shadow: 0 20px 50px rgba(180, 104, 132, 0.18);
      --border: rgba(255,255,255,0.55);
    }

    * { box-sizing: border-box; margin: 0; padding: 0; }

    html { scroll-behavior: smooth; }

    body {
      font-family: 'Inter', sans-serif;
      color: var(--text);
      background:
        radial-gradient(circle at 10% 20%, rgba(255, 214, 230, 0.75), transparent 28%),
        radial-gradient(circle at 85% 15%, rgba(255, 238, 214, 0.8), transparent 25%),
        radial-gradient(circle at 50% 80%, rgba(255, 220, 234, 0.6), transparent 30%),
        linear-gradient(180deg, var(--bg-1), var(--bg-2));
      min-height: 100vh;
      overflow-x: hidden;
    }

    .particles {
      position: fixed;
      inset: 0;
      pointer-events: none;
      z-index: 0;
      overflow: hidden;
    }

    .particle {
      position: absolute;
      bottom: -30px;
      font-size: 14px;
      opacity: 0.22;
      animation: floatUp linear infinite;
      color: var(--rose);
      filter: blur(0.2px);
    }

    @keyframes floatUp {
      from { transform: translateY(0) translateX(0) rotate(0deg); opacity: 0; }
      10% { opacity: 0.25; }
      90% { opacity: 0.18; }
      to { transform: translateY(-110vh) translateX(20px) rotate(180deg); opacity: 0; }
    }

    .container {
      width: min(1120px, 92%);
      margin: 0 auto;
      position: relative;
      z-index: 1;
    }

    nav {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 24px 0;
    }

    .logo {
      font-family: 'Cormorant Garamond', serif;
      font-size: 1.5rem;
      font-weight: 700;
      letter-spacing: 0.5px;
    }

    .nav-links {
      display: flex;
      gap: 18px;
      flex-wrap: wrap;
    }

    .nav-links a {
      text-decoration: none;
      color: var(--muted);
      font-size: 0.95rem;
      transition: 0.3s ease;
    }

    .nav-links a:hover { color: var(--deep-rose); }

    .hero {
      min-height: 88vh;
      display: grid;
      place-items: center;
      text-align: center;
      padding: 30px 0 70px;
    }

    .hero-box {
      background: var(--card);
      border: 1px solid var(--border);
      backdrop-filter: blur(18px);
      -webkit-backdrop-filter: blur(18px);
      border-radius: 28px;
      box-shadow: var(--shadow);
      padding: 54px 28px;
      width: min(900px, 100%);
      position: relative;
      overflow: hidden;
    }

    .hero-box::before {
      content: "";
      position: absolute;
      inset: 0;
      background: linear-gradient(135deg, rgba(255,255,255,0.35), transparent 40%, rgba(255, 228, 236, 0.35));
      pointer-events: none;
    }

    .eyebrow {
      letter-spacing: 3px;
      text-transform: uppercase;
      font-size: 0.82rem;
      color: var(--deep-rose);
      margin-bottom: 14px;
    }

    h1, h2, h3 {
      font-family: 'Cormorant Garamond', serif;
      line-height: 1.1;
    }

    h1 {
      font-size: clamp(3rem, 8vw, 5.6rem);
      margin-bottom: 18px;
      font-weight: 700;
    }

    .hero p {
      max-width: 700px;
      margin: 0 auto;
      color: var(--muted);
      font-size: 1.08rem;
      line-height: 1.9;
    }

    .hero-buttons {
      display: flex;
      justify-content: center;
      gap: 14px;
      flex-wrap: wrap;
      margin-top: 30px;
    }

    .btn {
      border: none;
      text-decoration: none;
      padding: 14px 24px;
      border-radius: 999px;
      font-weight: 600;
      cursor: pointer;
      transition: transform 0.25s ease, box-shadow 0.25s ease, background 0.25s ease;
      box-shadow: 0 10px 25px rgba(185, 107, 131, 0.18);
    }

    .btn-primary {
      background: linear-gradient(135deg, var(--deep-rose), var(--rose));
      color: white;
    }

    .btn-secondary {
      background: rgba(255,255,255,0.6);
      color: var(--text);
      border: 1px solid rgba(255,255,255,0.7);
    }

    .btn:hover {
      transform: translateY(-2px);
      box-shadow: 0 16px 30px rgba(185, 107, 131, 0.22);
    }

    section {
      padding: 80px 0;
    }

    .section-title {
      text-align: center;
      margin-bottom: 18px;
      font-size: clamp(2.2rem, 4vw, 3.4rem);
    }

    .section-sub {
      text-align: center;
      max-width: 760px;
      margin: 0 auto 40px;
      color: var(--muted);
      line-height: 1.8;
    }

    .glass {
      background: var(--card);
      border: 1px solid var(--border);
      backdrop-filter: blur(18px);
      -webkit-backdrop-filter: blur(18px);
      box-shadow: var(--shadow);
      border-radius: 24px;
    }

    .love-letter {
      padding: 38px 28px;
      line-height: 2;
      font-size: 1.02rem;
      color: var(--text);
    }

    .love-letter p + p { margin-top: 16px; }

    .signature {
      margin-top: 24px;
      font-family: 'Cormorant Garamond', serif;
      font-size: 1.6rem;
      color: var(--deep-rose);
    }

    .grid {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 22px;
    }

    .card {
      padding: 28px 22px;
      transition: transform 0.3s ease, box-shadow 0.3s ease;
      position: relative;
      overflow: hidden;
    }

    .card::after {
      content: "";
      position: absolute;
      inset: auto -20% -50% auto;
      width: 120px;
      height: 120px;
      background: radial-gradient(circle, rgba(255,255,255,0.35), transparent 70%);
      pointer-events: none;
    }

    .card:hover {
      transform: translateY(-6px);
      box-shadow: 0 24px 50px rgba(185, 107, 131, 0.2);
    }

    .card h3 {
      font-size: 1.7rem;
      margin-bottom: 10px;
    }

    .card p {
      color: var(--muted);
      line-height: 1.8;
      font-size: 0.96rem;
    }

    .gallery {
      display: grid;
      grid-template-columns: repeat(3, 1fr);
      gap: 22px;
    }

    .memory {
      min-height: 240px;
      border-radius: 24px;
      padding: 22px;
      display: flex;
      align-items: end;
      position: relative;
      overflow: hidden;
      background:
        linear-gradient(180deg, rgba(255,255,255,0.15), rgba(110, 58, 78, 0.25)),
        linear-gradient(135deg, rgba(255, 228, 236, 0.7), rgba(255,255,255,0.35));
      border: 1px solid rgba(255,255,255,0.6);
      box-shadow: var(--shadow);
    }

    .memory::before {
      content: "Photo / Memory";
      position: absolute;
      inset: 18px auto auto 18px;
      font-size: 0.78rem;
      letter-spacing: 2px;
      text-transform: uppercase;
      color: rgba(75, 46, 57, 0.62);
    }

    .memory span {
      background: rgba(255,255,255,0.55);
      backdrop-filter: blur(10px);
      padding: 10px 14px;
      border-radius: 999px;
      color: var(--text);
      font-size: 0.95rem;
    }

    blockquote {
      padding: 34px 26px;
      text-align: center;
      font-family: 'Cormorant Garamond', serif;
      font-size: clamp(1.9rem, 3vw, 2.7rem);
      line-height: 1.5;
    }

    blockquote footer {
      display: block;
      margin-top: 18px;
      font-family: 'Inter', sans-serif;
      font-size: 0.98rem;
      color: var(--muted);
    }

    .final {
      text-align: center;
      padding: 46px 28px;
    }

    .final p {
      max-width: 760px;
      margin: 0 auto;
      line-height: 2;
      color: var(--muted);
    }

    .final strong {
      color: var(--deep-rose);
    }

    .footer {
      text-align: center;
      padding: 28px 0 40px;
      color: var(--muted);
      font-size: 0.92rem;
    }

    .music-note {
      margin-top: 18px;
      color: var(--deep-rose);
      font-size: 0.95rem;
    }

    audio { display: none; }

    @media (max-width: 900px) {
      .grid, .gallery { grid-template-columns: 1fr 1fr; }
      .nav-links { justify-content: center; }
      nav { flex-direction: column; gap: 16px; }
    }

    @media (max-width: 640px) {
      .grid, .gallery { grid-template-columns: 1fr; }
      .hero-box { padding: 42px 18px; border-radius: 22px; }
      .hero p { font-size: 1rem; }
      section { padding: 64px 0; }
      .love-letter, .final, blockquote { padding-left: 18px; padding-right: 18px; }
    }
  </style>
</head>
<body>
  <div class="particles" id="particles"></div>

  <div class="container">
    <nav>
      <div class="logo">For My BABUUUUU ♡</div>
      <div class="nav-links">
        <a href="#letter">Letter</a>
        <a href="#special">Why You</a>
        <a href="#memories">Memories</a>
        <a href="#promise">Promise</a>
      </div>
    </nav>

    <header class="hero">
      <div class="hero-box glass">
        <div class="eyebrow">A Special Surprise</div>
        <h1>Anamika Islam Mim(MY BACCA)</h1>
        <p>
          A rare soul, a soft heart, and one of the most beautiful blessings in my life.
          This little website is only for you — to remind you how deeply you are loved,
          admired, and cherished.
        </p>
        <div class="hero-buttons">
          <a class="btn btn-primary" href="#letter">Open My Heart</a>
          <button class="btn btn-secondary" id="musicBtn">Play Music</button>
        </div>
        <div class="music-note">You deserve something soft, beautiful, and unforgettable.</div>
      </div>
    </header>

    <section id="letter">
      <h2 class="section-title">A Letter From My Heart</h2>
      <p class="section-sub">
        Some feelings are too deep for ordinary words. But even then, I still wanted to try — because you deserve to know how special you are.
      </p>
      <div class="glass love-letter">
        <p>
          My dear Bou,,,my bacca, from the moment you became such an important part of my life, everything started to feel softer, warmer, and more meaningful. There is something so special about you that words can never fully explain. Your presence brings a kind of peace that is rare, and your smile has a way of making even ordinary moments feel beautiful.
        </p>
        <p>
          I admire your heart, your kindness, your beauty, and the warmth you carry within you. You are not only precious to me because of how lovely you are, but because of how deeply you touch my life with your care, your grace, and your existence. You make life feel more complete.
        </p>
        <p>
          This website is just a small gift, but the feeling behind it is real. I wanted to create something that reflects how I see you — elegant, unforgettable, and deeply treasured. No matter how busy life becomes, I never want you to forget that you are appreciated, respected, and loved more than these simple lines can ever express.
        </p>
        <p>
          In a world full of ordinary things, you are one of the rarest and most beautiful parts of my heart.
        </p>
        <div class="signature">— With love, always</div>
      </div>
    </section>

    <section id="special">
      <h2 class="section-title">Why You Are So Special</h2>
      <p class="section-sub">
        There are so many reasons, but these are some of the ones that shine the most in my heart.
      </p>
      <div class="grid">
        <div class="glass card">
          <h3>Your Smile</h3>
          <p>Your smile has a quiet magic. It can soften my heart, brighten my mood, and make everything around me feel lighter.</p>
        </div>
        <div class="glass card">
          <h3>Your Kindness</h3>
          <p>The way you carry care and softness within you is something truly beautiful. Your kindness makes you unforgettable.</p>
        </div>
        <div class="glass card">
          <h3>Your Presence</h3>
          <p>Just knowing you are there brings comfort. You have a way of making life feel calmer, sweeter, and more complete.</p>
        </div>
        <div class="glass card">
          <h3>Your Beauty</h3>
          <p>Your beauty is not only in how you look, but in your soul, your grace, and the warmth you bring into every moment.</p>
        </div>
        <div class="glass card">
          <h3>Your Support</h3>
          <p>The encouragement, understanding, and softness you give mean more than I can explain. It stays with me in the deepest way.</p>
        </div>
        <div class="glass card">
          <h3>Your Place In My Heart</h3>
          <p>You are not just special to me — you are deeply valued, remembered, and held close in a place that belongs only to you.</p>
        </div>
      </div>
    </section>

    <section id="memories">
      <h2 class="section-title">Our Beautiful Memories</h2>
      <p class="section-sub">
        You can replace these placeholders with your own photos, sweet moments, or captions that are meaningful to both of you.
      </p>
      <div class="gallery">
        <div class="memory"><span>The moment that stayed in my heart</span></div>
        <div class="memory"><span>A memory that still makes me smile</span></div>
        <div class="memory"><span>A beautiful chapter with you</span></div>
      </div>
    </section>

    <section id="promise">
      <h2 class="section-title">A Promise For You</h2>
      <p class="section-sub">
        Not just words — a feeling meant to stay.
      </p>
      <div class="glass">
        <blockquote>
          “No matter where life takes us, you will always have a deeply cherished place in my heart — with love, respect, and a tenderness that words can never fully measure.”
          <footer>Made with love, only for YOU SONAMONI.</footer>
        </blockquote>
      </div>
    </section>

    <section>
      <div class="glass final">
        <h2 class="section-title">My Final Little Surprise</h2>
        <p>
          Mim, this website may be simple, but the feeling behind it is not. It carries admiration, gratitude, and a very sincere place in my heart for you. <strong>You are deeply special</strong>, and I wanted to create something beautiful enough to remind you of that. If you ever read this again in a quiet moment, I hope it makes you smile and feel just how much you are valued.
          <br><br>
          In this life, and in every soft dream of mine, you will always remain someone precious to me.
        </p>
      </div>
    </section>

    <div class="footer">
      Crafted with love for Anamika Islam Mim ✨
    </div>
  </div>

  <audio id="bgMusic" loop>
    <source src="" type="audio/mpeg">
  </audio>

  <script>
    const particles = document.getElementById('particles');
    const symbols = ['♡', '♥', '✦', '✨'];

    for (let i = 0; i < 28; i++) {
      const el = document.createElement('span');
      el.className = 'particle';
      el.textContent = symbols[Math.floor(Math.random() * symbols.length)];
      el.style.left = Math.random() * 100 + 'vw';
      el.style.animationDuration = (8 + Math.random() * 10) + 's';
      el.style.animationDelay = (Math.random() * 8) + 's';
      el.style.fontSize = (10 + Math.random() * 16) + 'px';
      particles.appendChild(el);
    }

    const music = document.getElementById('bgMusic');
    const musicBtn = document.getElementById('musicBtn');
    let playing = false;

    musicBtn.addEventListener('click', () => {
      if (!music.getAttribute('src') && !music.querySelector('source').src) {
        alert('Add your music link inside the <audio> tag first, then the button will work.');
        return;
      }

      if (!playing) {
        music.play();
        musicBtn.textContent = 'Pause Music';
        playing = true;
      } else {
        music.pause();
        musicBtn.textContent = 'Play Music';
        playing = false;
      }
    });
  </script>
</body>
</html>
