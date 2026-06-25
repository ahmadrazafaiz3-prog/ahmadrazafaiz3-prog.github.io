---
layout: home
title: Home
---

# Welcome to My Engineering Journey

Welcome to my personal portfolio blog website. I am a Computer Engineering student at UET Faisalabad. This website serves as my digital footprint where I document my academic journey, learning experiences, projects, and lessons learned throughout my university life. The idea of creating this blog was inspired by my professor, Dr. Bilal Ahmad, who encouraged students to maintain a professional online presence and continuously share their learning experiences.

![My Study Desk](/assets/images/my-study-picture.jpg)

This website documents my learning journey, projects, database systems experience, and university life.

![Database Learning](/assets/images/database-lab.jpg)

I created this portfolio blog following the advice of Dr. Bilal Ahmad to build a professional digital footprint.

![GitHub Work](/assets/images/github-work.jpg)

![First Day at UET Faisalabad](https://images.unsplash.com/photo-1541339907198-e08756dedf3f?auto=format&fit=crop&w=1200&q=80)
Welcome to my Computer Engineering journey.
---
layout: default
title: Home
---

<style>
  .hero {
    margin: -2rem -2rem 2.5rem -2rem;
  }
  .hero img {
    width: 100%;
    display: block;
  }
  .intro {
    max-width: 720px;
    margin: 0 auto 2.5rem auto;
    text-align: center;
    padding: 0 1rem;
  }
  .intro h2 {
    font-size: 1.8rem;
    margin-bottom: 0.6rem;
  }
  .intro p {
    color: #555;
    font-size: 1.05rem;
    line-height: 1.6;
  }
  .mentor-card {
    max-width: 720px;
    margin: 0 auto 3rem auto;
    background: #f6f7fb;
    border-left: 4px solid #6c63ff;
    border-radius: 8px;
    padding: 1.2rem 1.5rem;
  }
  .mentor-card strong { color: #2a2a45; }
  .mentor-card .links a {
    margin-right: 12px;
    font-size: 0.95rem;
    text-decoration: none;
    color: #6c63ff;
  }
  .section-title {
    text-align: center;
    font-size: 1.6rem;
    margin: 2.5rem 0 1.5rem 0;
    color: #2a2a45;
  }
  .post-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
    gap: 24px;
    margin-bottom: 3rem;
  }
  .post-card {
    border: 1px solid #e6e6ef;
    border-radius: 10px;
    overflow: hidden;
    background: #fff;
    transition: transform 0.15s ease, box-shadow 0.15s ease;
    text-decoration: none;
    color: inherit;
    display: block;
  }
  .post-card:hover {
    transform: translateY(-4px);
    box-shadow: 0 8px 20px rgba(0,0,0,0.08);
  }
  .post-card .thumb {
    background: #f0f1f7;
    height: 150px;
    display: flex;
    align-items: center;
    justify-content: center;
    overflow: hidden;
  }
  .post-card .thumb img {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }
  .post-card .card-body {
    padding: 14px 16px;
  }
  .post-card .card-body .tag {
    display: inline-block;
    font-size: 0.7rem;
    text-transform: uppercase;
    letter-spacing: 0.05em;
    color: #6c63ff;
    font-weight: 600;
    margin-bottom: 6px;
  }
  .post-card .card-body h3 {
    font-size: 1.05rem;
    margin: 0 0 4px 0;
    line-height: 1.3;
  }
  .post-card .card-body .date {
    font-size: 0.8rem;
    color: #999;
  }
</style>

<div class="hero">
  <img src="{{ '/images/hero-banner.svg' | relative_url }}" alt="Ahmad Raza Blog Banner">
</div>

<div class="intro">
  <h2>Welcome to My Engineering Journey</h2>
  <p>
    This blog is my digital footprint as a Computer Engineering student at UET Lahore, Faisalabad Campus —
    a running record of what I learned this semester in Python and Database Systems, written as it actually happened,
    mistakes included.
  </p>
</div>

<div class="mentor-card">
  <p><strong>About the mentor referenced throughout this blog:</strong> Dr. Bilal Ahmad is a Professor at UET Lahore, Faisalabad Campus, and an expert in Artificial Intelligence, Machine Learning, and Deep Learning model training. His guidance and encouragement inspired this entire portfolio project.</p>
  <p class="links">
    <a href="https://www.linkedin.com/in/drbilalphd/" target="_blank" rel="noopener">LinkedIn</a>
    <a href="https://scholar.google.com.au/citations?user=8nZ0jVkAAAAJ&hl=en" target="_blank" rel="noopener">Google Scholar</a>
    <a href="https://www.facebook.com/Dr.BilalAhm" target="_blank" rel="noopener">Facebook</a>
  </p>
</div>

<h3 class="section-title">Latest Posts</h3>

<div class="post-grid">
  {% for post in site.posts %}
  <a class="post-card" href="{{ post.url | relative_url }}">
    <div class="thumb">
      <img src="{{ post.thumbnail | default: '/images/hero-banner.svg' | relative_url }}" alt="{{ post.title }}">
    </div>
    <div class="card-body">
      <span class="tag">{{ post.categories | first }}</span>
      <h3>{{ post.title }}</h3>
      <span class="date">{{ post.date | date: "%b %-d, %Y" }}</span>
    </div>
  </a>
  {% endfor %}
</div>



