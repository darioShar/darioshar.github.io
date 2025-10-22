---
layout: archive
title: "News"
permalink: /news/
author_profile: true
collection: news
---

{% include base_path %}

{% if site.features.show_news %}
  {% assign news_items = site.news | sort: "date" | reverse %}
  {% for item in news_items %}
    {% assign post = item %}
    {% include archive-single.html %}
  {% endfor %}
{% else %}
  <p>News updates are currently hidden.</p>
{% endif %}
