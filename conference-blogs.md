---
layout: default
title: Conference Blogs
permalink: /blog/
---

<style>
/* ===== page wrapper ===== */
.blog-wrap{
  max-width: 1150px;
  width: min(1150px, 96vw);
  margin: 0 auto;
  padding: 2.2rem clamp(16px, 3vw, 48px) 2.8rem;
}

.blog-wrap h1{
  margin: 0 0 1.4rem 0;
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

/* ===== card (matches your screenshot style) ===== */
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

/* whole card clickable */
.post-link{
  display: grid;
  grid-template-columns: 420px 1fr;
  gap: 1.8rem;
  align-items: stretch;
  text-decoration: none;
  color: inherit;
}

@media (max-width: 900px){
  .post-link{
    grid-template-columns: 1fr;
  }
}

/* ===== LEFT: media stack (logo + 2 photos) ===== */
.post-media{
  background: #f3f3f3;
  padding: 1.2rem;
  display: grid;
  grid-template-rows: auto 1fr;
  gap: 1rem;
  min-height: 260px;
}

.post-logo{
  width: 100%;
  background: #ffffff;
  border-radius: 10px;
  overflow: hidden;
  border: 1px solid rgba(0,0,0,0.08);
  box-shadow: 0 10px 22px rgba(0,0,0,0.07);
}

.post-logo img{
  width: 100%;
  height: 180px;
  object-fit: contain; /* logos should not be cropped */
  display: block;
  padding: 12px;       /* gives the logo breathing room */
  background: white;
}

.photo-strip{
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 0.9rem;
}

.strip-photo{
  background: #e9e9e9;
  border-radius: 10px;
  overflow: hidden;
  border: 1px solid rgba(0,0,0,0.08);
  height: 140px;
}

.strip-photo img{
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
}

/* ===== RIGHT: text ===== */
.post-body{
  padding: 1.5rem 1.6rem 1.4rem;
}

.post-meta{
  display: flex;
  gap: 0.8rem;
  flex-wrap: wrap;
  align-items: center;
  color: rgba(0,0,0,0.62);
  font-size: 0.95rem;
  margin-bottom: 0.55rem;
}

.post-title{
  margin: 0 0 0.65rem 0;
  font-family: Georgia, "Times New Roman", serif;
  font-size: 2.25rem;
  line-height: 1.12;
}

.post-excerpt{
  margin: 0.2rem 0 0 0;
  color: rgba(0,0,0,0.80);
  font-size: 1.06rem;
  line-height: 1.65;
  max-width: 88ch;
}

/* focus ring for accessibility */
.post-link:focus{
  outline: 3px solid rgba(0,0,0,0.20);
  outline-offset: 3px;
  border-radius: 14px;
}

/* small helper line under excerpt */
.post-hint{
  margin-top: 0.9rem;
  color: rgba(0,0,0,0.55);
  font-size: 0.95rem;
}
</style>

<div class="blog-wrap">
  <h1>Conference Blogs</h1>

  <div class="post-list">
    {% for post in site.posts %}
      <article class="post-card">
        <a class="post-link" href="{{ post.url | relative_url }}" aria-label="Read {{ post.title }}">

          <!-- LEFT: logo + optional photos -->
          <div class="post-media">
            <div class="post-logo">
              {% if post.conference_logo %}
                <img src="{{ post.conference_logo | relative_url }}" alt="Conference logo for {{ post.title }}">
              {% elsif post.cover_image %}
                <!-- fallback: if you don’t set a logo yet, use cover_image -->
                <img src="{{ post.cover_image | relative_url }}" alt="Cover image for {{ post.title }}">
              {% else %}
                <img src="/assets/img/placeholder-logo.png" alt="Conference logo placeholder">
              {% endif %}
            </div>

            <div class="photo-strip">
              <div class="strip-photo">
                {% if post.photo1 %}
                  <img src="{{ post.photo1 | relative_url }}" alt="Photo 1 for {{ post.title }}">
                {% else %}
                  <img src="/assets/img/placeholder-photo.png" alt="Photo placeholder">
                {% endif %}
              </div>
              <div class="strip-photo">
                {% if post.photo2 %}
                  <img src="{{ post.photo2 | relative_url }}" alt="Photo 2 for {{ post.title }}">
                {% else %}
                  <img src="/assets/img/placeholder-photo.png" alt="Photo placeholder">
                {% endif %}
              </div>
            </div>
          </div>

          <!-- RIGHT: text -->
          <div class="post-body">
            <div class="post-meta">
              <span>{{ post.author | default: "Tyler Cohen" }}</span>
              <span>•</span>
              <span>{{ post.date | date: "%b %-d, %Y" }}</span>
              {% if post.read_time %}
                <span>•</span>
                <span>{{ post.read_time }} min read</span>
              {% endif %}
            </div>

            <h2 class="post-title">{{ post.title }}</h2>

            <p class="post-excerpt">
              {% if post.landing_excerpt %}
                {{ post.landing_excerpt | strip_html | truncate: 240 }}
              {% elsif post.excerpt %}
                {{ post.excerpt | strip_html | truncate: 240 }}
              {% else %}
                {{ post.content | strip_html | truncate: 240 }}
              {% endif %}
            </p>

            <div class="post-hint">Click to open full post →</div>
          </div>

        </a>
      </article>
    {% endfor %}
  </div>
</div>
