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
  grid-template-columns: 1.1fr 0.9fr;
  gap: 2.2rem;
  align-items: center;
}

@media (max-width: 900px){
  .hero{ grid-template-columns: 1fr; }
}

/* photo */
.hero-photo{
  width: 100%;
  max-width: 620px;   /* ⬅ bigger */
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
  background: #f4ead5;           /* warm tan like your screenshot */
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

/* brand-ish colors */
.ig{ background: #ff2ea6; }      /* instagram pink */
.tw{ background: #5fb7ff; }      /* twitter/x light blue */
.li{ background: #0a66c2; }      /* linkedin */
.icon-btn svg path{ fill: white; }

/* Email button */
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

/* name + tagline */
.hero-text h1{
  margin: 0 0 0.6rem 0;
  font-family: Georgia, "Times New Roman", serif;
  font-size: 2.6rem;
  line-height: 1.1;
}
.hero-text p{
  margin: 0.4rem 0 0 0;
  font-size: 1.1rem;
  line-height: 1.55;
  color: rgba(0,0,0,0.78);
  max-width: 60ch;
}

/* --- BIO SECTION --- */
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
.bio .quick{
  margin-top: 1.0rem;
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 0.8rem 1.2rem;
}
@media (max-width: 700px){
  .bio .quick{ grid-template-columns: 1fr; }
}
.bio .chip{
  background: #f4ead5;
  border: 1px solid rgba(0,0,0,0.06);
  padding: 0.65rem 0.8rem;
  border-radius: 10px;
  font-size: 0.98rem;
}
</style>

<div class="home-wrap">

  <div class="hero">

    <!-- LEFT: text + social bar -->
    <div class="hero-text">
      <h1>Tyler Chandross-Cohen</h1>
      <p>
        Food microbiologist focused on <em>Bacillus cereus</em> ecology and virulence, integrating whole-genome sequencing,
        quantitative models, and experimental microbiology to improve food safety risk assessment.
      </p>

      <div style="height:1.2rem"></div>

      <div class="social-bar">
        <div class="icon-row">

          <!-- Instagram -->
          <a class="icon-btn ig" href="REPLACE_INSTAGRAM_LINK" target="_blank" rel="noopener" aria-label="Instagram">
            <svg viewBox="0 0 24 24" aria-hidden="true">
              <path d="M7 2h10a5 5 0 0 1 5 5v10a5 5 0 0 1-5 5H7a5 5 0 0 1-5-5V7a5 5 0 0 1 5-5zm10 2H7a3 3 0 0 0-3 3v10a3 3 0 0 0 3 3h10a3 3 0 0 0 3-3V7a3 3 0 0 0-3-3zm-5 4a5 5 0 1 1 0 10 5 5 0 0 1 0-10zm0 2a3 3 0 1 0 0 6 3 3 0 0 0 0-6zm5.6-.9a1.1 1.1 0 1 1-2.2 0 1.1 1.1 0 0 1 2.2 0z"/>
            </svg>
          </a>

          <!-- X / Twitter -->
          <a class="icon-btn tw" href="REPLACE_TWITTER_LINK" target="_blank" rel="noopener" aria-label="X / Twitter">
            <svg viewBox="0 0 24 24" aria-hidden="true">
              <path d="M18.9 2H22l-6.8 7.8L23.2 22h-6.5l-5.1-6.6L5.7 22H2.6l7.3-8.4L1 2h6.7l4.6 6L18.9 2zm-1.1 18h1.8L6.7 3.9H4.8L17.8 20z"/>
            </svg>
          </a>

          <!-- LinkedIn -->
          <a class="icon-btn li" href="REPLACE_LINKEDIN_LINK" target="_blank" rel="noopener" aria-label="LinkedIn">
            <svg viewBox="0 0 24 24" aria-hidden="true">
              <path d="M4.98 3.5A2.48 2.48 0 1 1 5 8.46a2.48 2.48 0 0 1-.02-4.96zM3 21h4V9H3v12zm7 0h4v-6.3c0-1.7.3-3.3 2.4-3.3 2.1 0 2.1 1.9 2.1 3.4V21h4v-7c0-3.4-.7-6-4.7-6-1.9 0-3.2 1-3.7 2h-.1V9h-3.8v12z"/>
            </svg>
          </a>

        </div>

        <!-- Email button -->
        <a class="email-btn" href="mailto:REPLACE_YOUR_EMAIL">Email Me!</a>
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
     As a food scientist, I am constantly reminded of the integral role that microscopic organisms play in our food system. Understanding how these organisms can survive and grow in our food system is crucial to protect the safety and well-being of our population and the nutritive value of food. 
   </p>
During my undergraduate studies, I became fascinated with the field of food microbiology and food safety. I began working with Listeria monocytogenes, to understand how it can persist in biofilms with other microorganisms, and if anti-listerial cultures could reduce the
L. monocytogenes load.
  </p>
During my graduate studies, I shifted my focus to investigate the foodborne pathogen Bacillus cereus. I have worked on projects evaluating growth in HTST milk, to develop an exposure assessment model for industry use, and my thesis research involves using gene knockouts to better understand enterotoxin-mediated virulence potential and the role of an enterotoxin, Hemolysin BL, in surface colonization and biofilm formation.
  </p>
My career goal is to advance the control of foodborne pathogens and contribute to the development of safe, sustainable, and wholesome food for all.
  </p>

    <div class="quick">
      <div class="chip"><strong>Research themes:</strong> B. cereus virulence • psychrotolerance • surface colonization • toxin stability</div>
      <div class="chip"><strong>Methods:</strong> WGS (Illumina/Nanopore) • phylogenomics • RT-qPCR • cytotoxicity assays • modeling</div>
      <div class="chip"><strong>Interests:</strong> precision food safety • outbreak prevention • microbial ecology</div>
      <div class="chip"><strong>Links:</strong> CV • Publications • Posters • Contact</div>
    </div>
  </div>

</div>
