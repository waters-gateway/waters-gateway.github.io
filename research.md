---
layout: default
permalink: /research/
title: "Research"
lang: en
---

Plant leaves are key components to the global carbon and water cycle, as virtually all carbon going from the atmosphere to terrestrial ecosystems passes through them, as well as ~70% of all terrestrial evapotranspiration. Ecophysiological research has primarily focused on how stomata and mesophyll cells respond to changes in their environmental conditions. However, there is a large intercellular airspace between the stomata and the mesophyll cells, and this space has most often been overlooked.  
My current research focusses on plant structure and function relationship. I study leaf anatomy, both in 2- and 3D, in relation to photosynthesis, transpiration, and other diffusive processes along the path from the stomata to the chloroplast stroma. This research combines anatomical and ecophysiological measurements, as well as modeling.

Here is a selection of published papers from my two current research topics, as well as other projects I am or was involved. Full publication listing, with links to the full text when available, on the [_Publications_](/publications/) page.


<!-- Automated list generator -->

{% for theme in site.data.projects %}
<h2>{{ theme.title[site.active_lang] }}</h2>
{% for project in theme.subsection %}
<div class="toc">
<img src="{{ project.avatar }}" alt="{{ project.paper | smartify }}" class="avatar" style="width:200px" />
<a href="{{ project.url }}">{{ project.paper | markdownify }}</a>
<p>{% if site.active_lang == "en" %}{{ project.snippet.en | markdownify }}{% else %}{{ project.snippet.fr | markdownify }}{% endif %}</p>
</div>
{% endfor %}
{% endfor %}
