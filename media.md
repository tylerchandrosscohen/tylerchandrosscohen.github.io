---
layout: default
title: Media
permalink: /media/
---

<style>
.media-wrap{
  max-width: 1100px;
  margin: 0 auto;
  padding: 2.2rem 1.2rem 2.8rem;
}

.media-wrap h1{
  margin: 0 0 0.6rem 0;
  font-family: Georgia, "Times New Roman", serif;
  font-size: 3rem;
  line-height: 1.1;
}

.media-wrap p{
  max-width: 70ch;
  font-size: 1.1rem;
  line-height: 1.6;
  color: rgba(0,0,0,0.8);
}

/* Media card */
.media-card{
  margin-top: 2.2rem;
  background: #ffffff;
  border-radius: 16px;
  border: 1px solid rgba(0,0,0,0.08);
  box-shadow: 0 14px 32px rgba(0,0,0,0.10);
  overflow: hidden;
}

/* Header */
.media-header{
  padding: 1.1rem 1.4rem;
  background: #f4ead5;
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 1rem;
}

.media-header h2{
  margin: 0;
  font-family: Georgia, "Times New Roman", serif;
  font-size: 1.6rem;
  line-height: 1.2;
}

.media-header a{
  text-decoration: none;
  background: #000;
  color: #fff;
  padding: 0.55rem 1.2rem;
  border-radius: 8px;
  font-size: 0.95rem;
  white-space: nowrap;
  box-shadow: 0 8px 18px rgba(0,0,0,0.15);
  transition: transform 120ms ease, box-shadow 120ms ease;
}

.media-header a:hover{
  transform: translateY(-2px);
  box-shadow: 0 12px 26px rgba(0,0,0,0.22);
}

/* iframe wrapper */
.media-frame{
  width: 100%;
  height: 75vh; /* scrollable window */
  border: none;
}

/* fallback */
.media-fallback{
  padding: 1rem 1.4rem;
  background: #faf6ee;
  font-size: 1rem;
}
</style>

<div class="media-wrap">
  <h1>Media</h1>

  <p>
    Selected media coverage highlighting my research on foodborne pathogens,
    detection strategies, and food safety risk assessment.
  </p>

  <!-- RAPID MICROBIOLOGY ARTICLE -->
  <div class="media-card">
    <div class="media-header">
      <h2>
        New enrichment broth finds <em>Bacillus cereus</em> in half of powdered infant foods sampled
      </h2>
      <a href="https://www.rapidmicrobiology.com/journal-club/new-enrichment-broth-finds-b-cereus-in-half-of-powdered-infant-foods-sampled"
         target="_blank" rel="noopener">
        Read on Rapid Microbiology →
      </a>
    </div>

    <iframe
      class="media-frame"
      src="https://www.rapidmicrobiology.com/journal-club/new-enrichment-broth-finds-b-cereus-in-half-of-powdered-infant-foods-sampled"
      title="Rapid Microbiology Journal Club article on Bacillus cereus in powdered infant foods"
      loading="lazy">
    </iframe>

    <div class="media-fallback">
      If the article does not load due to browser or privacy settings,
      <a href="https://www.rapidmicrobiology.com/journal-club/new-enrichment-broth-finds-b-cereus-in-half-of-powdered-infant-foods-sampled"
         target="_blank" rel="noopener">
        click here to view it directly on Rapid Microbiology.
      </a>
    </div>
  </div>

  <!-- PENN STATE ARTICLE -->
  <div class="media-card">
    <div class="media-header">
      <h2>
        Researchers develop model to guide milk processors’ food safety decisions
      </h2>
      <a href="https://www.psu.edu/news/research/story/researchers-develop-model-guide-milk-processors-food-safety-decisions/"
         target="_blank" rel="noopener">
        Read on Penn State News →
      </a>
    </div>

    <iframe
      class="media-frame"
      src="https://www.psu.edu/news/research/story/researchers-develop-model-guide-milk-processors-food-safety-decisions/"
      title="Penn State News article on milk safety modeling"
      loading="lazy">
    </iframe>

    <div class="media-fallback">
      If the article does not load due to browser or privacy settings,
      <a href="https://www.psu.edu/news/research/story/researchers-develop-model-guide-milk-processors-food-safety-decisions/"
         target="_blank" rel="noopener">
        click here to view it directly on Penn State News.
      </a>
    </div>
  </div>

</div>
