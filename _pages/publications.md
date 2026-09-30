---
layout: page
permalink: /publications/
title: Publications
nav: true
nav_order: 2
---

<style>
  .post-header { display: none; }
  .publications h2.year, 
  .publications h2, 
  h2.year {
    border-top: none !important;
  }
  hr { display: none !important; }
</style>

<!-- _pages/publications.md -->

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

<div class="publications">

{% bibliography %}

</div>
