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
  }
  .about-wrap{
    display:flex; gap:28px; align-items:flex-start;
    margin: 0 0 2.5rem 0;
    flex-wrap:wrap;                   
  }
  .about-photo{
    width:260px; max-width:100%;
  }
  .about-photo img{
    width:100%; height:auto; display:block;
    border-radius:14px;
    box-shadow:0 6px 18px rgba(0,0,0,.08);
  }
  .about-main{ flex:1 1 420px; min-width:320px; }
  .about-name{ font-size:1.8rem; font-weight:700; margin:.25rem 0 0.75rem; }
  .introp{ font-size:1.3rem; line-height:1.3; color:var(--text); max-width:72ch; text-align: justify;}
  
  /* Education 样式 */
  .section-title{ 
    font-size:1.3rem; 
    letter-spacing:.02em; 
    margin:1.75rem 0 .75rem; 
    font-weight:700; 
  }
  .edu{
    max-width: 72ch; 
    margin-top: 0.5rem;
    padding-left:0; /* 去掉缩进 */
  }
  .edu-item{ 
    margin: .6rem 0 .6rem; 
    color:var(--text); 
    padding-left:0; 
    font-size:1.1rem; /* 每一项的字体大小 */
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
      <div class="edu">
        <div class="edu-item"><span class="edu-year">2022</span> Ph.D., Materials Science and Engineering — Clemson University</div>
        <div class="edu-item"><span class="edu-year">2016</span> M.S., Materials Science and Engineering — University of Florida</div>
        <div class="edu-item"><span class="edu-year">2014</span> B.E., Composite Materials Engineering — Wuhan University of Technology</div>
      </div>

      <a class="view-cv" href="{{ '/assets/cv/Yao_Xiong_CV.pdf' | relative_url }}" target="_blank" rel="noopener">View Full CV</a>
    </div>
  </div>
</div>
