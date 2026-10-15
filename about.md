---
layout: page
title: About
eyebrow: Profile
lede: An engineer whose versatility comes from a broad technical skill set — and from learning quickly in multidisciplinary teams.
permalink: /about/
---

## Background

I am an engineer with experience spanning mechanical, aerospace, and software
engineering. My career began in physical systems — glazing design, jet engine
thermal and lubrication analysis, external hardware design — and moved
deliberately toward software: full-stack web applications, cloud migration,
and data pipelines at Pratt &amp; Whitney, followed by an M.S. in Computer
Science at Johns Hopkins with a concentration in database systems and
knowledge management.

That path gives me an unusual working range: I can reason about a bearing
compartment seal and about the ingestion pipeline that reports on it.

## Skills

<div class="skills-groups">
{% for group in site.data.skills %}
  <div class="skill-group">
    <h3>{{ group.group }}</h3>
    <ul>
      {% for item in group.items %}<li>{{ item }}</li>{% endfor %}
    </ul>
  </div>
{% endfor %}
</div>

## Education

- **M.S. Computer Science**, Johns Hopkins University (2025) — concentration in
  Database Systems and Knowledge Management
- **B.S. Mechanical Engineering**, Florida International University (2016)
- **Engineering Physics / Interdisciplinary Studies**, Embry-Riddle Aeronautical
  University (attended 2012)

## Beyond work

Treasurer and Finance Chair for the National Society of Black Engineers (FIU
chapter, 2014–2016), and volunteer with the Algebra Project, an initiative
preparing students for college mathematics.
