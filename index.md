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



<style>
  body {
    background-image: url("{{ '/images/site-background.svg' | relative_url }}");
    background-size: 800px 800px;
    background-repeat: repeat;
    background-attachment: fixed;
  }
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
  .intro h2 { font-size: 1.8rem; margin-bottom: 0.6rem; }
  .intro p { color: #555; font-size: 1.05rem; line-height: 1.6; }

  .mentor-card {
    max-width: 720px;
    margin: 0 auto 3rem auto;
    background: #f6f7fbee;
    border-left: 4px solid #6c63ff;
    border-radius: 8px;
    padding: 1.2rem 1.5rem;
  }
  .mentor-card strong { color: #2a2a45; }
  .mentor-card .links a { margin-right: 12px; font-size: 0.95rem; text-decoration: none; color: #6c63ff; }

  .section-title { text-align: center; font-size: 1.6rem; margin: 2.5rem 0 1.5rem 0; color: #2a2a45; }

  .folder-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
    gap: 28px;
    margin-bottom: 3rem;
  }
  .folder-card {
    border-radius: 14px;
    padding: 2rem 1.5rem;
    text-decoration: none;
    color: #fff;
    display: block;
    text-align: center;
    transition: transform 0.15s ease, box-shadow 0.15s ease;
    box-shadow: 0 4px 14px rgba(0,0,0,0.12);
  }
  .folder-card:hover { transform: translateY(-6px); box-shadow: 0 12px 24px rgba(0,0,0,0.18); }
  .folder-card .icon { font-size: 2.6rem; margin-bottom: 0.6rem; display: block; }
  .folder-card h3 { margin: 0 0 6px 0; font-size: 1.25rem; }
  .folder-card p { margin: 0; font-size: 0.9rem; opacity: 0.9; }
  .folder-1 { background: linear-gradient(135deg, #1e2640, #3a2d6b); }
  .folder-2 { background: linear-gradient(135deg, #1b3a2b, #1e5631); }
  .folder-3 { background: linear-gradient(135deg, #3a2d1e, #6b4d2d); }
</style>

<div class="hero">
  <img src="{{ '/images/hero-banner.svg' | relative_url }}" alt="Ahmad Raza Blog Banner">
</div>


<div class="mentor-card">
  <p><strong>About the mentor referenced throughout this blog:</strong> Dr. Bilal Ahmad is a Professor at UET Lahore, Faisalabad Campus, and an expert in Artificial Intelligence, Machine Learning, and Deep Learning model training. His guidance and encouragement inspired this entire portfolio project.</p>
  <p class="links">
    <a href="https://www.linkedin.com/in/drbilalphd/" target="_blank" rel="noopener">LinkedIn</a>
    <a href="https://scholar.google.com.au/citations?user=8nZ0jVkAAAAJ&hl=en" target="_blank" rel="noopener">Google Scholar</a>
    <a href="https://www.facebook.com/Dr.BilalAhm" target="_blank" rel="noopener">Facebook</a>
  </p>
</div>

<h3 class="section-title">Explore by Folder</h3>

<div class="folder-grid">
  <a class="folder-card folder-1" href="{{ '/semester1/' | relative_url }}">
    <span class="icon">📁</span>
    <h3>1st Semester — Python</h3>
    <p>Variables, loops, functions, data structures, classes</p>
  </a>
  <a class="folder-card folder-2" href="{{ '/semester2/' | relative_url }}">
    <span class="icon">📁</span>
    <h3>2nd Semester — Database</h3>
    <p>Keys, ER modeling, SQL, relational algebra, normalization</p>
  </a>
  <a class="folder-card folder-3" href="{{ '/journey/' | relative_url }}">
    <span class="icon">📁</span>
    <h3>Journey of University</h3>
    <p>My GitHub portfolio story &amp; full post archive</p>
  </a>
</div>

