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
  :root {
    --primary-color: #6c63ff;
    --dark-blue: #1e1b4b;
    --text-main: #2a2a45;
    --text-muted: #555566;
    --light-bg: #f6f7fb;
    --border-color: #e6e6ef;
  }

  /* Premium Banner Header */
  .hero {
    position: relative;
    margin: -2rem -2rem 3rem -2rem;
    height: 320px;
    background: linear-gradient(135deg, rgba(30, 27, 75, 0.9) 0%, rgba(108, 99, 255, 0.75) 100%), 
               <img class="mentor-avatar" src="{{ '/assets/images/dr-bilal-ahmad.png' | relative_url }}" alt="Dr. Bilal Ahmad">
    background-size: cover;
    background-position: center;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    box-shadow: 0 4px 15px rgba(0,0,0,0.05);
  }

  .hero-text h1 {
    color: #ffffff;
    font-size: 2.8rem;
    font-weight: 800;
    margin: 0 0 0.5rem 0;
    letter-spacing: -0.03em;
  }

  .hero-text p {
    color: #e2e8f0;
    font-size: 1.2rem;
    margin: 0;
    font-weight: 300;
  }

  /* Intro Formatting */
  .intro {
    max-width: 760px;
    margin: 0 auto 3rem auto;
    text-align: center;
    padding: 0 1rem;
  }

  .intro h2 {
    font-size: 1.8rem;
    color: var(--dark-blue);
    margin-bottom: 0.8rem;
    font-weight: 700;
  }

  .intro p {
    color: var(--text-muted);
    font-size: 1.05rem;
    line-height: 1.65;
  }

  /* Redesigned Mentor Card with Your Provided Image Embedded */
  .mentor-card {
    max-width: 760px;
    margin: 0 auto 4rem auto;
    background: #ffffff;
    border: 1px solid var(--border-color);
    border-radius: 14px;
    padding: 1.8rem;
    box-shadow: 0 5px 20px rgba(0,0,0,0.02);
    display: flex;
    gap: 1.5rem;
    align-items: center;
  }

  .mentor-avatar {
    width: 100px;
    height: 100px;
    border-radius: 50%;
    object-fit: cover;
    border: 3px solid var(--primary-color);
    box-shadow: 0 4px 10px rgba(108, 99, 255, 0.15);
    flex-shrink: 0;
  }

  .mentor-content {
    flex-grow: 1;
  }

  .mentor-content h4 {
    margin: 0 0 0.3rem 0;
    font-size: 0.8rem;
    text-transform: uppercase;
    color: var(--primary-color);
    letter-spacing: 0.05em;
    font-weight: 700;
  }

  .mentor-content h3 {
    margin: 0 0 0.6rem 0;
    font-size: 1.35rem;
    color: var(--dark-blue);
  }

  .mentor-content p {
    color: var(--text-muted);
    font-size: 0.95rem;
    line-height: 1.5;
    margin: 0 0 1rem 0;
  }

  .mentor-card .links a {
    margin-right: 14px;
    font-size: 0.9rem;
    font-weight: 600;
    text-decoration: none;
    color: var(--primary-color);
    transition: color 0.2s;
  }

  .mentor-card .links a:hover {
    color: var(--dark-blue);
    text-decoration: underline;
  }

  /* Section Title styling */
  .section-title {
    text-align: center;
    font-size: 1.6rem;
    margin: 0 0 2rem 0;
    color: var(--dark-blue);
    font-weight: 700;
  }

  /* Grid and Cards for Dynamic Posts */
  .post-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 28px;
    margin-bottom: 4rem;
  }

  .post-card {
    border: 1px solid var(--border-color);
    border-radius: 12px;
    overflow: hidden;
    background: #fff;
    transition: transform 0.2s ease, box-shadow 0.2s ease;
    text-decoration: none;
    color: inherit;
    display: flex;
    flex-direction: column;
  }

  .post-card:hover {
    transform: translateY(-5px);
    box-shadow: 0 10px 25px rgba(0,0,0,0.06);
  }

  .post-card .thumb {
    height: 170px;
    overflow: hidden;
  }

  .post-card .thumb img {
    width: 100%;
    height: 100%;
    object-fit: cover;
  }

  /* Fallback Brand Card style when no post image exists */
  .post-card .fallback-thumb {
    height: 170px;
    background: linear-gradient(135deg, #1e1b4b 0%, #6c63ff 100%);
    display: flex;
    align-items: center;
    justify-content: center;
    color: rgba(255, 255, 255, 0.15);
    font-size: 4.5rem;
    font-weight: 900;
    letter-spacing: -0.05em;
    user-select: none;
  }

  .post-card .card-body {
    padding: 18px;
    display: flex;
    flex-direction: column;
    flex-grow: 1;
  }

  .post-card .card-body .tag {
    display: inline-block;
    font-size: 0.75rem;
    text-transform: uppercase;
    letter-spacing: 0.05em;
    color: var(--primary-color);
    font-weight: 700;
    margin-bottom: 8px;
  }

  .post-card .card-body h3 {
    font-size: 1.1rem;
    margin: 0 0 10px 0;
    line-height: 1.4;
    color: var(--dark-blue);
  }

  .post-card .card-body .date {
    font-size: 0.85rem;
    color: #999;
    margin-top: auto;
  }

  @media (max-width: 640px) {
    .mentor-card {
      flex-direction: column;
      text-align: center;
    }
    .hero-text h1 { font-size: 2.2rem; }
  }
</style>

<div class="hero">
  <div class="hero-text">
    <h1>Ahmad Raza</h1>
    <p>Computer Engineering Portfolio & Personal Blog</p>
  </div>
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
  <img class="mentor-avatar" src="https://images.unsplash.com/photo-1500648767791-00dcc994a43e?auto=format&fit=crop&w=256&h=256&q=80" alt="Dr. Bilal Ahmad">
  <div class="mentor-content">
    <h4>Academic Mentor</h4>
    <h3>Dr. Bilal Ahmad</h3>
    <p>Professor at UET Lahore, Faisalabad Campus. Expert in Artificial Intelligence, Machine Learning, and Deep Learning model training. His guidance and encouragement inspired this entire portfolio project.</p>
    <p class="links">
      <a href="https://www.linkedin.com/in/drbilalphd/" target="_blank" rel="noopener">LinkedIn</a>
      <a href="https://scholar.google.com.au/citations?user=8nZ0jVkAAAAJ&hl=en" target="_blank" rel="noopener">Google Scholar</a>
      <a href="https://www.facebook.com/Dr.BilalAhm" target="_blank" rel="noopener">Facebook</a>
    </p>
  </div>
</div>

<h3 class="section-title">Latest Posts</h3>

<div style="max-width:900px;margin:0 auto 4rem auto;">
  {% for post in site.posts %}
  <div style="
      background:#fff;
      border:1px solid #e6e6ef;
      border-radius:12px;
      padding:20px;
      margin-bottom:15px;
      transition:0.2s;">
      
      <a href="{{ post.url | relative_url }}"
         style="text-decoration:none;color:#1e1b4b;">
         
         <h3 style="margin:0 0 10px 0;">
           {{ post.title }}
         </h3>

         <p style="margin:0;color:#666;">
           📅 {{ post.date | date: "%B %-d, %Y" }}
         </p>

      </a>
  </div>
  {% endfor %}
</div>

