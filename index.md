---
layout: default
title: Home
---

<section class="hero">
  <p class="eyebrow">Software · Aerospace · Mechanical</p>
  <h1>Engineering from engine hardware to full-stack software.</h1>
  <p class="lede">
    I'm Finly Turnier — an engineer who started in aerospace and mechanical systems,
    spent years analyzing and designing jet engine hardware at Pratt &amp; Whitney,
    and now builds software full-time. This site collects my projects, notes,
    lessons, and the timeline that connects it all.
  </p>
  <div class="hero-actions">
    <a class="btn btn--solid" href="{{ '/projects/' | relative_url }}">View projects</a>
    <a class="btn" href="{{ '/timeline/' | relative_url }}">Career timeline</a>
    <a class="btn" href="{{ '/about/' | relative_url }}">About me</a>
  </div>
</section>

<section class="section">
  <p class="eyebrow">Selected work</p>
  <h2>Projects</h2>
  {% include card_grid.html collection="projects" limit=3 %}
  <p class="section-more"><a href="{{ '/projects/' | relative_url }}">All projects →</a></p>
</section>

<section class="section">
  <p class="eyebrow">Writing</p>
  <h2>Recent notes</h2>
  {% include card_grid.html collection="notes" limit=3 %}
  <p class="section-more"><a href="{{ '/notes/' | relative_url }}">All notes →</a></p>
</section>

<section class="section">
  <p class="eyebrow">The path</p>
  <h2>Timeline highlights</h2>
  {% include timeline.html %}
</section>
