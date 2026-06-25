---
layout: default
title: 2nd Semester — Database Systems
permalink: /semester2/
---

<style>
  .folder-hero {
    background: linear-gradient(135deg, #1b3a2b, #1e5631);
    border-radius: 12px;
    padding: 2.5rem 2rem;
    color: #fff;
    margin-bottom: 2rem;
    text-align: center;
  }
  .folder-hero h1 { margin: 0 0 0.5rem 0; font-size: 2rem; }
  .folder-hero p { color: #d6f5e3; margin: 0; }
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
  <h1>📁 2nd Semester — Database Systems</h1>
  <p>Keys, ER modeling, SQL queries, relational algebra, and normalization — taught by Dr. Bilal Ahmad.</p>
</div>

<div class="post-grid">
  {% for post in site.categories["semester-2"] %}
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
