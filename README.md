# startwithzero
<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>StartWithZero — Start Here</title>
  <meta name="description" content="StartWithZero helps African youth and beginners start earning online with little or no capital — practical steps, skills that pay, and scam-free guidance." />
  <style>
    :root{
      --bg:#0b1220;
      --muted:#9fb0c7;
      --text:#eaf0ff;
      --line:rgba(255,255,255,.10);
      --accent:#f59e0b;
      --shadow: 0 18px 60px rgba(0,0,0,.45);
      --radius: 18px;
    }*{box-sizing:border-box}
html{scroll-behavior:smooth}
body{
  margin:0;
  font-family: ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial, "Apple Color Emoji","Segoe UI Emoji";
  color:var(--text);
  background: radial-gradient(1200px 600px at 20% -10%, rgba(245,158,11,.20), transparent 60%),
              radial-gradient(1000px 500px at 100% 0%, rgba(30,58,138,.25), transparent 55%),
              linear-gradient(180deg, #070b14 0%, var(--bg) 55%, #070b14 100%);
  line-height:1.6;
}

a{color:inherit; text-decoration:none}
a:hover{opacity:.92}

.container{max-width:1100px; margin:0 auto; padding: 0 20px;}

/* Top nav */
.nav{
  position:sticky; top:0; z-index:50;
  backdrop-filter: blur(10px);
  background: rgba(7, 11, 20, .72);
  border-bottom:1px solid var(--line);
}
.nav-inner{
  display:flex; align-items:center; justify-content:space-between;
  padding:14px 0;
  gap:16px;
}
.brand{display:flex; align-items:center; gap:10px; font-weight:800; letter-spacing:.2px;}
.mark{
  width:34px; height:34px; border-radius:12px;
  background: linear-gradient(135deg, rgba(245,158,11,.95), rgba(245,158,11,.35));
  display:grid; place-items:center;
  box-shadow: 0 10px 30px rgba(245,158,11,.18);
}
.mark svg{display:block}
.brand span{font-size:15px}

.nav-links{display:flex; gap:8px; flex-wrap:wrap; justify-content:flex-end}
.nav-links a{
  font-size:13px;
  color:var(--muted);
  padding:8px 10px;
  border-radius:999px;
  border:1px solid transparent;
}
.nav-links a:hover{color:var(--text); border-color:var(--line); background: rgba(255,255,255,.04)}

/* Hero */
header{padding: 56px 0 24px;}
.hero{display:grid; grid-template-columns: 1.2fr .8fr; gap:22px; align-items:stretch;}
@media (max-width: 900px){.hero{grid-template-columns:1fr;}}

.hero-card{
  background: rgba(15, 26, 46, .70);
  border:1px solid var(--line);
  border-radius: var(--radius);
  padding:26px;
  box-shadow: var(--shadow);
  position:relative;
  overflow:hidden;
}
.hero-card:before{
  content:"";
  position:absolute; inset:-2px;
  background: radial-gradient(600px 220px at 30% 0%, rgba(245,158,11,.18), transparent 55%),
              radial-gradient(520px 240px at 100% 10%, rgba(30,58,138,.22), transparent 55%);
  pointer-events:none;
}
.hero-card > *{position:relative}

.kicker{
  display:inline-flex; align-items:center; gap:8px;
  font-size:12px; color:var(--muted);
  padding:6px 10px; border-radius:999px;
  background: rgba(255,255,255,.04);
  border: 1px solid var(--line);
}
.kicker b{color:var(--text)}
h1{margin:14px 0 10px; font-size:40px; line-height:1.1;}
.lead{margin:0; color: var(--muted); font-size:15px; max-width:60ch;}

.cta-row{display:flex; gap:12px; flex-wrap:wrap; margin-top:18px;}
.btn{
  display:inline-flex; align-items:center; gap:10px;
  padding:10px 14px;
  border-radius: 12px;
  border:1px solid var(--line);
  background: rgba(255,255,255,.04);
  font-size:13px;
  color:var(--text);
}
.btn.primary{
  border-color: rgba(245,158,11,.55);
  background: linear-gradient(135deg, rgba(245,158,11,.22), rgba(245,158,11,.06));
  box-shadow: 0 14px 40px rgba(245,158,11,.12);
}
.btn:hover{transform: translateY(-1px); transition: transform .15s ease;}

/* Side info */
.side{display:grid; gap:14px;}
.mini{
  background: rgba(15, 26, 46, .55);
  border:1px solid var(--line);
  border-radius: var(--radius);
  padding:16px;
}
.mini h3{margin:0 0 8px; font-size:14px;}
.mini p{margin:0; color:var(--muted); font-size:13px;}

/* Sections */
section{padding: 18px 0;}
.section-card{
  background: rgba(15, 26, 46, .55);
  border:1px solid var(--line);
  border-radius: var(--radius);
  padding:22px;
}
.section-title{
  display:flex; align-items:center; justify-content:space-between;
  gap:12px;
  margin-bottom:10px;
}
.section-title h2{margin:0; font-size:20px;}
.pill{
  font-size:12px; color:var(--muted);
  padding:6px 10px; border-radius:999px;
  border: 1px solid var(--line);
  background: rgba(255,255,255,.03);
  white-space:nowrap;
}

.grid{display:grid; grid-template-columns: repeat(12, 1fr); gap:14px; margin-top:14px;}
.col-6{grid-column: span 6;}
.col-4{grid-column: span 4;}
.col-12{grid-column: span 12;}
@media (max-width: 900px){.col-6,.col-4{grid-column: span 12;}}

.item{border:1px solid var(--line); border-radius: 16px; padding:16px; background: rgba(255,255,255,.03);}
.item h3{margin:0 0 8px; font-size:14px;}
.item p{margin:0; color:var(--muted); font-size:13px;}

ul.clean{margin:8px 0 0; padding-left:18px; color: var(--muted)}
ul.clean li{margin: 8px 0;}

blockquote{
  margin: 14px 0 0;
  padding: 14px 16px;
  border-left: 3px solid rgba(245,158,11,.75);
  background: rgba(245,158,11,.06);
  border-radius: 12px;
  color: var(--text);
}

.callout{
  margin-top:14px;
  padding: 14px 16px;
  border-radius: 16px;
  border: 1px solid rgba(245,158,11,.35);
  background: linear-gradient(135deg, rgba(245,158,11,.12), rgba(245,158,11,.04));
  color: var(--muted);
  font-size: 13px;
}

.contact-box{display:flex; gap:12px; flex-wrap:wrap; margin-top:10px;}
.contact-pill{display:inline-flex; align-items:center; gap:10px; padding:10px 12px; border-radius: 14px; border:1px solid var(--line); background: rgba(255,255,255,.03); color: var(--muted); font-size:13px;}
.contact-pill b{color:var(--text); font-weight:700}

footer{padding: 34px 0 44px; color: var(--muted); font-size: 13px; border-top: 1px solid var(--line); margin-top: 18px;}

  </style>
</head><body>
  <div class="nav">
    <div class="container">
      <div class="nav-inner">
        <a class="brand" href="#top" aria-label="StartWithZero home">
          <span class="mark" aria-hidden="true">
            <svg width="18" height="18" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M12 2l7 7h-4v8H9V9H5l7-7z" fill="rgba(15,26,46,.88)"/>
            </svg>
          </span>
          <span>StartWithZero</span>
        </a><nav class="nav-links" aria-label="On-page navigation">
      <a href="#start">Start Here</a>
      <a href="#gain">What You’ll Gain</a>
      <a href="#steps">3 Steps</a>
      <a href="#resource">Free Resource</a>
      <a href="#why">Why It Exists</a>
      <a href="#creator">Creator</a>
      <a href="#contact">Contact</a>
    </nav>
  </div>
</div>

  </div>  <div id="top"></div>
  <header class="container">
    <div class="hero">
      <div class="hero-card">
        <div class="kicker"><b>StartWithZero</b> • Start earning with zero capital</div>
        <h1>Start earning online with little or no capital.</h1>
        <p class="lead">A single-page preview of your Start Here content — structured, scannable, and easy to navigate.</p><div class="cta-row">
      <a class="btn primary" href="#steps">See the 3-step path</a>
      <a class="btn" href="#contact">Contact Amide</a>
    </div>
  </div>

  <div class="side">
    <div class="mini">
      <h3>Audience</h3>
      <p>African teens and youth, beginners, and anyone starting from zero and building steadily.</p>
    </div>
    <div class="mini">
      <h3>Approach</h3>
      <p>Practical steps, realistic expectations, and scam-free guidance — no hype.</p>
    </div>
    <div class="mini">
      <h3>Core message</h3>
      <p>Start small. Stay consistent. Grow steadily.</p>
    </div>
  </div>
</div>

  </header>  <main class="container"><section id="start">
  <div class="section-card">
    <div class="section-title">
      <h2>Start Here 👋</h2>
      <span class="pill">Overview</span>
    </div>
    <p>Welcome to <strong>StartWithZero</strong> — a practical platform helping African youth and beginners start earning online with little or no capital.</p>
    <p>If you’ve tried different online methods without results, felt overwhelmed by information, or believed you needed money to start — you’re not alone.</p>
    <p>StartWithZero exists to show you a realistic, practical path forward.</p>
  </div>
</section>

<section id="gain">
  <div class="section-card">
    <div class="section-title">
      <h2>What You’ll Gain Here</h2>
      <span class="pill">Outcomes</span>
    </div>

    <div class="grid">
      <div class="item col-6">
        <h3>Practical ways to earn online with zero capital</h3>
        <p>Beginner-friendly paths you can start today using simple tools.</p>
      </div>
      <div class="item col-6">
        <h3>Skills that pay in Africa and globally</h3>
        <p>Clear guidance on skills that have real demand.</p>
      </div>
      <div class="item col-6">
        <h3>How to avoid scams and fake opportunities</h3>
        <p>Red flags, verification tips, and how to protect yourself online.</p>
      </div>
      <div class="item col-6">
        <h3>Real lessons from lived experiences</h3>
        <p>What worked, what didn’t, and how to move forward with clarity.</p>
      </div>
    </div>

    <div class="callout"><strong style="color:var(--text)">No hype.</strong> No unrealistic promises. Just clear, actionable steps.</div>
  </div>
</section>

<section id="steps">
  <div class="section-card">
    <div class="section-title">
      <h2>Your Path Starts in 3 Simple Steps</h2>
      <span class="pill">Follow in order</span>
    </div>

    <div class="grid">
      <div class="item col-4">
        <h3>1️⃣ Read the Beginner Guide</h3>
        <p><strong>How African Youth Can Start Earning Online This Week</strong> <span style="color:var(--muted)">(Coming soon)</span></p>
        <p style="margin-top:8px">This guide will help you understand where to begin and what to avoid.</p>
      </div>

      <div class="item col-4">
        <h3>2️⃣ Choose One Skill to Start</h3>
        <p>Focus on one practical skill you can begin immediately:</p>
        <ul class="clean">
          <li>Video editing using free tools</li>
          <li>Social media caption writing</li>
          <li>Canva design for small businesses</li>
          <li>WhatsApp TV advertising</li>
        </ul>
        <p style="margin-top:10px">You don’t need to master everything. Start small and build confidence.</p>
      </div>

      <div class="item col-4">
        <h3>3️⃣ Avoid the Mistakes That Slow Beginners Down</h3>
        <p>Most people struggle because they:</p>
        <ul class="clean">
          <li>Chase too many methods at once</li>
          <li>Pay for courses they can’t afford</li>
          <li>Believe unrealistic income promises</li>
        </ul>
        <p style="margin-top:10px">Here, you’ll learn how to move forward with clarity and avoid wasted time.</p>
      </div>
    </div>
  </div>
</section>

<section id="resource">
  <div class="section-card">
    <div class="section-title">
      <h2>Free Resource (Coming Soon)</h2>
      <span class="pill">Checklist</span>
    </div>
    <p>📥 <strong>7 Legit Ways African Youth Can Earn Online With Zero Capital</strong></p>
    <p style="color:var(--muted)">A practical checklist showing simple options you can start today.</p>
  </div>
</section>

<section id="why">
  <div class="section-card">
    <div class="section-title">
      <h2>Why StartWithZero Exists</h2>
      <span class="pill">Story</span>
    </div>
    <p>StartWithZero was created from real experiences — not theory.</p>
    <p style="color:var(--muted)">After trying multiple online paths without success, attending webinars I couldn’t afford, and starting things I couldn’t sustain, I experienced the same frustration many young Africans face.</p>
    <p>But I learned something important:</p>
    <blockquote>You don’t need everything to start — you need to start with what you have.</blockquote>
    <p style="margin-top:12px; color:var(--muted)">StartWithZero is built on that belief.</p>
  </div>
</section>

<section id="creator">
  <div class="section-card">
    <div class="section-title">
      <h2>About the Creator</h2>
      <span class="pill">Amide</span>
    </div>
    <p><strong>Amide</strong> — Software developer, nurse, video editor, and digital marketing enthusiast.</p>
    <p style="color:var(--muted)">I built StartWithZero to help beginners avoid confusion, wasted money, and false promises by sharing practical, real-world pathways to earning online.</p>
  </div>
</section>

<section id="contact">
  <div class="section-card">
    <div class="section-title">
      <h2>Stay Connected</h2>
      <span class="pill">Reach out</span>
    </div>
    <p>Have questions or need guidance?</p>

    <div class="contact-box">
      <div class="contact-pill"><b>Email</b> <span>amidejackie3@gmail.com</span></div>
      <div class="contact-pill"><b>WhatsApp</b> <span>08063470925</span></div>
    </div>

    <p style="margin-top:12px; color:var(--muted)">More community support options are coming soon.</p>
  </div>
</section>

<section>
  <div class="section-card">
    <div class="section-title">
      <h2>Your journey starts now.</h2>
      <span class="pill">Closing</span>
    </div>
    <p style="color:var(--muted)">Start small. Stay consistent. Grow steadily.</p>
  </div>
</section>

<footer>
  <div class="container" style="padding:0">
    <div style="display:flex; gap:10px; flex-wrap:wrap; align-items:center; justify-content:space-between;">
      <div>© <span id="y"></span> StartWithZero — Built by Amide</div>
      <div style="opacity:.9">Single-page HTML preview.</div>
    </div>
  </div>
</footer>

  </main>  <script>
    document.getElementById('y').textContent = new Date().getFullYear();
  </script></body>
</html>
