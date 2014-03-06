---
layout: page
title: prsolans
tagline: Onward and Upward
---

*We'll just see how long this lasts.*
    
### Posts

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

### To-Do

Keep doing it!


