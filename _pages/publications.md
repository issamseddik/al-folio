---
layout: page
permalink: /publications/
title: Publications
nav: true
nav_order: 2
---

<style>
  .post-header { display: none; }
  /* Remove the top border only for the very first year group */
  .publications h2.year:first-of-type {
    border-top: none !important;
    margin-top: 0 !important;
  }
</style>

<!-- _pages/publications.md -->

<!-- Bibsearch Feature -->

{% include bib_search.liquid %}

<div class="publications">

{% bibliography %}

</div>
