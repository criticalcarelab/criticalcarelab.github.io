---
title: Publications
nav:
  order: 2
  tooltip: "Peer-reviewed papers, software, datasets, and lab outputs"
---

# {% include icon.html icon="fa-solid fa-wrench" %}Publications

Welcome to the Critical Care Research Lab’s publications page. Here you’ll find our peer-reviewed journal articles, conference presentations, and other research outputs, including software and datasets. Our work focuses on the microvascular physiology of sepsis and critical illness, with an emphasis on developing innovative monitoring tools and translational models to improve patient care.

We are committed to advancing knowledge and open science. For questions about our research or collaboration opportunities, please reach out through our [faculty contact page](https://umanitoba.ca/medicine/faculty-staff/asher-mendelson).

{% include tags.html tags="publications, journal papers, conferences, abstracts, datasets, software" %}

## Search & Filter

{% include search-info.html %}


{% include section.html %}

## Featured Publications

{% assign featured_pubs = site.publications | where: "group", "featured" | sort: "year" | reverse %}
<div class="featured-publications">
  {% for pub in featured_pubs %}
    <div class="pub-card">
      <h3>{{ pub.title }}</h3>
      <p>
        <strong>{{ pub.authors }}</strong> <br />
        {{ pub.publication }}{% if pub.year %}, {{ pub.year }}{% endif %}{% if pub.doi %} • <a href="{{ pub.doi }}" target="_blank">DOI</a>{% endif %}
      </p>
      {% if pub.summary %}
        <p>{{ pub.summary }}</p>
      {% endif %}
    </div>
  {% endfor %}
</div>

---

## All Publications

Below is a chronological list of all lab publications.

{% assign all_pubs = site.publications | sort: "year" | reverse %}
<ul class="publication-list">
  {% for pub in all_pubs %}
    <li>
      <strong>{{ pub.title }}</strong> ({{ pub.year }})<br/>
      {{ pub.authors }}.<br />
      <em>{{ pub.publication }}</em>
      {% if pub.doi %}&bull; <a href="{{ pub.doi }}" target="_blank">DOI</a>{% endif %}
      {% if pub.pdf %}&bull; <a href="{{ pub.pdf }}" target="_blank">PDF</a>{% endif %}
      {% if pub.data %}&bull; <a href="{{ pub.data }}" target="_blank">Data</a>{% endif %}
    </li>
  {% endfor %}
</ul>
