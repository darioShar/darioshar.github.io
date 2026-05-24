---
layout: page
permalink: /talks/
title: talks
description: Talks and presentations.
nav: false
nav_order: 4
---

{% assign talks = site.talks | sort: 'date' | reverse %}

| Date | Title | Venue | Location |
| ---- | ----- | ----- | -------- |

{% for talk in talks %}
| {{ talk.date | date: "%b %d, %Y" }} | {{ talk.title }} | {{ talk.venue }} | {{ talk.location }} |
{% endfor %}
