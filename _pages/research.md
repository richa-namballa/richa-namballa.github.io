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

<!-- ### Presentations

* Simões Maia, Lucas. Namballa, Richa. Rocamora, Martín. Fuentes, Magdalena. Guedes, Carlos. "Characterizing Audio Problems in a Large Dataset of Field Recordings for Computational Analysis". Presentation delivered at the 8th International Conference on Analytical Approaches to World Musics. June 11, 2024. Bologna, Italy.
* Wu, Cecilia. Namballa, Richa. Mazurek Mary. "Advancing DEI in AES: A Pilot Analysis of AES Convention Participants Data". Presentation delivered at the 155th Audio Engineering Convention hosted by the Audio Engineering Society. October 25, 2023.
* Wu, Cecilia. Mazurek, Mary. Wyner, Jonathan. Loiacono, Eleanor T. Hill, Lucas. Namballa, Richa. “Moving Forward: AES DE&I Data Collection Task Force Initiative”. Panel discussion at the 153rd Audio Engineering Convention hosted by the Audio Engineering Society. October 26, 2022. Online.
* Namballa, Richa. Muñoz Vidal, Eva Luna. Ripollés, Pablo. “CHILLER 2.0”. Poster presented at the Society for Music Perception and Cognition. August 4, 2022. Portland, OR, USA. [View Poster Here.](https://drive.google.com/file/d/1HixiwcntK9mD1jgWOiL0oRPiYgYzbrpr/view?usp=share_link)
* Namballa, Richa. Bhargava, Shruti. “Like a Pro: Making Your Data Science Code Production-Ready”. Presentation delivered at the 3rd Women in Data Science Silicon Valley @ SAP Conference. June 4, 2020. Online.
* Li, Yue. Namballa, Richa. Bhargava, Shruti. “Active Learning Strategies for Extracting Product At- tributes using Deep Neural Networks”. Poster presented at the 13th Women in Machine Learning Work- shop co-located with NeurIPS. December 3, 2018. Montreal, Quebec, CA.
* Namballa, Richa. “Getting Started with SAP Leonardo Machine Learning”. Presentation delivered at the Women in Big Data Democratizing AI event co-hosted by Women in Technology at SAP. June 14, 2018. Palo Alto, CA, USA. -->