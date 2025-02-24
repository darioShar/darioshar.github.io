---
permalink: /
title: "Bio"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a 2nd year PhD student at INRIA Paris ([Sierra Project team](https://sierra-mlopt.github.io), led by Francis Bach). I am working under the supervision of [Umut Simsekli](https://www.di.ens.fr/umut.simsekli/) and [Alain Durmus](https://alain.perso.math.cnrs.fr). 

Before that, I obtained an MSc in Mathematics from the University of Oxford, and a BSc/MSc from Ecole Polytechnique. More information about professional and academic experiences can be found in my [CV](/files/dario_resume.pdf).

**Join our reading group on diffusion models** I am co-organising a discussion-based reading group on *generative models, diffusion models and related topics* in Inria Paris, taking place once every 2-3 weeks. If you would like to join just send me an e-mail. 
- [Here](https://docs.google.com/document/d/1XxFj70hNiBjkjQEWdlCd2U499FIhGfAiaW9Ud5xz_tE/edit?usp=sharing) is a selection of relevant articles to inspire presentations and discussions
- [Here](https://docs.google.com/document/d/1sjmmSj1XZW126yRTvy56WnQnU8vZqqdKuOVbKOXXjXw/edit?usp=sharing) is a schedule of upcoming sessions and potential topics.


# Preprints

<ul>{% for post in site.publications reversed %}
  {% if post.category == "preprints" %}
    {% include archive-single-cv.html %}
  {% endif %}
{% endfor %}</ul>

# Publications
<ul>{% for post in site.publications reversed %}
  {% if post.category == "conferences" %}
    {% include archive-single-cv.html %}
  {% endif %}
{% endfor %}</ul>