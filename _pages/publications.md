---
title: Publications
permalink: /publications/
---

## Journal Articles

{% assign journal_papers = site.publications | where: "type", "journal" | sort: "date" | reverse %}
{% for post in journal_papers %}
  {% include archive-single-publication.html %}
{% endfor %}

## Conference Proceedings

{% assign conference_papers = site.publications | where: "type", "conference" | sort: "date" | reverse %}
{% for post in conference_papers %}
  {% include archive-single-publication.html %}
{% endfor %}
