---
permalink: /
title: "Bio"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a 3rd and final year PhD student at INRIA Paris ([Sierra Project team](https://sierra-mlopt.github.io), led by [Francis Bach](https://www.di.ens.fr/~fbach/)). I am working under the supervision of [Umut Simsekli](https://www.di.ens.fr/umut.simsekli/) and [Alain Durmus](https://alain.perso.math.cnrs.fr). 

Before that, I obtained an MSc in Mathematics from the University of Oxford, and a BSc/MSc from Ecole Polytechnique. More information about professional and academic experiences can be found in my [CV](/files/dario_resume.pdf).

**Join our reading group on diffusion models** I am co-organising a discussion-based reading group on *generative models, diffusion models and related topics* in Inria Paris, taking place once every 2-3 weeks. If you would like to join just send me an e-mail. 
- [Here](https://docs.google.com/document/d/1XxFj70hNiBjkjQEWdlCd2U499FIhGfAiaW9Ud5xz_tE/edit?usp=sharing) is a selection of relevant articles to inspire presentations and discussions
- [Here](https://docs.google.com/document/d/1sjmmSj1XZW126yRTvy56WnQnU8vZqqdKuOVbKOXXjXw/edit?usp=sharing) is a schedule of upcoming sessions and potential topics.

{% assign preprint_posts = site.publications | where: "category", "preprints" %}
{% if preprint_posts.size > 0 %}
# Preprints

<ul>{% for post in preprint_posts reversed %}
  {% include archive-single-cv.html %}
{% endfor %}</ul>
{% endif %}

# Publications
<ul>{% for post in site.publications reversed %}
  {% if post.category == "conferences" %}
    {% include archive-single-cv.html %}
  {% endif %}
{% endfor %}</ul>

{% if site.features.show_news %}
# News

{% assign news_items = site.news | sort: "date" | reverse %}
<ul class="news-list" style="font-size: 0.8em;">
{% for item in news_items %}
  <li><strong>{{ item.date | date: "%b %d, %Y" }}:</strong> {{ item.excerpt | default: item.content | markdownify | strip_html }}</li>
{% endfor %}
</ul>
{% endif %}
