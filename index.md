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
  font-size: clamp(2.2rem, 3.2vw, 3.0rem);
  line-height: 1.05;

  /* prevent breaking */
  white-space: nowrap;
  hyphens: none;
  overflow-wrap: normal;
  word-break: keep-all;
}

@media (max-width: 520px){
  .hero-text h1{ white-space: normal; }
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
  max-width: 720px;
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

/* top bar like your screenshot */
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

@media (max-width: 520px){
  .social-bar{
    flex-direction: column;
    align-items: flex-start;
  }
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
  letter-spacing: 0.2px;
  box-shadow: 0 12px 26px rgba(0,0,0,0.18);
  transition: transform 120ms ease, box-shadow 120ms ease;
  white-space: nowrap;
}
.email-btn:hover{
  transform: translateY(-2px);
  box-shadow: 0 16px 34px rgba(0,0,0,0.22);
}

/* --- BIO (wider) --- */
.bio{
  margin: 3.2rem auto 0;
  max-width: 1250px;          /* wider */
  background: #ffffff;
  border-radius: 14px;
  padding: 2.2rem 2.4rem;     /* more breathing room */
  border: 1px solid rgba(0,0,0,0.06);
  box-shadow: 0 12px 30px rgba(0,0,0,0.08);
}

.bio h2{
  margin: 0 0 1.1rem 0;
  font-family: Georgia, "Times New Roman", serif;
  font-size: 2.1rem;
}

.bio p{
  margin: 0.9rem 0;
  font-size: 1.08rem;
  line-height: 1.7;
  color: rgba(0,0,0,0.82);
  max-width: 85ch;            /* readable line length */
}

/* --- PHOTO GRID: locked 2x2 --- */
.photo-grid{
  margin-top: 2.2rem;
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 1.6rem;
}

@media (max-width: 900px){
  .photo-grid{ grid-template-columns: 1fr; }
}

.photo-card{
  background: #ffffff;
  border-radius: 18px;
  overflow: hidden;
  border: 1px solid rgba(0,0,0,0.06);
  box-shadow: 0 14px 32px rgba(0,0,0,0.12);
}

/* Fixed image height: consistent, no whitespace */
.photo-img{
  width: 100%;
  height: 420px;
  overflow: hidden;
  cursor: zoom-in; /* indicates click-to-zoom */
}

.photo-img img{
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
}

.photo-cap{
  background: #f7f0e1;
  padding: 1rem 1.1rem;
  font-size: 1.05rem;
  line-height: 1.35;
  color: rgba(0,0,0,0.85);
}

/* --- LIGHTBOX --- */
.lightbox{
  position: fixed;
  inset: 0;
  background: rgba(0,0,0,0.85);
  display: none;
  align-items: center;
  justify-content: center;
  z-index: 9999;
  padding: 2rem;
}

.lightbox.active{
  display: flex;
}

.lightbox img{
  max-width: 95%;
  max-height: 90vh;
  border-radius: 12px;
  box-shadow: 0 24px 60px rgba(0,0,0,0.6);
}
</style>

<div class="home-wrap">

  <div class="hero">

    <!-- LEFT: text + social bar -->
    <div class="hero-text">
      <h1>Tyler Chandross&#8209;Cohen</h1>

      <p>
        Food microbiology researcher with a strong record of conducting interdisciplinary research at the interface of microbial genomics, molecular biology, and food safety. My work centers on the foodborne pathogen <em>Bacillus cereus</em>, with a particular focus on how genetic diversity and environmental conditions govern virulence expression and cytotoxic potential across diverse isolates, including psychrotolerant strains relevant to refrigerated foods.
      </p>

      <div style="height:1.2rem"></div>

      <div class="social-bar">
        <div class="icon-row">

          <!-- Instagram -->
          <a class="icon-btn ig" href="https://www.instagram.com/tyler.cc_/" target="_blank" rel="noopener" aria-label="Instagram">
            <svg viewBox="0 0 24 24" aria-hidden="true">
              <path d="M7 2h10a5 5 0 0 1 5 5v10a5 5 0 0 1-5 5H7a5 5 0 0 1-5-5V7a5 5 0 0 1 5-5zm10 2H7a3 3 0 0 0-3 3v10a3 3 0 0 0 3 3h10a3 3 0 0 0 3-3V7a3 3 0 0 0-3-3zm-5 4a5 5 0 1 1 0 10 5 5 0 0 1 0-10zm0 2a3 3 0 1 0 0 6 3 3 0 0 0 0-6zm5.6-.9a1.1 1.1 0 1 1-2.2 0 1.1 1.1 0 0 1 2.2 0z"/>
            </svg>
          </a>

          <!-- X / Twitter -->
          <a class="icon-btn tw" href="https://x.com/tyler_cc_" target="_blank" rel="noopener" aria-label="X / Twitter">
            <svg viewBox="0 0 24 24" aria-hidden="true">
              <path d="M18.9 2H22l-6.8 7.8L23.2 22h-6.5l-5.1-6.6L5.7 22H2.6l7.3-8.4L1 2h6.7l4.6 6L18.9 2zm-1.1 18h1.8L6.7 3.9H4.8L17.8 20z"/>
            </svg>
          </a>

          <!-- LinkedIn -->
          <a class="icon-btn li" href="https://www.linkedin.com/in/tscc/" target="_blank" rel="noopener" aria-label="LinkedIn">
            <svg viewBox="0 0 24 24" aria-hidden="true">
              <path d="M4.98 3.5A2.48 2.48 0 1 1 5 8.46a2.48 2.48 0 0 1-.02-4.96zM3 21h4V9H3v12zm7 0h4v-6.3c0-1.7.3-3.3 2.4-3.3 2.1 0 2.1 1.9 2.1 3.4V21h4v-7c0-3.4-.7-6-4.7-6-1.9 0-3.2 1-3.7 2h-.1V9h-3.8v12z"/>
            </svg>
          </a>

        </div>

        <a class="email-btn" href="mailto:tfc5209@psu.edu">Email Me!</a>
      </div>
    </div>

    <!-- RIGHT: your photo -->
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

    <!-- PHOTO GRID -->
    <div class="photo-grid">

      <figure class="photo-card">
        <div class="photo-img" data-full="/assets/img/photo1.jpg">
          <img src="/assets/img/photo1.jpg" alt="Receiving the IAFP Student Travel Scholarship in 2024 in Long Beach, California">
        </div>
        <figcaption class="photo-cap">
          Receiving the IAFP Student Travel Scholarship in 2024 in Long Beach, California.
        </figcaption>
      </figure>

      <figure class="photo-card">
        <div class="photo-img" data-full="/assets/img/photo2.jpg">
          <img src="/assets/img/photo2.jpg" alt="Working in the lab">
        </div>
        <figcaption class="photo-cap">
          Working in the lab!
        </figcaption>
      </figure>

      <figure class="photo-card">
        <div class="photo-img" data-full="/assets/img/photo3.jpg">
          <img src="/assets/img/photo3.jpg" alt="Kovac Lab out for dinner">
        </div>
        <figcaption class="photo-cap">
          Kovac Lab out for dinner.
        </figcaption>
      </figure>

      <figure class="photo-card">
        <div class="photo-img" data-full="/assets/img/photo4.jpg">
          <img src="/assets/img/photo4.jpg" alt="My mom (Karen Chandross) and I (Scientist!)">
        </div>
        <figcaption class="photo-cap">
          My mom (Dr. Karen Chandross) and I.
        </figcaption>
      </figure>

    </div>

  </div>

</div>

<!-- LIGHTBOX (click photos to enlarge) -->
<div class="lightbox" id="lightbox" aria-hidden="true">
  <img src="" alt="Expanded photo">
</div>

<script>
  const lightbox = document.getElementById('lightbox');
  const lightboxImg = lightbox.querySelector('img');

  document.querySelectorAll('.photo-img').forEach(item => {
    item.addEventListener('click', () => {
      const fullSrc = item.getAttribute('data-full');
      lightboxImg.src = fullSrc;
      lightbox.classList.add('active');
      lightbox.setAttribute('aria-hidden', 'false');
    });
  });

  function closeLightbox(){
    lightbox.classList.remove('active');
    lightboxImg.src = '';
    lightbox.setAttribute('aria-hidden', 'true');
  }

  lightbox.addEventListener('click', closeLightbox);

  document.addEventListener('keydown', (e) => {
    if (e.key === 'Escape') closeLightbox();
  });
</script>
