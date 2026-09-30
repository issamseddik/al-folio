---
layout: about
title: about
permalink: /
subtitle: <span class="cultural-subtitle">Scientist | Researcher | Innovator</span>
profile:
  align: right
  image: prof_pic.jpg
  image_circular: true
  more_info: >
    <p class="contact-info">📍 Lab 404, Science Block</p>
    <p class="contact-info">📧 issam.seddik@example.com</p>

# We disable default sections so we can reorder them creatively below!
selected_papers: false
social: true
announcements:
  enabled: false
latest_posts:
  enabled: false
---

<style>
/* Custom Cultural & Scientific Theme */
:root {
  --primary-cultural: #047857; /* Emerald Green */
  --secondary-cultural: #b45309; /* Golden Amber */
  --scientific-blue: #1d4ed8;
  --bg-timeline: rgba(4, 120, 87, 0.05);
}

.cultural-subtitle {
  font-family: 'Georgia', serif;
  color: var(--secondary-cultural);
  letter-spacing: 2px;
  text-transform: uppercase;
  font-size: 0.9rem;
  font-weight: bold;
}

.contact-info {
  font-family: monospace;
  color: var(--scientific-blue);
  margin-bottom: 0.2rem;
}

/* Timeline Container */
.scientific-timeline {
  position: relative;
  max-width: 800px;
  margin: 3rem auto;
  padding: 2rem 0;
}

/* The vertical line */
.scientific-timeline::after {
  content: '';
  position: absolute;
  width: 4px;
  background-color: var(--primary-cultural);
  top: 0;
  bottom: 0;
  left: 50%;
  margin-left: -2px;
  border-radius: 2px;
}

/* Container around each step */
.timeline-step {
  padding: 10px 40px;
  position: relative;
  background-color: inherit;
  width: 50%;
}

/* Left/Right alignments */
.timeline-step.left { left: 0; }
.timeline-step.right { left: 50%; }

/* The Hexagon Node (Scientific + Geometric Culture) */
.timeline-step::after {
  content: '⬡'; /* Hexagon symbol */
  font-size: 24px;
  color: var(--secondary-cultural);
  position: absolute;
  top: 15px;
  right: -13px;
  background-color: white;
  line-height: 24px;
  z-index: 1;
}
.timeline-step.right::after { left: -11px; }

/* Content Box */
.timeline-content {
  padding: 20px 30px;
  background-color: white;
  position: relative;
  border-radius: 8px;
  border-left: 4px solid var(--scientific-blue);
  box-shadow: 0 4px 15px rgba(0,0,0,0.05);
  transition: transform 0.3s ease;
}

html[data-theme='dark'] .timeline-content {
  background-color: #1e1e1e;
  border-left: 4px solid var(--secondary-cultural);
  box-shadow: 0 4px 15px rgba(255,255,255,0.05);
}

html[data-theme='dark'] .timeline-step::after {
  background-color: #1e1e1e;
}

.timeline-content:hover {
  transform: translateY(-5px);
  border-left-color: var(--primary-cultural);
}

.timeline-content h3 {
  margin-top: 0;
  color: var(--primary-cultural);
  font-size: 1.2rem;
}

.timeline-content p {
  margin: 0;
  font-size: 0.95rem;
  line-height: 1.5;
}

.timeline-date {
  font-family: monospace;
  color: var(--secondary-cultural);
  font-weight: bold;
  display: block;
  margin-bottom: 0.5rem;
}

/* Reordering titles */
.section-title {
  text-align: center;
  font-family: 'Georgia', serif;
  color: var(--primary-cultural);
  margin-top: 3rem;
  margin-bottom: 2rem;
  border-bottom: 2px dashed var(--secondary-cultural);
  display: inline-block;
  padding-bottom: 0.5rem;
}

.section-wrapper {
  text-align: center;
}
</style>

<div class="intro-text" style="text-align: justify; font-size: 1.1rem; margin-bottom: 2rem;">
  Welcome to my digital space. Here, the precision of <strong>science</strong> meets the richness of <strong>culture</strong>. 
  I believe that research is a continuous journey—a step-by-step evolution of ideas, much like building a complex molecule or weaving a traditional geometric pattern.
</div>

<div class="section-wrapper">
  <h2 class="section-title">My Scientific Journey</h2>
</div>

<div class="scientific-timeline">
  
  <div class="timeline-step left">
    <div class="timeline-content">
      <span class="timeline-date">Present</span>
      <h3>Lead Researcher</h3>
      <p>Exploring the boundaries of technology and innovation. Currently focused on integrating complex systems with elegant solutions.</p>
    </div>
  </div>

  <div class="timeline-step right">
    <div class="timeline-content">
      <span class="timeline-date">2023 - 2024</span>
      <h3>Postdoctoral Fellowship</h3>
      <p>Conducted advanced experiments combining computational models with cultural heritage preservation algorithms.</p>
    </div>
  </div>

  <div class="timeline-step left">
    <div class="timeline-content">
      <span class="timeline-date">2019 - 2023</span>
      <h3>Ph.D. in Applied Sciences</h3>
      <p>Defended my thesis on the intersection of structured data networks and traditional algorithmic geometries.</p>
    </div>
  </div>

  <div class="timeline-step right">
    <div class="timeline-content">
      <span class="timeline-date">2015 - 2019</span>
      <h3>Foundation & Culture</h3>
      <p>Built a strong scientific foundation while actively engaging in cultural enrichment programs.</p>
    </div>
  </div>

</div>

<!-- Reordered Dynamic Sections -->
<div class="section-wrapper">
  <h2 class="section-title">Selected Publications</h2>
</div>
<div style="text-align: left;">
  {% include selected_papers.liquid %}
</div>

<div class="section-wrapper">
  <h2 class="section-title">Latest Announcements</h2>
</div>
<div style="text-align: left;">
  {% include news.liquid limit=true %}
</div>

<div class="section-wrapper">
  <h2 class="section-title">Recent Writings</h2>
</div>
<div style="text-align: left;">
  {% include latest_posts.liquid %}
</div>
