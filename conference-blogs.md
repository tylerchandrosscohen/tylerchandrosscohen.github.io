---
layout: default
title: Conference Blogs
permalink: /blog/
---

<style>
.blog-wrap{
  max-width: 1100px;
  margin: 0 auto;
  padding: 2.2rem 1.2rem 2.8rem;
}

.blog-wrap h1{
  margin: 0 0 1.4rem 0;
  font-family: Georgia, "Times New Roman", serif;
  font-size: 3rem;
  line-height: 1.08;
}

/* cards list */
.post-list{
  display: grid;
  grid-template-columns: 1fr;
  gap: 1.6rem;
}

/* card */
.post-card{
  display: grid;
  grid-template-columns: 360px 1fr;
  gap: 1.6rem;
  align-items: stretch;

  background: #fff;
  border: 1px solid rgba(0,0,0,0.10);
  border-radius: 14px;
  overflow: hidden;
  box-shadow: 0 10px 22px rgba(0,0,0,0.06);
  transition: transform 140ms ease, box-shadow 140ms ease;
}

.post-card:hover{
  transform: translateY(-2px);
  box-shadow: 0 14px 30px rgba(0,0,0,0.10);
}

@media (max-width: 900px){
  .post-card{
    grid-template-columns: 1fr;
  }
}

/* image */
.post-cover{
  background: #f3f3f3;
  min-height: 220px;
}
.post-cover img{
  width: 100%;
  height: 100%;
  object-fit: cover;
  display: block;
}

/* right side content */
.post-body{
  padding: 1.4rem 1.4rem 1.2rem;
}

.post-meta{
  display: flex;
  gap: 0.8rem;
  flex-wrap: wrap;
  align-items: center;
  color: rgba(0,0,0,0.62);
  font-size: 0.95rem;
  margin-bottom: 0.5rem;
}

.post-title{
  margin: 0 0 0.55rem 0;
  font-family: Georgia, "Times New Roman", serif;
  font-size: 2.1rem;
  line-height: 1.12;
}

.post-excerpt{
  margin: 0;
  color: rgba(0,0,0,0.78);
  font-size: 1.05rem;
  line-height: 1.6;
  max-width: 80ch;
}

/* make entire card clickable */
.post-card a{
  text-decoration: none;
  color: inherit;
}
.post-card a:focus{
  outline: 3px solid rgba(0,0,0,0.2);
  outline-offset: -3px;
}
</style>

<div class="blog-wrap">
  <h1>Conference Blogs</h1>

  <div class="post-list">
    {% for post in site.posts %}
      <div class="post-card">
        <a href="{{ post.url | relative_url }}" aria-label="Read {{ post.title }}">
          <div class="post-cover">
            {% if post.cover_image %}
              <img src="{{ post.cover_image | relative_url }}" alt="Cover image for {{ post.title }}">
            {% endif %}
          </div>
        </a>

        <div class="post-body">
          <div class="post-meta">
            <span>{{ post.date | date: "%b %-d, %Y" }}</span>
            {% if post.read_time %}
              <span>•</span>
              <span>{{ post.read_time }} min read</span>
            {% endif %}
          </div>

          <h2 class="post-title">
            <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
          </h2>

          <p class="post-excerpt">
            {% if post.excerpt %}
              {{ post.excerpt | strip_html | truncate: 220 }}
            {% else %}
              {{ post.content | strip_html | truncate: 220 }}
            {% endif %}
          </p>
        </div>
      </div>
    {% endfor %}
  </div>
</div>
