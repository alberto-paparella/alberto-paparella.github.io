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
* Visiting Ph.D student, University of Queensland, 2024
* M.S. in Computer Science, University of Bologna, 2023
* B.S. in Computer Science, University of Ferrara, 2021

Work experience
======
* 2023.02 - 2023.07: Intership at University of Bologna
  * Department of Computer Science and Engineering, University of Bologna
  * Duties includes: study of the application of Probabilistic Diffusion Models to
    Precipitation Nowcasting
  * Supervisor: Andrea Asperti
* 2021.03 - 2021.09: Intership at Applied Computational Logic and Artificial Intelligence
  Lab
  * Department of Mathematics and Computer Science, University of Ferrara
  * Duties included: development of an open source Laravel package for rule extraction from
    MySQL databases, which has been applied for the creation of a rule-based system targeted
    at physicians of the Menopause and Osteoporosis Center (CMO) in Ferrara for treatment
    suggestion based on previous successful choices of the physician for similar patients 
  * Supervisor: Guido Sciavicco
  
Skills
======
* Coding
  * Julia
  * Python
  * MATLAB
  * C
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
  
Service and leadership
======
* 10.2019 - 9.2021: Student Representative in the Joint Commitee (Commissione Paritetica) of
  the Department of Mathematics and Computer Science at the University of Ferrara
* 10.2018 - 9.2021: Student Representative for Bachelor students at the University of
  Ferrara
