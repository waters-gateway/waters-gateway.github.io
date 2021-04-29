---
layout: page
permalink: /about/
title: "About"
show_title: false
lang: en
---

<!-- {% include image.html url="/images/GTR-Palmenhaus-400px.jpg" width=200 style="float:right" %} -->

Our project focusses on the stomata, tiny pores on the surface of plant leaves. Stomata play a central role in global water and carbon cycles while covering less than 5% of the leaf surface. Stomata open and close to provide CO<sub>2</sub> for photosynthesis and to limit water loss, but this process varies in speed and dynamism between different species and phenotypes, as well as under fluctuating environmental conditions, like under changing light or humidity. The speed at which stomata respond influences the productivity and water use of both crops and natural ecosystems.

In this project, we will use novel temporal 3D imaging to provide a better description of stomatal movements in order to get a mechanistic undertanding of how transient stomatal movement. To fully harness the high volume of 3D imaging data, we will develop novel computational methods to automatically segment images and track single 3D cells over time. This project will answer long-standing questions about stomatal movements and will generate basic knowledge on how to improve stomatal responses under dynamic environments in order to increase net productivity and water-use efficiency.

---

{% for theme in site.data.people %}
<h2>{{ theme.title }}</h2>
{% for person in theme.subsection %}
<div class="toc">
<img src="{{ person.avatar }}" alt="{{ person.person | smartify }}" class="avatar" style="width:200px" />
<a href="{{ person.url }}">{{ person.person | markdownify }}</a>
<p>{{ person.snippet | markdownify }}</p>
</div>
{% endfor %}
{% endfor %}

<!-- Core members in this people are:  
  [Guillaume Théroux-Rancourt (University of Natural Resources and Life Sciences, Vienna (BOKU)](http://gtrancourt.gitlab.io)  
  [Danny Tholen (BOKU)](https://scholar.google.com/citations?user=iQUjOxAAAAAJ&hl=en&num=20&oi=ao)  
  [Ingeborg Lang (University of Vienna)](https://scholar.google.com/citations?user=8tzh90wAAAAJ&hl=en&num=20&oi=ao)  
  [Walter Kropatsch and Jiří Hladůvka (TU Wien)](https://www.prip.tuwien.ac.at/)  

With collaborators:  
  [Anja Geitmann (plant cell biologist, McGill University)](https://www.plantbiomechanics.net/)  
  [Anne Bonnin (radiation physicist, Swiss Light Source)](https://www.psi.ch/en/x-ray-tomography-group/people/anne-bonnin)
 -->