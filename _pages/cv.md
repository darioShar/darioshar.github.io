---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

Here is my full [CV](/files/dario_resume.pdf).

# Education

* **PhD Student**, *INRIA, Paris*, October 2023 - now
* **MSc in Mathematics (Distinction)**, *University of Oxford, United Kingdom*, 2022 - 2023
* **MSc in Applied Mathematics**, *Ecole Polytechnique, France*, 2019 - 2022
* **Preparatory Program MPSI/MP**, *Lycee Saint-louis, Paris, France*, 2017 - 2019

# Work Experience

* **Quantitative research intern**, *Squarepoint Capital, London, United Kingdom*, March-August 2022
* **Firmware engineer intern**, *Ledger, Paris, France*, June-September 2021
* **R&D intern**, *Gendarmerie Elite Unit (GIGN), Versailles, France*, November-April 2020


# Publications
  <ul>{% for post in site.publications reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
# Talks
  <ul>{% for post in site.talks reversed %}
    {% include archive-single-talk-cv.html  %}
  {% endfor %}</ul>
  
# Teaching
  <ul>{% for post in site.teaching reversed %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
