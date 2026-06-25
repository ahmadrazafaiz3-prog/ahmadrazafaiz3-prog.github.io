---
layout: default
title: Journey of University — My GitHub Portfolio
permalink: /journey/
---

<style>
  .folder-hero {
    background: linear-gradient(135deg, #3a2d1e, #6b4d2d);
    border-radius: 12px;
    padding: 2.5rem 2rem;
    color: #fff;
    margin-bottom: 2rem;
    text-align: center;
  }
  .folder-hero h1 { margin: 0 0 0.5rem 0; font-size: 2rem; }
  .folder-hero p { color: #f5e3d0; margin: 0; }
  .about-box {
    max-width: 720px;
    margin: 0 auto 2.5rem auto;
    line-height: 1.7;
    color: #444;
  }
  .mentor-card {
    max-width: 720px;
    margin: 0 auto 2.5rem auto;
    background: #f6f7fb;
    border-left: 4px solid #6c63ff;
    border-radius: 8px;
    padding: 1.2rem 1.5rem;
  }
  .mentor-card .links a { margin-right: 12px; font-size: 0.95rem; text-decoration: none; color: #6c63ff; }
  .post-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
    gap: 24px;
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
  .post-card:hover { transform: translateY(-4px); box-shadow: 0 8px 20px rgba(0,0,0,0.08); }
  .post-card .thumb { background: #f0f1f7; height: 150px; display: flex; align-items: center; justify-content: center; overflow: hidden; }
  .post-card .thumb img { width: 100%; height: 100%; object-fit: cover; }
  .post-card .card-body { padding: 14px 16px; }
  .post-card .card-body h3 { font-size: 1.05rem; margin: 0 0 4px 0; line-height: 1.3; }
  .post-card .card-body .date { font-size: 0.8rem; color: #999; }
  .back-link { display: inline-block; margin-bottom: 1.5rem; color: #6c63ff; text-decoration: none; font-size: 0.9rem; }
</style>

<a class="back-link" href="{{ '/' | relative_url }}">&larr; Back to Home</a>

<div class="folder-hero">
  <h1>📁 Journey of University — My Portfolio</h1>
  <p>Why I built this GitHub portfolio blog, and the full archive of everything in it.</p>
</div>

<div class="about-box">
  <p>I am a Computer Engineering student at UET Lahore, Faisalabad Campus. This portfolio blog is my digital footprint — a place to document my academic journey, learning experiences, projects, and the lessons learned throughout university life, hosted directly on GitHub Pages.</p>
  <p>The idea for this blog came from my professor, Dr. Bilal Ahmad, who encouraged students to build and maintain a professional online presence and to keep sharing what they learn as they go, rather than only looking back on it at the end.</p>
  <p>This page is the full archive of that journey: every post from both semesters, in one place.</p>
</div>

<div class="mentor-card">
  <p><strong>Dr. Bilal Ahmad</strong> — Professor, UET Lahore, Faisalabad Campus. Expert in Artificial Intelligence, Machine Learning, and Deep Learning model training.</p>
  <p class="links">
    <a href="https://www.linkedin.com/in/drbilalphd/" target="_blank" rel="noopener">LinkedIn</a>
    <a href="https://scholar.google.com.au/citations?user=8nZ0jVkAAAAJ&hl=en" target="_blank" rel="noopener">Google Scholar</a>
    <a href="https://www.facebook.com/Dr.BilalAhm" target="_blank" rel="noopener">Facebook</a>
  </p>
</div>

<div class="post-grid">
  {% for post in site.posts %}
  <a class="post-card" href="{{ post.url | relative_url }}">
    <div class="thumb">
      <img src="{{ post.thumbnail | default: '/images/hero-banner.svg' | relative_url }}" alt="{{ post.title }}">
    </div>
    <div class="card-body">
      <h3>{{ post.title }}</h3>
      <span class="date">{{ post.date | date: "%b %-d, %Y" }}</span>
    </div>
  </a>
  {% endfor %}
</div>
