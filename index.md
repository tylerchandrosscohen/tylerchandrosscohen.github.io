---
layout: default
title: Home
---

<style>
/* --- page-wide tweaks --- */
.home-wrap{
  max-width: 1100px;
  margin: 0 auto;
  padding: 2.2rem 1.2rem 2.8rem;
}

/* --- HERO --- */
.hero{
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 2.6rem;
  align-items: center;
}

@media (max-width: 900px){
  .hero{ grid-template-columns: 1fr; }
}

/* name + tagline */
.hero-text h1{
  margin: 0 0 0.6rem 0;
  font-family: Georgia, "Times New Roman", serif;
  font-size: 2.6rem;
  line-height: 1.1;

  white-space: nowrap;
  hyphens: none;
  overflow-wrap: normal;
  word-break: keep-all;
}

.hero-text p{
  margin: 0.4rem 0 0 0;
  font-size: 1.1rem;
  line-height: 1.55;
  color: rgba(0,0,0,0.78);
  max-width: 60ch;
}

/* photo */
.hero-photo{
  width: 100%;
  max-width: 620px;
  border-radius: 18px;
  overflow: hidden;
  box-shadow: 0 16px 40px rgba(0,0,0,0.22);
  border: 1px solid rgba(0,0,0,0.08);
}

.hero-photo img{
  width: 100%;
  height: auto;
  display: block;
}

/* social bar */
.social-bar{
  background: #f4ead5;
  border-radius: 10px;
  padding: 1.1rem 1.2rem;
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 1.2rem;
  border: 1px solid rgba(0,0,0,0.06);
}

.icon-row{
  display:flex;
  gap: 0.9rem;
  align-items:center;
}

.icon-btn{
  width: 54px;
  height: 54px;
  border-radius: 12px;
  display:flex;
  align-items:center;
  justify-content:center;
  text-decoration:none;
  box-shadow: 0 10px 22px rgba(0,0,0,0.12);
  transition: transform 120ms ease, box-shadow 120ms ease;
}
.icon-btn:hover{
  transform: translateY(-2px);
  box-shadow: 0 14px 28px rgba(0,0,0,0.16);
}
.icon-btn svg{ width: 30px; height: 30px; }

.ig{ background: #ff2ea6; }
.tw{ background: #5fb7ff; }
.li{ background: #0a66c2; }
.icon-btn svg path{ fill: white; }

.email-btn{
  background: #000;
  color: #fff;
  padding: 1rem 2.4rem;
  border-radius: 10px;
  text-decoration:none;
  font-size: 1.35rem;
  font-family: Georgia, "Times New Roman", serif;
  box-shadow: 0 12px 26px rgba(0,0,0,0.18);
  transition: transform 120ms ease, box-shadow 120ms ease;
  white-space: nowrap;
}
.email-btn:hover{
  transform: translateY(-2px);
  box-shadow: 0 16px 34px rgba(0,0,0,0.22);
}

/* --- BIO --- */
.bio{
  margin-top: 2.6rem;
  background: #ffffff;
  border-radius: 12px;
  padding: 1.7rem 1.6rem;
  border: 1px solid rgba(0,0,0,0.06);
  box-shadow: 0 10px 26px rgba(0,0,0,0.08);
}

.bio h2{
  margin: 0 0 0.9rem 0;
  font-family: Georgia, "Times New Roman", serif;
  font-size: 2.0rem;
}
.bio p{
  margin: 0.7rem 0;
  font-size: 1.06rem;
  line-height: 1.65;
  color: rgba(0,0,0,0.82);
}

/* --- PHOTO STRIP --- */
.photo-strip{
  margin-top: 2.8rem;
}

.photo-grid{
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 1.4rem;
}

@media (max-width: 1000px){
  .photo-grid{ grid-template-columns: 1fr 1fr; }
}
@media (max-width: 600px){
  .photo-grid{ grid-template-columns: 1fr; }
}

.photo-card{
  background: #ffffff;
  border-radius: 14px;
  overflow: hidden;
  border: 1px solid rgba(0,0,0,0.06);
  box-shadow: 0 10px 24px rgba(0,0,0,0.10);
}

.photo-card img{
  width: 100%;
  height: auto;
  display: block;
}

.photo-caption{
  padding: 0.75rem 0.9rem;
  font-size: 0.95rem;
  line-height: 1.4;
  color: rgba(0,0,0,0.80);
  background: #f9f6ef;
}
</style>

<div class="home-wrap">

  <div class="hero">

    <div class="hero-text">
      <h1>Tyler Chandross&#8209;Cohen</h1>
      <p>
        Food microbiology researcher with a strong record of conducting interdisciplinary research at the interface of microbial genomics, molecular biology, and food safety. My work centers on the foodborne pathogen <em>Bacillus cereus</em>, with a particular focus on how genetic diversity and environmental conditions govern virulence expression and cytotoxic potential across diverse isolates, including psychrotolerant strains relevant to refrigerated foods.
      </p>

      <div style="height:1.2rem"></div>

      <div class="social-bar">
        <div class="icon-row">
          <a class="icon-btn ig" href="https://www.instagram.com/tyler.cc_/" target="_blank" rel="noopener"></a>
          <a class="icon-btn tw" href="https://x.com/tyler_cc_" target="_blank" rel="noopener"></a>
          <a class="icon-btn li" href="https://www.linkedin.com/in/tscc/" target="_blank" rel="noopener"></a>
        </div>
        <a class="email-btn" href="mailto:tfc5209@psu.edu">Email Me!</a>
      </div>
    </div>

    <div style="display:flex; justify-content:center;">
      <div class="hero-photo">
        <img src="/assets/img/tyler.jpg" alt="Photo of Tyler Chandross-Cohen">
      </div>
    </div>

  </div>

  <!-- BIO -->
  <div class="bio">
    <h2>Biography</h2>

    <p>
      As a food scientist, I am continually reminded of the integral role that microscopic organisms play in our food system. Understanding how these organisms survive, grow, and interact within food environments is essential for protecting public health and preserving the nutritional quality of foods.
    </p>

    <p>
      During my undergraduate studies, I became fascinated with food microbiology and food safety. I began working with <em>Listeria monocytogenes</em> to understand how it persists within biofilms formed alongside other microorganisms, and to evaluate whether antilisterial cultures could reduce <em>L. monocytogenes</em> loads in food-associated environments.
    </p>

    <p>
      During my graduate studies, I shifted my focus to the foodborne pathogen <em>Bacillus cereus</em>. I have contributed to projects evaluating growth dynamics in high-temperature short-time (HTST) milk to inform exposure assessment models for industry use. My thesis research, funded by a USDA NIFA predoctoral fellowship, centers on using targeted gene knockouts to better understand enterotoxin-mediated virulence potential, with particular emphasis on the role of the enterotoxin hemolysin BL in surface colonization and biofilm formation.
    </p>

    <p>
      My long-term career goal is to advance strategies for controlling foodborne pathogens and to contribute to the development of a safe, sustainable, and wholesome food supply.
    </p>
  </div>

  <!-- PHOTO STRIP -->
  <div class="photo-strip">
    <div class="photo-grid">

      <div class="photo-card">
        <img src="/assets/img/photo1.jpg" alt="Receiving the IAFP Student Travel Scholarship in 2024">
        <div class="photo-caption">
          Receiving the IAFP Student Travel Scholarship in 2024 in Long Beach, California.
        </div>
      </div>

      <div class="photo-card">
        <img src="/assets/img/photo2.jpg" alt="Working in the lab">
        <div class="photo-caption">
          Working in the lab!
        </div>
      </div>

      <div class="photo-card">
        <img src="/assets/img/photo3.jpg" alt="Kovac Lab out for dinner">
        <div class="photo-caption">
          Kovac Lab out for dinner.
        </div>
      </div>

      <div class="photo-card">
        <img src="/assets/img/photo4.jpg" alt="Tyler Chandross-Cohen and his mom Karen Chandross">
        <div class="photo-caption">
          My mom (Karen Chandross) and I (Scientist!).
        </div>
      </div>

    </div>
  </div>

</div>
