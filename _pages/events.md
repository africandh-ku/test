---
layout: single
title: Events
permalink: events
header:
  image: /assets/cover-images/header-sea-1280x200.jpg
---



<div id="posts">
  <ul>
    {% for post in site.posts %}
       {% if post.category == "event" %}
      <li><span>{{ post.date | date_to_string }}</span> - <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
      {% endif %}
{% endfor %}
  </ul>
</div>
