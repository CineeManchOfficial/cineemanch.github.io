---
layout: default
title: CineeManch Home
---
# Welcome to CineeManch
The official home for movie reviews and cinema analysis. 

### Latest Reviews
{% for post in site.posts %}
* [{{ post.title }}]({{ post.url }}) — ⭐ {{ post.rating }}/10
{% endfor %}
