---
layout: about
title: About
nav: false
permalink: /
subtitle: AGI/AI Safety Researcher

profile:
  align: left
  image: new_prof_pic.png
  image_circular: true # ensures the image is a circle
  more_info: >
    <p>CEA LIST</p>
    <p>Université Paris-Saclay</p>
    <p>Palaiseau, France</p>

announcements:
  enabled: false
---

<style>
  .profile {
    width: 200px;
    margin-right: 40px !important;
  }
  .more-info p {
    font-size: 0.85rem;
    margin-bottom: 0.2rem;
    line-height: 1.2;
    color: var(--global-text-color);
    opacity: 0.8;
  }
  ul {
    padding-left: 0 !important;
    margin-left: 0 !important;
    list-style-position: inside; /* Puts the bullets in line with the text */
  }
  li {
    margin-bottom: 0.5rem; /* Adds nice vertical space between items */
  }
  .news table th, .news table td {
    padding-left: 0 !important; /* Forces the news table to perfectly align left with the lists above */
  }
</style>

I am a researcher specializing in **Machine Learning**, **Cybersecurity**, and **Large Language Models (LLMs)** at CEA LIST and Université Paris-Saclay. 

My current work primarily explores the vulnerabilities of AI systems, specifically focusing on the mechanics of **Neural Network Backdoors**. I investigate how backdoors can be absorbed during community training and design robust detection mechanisms, such as Proof-of-Training-Steps (POTS), to secure LLMs against malicious manipulations.

### Research Interests
- **Security of Large Language Models**
- **Backdoor Attacks and Defenses in Deep Learning**
- **Distributed and Collaborative Training Security**

### News
<div class="news">
  {% include news.liquid limit=true %}
</div>
