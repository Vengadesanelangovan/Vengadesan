<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8" />
<meta name="viewport" content="width=device-width,initial-scale=1" />
<title>Your Name — Portfolio</title>
<meta name="description" content="Your Name — Full-Stack Developer. Short intro and projects." />
<link rel="icon" href="data:," />
<style>
  :root{
    --bg:#0f1724; --card:#0b1220; --muted:#94a3b8; --accent1:#7b2ff7; --accent2:#ff7a18;
    --glass: rgba(255,255,255,0.04);
    --radius:14px; font-family: Inter,system-ui,Segoe UI,Roboto,Arial;
  }
  *{box-sizing:border-box}
  body{margin:0; background:
    radial-gradient(800px 400px at 10% 10%, rgba(123,47,247,0.09), transparent 8%),
    radial-gradient(700px 300px at 90% 80%, rgba(255,122,24,0.05), transparent 10%),
    var(--bg); color:#e6eef8; -webkit-font-smoothing:antialiased}
  .wrap{max-width:1100px;margin:48px auto;padding:36px}
  header{display:flex;align-items:center;gap:18px}
  .avatar{width:96px;height:96px;border-radius:14px;background:linear-gradient(135deg,var(--accent1),var(--accent2));display:flex;align-items:center;justify-content:center;font-weight:700;font-size:28px;box-shadow:0 8px 30px rgba(11,18,32,.6)}
  .intro{flex:1}
  h1{margin:0;font-size:28px;letter-spacing:-0.4px}
  p.lead{margin:6px 0 12px;color:var(--muted)}
  .cta{display:flex;gap:10px}
  .btn{background:linear-gradient(90deg,var(--accent1),var(--accent2));color:white;padding:10px 14px;border-radius:10px;text-decoration:none;font-weight:600;box-shadow:0 6px 18px rgba(123,47,247,.12);transition:transform .18s}
  .btn.secondary{background:transparent;border:1px solid rgba(255,255,255,.06);color:var(--muted)}
  .btn:hover{transform:translateY(-4px)}
  .grid{display:grid;grid-template-columns:repeat(3,1fr);gap:18px;margin-top:28px}
  .card{background:var(--card);padding:18px;border-radius:12px;box-shadow:0 6px 30px rgba(2,6,23,.6);border:1px solid rgba(255,255,255,.02)}
  .project-title{font-weight:700;margin:0 0 6px}
  .meta{color:var(--muted);font-size:13px;margin-bottom:10px}
  .project-thumb{height:120px;border-radius:10px;background:linear-gradient(180deg, rgba(255,255,255,0.02), transparent);display:flex;align-items:center;justify-content:center;margin-bottom:12px;color:var(--muted)}
  .skills{display:flex;gap:8px;flex-wrap:wrap}
  .chip{background:var(--glass);padding:6px 8px;border-radius:999px;font-size:13px;color:var(--muted);border:1px solid rgba(255,255,255,.02)}
  section + section{margin-top:40px}
  footer{color:var(--muted);font-size:13px;margin-top:42px;text-align:center}
  /* Animations */
  .hero-anim {position:relative;overflow:visible}
  .blob{position:absolute;width:220px;height:220px;border-radius:50%;filter:blur(36px);opacity:.9;mix-blend-mode:screen}
  .b1{left:-60px;top:-40px;background:linear-gradient(120deg,var(--accent1),#6EE7B7);animation:float1 8s ease-in-out infinite}
  .b2{right:-60px;bottom:-50px;background:linear-gradient(120deg,var(--accent2),#f107a3);width:180px;height:180px;animation:float2 10s ease-in-out infinite}
  @keyframes float1{0%{transform:translateY(0)}50%{transform:translateY(-18px)}100%{transform:translateY(0)}}
  @keyframes float2{0%{transform:translateY(0) scale(.96)}50%{transform:translateY(-24px) scale(1.03)}100%{transform:translateY(0) scale(.96)}}
  /* Responsive */
  @media (max-width:980px){.grid{grid-template-columns:repeat(2,1fr)}}
  @media (max-width:640px){.wrap{padding:20px;margin:20px} .grid{grid-template-columns:1fr} header{flex-direction:row;gap:12px} .avatar{width:72px;height:72px;font-size:22px}}
</style>
</head>
<body>
  <div class="wrap">
    <header class="hero-anim">
      <div class="blob b1" aria-hidden="true"></div>
      <div class="blob b2" aria-hidden="true"></div>

  <div class="avatar">YN</div>
      <div class="intro">
        <h1>Hi — I’m <strong>Your Name</strong>.<br/><span style="color:var(--muted);font-weight:600;font-size:15px">Full-Stack Developer / React • Node • MongoDB</span></h1>
        <p class="lead">I build fast, accessible web apps. Currently learning DevOps and shipping small OSS tools. I enjoy clean design and readable code.</p>
        <div class="cta">
          <a class="btn" href="#projects">See projects</a>
          <a class="btn secondary" href="mailto:you@example.com">Contact</a>
          <a class="btn secondary" href="resume.pdf" target="_blank" rel="noopener">Resume</a>
        </div>
      </div>
    </header>

    <section id="projects">
  <h2 style="margin:18px 0 12px">Featured Projects</h2>
      <div class="grid">
        <!-- Project 1 -->
        <article class="card">
          <div class="project-thumb">Screenshot / GIF</div>
          <h3 class="project-title">Project One</h3>
          <div class="meta">Realtime chat app — React, Node, Socket.IO</div>
          <p style="color:var(--muted);font-size:14px;margin:0 0 12px">A realtime chat with rooms, user presence, and emoji reactions. Deployed on Vercel/Heroku.</p>
          <div style="display:flex;gap:8px;align-items:center;justify-content:space-between">
            <div class="skills">
              <span class="chip">React</span>
              <span class="chip">Node</span>
              <span class="chip">Socket.IO</span>
            </div>
            <div style="display:flex;gap:8px">
              <a class="btn secondary" href="https://example.com" target="_blank" rel="noopener">Live</a>
              <a class="btn secondary" href="https://github.com/YourUserName/project-one" target="_blank" rel="noopener">Code</a>
            </div>
          </div>
        </article>
        <!-- Project 2 -->
        <article class="card">
          <div class="project-thumb">Screenshot / GIF</div>
          <h3 class="project-title">Project Two</h3>
          <div class="meta">Personal blog platform — Next.js, MDX</div>
          <p style="color:var(--muted);font-size:14px;margin:0 0 12px">A lightweight blog with MDX, RSS, and SEO optimizations. Fast and accessible.</p>
          <div style="display:flex;gap:8px;align-items:center;justify-content:space-between">
            <div class="skills">
              <span class="chip">Next.js</span>
              <span class="chip">MDX</span>
              <span class="chip">Vercel</span>
            </div>
            <div style="display:flex;gap:8px">
              <a class="btn secondary" href="https://example.com" target="_blank" rel="noopener">Live</a>
              <a class="btn secondary" href="https://github.com/YourUserName/project-two" target="_blank" rel="noopener">Code</a>
            </div>
          </div>
        </article>
        <!-- Project 3 -->
        <article class="card">
          <div class="project-thumb">Screenshot / GIF</div>
          <h3 class="project-title">Project Three</h3>
          <div class="meta">Analytics dashboard — React, Recharts</div>
          <p style="color:var(--muted);font-size:14px;margin:0 0 12px">An analytics dashboard showing custom charts and exports. Focused on performance and clarity.</p>
          <div style="display:flex;gap:8px;align-items:center;justify-content:space-between">
            <div class="skills">
              <span class="chip">React</span>
              <span class="chip">Charting</span>
              <span class="chip">Postgres</span>
            </div>
            <div style="display:flex;gap:8px">
              <a class="btn secondary" href="https://example.com" target="_blank" rel="noopener">Live</a>
              <a class="btn secondary" href="https://github.com/YourUserName/project-three" target="_blank" rel="noopener">Code</a>
            </div>
          </div>
        </article>
      </div>
    </section>
    <section>
      <h2 style="margin:18px 0 12px">Skills</h2>
      <div style="display:flex;gap:8px;flex-wrap:wrap">
        <span class="chip">JavaScript</span>
        <span class="chip">TypeScript</span>
        <span class="chip">React</span>
        <span class="chip">Node.js</span>
        <span class="chip">Express</span>
        <span class="chip">MongoDB</span>
        <span class="chip">Docker</span>
        <span class="chip">Git</span>
        <span class="chip">AWS</span>
      </div>
    </section>
    <section>
      <h2 style="margin:18px 0 12px">Contact</h2>
      <p style="color:var(--muted);margin:0 0 12px">Email: <a href="mailto:you@example.com" style="color:inherit">you@example.com</a> • <a href="https://linkedin.com/in/yourusername" target="_blank" rel="noopener" style="color:inherit">LinkedIn</a> • <a href="https://github.com/YourUserName" target="_blank" rel="noopener" style="color:inherit">GitHub</a></p>
      <div style="margin-top:10px">
        <a class="btn" href="mailto:you@example.com?subject=Hi%20from%20portfolio">Say Hello</a>
      </div>
    </section>
    <footer>
      © <span id="year"></span> Your Name — Built with ❤️ • <a href="resume.pdf" style="color:var(--muted)">Resume</a>
    </footer>
  </div>

<script>
  // small script for dynamic year and replacing avatar initials if you like
  document.getElementById('year').textContent = new Date().getFullYear();
  // Optionally set avatar initials from name:
  const name = "Your Name";
  const initials = name.split(' ').map(s => s[0]).slice(0,2).join('').toUpperCase();
  document.querySelector('.avatar').textContent = initials;
</script>
</body>
</html>
