---
layout: bare
title: About Sao Win
section: about
description: "About Dr Sao Win, founder of Win Laboratories, and how this archive preserves the record."
---

<!-- Page Header -->
<h1>About Sao Win</h1>
<p><em>Placeholder: a short, sourced introduction to Dr Sao Win will go here.</em></p>

{% include section-list.html %}

<!-- Key Figures -->
<h2 id="key-figures">Key Figures</h2>

<section class="about-people">
  <article class="person-card">
    <!-- Portrait placeholder: add assets/about/sao-win.png (credited) and uncomment.
    <img src="/assets/about/sao-win.png" alt="Portrait of Dr Sao Win" loading="lazy">
    -->
    <div class="person-body">
      <h3>Dr Sao Win <span class="role">Founder</span></h3>
      <p><strong>[Placeholder: biography to be added from sourced material.]</strong></p>
      <!--
      <ul class="highlights">
        <li>Sourced highlight.</li>
      </ul>
      -->
    </div>
  </article>
</section>

<!-- Legacy -->
<section id="legacy" class="about-card">
  <h2>Legacy and Preservation</h2>
  <p>This <strong>Win Laboratories Archive</strong> exists to preserve the technical, visual and historical record of the company’s work. <em>Placeholder: more detail to follow.</em></p>
</section>

<!-- Sources -->
<h2>Sources and Acknowledgements</h2>
<ul>
  <li><em>Placeholder: sources will be listed here as material is added.</em></li>
  <li>Leads and source checks are logged in the <a href="/research-notes/">Research Notes</a>.</li>
</ul>

<p><a href="https://win-laboratories.github.io">Return to Archive Home</a></p>

<style>
  :root{
    --paper:#f7f5ee;
    --ink:#111;
    --muted:#666;
    --card:#fff;
    --border:#e5dfc9;
    --shadow:0 6px 24px rgba(0,0,0,.06);
    --radius:14px;
    --gap:18px;
    --wrap:1100px;
    --accent:#6e9fff; 
    --avatar:150px;   /* desktop/tablet portrait width */
  }

  body{color:var(--ink)}
  h1{margin:.2em 0 .6em}
  h2{margin:1.2em 0 .6em}

  /* Container */
  main, .page-content, body > div, body > section{
    max-width:var(--wrap);
    margin-inline:auto;
    padding-inline:14px;
  }

  /* Key figures: grid on larger screens */
  .about-people{
    display:grid;
    grid-template-columns:1fr;
    gap:14px;
    margin:1rem 0 2rem;
  }
  .person-card{
    display:grid;
    grid-template-columns: var(--avatar) 1fr;
    gap:14px;
    align-items:start;
    background:var(--paper);
    border:1px solid var(--border);
    border-radius:var(--radius);
    box-shadow:var(--shadow);
    padding:12px;
  }
  .person-card img{
    width:100%;
    max-width:var(--avatar);
    height:auto;
    border-radius:12px;
    display:block;
    object-fit:cover;
  }
  .person-body h3{ margin:.1rem 0 .4rem; font-size:1.05rem; }
  .role{
    display:inline-block; margin-left:.4rem; font-size:.84rem; font-weight:600;
    color:#0b1b3a; background:#e9f0ff; border:1px solid #d6e3ff;
    padding:.15rem .45rem; border-radius:999px;
  }
  .highlights{ margin:.4rem 0 0 1rem; }
  .highlights li{ margin:.25rem 0; }

  /* --- Mobile full-width portrait layout --- */
  @media (max-width:640px){
    .person-card{
      display:block;           /* stack */
      padding:0;
    }
    .person-card img{
      width:100%;
      max-width:none;
      border-radius:14px 14px 0 0; /* rounded top */
      margin:0;
      display:block;
    }
    .person-body{
      padding:1rem 1rem 1.2rem;
      text-align:left;
    }
    .person-body h3{ text-align:center; }
    .person-body .role{
      display:block; margin:.3rem auto .8rem; text-align:center;
    }
  }
  /* Larger portraits on very wide screens */
  @media (min-width:1100px){ :root{ --avatar:180px; } }

  /* Content cards */
  .about-card{
    background:var(--card);
    border:1px solid var(--border);
    border-radius:var(--radius);
    box-shadow:var(--shadow);
    padding:clamp(1rem, 2vw, 1.4rem);
    margin:1.4rem 0;
  }

  /* Split layout */
  .split{
    display:grid;
    grid-template-columns:1.1fr 1.4fr;
    gap:var(--gap);
    align-items:start;
  }
  .split.reverse{ grid-template-columns:1.4fr 1.1fr; }
  @media (max-width:860px){
    .split, .split.reverse{ grid-template-columns:1fr; }
  }

  .media{ margin:0; }
  .media img{
    display:block; width:100%; height:auto;
    border-radius:12px; box-shadow:0 8px 28px rgba(0,0,0,.10);
  }
  .media figcaption{ font-size:.9rem; color:var(--muted); margin-top:.45rem; }

  .copy p{ line-height:1.6; }
  .copy em{ color:#333; }

  blockquote{
    margin:1rem 0; padding:.8rem 1rem;
    border-left:4px solid var(--accent);
    background:#f0f6ff; border-radius:10px;
  }
</style>
