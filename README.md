<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Bryan Barrett • SaaS Revenue Leader</title>
  <meta name="viewport" content="width=device-width,initial-scale=1">
  <!-- Font & Icons -->
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@400;600;700&display=swap" rel="stylesheet">
  <style>
    /* ----- Base Styles ----- */
    :root{
      --bg-grad: linear-gradient(135deg,#1f2937 0%,#0f172a 100%);
      --accent:#3b82f6;           /* blue-500 */
      --text:#f1f5f9;             /* slate-100 */
      --subtext:#94a3b8;          /* slate-400 */
    }
    *{box-sizing:border-box;margin:0;padding:0}
    body{
      font-family:'Inter',sans-serif;
      min-height:100vh;
      background:var(--bg-grad);
      color:var(--text);
      display:flex;
      flex-direction:column;
      align-items:center;
      scroll-behavior:smooth;
      -webkit-font-smoothing:antialiased;
    }
    h1{font-size:clamp(2.2rem,6vw,3.5rem);font-weight:700;line-height:1.1;margin-bottom:.5rem}
    h2{font-size:1.25rem;color:var(--accent);letter-spacing:.08em;font-weight:600;margin-bottom:1.2rem;text-transform:uppercase}
    p{font-size:1rem;color:var(--subtext);line-height:1.6;margin-bottom:1.1rem;max-width:720px}
    a{color:var(--accent);text-decoration:none}
    .btn{display:inline-block;padding:.75rem 1.5rem;border:1px solid var(--accent);border-radius:6px;transition:.25s}
    .btn:hover{background:var(--accent);color:#fff}
    section{padding:4.5rem 1.2rem;width:100%;max-width:1000px;text-align:center;opacity:0;transform:translateY(40px);transition:opacity .6s ease,transform .6s ease}
    section.reveal{opacity:1;transform:none}
    /* ----- Layout Helpers ----- */
    .metrics{display:flex;flex-wrap:wrap;justify-content:center;gap:1.5rem;margin-top:2rem}
    .metric{flex:1 1 220px;padding:1.3rem;border:1px solid rgba(255,255,255,.08);border-radius:8px;background:rgba(255,255,255,.02)}
    .metric strong{font-size:1.5rem;display:block;color:#fff;font-weight:700;margin-bottom:.25rem}
    /* ----- Footer ----- */
    footer{margin-top:auto;padding:2rem;color:var(--subtext);font-size:.9rem;text-align:center}
  </style>
</head>
<body>

<!-- ===== Hero ===== -->
<section id="hero" class="reveal">
  <h1>Bryan Barrett</h1>
  <h2>Mid-Market AE • Strategic Partnerships • Enterprise Revenue</h2>
  <p>
    25+ years closing B2B deals, building partner ecosystems, and most recently <strong>adding&nbsp;$4.5&nbsp;M in Q1 ‘25</strong> while weaving GPT-powered automations into the sales stack.
    I scale revenue where ops, tech & people intersect.
  </p>
  <a class="btn" href="#contact">Let's Talk</a>
  &nbsp;
  <a class="btn" href="Bryan_Barrett_Resume.pdf" target="_blank">Download Résumé</a>
</section>

<!-- ===== Metrics ===== -->
<section id="wins" class="reveal">
  <h2>Key Wins</h2>
  <div class="metrics">
    <div class="metric"><strong>$4.5M</strong>New revenue closed in Q1 ‘25</div>
    <div class="metric"><strong>$7M</strong>Annual territory managed</div>
    <div class="metric"><strong>25 yrs</strong>B2B sales &amp; partnerships</div>
    <div class="metric"><strong>GPT&nbsp;+ Python</strong>AI workflow builder</div>
  </div>
</section>

<!-- ===== Tech Stack / Projects ===== -->
<section id="ai" class="reveal">
  <h2>AI &amp; Workflow Highlights</h2>
  <p>
    • Deployed GPT prompts + Zapier webhooks to auto-score inbound leads.<br>
    • Built Python script to push closed-won data to Slack + Notion analytics.<br>
    • Trimmed proposal turnaround time by <strong>47%</strong> using custom ChatGPT templates.
  </p>
</section>

<!-- ===== Contact ===== -->
<section id="contact" class="reveal">
  <h2>Connect</h2>
  <p>Open to remote AE or Partnership roles in SaaS / AI—targeting $150K+ OTE.</p>
  <a class="btn" href="mailto:brybarrett@ymail.com">Email Bryan</a>
  &nbsp;
  <a class="btn" href="https://linkedin.com/in/bryansbarrett" target="_blank">LinkedIn</a>
</section>

<footer>
  © 2025 Bryan Barrett — Built with recruiter psychology & a touch of GPT magic.
</footer>

<!-- ===== Scroll Reveal Script ===== -->
<script>
  const sections = document.querySelectorAll('section');
  const observer = new IntersectionObserver(entries=>{
    entries.forEach(entry=>{
      if(entry.isIntersecting){entry.target.classList.add('reveal')}
    });
  },{threshold:0.15});
  sections.forEach(sec=>observer.observe(sec));
</script>

</body>
</html>
