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

