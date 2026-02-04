---
layout: default
title: CV
permalink: /cv/
---

<style>
.cv-wrap{
  max-width: 1100px;
  margin: 0 auto;
  padding: 2.2rem 1.2rem 2.8rem;
}

.cv-header{
  display:flex;
  align-items: flex-end;
  justify-content: space-between;
  gap: 1rem;
  flex-wrap: wrap;
  margin-bottom: 1.2rem;
}

.cv-header h1{
  margin: 0;
  font-family: Georgia, "Times New Roman", serif;
  font-size: 2.4rem;
}

.cv-links{
  display:flex;
  gap: 0.7rem;
  flex-wrap: wrap;
}

.cv-btn{
  display:inline-block;
  background: #000;
  color:#fff;
  text-decoration:none;
  padding: 0.65rem 1.0rem;
  border-radius: 10px;
  font-family: Georgia, "Times New Roman", serif;
  font-size: 1.05rem;
  box-shadow: 0 10px 22px rgba(0,0,0,0.14);
  transition: transform 120ms ease, box-shadow 120ms ease;
}
.cv-btn:hover{
  transform: translateY(-2px);
  box-shadow: 0 14px 28px rgba(0,0,0,0.18);
}

.cv-note{
  margin: 0.4rem 0 1.2rem 0;
  color: rgba(0,0,0,0.72);
  line-height: 1.55;
}

/* PDF viewer */
.pdf-frame{
  width: 100%;
  height: 82vh;
  border: 1px solid rgba(0,0,0,0.10);
  border-radius: 12px;
  overflow: hidden;
  box-shadow: 0 10px 26px rgba(0,0,0,0.08);
  background: #fff;
}

/* fallback box (for browsers that block embedding) */
.fallback{
  margin-top: 1rem;
  padding: 1rem 1.1rem;
  border-radius: 12px;
  background: #f4ead5;
  border: 1px solid rgba(0,0,0,0.06);
}
</style>

<div class="cv-wrap">

  <div class="cv-header">
    <h1>Curriculum Vitae</h1>

    <div class="cv-links">
      <a class="cv-btn" href="/assets/cv/Tyler_Chandross-Cohen_CV.pdf" target="_blank" rel="noopener">Open PDF</a>
      <a class="cv-btn" href="/assets/cv/Tyler_Chandross-Cohen_CV.pdf" download>Download PDF</a>
      <a class="cv-btn" href="/assets/cv/Tyler_Chandross-Cohen_CV.docx" download>Download Word</a>
    </div>
  </div>

  <p class="cv-note">
    View the CV below or download the PDF/Word version using the buttons above.
  </p>

  <!-- Embedded PDF viewer -->
  <iframe
    class="pdf-frame"
    src="/assets/cv/Tyler_Chandross-Cohen_CV.pdf#view=FitH"
    title="Tyler Chandross-Cohen CV (PDF)"
  ></iframe>

  <div class="fallback">
    <strong>Having trouble viewing the PDF?</strong>
    Some browsers or privacy settings block embedded PDFs. Use:
    <a href="/assets/cv/Tyler_Chandross-Cohen_CV.pdf" target="_blank" rel="noopener">Open PDF</a>
    or
    <a href="/assets/cv/Tyler_Chandross-Cohen_CV.pdf" download>Download PDF</a>.
  </div>

</div>
