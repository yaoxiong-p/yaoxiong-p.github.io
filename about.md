---
layout: default
title: About Yao Xiong
---

<style>
  :root{
    --accent: seagreen;
    --text: #222;
    --muted: #666;
    --bg-soft: #f6f8f8;

    /* 统一控制 bullet 与文本对齐的缩进变量 */
    --bullet-size: 10px;   /* 圆点直径 */
    --bullet-gap: 0.6rem;  /* 圆点与文字间距 */
  }

  .about-wrap{
    display:flex; gap:28px; align-items:flex-start;
    margin: 0 0 2.5rem 0;
    flex-wrap:wrap;
  }
  .about-photo{
    width:260px; max-width:100%;
    align-self: center;            /* 头像对齐到右侧内容的中部 */
  }
  .about-photo img{
    width:100%; height:auto; display:block;
    border-radius:14px;
    box-shadow:0 6px 18px rgba(0,0,0,.08);
  }

  .about-main{ flex:1 1 420px; min-width:320px; }
  .about-name{ font-size:1.8rem; font-weight:700; margin:.25rem 0 0.75rem; }
  .introp{ font-size:1.3rem; line-height:1.5; color:var(--text); max-width:72ch; text-align: justify;}

  /* ---------- Education ---------- */
  .section-title{
    font-size:1.3rem;              /* 标题 1.3rem */
    letter-spacing:.02em;
    margin:1.75rem 0 .75rem;
    font-weight:700;
  }

  /* 列表容器，仅控制最大宽度与外边距 */
  .edu{
    max-width:72ch;
    margin:.5rem 0 0 0;
    padding:0;
    list-style:none;
  }

  .edu-item{
    font-size:1.1rem;              /* 每项 1.1rem */
    color:var(--text);
    line-height:1.45;
    margin:.6rem 0;
    display:flex;                  /* 用 flex 让圆点与文本自然对齐 */
    align-items:flex-start;
  }
  .edu-item::before{
    content:"";
    width:var(--bullet-size); height:var(--bullet-size);
    border-radius:50%;
    background: var(--accent);
    flex: 0 0 var(--bullet-size);
    margin-right: var(--bullet-gap);
    margin-top: .5em;              /* 让圆点大致落在首行的中线上，可微调 */
    box-shadow: 0 0 0 3px rgba(46,139,87,.15);
  }
  .edu-year{ font-weight:700; margin-right:.4rem; }

  /* 让“View Full CV”与列表文本左边界对齐：左侧缩进 = 圆点宽度 + 间距 */
  .view-cv{
    display:block;
    margin-top: 0.1rem;
    margin-left: 8rem;
    font-size: 1.3rem;             /* 与 Education 标题一致 */
    font-weight: 700;
    color: var(--accent);
    text-decoration: none;
    border-bottom: 2px solid transparent;
    width: fit-content;
  }
  .view-cv:hover{ border-color: var(--accent); }

  /* 小屏时堆叠，让头像从顶部开始以免过度居中 */
  @media (max-width: 768px){
    .about-photo{ align-self: flex-start; }
  }
</style>

<div class="post">
  <div class="about-wrap">
    <!-- 左侧头像 -->
    <div class="about-photo">
      <img src="{{ '/assets/img/Yao Xiong_headshot_Transp.jpg' | relative_url }}" alt="Yao Xiong headshot">
    </div>

    <!-- 右侧主内容 -->
    <div class="about-main">
      <h1 class="about-name">Yao Xiong</h1>
      <p class="introp">
        I am currently a postdoctoral researcher in Prof. Glenn Fredrickson’s group at UC Santa Barbara and previously worked with Prof. Monica Olvera de la Cruz at Northwestern University, after earning my Ph.D. in Materials Science and Engineering from Clemson University under the guidance of Prof. Olga Kuksenok. My research focuses on multiscale modeling and simulation of active and responsive soft matter systems. I employ approaches such as dissipative particle dynamics (DPD), field-theoretic simulations (FTS), and finite element methods (FEM) to investigate a wide range of thermodynamic and dynamic phenomena in polymers, gels, and biomaterials. I am passionate about advancing computational frameworks that bridge molecular, mesoscopic, and continuum scales to uncover new design principles for soft materials. Feel free to reach out—I’m always happy to connect and discuss science!
      </p>

      <h2 class="section-title">Education</h2>
      <ul class="edu">
        <li class="edu-item"><span class="edu-year">2022</span> Ph.D., Materials Science and Engineering — Clemson University</li>
        <li class="edu-item"><span class="edu-year">2016</span> M.S., Materials Science and Engineering — University of Florida</li>
        <li class="edu-item"><span class="edu-year">2014</span> B.E., Composite Materials Engineering — Wuhan University of Technology</li>
      </ul>

      <a class="view-cv" href="{{ '/assets/img/ToC/CV_YX_Sep2025.pdf' | relative_url }}" target="_blank" rel="noopener">View Full CV</a>
    </div>
  </div>
</div>
