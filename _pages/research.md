---
title: "Research"
layout: single
permalink: /research/
author_profile: true
toc: true
toc_icon: fa-solid fa-bookmark
toc_label: RESEARCH
toc_sticky: true
---

## Papers

{% assign sorted_papers = site.papers | sort: 'date' | reverse %}
{% for pub in sorted_papers %}
- **{{ pub.title }}**
  <br>{{ pub.authors }}
  <br> ({{ pub.date | date: "%Y" }})
  <br>In _{{ pub.journal }}_ [<i class="fas fa-external-link-alt"></i>]({{ pub.link }})
{% endfor %}


## Abstracts
{% assign sorted_abstracts = site.abstracts | sort: 'date' | reverse %}
{% for pub in sorted_abstracts %}
- **{{ pub.title }}**
  <br>{{ pub.authors }}
  <br> ({{ pub.date | date: "%Y" }})
  <br>In _{{ pub.venue }}_ [<i class="fas fa-external-link-alt"></i>]({{ pub.link }})
{% endfor %}

## Patents

{% assign sorted_patents = site.patents | sort: 'issue_date' | reverse %}
{% for pat in sorted_patents %}
- **{{ pat.title }}**
  <br>{{ pat.authors }}
  <br> _U.S. Patent No._ {{pat.patent_no}} [<i class="fas fa-external-link-alt"></i>]({{ pat.link }})
  <br> Filed {{ pat.file_date | date: "%Y-%m-%d" }}
  <br> Issued {{ pat.issue_date | date: "%Y-%m-%d" }}
{% endfor %}
