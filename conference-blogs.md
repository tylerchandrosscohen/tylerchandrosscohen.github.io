---
layout: default
title: Conference Blogs
permalink: /blog/
---

<style>
/* ===== HEADER FIX (matches Media page) ===== */
.site-header{
  padding: 0 !important;
  min-height: auto !important;
  border-bottom: 1px solid rgba(0,0,0,0.08);
}

.site-header .wrapper{
  padding-top: 0.3rem !important;
  padding-bottom: 0.3rem !important;
}

.site-title{
  line-height: 1.2;
  padding: 0 !important;
}

.site-nav{
  line-height: 1.2;
}

.site-nav a{
  padding-top: 0.25rem !important;
  padding-bottom: 0.25rem !important;
}

/* ===== page wrapper ===== */
.blog-wrap{
  max-width: 900px;
  width: min(900px, 94vw);
  margin: 0 auto;
  padding: 1.6rem clamp(12px, 2.5vw, 28px) 2.2rem;
}

.blog-wrap h1{
  margin: 0 0 0.6rem 0;
  font-family: Georgia, "Times New Roman", serif;
  font-size: 3.2rem;
  line-height: 1.08;
}

/* ===== cards list ===== */
.post-list{
  display: grid;
  grid-template-columns: 1fr;
  gap: 1.8rem;
}

/* ===== card ===== */
.post-card{
  background: #fff;
  border: 1px solid rgba(0,0,0,0.12);
  border-radius: 14px;
  overflow: hidden;
  box-shadow: 0 10px 24px rgba(0,0,0,0.06);
  transition: transform 140ms ease, box-shadow 140ms ease;
}

.post-card:hover{
  transform: translateY(-2px);
  box-shadow: 0 14px 34px rgba(0,0,0,0.10);
}

.post-link{
  display: grid;
  grid-template-columns: 420px 1fr;
  gap: 1.8rem;
  text-decoration: none;
  color: inherit;
}

@media (max-width: 900px){
  .post-link{
    grid-template-columns: 1fr;
  }
}

/* ===== LEFT: media ===== */
.post-media{
  background: #f3f3f3;
  padding: 1.2rem;
  display: grid;
  grid-template-rows: auto 1fr;
  gap: 1rem;
}

.post-logo img{
  width: 100%;
  height: 100px;
  object-fit: contain;
  padding: 10px;
  background: white;
}

/* ===== photos ===== */
.photo-strip{
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 0.9rem;
}

.strip-photo{
  height: 140px;
  overflow: hidden;
  border-radius: 10px;
}

.strip-photo img{
  width: 100%;
  height: 100%;
  object-fit: cover;
}

/* ===== text ===== */
.post-body{
  padding: 1.5rem 1.6rem;
}

.post-title{
  font-size: 2.25rem;
  margin: 0 0 0.6rem 0;
}

.post-excerpt{
  font-size: 1.05rem;
  line-height: 1.6;
}
</style>

<div class="blog-wrap">
  <h1>Conference Blogs</h1>

  <div class="post-list">
    {% for post in site.posts %}
      <article class="post-card">
        <a class="post-link" href="{{ post.url | relative_url }}">

          <div class="post-media">
            <div class="post-logo">
              <img src="{{ post.conference_logo | relative_url }}">
            </div>

            <div class="photo-strip">
              <div class="strip-photo">
                <img src="{{ post.photo1 | relative_url }}">
              </div>
              <div class="strip-photo">
                <img src="{{ post.photo2 | relative_url }}">
              </div>
            </div>
          </div>

          <div class="post-body">
            <h2 class="post-title">{{ post.title }}</h2>
            <p class="post-excerpt">{{ post.landing_excerpt }}</p>
          </div>

        </a>
      </article>
    {% endfor %}
  </div>
</div>
