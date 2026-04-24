---
layout: default
title: CineeManch Video Archive
---

# 🎬 CineeManch Video Archive
Welcome to the official home for our technical cinema breakdowns and movie reviews.

---

### Latest Reviews & Analysis
{% for post in site.posts %}
<div style="margin-bottom: 30px; border-left: 4px solid #d32f2f; padding-left: 15px;">
  <h2 style="margin-top: 0;">
    <a href="{{ post.url }}">{{ post.title }}</a>
  </h2>
  <p style="margin: 5px 0;"><strong>CineeManch Rating:</strong> ⭐ {{ post.rating }}/10</p>
  <p><em>{{ post.description }}</em></p>
  <a href="{{ post.url }}" style="font-weight: bold;">Watch Video & Read Analysis →</a>
</div>
{% endfor %}
