---
layout: default
title: Research Areas
permalink: /research/
---

<style>
.research-wrap{
  max-width: 1400px;
  margin: 0 auto;
  padding: 2.4rem 1.2rem 3rem;
}

/* page title */
.research-wrap h1{
  font-family: Georgia, "Times New Roman", serif;
  font-size: 2.8rem;
  margin-bottom: 1.4rem;
}

/* individual research blocks */
.research-block{
  display: grid;
  grid-template-columns: 1.1fr 0.9fr;
  gap: 2.4rem;
  align-items: center;
  margin-bottom: 3.2rem;
}

@media (max-width: 900px){
  .research-block{
    grid-template-columns: 1fr;
  }
}

.research-text h2{
  font-family: Georgia, "Times New Roman", serif;
  font-size: 2.0rem;
  margin-bottom: 0.8rem;
}

.research-text p{
  font-size: 1.08rem;
  line-height: 1.7;
  color: rgba(0,0,0,0.82);
  margin-bottom: 0.8rem;
  max-width: 70ch;
}

/* image styling */
.research-img{
  width: 100%;
  border-radius: 16px;
  overflow: hidden;
  box-shadow: 0 16px 36px rgba(0,0,0,0.18);
  border: 1px solid rgba(0,0,0,0.06);
}

.research-img img{
  width: 100%;
  height: 360px;
  object-fit: cover;
  display: block;
}

/* subtle divider */
.section-divider{
  height: 1px;
  background: rgba(0,0,0,0.08);
  margin: 3rem 0;
}
</style>

<div class="research-wrap">

  <h1>Research Areas</h1>

  <!-- ========================= -->
  <!-- AREA 1 -->
  <!-- ========================= -->
  <div class="research-block">

    <div class="research-text">
      <h2>
        Integrating Whole Genome Sequencing and Cytotoxicity to Better Understand
        <em>Bacillus cereus</em> Virulence Potential
      </h2>

      <p>
        A central focus of my research is improving how we assess the virulence
        potential of <em>Bacillus cereus</em> beyond species-level classification.
        Although <em>B. cereus</em> is routinely found in food systems; only a subset of
        strains may pose a meaningful risk to human health. Distinguishing these
        strains remains a major challenge for food safety risk assessment.
      </p>

      <p>
        I address this challenge by combining whole genome sequencing (WGS) with
        phenotypic cytotoxicity assays to link genetic content to functional
        outcomes. The goal is to integrate these genomic data with in vitro cytotoxicity measurements and targeted validation of single-nucleotide polymorphisms in enterotoxin genes associated with cytotoxicity within an exposure assessment framework, to determine whether virulence potential and risk can be predicted. This integrated approach enables a more nuanced, strain-specific evaluation of virulence potential by directly linking genomic variation to functional cytotoxic outcomes, thereby strengthening exposure assessment and informing food safety decision-making.
      </p>
      
    </div>

    <div class="research-img">
      <!-- replace with your own image -->
      <img src="/assets/img/research_wgs.jpg"
           alt="Whole genome sequencing and cytotoxicity analysis of Bacillus cereus">
    </div>

  </div>

  <div class="section-divider"></div>

  <!-- ========================= -->
  <!-- AREA 2 -->
  <!-- ========================= -->
  <div class="research-block">

    <div class="research-text">
      <h2>
        Psychrotolerant <em>Bacillus cereus</em> and Food Safety Risk in
        Refrigerated Foods
      </h2>

      <p>
        Another major area of my research focuses on psychrotolerant members of
        the <em>Bacillus cereus</em> group that are capable of growth at
        refrigeration temperatures. These strains present a unique food safety
        concern because they can proliferate in chilled foods that are otherwise
        considered low-risk due to cold storage.
      </p>

      <p>
        I investigate how low-temperature growth influences virulence gene
        transcription and cytotoxicity. By comparing
        psychrotolerant and mesophilic isolates across a range of temperatures and
        food-relevant matrices, my work aims to identify conditions under which
        psychrotolerant strains may pose an elevated risk.
      </p>

      <p>
        This research has particular relevance for refrigerated dairy products, where psychrotolerant
        <em>B. cereus</em> strains may evade traditional detection or risk
        categorization frameworks.
      </p>
    </div>

    <div class="research-img">
      <!-- replace with your own image -->
      <img src="/assets/img/research_cold.jpg"
           alt="Psychrotolerant Bacillus cereus growth at low temperature">
    </div>

  </div>

</div>
