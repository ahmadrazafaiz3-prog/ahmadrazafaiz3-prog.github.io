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

   <div class="mentor-card">
<img class="mentor-avatar" src="{{ '/assets/images/dr-bilal-ahmad.png' | relative_url }}" alt="Dr. Bilal Ahmad">
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
                url('https://images.unsplash.com/photo-1517694712202-14dd9538aa97?auto=format&fit=crop&w=1200&q=80');
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

  /* Mentor Card featuring the uploaded image directly encoded */
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
    width: 105px;
    height: 105px;
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

  /* Text-Only Clean Post Grid Layout */
  .post-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 24px;
    margin-bottom: 4rem;
  }

  .post-card {
    border: 1px solid var(--border-color);
    border-radius: 12px;
    background: #fff;
    transition: transform 0.2s ease, box-shadow 0.2s ease;
    text-decoration: none;
    color: inherit;
    display: flex;
    flex-direction: column;
  }

  .post-card:hover {
    transform: translateY(-4px);
    box-shadow: 0 10px 20px rgba(0,0,0,0.05);
    border-color: var(--primary-color);
  }

  .post-card .card-body {
    padding: 22px;
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
    margin-bottom: 10px;
  }

  .post-card .card-body h3 {
    font-size: 1.2rem;
    margin: 0 0 12px 0;
    line-height: 1.45;
    color: var(--dark-blue);
    font-weight: 700;
  }

  .post-card .card-body .date {
    font-size: 0.85rem;
    color: #999;
    margin-top: auto;
    display: flex;
    align-items: center;
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
  <img class="mentor-avatar" src="data:image/png;base64,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


</div>

