---
layout: page
navigation_title: Organizers
title: The Organizers
cover: '/assets/images/banner.png'
permalink: /organizers/
---

<div class="home">

<ul>
{% for organiser in site.data.organisers %}
 <a >
  <div class="event-sqaure" style="background-image:url({{organiser.photo}});">
  <h2><span>
  {{organiser.name}}<br>
  ({{organiser.affiliation}})
  </span></h2>
  <div class='event-square-overlay'></div>
  </div>

</a>

{% endfor %}
</ul>

</div>
