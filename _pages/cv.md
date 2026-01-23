---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Education
======
* Ph.D in Mathematics, University of Ferrara, 2026 (expected)
* Visiting Ph.D student, University of Queensland, 2024, 2025
* M.S. in Computer Science, University of Bologna, 2023
* B.S. in Computer Science, University of Ferrara, 2021
  
Skills
======
* Coding
  * Julia
  * C/C++
  * Python
  * MATLAB
* Artificial Intelligence
  * Symbolic Machine Learning
  * Interpretable AI
* Logics and Mathematics
  * Modal Logic
  * Many-Valued Logic
  * Automated Theorem Proving

Publications
======

<ul>{% for post in site.publications reversed %}
  {% include archive-single-cv.html %}
{% endfor %}</ul>
  
Talks
======

<ul>{% for post in site.talks reversed %}
  {% include archive-single-talk-cv.html  %}
{% endfor %}</ul>
  
Teaching
======
<ul>{% for post in site.teaching reversed %}
  {% include archive-single-cv.html %}
{% endfor %}</ul>
