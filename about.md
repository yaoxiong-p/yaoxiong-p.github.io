---
layout: default
title: About Yao Xiong
---

<style>
  :root{
    --accent: seagreen;              /* 主题色：与你之前想要的 seagreen 一致 */
    --text: #222;
    --muted: #666;
    --bg-soft: #f6f8f8;
  }
  .about-wrap{
    display:flex; gap:28px; align-items:flex-start;
    margin: 0 0 2.5rem 0;
    flex-wrap:wrap;                   /* 移动端自动换行 */
  }
  .about-photo{
    width:260px; max-width:100%;
  }
  .about-photo img{
    width:100%; height:auto; display:block;
    border-radius:14px;
    box-shadow:0 6px 18px rgba(0,0,0,.08);
  }
  .social-row{
    margin-top:14px; display:flex; gap:12px; flex-wrap:wrap;
  }
  .social-btn{
    width:38px; height:38px; border-radius:50%;
    display:grid; place-items:center; background:var(--bg-soft);
    box-shadow: inset 0 0 0 1px rgba(0,0,0,.06);
    transition:transform .12s ease, box-shadow .2s ease, background .2s ease;
  }
  .social-btn:hover{ transform:translateY(-1px); box-shadow:0 6px 14px rgba(0,0,0,.10); background:#fff; }
  .social-btn svg{ width:20px; height:20px; fill:var(--text); }
  .social-btn.orcid svg circle{ fill: var(--accent); }
  .social-btn.orcid svg path{ fill:#fff; }
  .about-main{ flex:1 1 420px; min-width:320px; }
  .about-name{ font-size:1.8rem; font-weight:700; margin:.25rem 0 0.75rem; }
  .introp{ font-size:0.8rem; line-height:1.0; color:var(--text); max-width:72ch; }
  .section-title{ font-size:1.1rem; letter-spacing:.02em; margin:1.75rem 0 .75rem; font-weight:700; }

  /* 教育时间轴 */
  .edu{
    position:relative; padding-left:26px;
  }
  .edu::before{
    content:""; position:absolute; left:8px; top:6px; bottom:6px; width:2px; background:rgba(46,139,87,.25);
  }
  .edu-item{ position:relative; margin: .6rem 0 .6rem; color:var(--text); }
  .edu-item::before{
    content:""; position:absolute; left:-18px; top:.45rem;
    width:10px; height:10px; border-radius:50%; background:var(--accent);
    box-shadow: 0 0 0 3px rgba(46,139,87,.15);
  }
  .edu-year{ font-weight:700; margin-right:.4rem; }
  .view-cv{
    display:inline-block; margin-top: .75rem; text-decoration:none; font-weight:600;
    color:var(--accent); border-bottom:2px solid transparent;
  }
  .view-cv:hover{ border-color:var(--accent); }
</style>

<div class="post">
  <div class="about-wrap">
    <!-- 左侧头像 + 社交 -->
    <div class="about-photo">
      <img src="{{ '/assets/img/Yao Xiong_headshot_Transp.jpg' | relative_url }}" alt="Yao Xiong headshot">
      <div class="social-row">
        <!-- 邮件 -->
        <a class="social-btn" href="mailto:yao@example.edu" aria-label="Email">
          <svg viewBox="0 0 24 24" aria-hidden="true"><path d="M20 4H4a2 2 0 0 0-2 2v12c0 1.1.9 2 2 2h16a2 2 0 0 0 2-2V6c0-1.1-.9-2-2-2Zm0 4-8 5L4 8V6l8 5 8-5v2Z"/></svg>
        </a>
        <!-- Google Scholar -->
        <a class="social-btn" href="https://scholar.google.com/citations?user=YOUR_ID" target="_blank" rel="noopener" aria-label="Google Scholar">
          <svg viewBox="0 0 24 24" aria-hidden="true"><path d="m12 3 9 7-3.5 2.7L12 8.5 6.5 12.7 3 10l9-7Zm0 9.7 5.5 4-5.5 4-5.5-4 5.5-4Z"/></svg>
        </a>
        <!-- GitHub -->
        <a class="social-btn" href="https://github.com/yaoxiong-p" target="_blank" rel="noopener" aria-label="GitHub">
          <svg viewBox="0 0 24 24" aria-hidden="true"><path d="M12 .5A12 12 0 0 0 0 12.7c0 5.4 3.4 9.9 8.2 11.5.6.1.8-.3.8-.6v-2c-3.3.7-4-1.6-4-1.6-.5-1.3-1.2-1.6-1.2-1.6-1-.7.1-.7.1-.7 1.1.1 1.7 1.1 1.7 1.1 1 .1 1.7-.7 1.9-1a3.1 3.1 0 0 1 .9-1.8C5.2 14.7 3.2 13.8 3.2 10a4.7 4.7 0 0 1 1.3-3.3 4.4 4.4 0 0 1 .1-3.3s1-.3 3.4 1.3a11.8 11.8 0 0 1 6.2 0c2.3-1.6 3.3-1.3 3.3-1.3.5 1 .5 2.3.1 3.3a4.7 4.7 0 0 1 1.3 3.3c0 3.8-2 4.7-4 5a3.4 3.4 0 0 1 1 2.6v3.8c0 .3.2.7.9.6 4.8-1.6 8.2-6.1 8.2-11.5A12 12 0 0 0 12 .5Z"/></svg>
        </a>
        <!-- LinkedIn -->
        <a class="social-btn" href="https://www.linkedin.com/in/YOUR_ID" target="_blank" rel="noopener" aria-label="LinkedIn">
          <svg viewBox="0 0 24 24" aria-hidden="true"><path d="M4.98 3.5C4.98 4.88 3.86 6 2.5 6S0 4.88 0 3.5 1.12 1 2.5 1s2.48 1.12 2.48 2.5ZM.5 8.5h4V23h-4V8.5Zm7 0h3.8v2h.1c.5-1 1.9-2.2 3.9-2.2 4.2 0 5 2.7 5 6.3V23h-4v-5.9c0-1.4 0-3.2-2-3.2s-2.3 1.5-2.3 3.1V23h-4V8.5Z"/></svg>
        </a>
        <!-- ORCID（绿色圆底 + 白色“iD”） -->
        <a class="social-btn orcid" href="https://orcid.org/0000-0000-0000-0000" target="_blank" rel="noopener" aria-label="ORCID">
          <svg viewBox="0 0 100 100" aria-hidden="true">
            <circle cx="50" cy="50" r="48"/>
            <path d="M34.8 68.5V41.5h-6.3v27h6.3Zm-3.1-29.9a3.7 3.7 0 1 0 0-7.4 3.7 3.7 0 0 0 0 7.4ZM44 68.5V34.1h6.2v13.1h12.4V34.1h6.2v34.4h-6.2V52.8H50.2v15.7H44Z"/>
          </svg>
        </a>
      </div>
    </div>

    <!-- 右侧主内容 -->
    <div class="about-main">
      <h1 class="about-name">Yao Xiong</h1>
      <p class="introp">
        I am a postdoctoral researcher at the University of California, Santa Barbara, working in the group of Prof. Glenn Fredrickson. 
        My research focuses on multiscale modeling and simulation of active and responsive soft matter systems. I employ approaches such as
        dissipative particle dynamics (DPD), field-theoretic simulations (FTS), and finite element methods (FEM) to investigate a wide
        range of thermodynamic and dynamic phenomena in polymers, gels, and biomaterials. I am passionate about advancing computational
        frameworks that bridge molecular, mesoscopic, and continuum scales to uncover new design principles for soft materials.
        Feel free to reach out—I’m always happy to connect and discuss science!
      </p>

      <h2 class="section-title">Education</h2>
      <div class="edu">
        <!-- 按需修改条目 -->
        <div class="edu-item"><span class="edu-year">2022</span> Ph.D., Materials Science and Engineering — Clemson University</div>
        <div class="edu-item"><span class="edu-year">2016</span> M.S., Materials Science and Engineering — University of Florida</div>
        <div class="edu-item"><span class="edu-year">2014</span> B.E., Composite Materials Engineering — Wuhan University of Technology</div>
      </div>

      <a class="view-cv" href="{{ '/assets/cv/Yao_Xiong_CV.pdf' | relative_url }}" target="_blank" rel="noopener">View Full CV</a>
    </div>
  </div>
</div>
