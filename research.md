---
layout: default
permalink: /research/
title: "Research"
lang: en
---

Our research project link plant biology and anatomy to image analysis and pattern recognition to leverage time-resolved 3D images of plant leaves responding to dynamic environmental changes. Here is a list of some of our ongoing and completed projects.

<!-- Automated list generator -->

{% for theme in site.data.projects %}
<h2>{{ theme.title }}</h2>
{% for project in theme.subsection %}
<div class="toc">
<img src="{{ project.avatar }}" alt="{{ project.project | smartify }}" class="avatar" style="width:200px" />
<a href="{{ project.url }}">{{ project.project | markdownify }}</a>
<p>{{ project.snippet | markdownify }}</p>
</div>
{% endfor %}
{% endfor %}
