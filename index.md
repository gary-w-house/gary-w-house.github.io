---
permalink: /index.html
title: Gary W House
---

## [About](/about.html) | [Contact](/contact.html)

# Most Recent Posts

<ul class="entries">
  {% for post in site.posts limit:5 %}
  <li>
    <a href="{{ post.url }}"><h3>{{ post.title }}</h3></a>
    <p class="blogdate">{{ post.date | date: "%d %B %Y" }}</p>
    <div>{{ post.content |truncatehtml | truncatewords: 60 }}</div>
    
  </li>
  {% endfor %}
</ul>