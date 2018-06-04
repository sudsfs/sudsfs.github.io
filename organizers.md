---
layout: page
navigation_title: Organizers
title: The Organizers
cover: 'http://www.deesidebusinessforum.co.uk/wp-content/uploads/2016/10/conference.jpg'
permalink: /organizers/
---

<div class="home">

<ul>
{% for organiser in site.data.organisers %}
 <a >
  <div class="event-sqaure" style="background-image:url({{organiser.photo}});">
  <h2>{{ post.title }} <span>
  {{organiser.name}}<br>
  ({{organiser.affiliation}})
  </span></h2>
  <div class='event-square-overlay'></div>
  </div>

</a>

{% endfor %}
</ul>

</div>
