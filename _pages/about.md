---
layout: about
title: about
permalink: /
subtitle: 
profile:
  align: right
  image: prof_pic.jpg
  image_circular: true
  more_info: >
    <p class="contact-info">📍 Lab 404, Science Block</p>
    <p class="contact-info">📧 issam.seddik@example.com</p>

selected_papers: false
social: false
announcements:
  enabled: false
latest_posts:
  enabled: false
---

<style>
/* Reset container constraints if necessary to allow full width */
.post {
  max-width: 100% !important;
  margin: 0 !important;
  padding: 0 !important;
}

/* Hide the default page header to make room for full blocks */
.post-header {
  display: none !important;
}

/* Horizontal Scroll Container */
.swipe-container {
  display: flex;
  overflow-x: auto;
  overflow-y: hidden;
  scroll-snap-type: x mandatory;
  -webkit-overflow-scrolling: touch;
  width: 100vw;
  height: 80vh; /* Adjust height as needed */
  margin-left: calc(-50vw + 50%); /* Break out of jekyll container */
  margin-right: calc(-50vw + 50%);
  scrollbar-width: none; /* Firefox */
}

.swipe-container::-webkit-scrollbar {
  display: none; /* Chrome/Safari */
}

/* Individual Blocks */
.swipe-block {
  scroll-snap-align: center;
  flex: 0 0 100vw;
  width: 100vw;
  height: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 2rem;
  box-sizing: border-box;
  overflow-y: auto;
}

/* Styling the Blocks with Culture/Science colors */
.block-about { background-color: #f8fafc; color: #0f172a; }
.block-publications { background-color: #047857; color: #ffffff; }
.block-talks { background-color: #fef3c7; color: #92400e; }
.block-collaborators { background-color: #1d4ed8; color: #ffffff; }
.block-blogs { background-color: #f1f5f9; color: #0f172a; }
.block-contacts { background-color: #0f172a; color: #f8fafc; }

html[data-theme='dark'] .block-about { background-color: #0f172a; color: #f8fafc; }
html[data-theme='dark'] .block-talks { background-color: #451a03; color: #fef3c7; }
html[data-theme='dark'] .block-blogs { background-color: #1e293b; color: #f8fafc; }

.block-title {
  font-family: 'Georgia', serif;
  font-size: 2.5rem;
  margin-bottom: 2rem;
  text-transform: uppercase;
  letter-spacing: 3px;
  text-align: center;
}

.block-content {
  max-width: 800px;
  width: 100%;
  text-align: center;
  font-size: 1.1rem;
}

/* Links inside dark blocks */
.block-publications a, .block-collaborators a, .block-contacts a {
  color: #fbbf24;
}

/* Navigation hints */
.swipe-hint {
  position: fixed;
  bottom: 20px;
  left: 50%;
  transform: translateX(-50%);
  font-size: 0.9rem;
  color: #94a3b8;
  pointer-events: none;
  animation: pulse 2s infinite;
  z-index: 10;
}

@keyframes pulse {
  0% { opacity: 0.5; }
  50% { opacity: 1; }
  100% { opacity: 0.5; }
}

/* Fix text alignment for includes */
.block-publications .publications, .block-blogs .post-list {
  text-align: left;
}
</style>

<div class="swipe-hint">← Swipe horizontally to explore →</div>

<div class="swipe-container" id="swipe-container">

  <!-- BLOCK 1: ABOUT -->
  <div class="swipe-block block-about">
    <div class="block-content">
      <h2 class="block-title">About Me</h2>
      <img src="{{ 'assets/img/prof_pic.jpg' | relative_url }}" alt="Profile Picture" style="width: 150px; height: 150px; border-radius: 50%; margin-bottom: 1rem; border: 4px solid #047857;">
      <h3>Issam Seddik</h3>
      <p style="font-family: monospace; color: #047857;">Scientist | Researcher | Innovator</p>
      <p style="margin-top: 1rem; text-align: justify;">
        Welcome to my digital space. Here, the precision of science meets the richness of culture. I am currently focused on integrating complex systems with elegant solutions, bringing structural geometry into applied sciences.
      </p>
    </div>
  </div>

  <!-- BLOCK 2: PUBLICATIONS -->
  <div class="swipe-block block-publications">
    <div class="block-content">
      <h2 class="block-title">Publications</h2>
      <div style="background: rgba(255,255,255,0.1); padding: 20px; border-radius: 8px;">
        {% include selected_papers.liquid %}
      </div>
    </div>
  </div>

  <!-- BLOCK 3: TALKS -->
  <div class="swipe-block block-talks">
    <div class="block-content">
      <h2 class="block-title">Talks & Presentations</h2>
      <ul style="list-style-type: none; padding: 0; text-align: left;">
        <li style="margin-bottom: 15px; border-bottom: 1px dashed #d97706; padding-bottom: 10px;">
          <strong>International Conference on Applied Geometry (2023)</strong><br>
          <em>"Bridging the Gap: Cultural Heritage in Computational Models"</em>
        </li>
        <li style="margin-bottom: 15px; border-bottom: 1px dashed #d97706; padding-bottom: 10px;">
          <strong>Tech & Science Summit (2022)</strong><br>
          <em>"Algorithmic Approaches to Molecule Generation"</em>
        </li>
      </ul>
      <p style="font-style: italic; margin-top: 2rem;">(Swipe right for more...)</p>
    </div>
  </div>

  <!-- BLOCK 4: COLLABORATORS -->
  <div class="swipe-block block-collaborators">
    <div class="block-content">
      <h2 class="block-title">Collaborators</h2>
      <p>I have the pleasure of working with brilliant minds across the globe:</p>
      <div style="display: flex; justify-content: space-around; flex-wrap: wrap; margin-top: 2rem;">
        <div style="margin: 10px;">
          <div style="width: 80px; height: 80px; background: #3b82f6; border-radius: 50%; margin: 0 auto; display: flex; align-items: center; justify-content: center; font-size: 2rem;">👨‍🔬</div>
          <p>Dr. Smith</p>
        </div>
        <div style="margin: 10px;">
          <div style="width: 80px; height: 80px; background: #10b981; border-radius: 50%; margin: 0 auto; display: flex; align-items: center; justify-content: center; font-size: 2rem;">👩‍🔬</div>
          <p>Prof. Amina</p>
        </div>
        <div style="margin: 10px;">
          <div style="width: 80px; height: 80px; background: #f59e0b; border-radius: 50%; margin: 0 auto; display: flex; align-items: center; justify-content: center; font-size: 2rem;">👨‍💻</div>
          <p>Dev. Karim</p>
        </div>
      </div>
    </div>
  </div>

  <!-- BLOCK 5: BLOGS -->
  <div class="swipe-block block-blogs">
    <div class="block-content">
      <h2 class="block-title">Writings & Blogs</h2>
      <div style="text-align: left;">
        {% include latest_posts.liquid %}
      </div>
    </div>
  </div>

  <!-- BLOCK 6: CONTACTS -->
  <div class="swipe-block block-contacts">
    <div class="block-content">
      <h2 class="block-title">Get In Touch</h2>
      <p style="font-size: 1.2rem; margin-bottom: 2rem;">Let's collaborate and build something unique.</p>
      
      <p>📍 Lab 404, Science Block</p>
      <p>📧 <a href="mailto:issam.seddik@example.com" style="color: #38bdf8;">issam.seddik@example.com</a></p>
      
      <div style="margin-top: 3rem; font-size: 2rem;">
        <a href="#" style="margin: 0 10px; color: white;"><i class="fab fa-twitter"></i></a>
        <a href="#" style="margin: 0 10px; color: white;"><i class="fab fa-linkedin"></i></a>
        <a href="#" style="margin: 0 10px; color: white;"><i class="fab fa-github"></i></a>
      </div>
    </div>
  </div>

</div>

<!-- Small JavaScript to allow mouse-wheel horizontal scrolling -->
<script>
  const container = document.getElementById('swipe-container');
  container.addEventListener('wheel', (evt) => {
    // Only scroll horizontally if vertical scroll is less dominant
    if (Math.abs(evt.deltaY) > Math.abs(evt.deltaX)) {
      evt.preventDefault();
      container.scrollLeft += evt.deltaY;
    }
  });
</script>
