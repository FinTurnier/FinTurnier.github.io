---
layout: page
title: Resume
eyebrow: Summary
lede: A structured overview of experience, education, and skills.
permalink: /resume/
---

## Experience

### Senior Software Engineer — Methods & Tools, Full-Stack Development
**Pratt & Whitney** · East Hartford, CT · Aug 2019 – Jan 2025

- Built, maintained, and improved a web application used to track engine repairs and parts.
- Developed applications driving migration of in-production digital maintenance,
  repair, and overhaul web tools to AWS cloud services.
- Drove deployment of an ingestion use case moving extracted data to AWS storage.
- Produced a turnaround-time monitoring method (incoming, approved, outgoing
  tasks) adopted to measure operational performance.

### Mechanical Engineer — Lubrication & Thermal Management Systems Analyst
**Pratt & Whitney** · East Hartford, CT · Jul 2016 – Aug 2019

- Owned fleet trending reports for PW1500G and PW1900G engines; reported fleet
  health to the System Integration Product Team during ramp-up.
- Analyzed lubrication and thermal system performance for NGPF development and
  fleet engines; produced thermal predictions within 5-degree accuracy using
  statistical models in MATLAB and Simulink.
- Supported PW1100G ground and flight testing aboard the flying testbed,
  informing leadership on critical engine component performance.
- Developed ad-hoc scripts to automate tasks and synthesize engine parameters
  for team decision-making.

### Mechanical Engineer — External Design, Producibility & Product Delivery
**Pratt & Whitney** · Nov 2017 – Feb 2019 (concurrent rotation)

- Conducted tolerance studies and interface checks; completed design phases for
  changes to external engine hardware.
- Resolved supplier producibility issues for critical external components;
  completed integration of redesigned Cold Fuel hardware.

### Design Engineer
**AL Farooq Corporation** · Miami, FL · May 2014 – Nov 2015

- Designed and evaluated glazing systems; consulted contractors on thermal
  properties, structural limits, and zoning regulations.
- Reduced cost via finite element analysis for preliminary structural
  assessments; verified thermal compliance with Florida Building Code energy
  requirements.

## Education

- **M.S. Computer Science** — Johns Hopkins University, 2025.
  Concentration: Database Systems and Knowledge Management.
- **B.S. Mechanical Engineering** — Florida International University, 2016.
- **Engineering Physics / Interdisciplinary Studies** — Embry-Riddle Aeronautical
  University, attended 2012.

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

## Organizations

- National Society of Black Engineers, FIU Chapter — Treasurer / Finance Chair
  (2014–2016); Algebra Project volunteer.

<p><a class="btn" href="mailto:{{ site.author.email }}">Request full PDF resume</a></p>
