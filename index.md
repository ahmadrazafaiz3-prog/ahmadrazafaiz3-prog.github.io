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
    --primary: #4f46e5;
    --primary-hover: #4338ca;
    --text-dark: #1e1b4b;
    --text-muted: #475569;
    --bg-light: #f8fafc;
    --card-border: #e2e8f0;
  }

  /* Hero Section Redesign */
  .hero-container {
    position: relative;
    margin: -2rem -2rem 3rem -2rem;
    height: 380px;
    background: linear-gradient(135deg, rgba(30, 27, 75, 0.95), rgba(79, 70, 229, 0.85)), 
                url('https://images.unsplash.com/photo-1517694712202-14dd9538aa97?auto=format&fit=crop&w=1200&q=80');
    background-size: cover;
    background-position: center;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    color: #ffffff;
    padding: 0 1.5rem;
  }

  .hero-content h1 {
    font-size: 2.8rem;
    font-weight: 800;
    margin-bottom: 0.5rem;
    letter-spacing: -0.02em;
    text-shadow: 0 4px 12px rgba(0,0,0,0.2);
  }

  .hero-content p {
    font-size: 1.25rem;
    color: #e2e8f0;
    max-width: 600px;
    margin: 0 auto;
    font-weight: 300;
  }

  /* Intro Section */
  .intro-box {
    max-width: 800px;
    margin: 0 auto 3.5rem auto;
    text-align: center;
    padding: 0 1rem;
  }

  .intro-box h2 {
    font-size: 1.8rem;
    color: var(--text-dark);
    margin-bottom: 1rem;
    font-weight: 700;
  }

  .intro-box p {
    color: var(--text-muted);
    font-size: 1.1rem;
    line-height: 1.7;
  }

  /* Premium Mentor Section */
  .mentor-showcase {
    max-width: 800px;
    margin: 0 auto 4rem auto;
    background: #ffffff;
    border: 1px solid var(--card-border);
    border-radius: 16px;
    padding: 2rem;
    box-shadow: 0 4px 20px rgba(0, 0, 0, 0.02);
    display: flex;
    gap: 1.5rem;
    align-items: center;
  }

  .mentor-img {
    width: 90px;
    height: 90px;
    border-radius: 50%;
    object-fit: cover;
    border: 3px solid var(--primary);
    flex-shrink: 0;
  }

  .mentor-info h4 {
    margin: 0 0 0.2rem 0;
    font-size: 0.85rem;
    text-transform: uppercase;
    color: var(--primary);
    letter-spacing: 0.05em;
  }

  .mentor-info h3 {
    margin: 0 0 0.75rem 0;
    font-size: 1.4rem;
    color: var(--text-dark);
  }

  .mentor-info p {
    color: var(--text-muted);
    font-size: 0.95rem;
    line-height: 1.5;
    margin-bottom: 1rem;
  }

  .mentor-links a {
    margin-right: 16px;
    font-size: 0.9rem;
    font-weight: 600;
    text-decoration: none;
    color: var(--primary);
    transition: color 0.2s;
  }

  .mentor-links a:hover {
    color: var(--primary-hover);
    text-decoration: underline;
  }

  /* Grid Layout for Posts */
  .section-heading {
    text-align: center;
    font-size: 1.75rem;
    font-weight: 700;
    margin-bottom: 2rem;
    color: var(--text-dark);
    position: relative;
  }

  .section-heading::after {
    content: '';
    display: block;
    width: 50px;
    height: 4px;
    background: var(--primary);
    margin: 0.5rem auto 0 auto;
    border-radius: 2px;
  }

  .post-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 30px;
    margin-bottom: 4rem;
  }

  .post-card {
    border: 1px solid var(--card-border);
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
    box-shadow: 0 12px 24px rgba(79, 70, 229, 0.08);
  }

  .post-card .thumb {
    height: 180px;
    overflow: hidden;
    background: #f1f5f9;
  }

  .post-card .thumb img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: transform 0.3s ease;
  }

  .post-card:hover .thumb img {
    transform: scale(1.04);
  }

  .post-card .card-body {
    padding: 1.25rem;
    display: flex;
    flex-direction: column;
    flex-grow: 1;
  }

  .post-card .card-body .tag {
    font-size: 0.75rem;
    text-transform: uppercase;
    letter-spacing: 0.05em;
    color: var(--primary);
    font-weight: 700;
    margin-bottom: 8px;
  }

  .post-card .card-body h3 {
    font-size: 1.15rem;
    margin: 0 0 10px 0;
    line-height: 1.4;
    color: var(--text-dark);
  }

  .post-card .card-body .date {
    font-size: 0.85rem;
    color: #64748b;
    margin-top: auto;
  }

  @media (max-width: 600px) {
    .hero-container { height: 280px; }
    .hero-content h1 { font-size: 2rem; }
    .mentor-showcase { flex-direction: column; text-align: center; }
  }
</style>

<div class="hero-container">
  <div class="hero-content">
    <h1>Ahmad Raza</h1>
    <p>Computer Engineering Portfolio & Personal Blog</p>
  </div>
</div>

<div class="intro-box">
  <h2>Welcome to My Engineering Journey</h2>
  <p>
    This blog serves as my official digital footprint at <strong>UET Lahore, Faisalabad Campus</strong>. 
    Inside, you will find a raw, running documentation of my engineering laboratory discoveries, deep dives into Python data analysis, 
    and Database Systems architectures—built systematically as milestones along my degree track.
  </p>
</div>

<div class="mentor-showcase">
  <img class="mentor-img" src="https://images.unsplash.com/photo-1534528741775-53994a69daeb?auto=format&fit=crop&w=200&q=80" alt="Dr. Bilal Ahmad Blueprint Profile">
  <div class="mentor-info">
    <h4>Academic Mentor</h4>
    <h3>Dr. Bilal Ahmad</h3>
    <p>
      Professor at UET Lahore, Faisalabad Campus. Specialist in Artificial Intelligence, Machine Learning, and Deep Learning engineering frameworks. His curriculum guidance holds high influence over the practical engineering logs detailed in this portal.
    </p>
    <div class="mentor-links">
      <a href="https://www.linkedin.com/in/drbilalphd/" target="_blank" rel="noopener">🔗 LinkedIn</a>
      <a href="https://scholar.google.com.au/citations?user=8nZ0jVkAAAAJ&hl=en" target="_blank" rel="noopener">🎓 Scholar</a>
      <a href="https://www.facebook.com/Dr.BilalAhm" target="_blank" rel="noopener">🌐 Facebook</a>
    </div>
  </div>
</div>

<h3 class="section-heading">Latest Academic Logs</h3>
<div class="post-grid">
  {% for post in site.posts %}
  <a class="post-card" href="{{ post.url | relative_url }}">
    <div class="thumb">
      <img src="{{ post.thumbnail | default: 'https://images.unsplash.com/photo-1618401471353-b98aedd07871?auto=format&fit=crop&w=600&q=80' | relative_url }}" alt="{{ post.title }}">
    </div>
    <div class="card-body">
      <span class="tag">{{ post.categories | first | default: 'Engineering' }}</span>
      <h3>{{ post.title }}</h3>
      <span class="date">📅 {{ post.date | date: "%b %-d, %Y" }}</span>
    </div>
  </a>
  {% endfor %}
</div>



