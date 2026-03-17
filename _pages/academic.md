---
layout: page
permalink: /academic/
title: academic
description: Academic service, teaching, talks, and research visits.
nav: true
nav_order: 4
---

## Academic Service

- Reviewer: ICML 2024, NeurIPS 2024, AAAI 2025, TMLR, ICLR 2025, ICML 2025, ICML 2026
- Organizer: Diffusion models reading group, INRIA Paris (2025)
- Organizer: Sakana AI research retreat (2025)


## Research Visit

**Universita di Padova**  
Departments of Mathematics and Physics & Astronomy, Italy (March 2025)

Initiated a joint mathematics/physics project on diffusion-based generative models for cosmology with Giovanni Conforti.


## Teaching

{% assign teachings = site.teachings | sort: 'year' | reverse %}

<div class="table-responsive">
  <table class="table table-sm">
    <thead>
      <tr>
        <th>Period</th>
        <th>Role</th>
        <th>Institution</th>
      </tr>
    </thead>
    <tbody>
      {% for t in teachings %}
        <tr>
          <td>{{ t.term }}</td>
          <td>{{ t.title }}</td>
          <td>{{ t.location }}</td>
        </tr>
      {% endfor %}
    </tbody>
  </table>
</div>

## Selected Talks

{% assign talks = site.talks | sort: 'date' | reverse %}

<div class="table-responsive">
  <table class="table table-sm">
    <thead>
      <tr>
        <th>Date</th>
        <th>Talk</th>
        <th>Venue</th>
        <th>Location</th>
      </tr>
    </thead>
    <tbody>
      {% for talk in talks %}
        <tr>
          <td>{{ talk.date | date: "%b %Y" }}</td>
          <td>{{ talk.title }}</td>
          <td>{{ talk.venue }}</td>
          <td>{{ talk.location }}</td>
        </tr>
      {% endfor %}
    </tbody>
  </table>
</div>



## Selected Workshops and Schools

<div class="table-responsive">
  <table class="table table-sm">
    <thead>
      <tr>
        <th>Event</th>
        <th>Date</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>Summer School on Fundamentals and Applications of Diffusion Models, Alan Turing Institute / Isaac Newton Institute, London</td>
        <td><em>June 2024</em></td>
      </tr>
      <tr>
        <td>Mini-Workshop: Statistical Challenges for Deep Generative Models, Oberwolfach</td>
        <td><em>February 2025</em></td>
      </tr>
      <tr>
        <td>Machine Learning Winter School: Representation Learning &amp; GenAI, MBZUAI, Abu Dhabi</td>
        <td><em>February 2026</em></td>
      </tr>
    </tbody>
  </table>
</div>
