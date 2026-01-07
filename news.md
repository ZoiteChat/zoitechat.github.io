---
layout: default
title: News
---

<div class="card">
  <h1 style="margin:.1rem 0 .6rem;">News</h1>
  <p class="lead" style="margin:0;">Release notes and project updates.</p>
</div>

<div class="card" style="margin-top:1rem;">
  {% if site.posts.size == 0 %}
    <p class="muted" style="margin:0;">No posts yet. Humans are clearly busy doing human things.</p>
  {% else %}
    <ul class="postlist">
      {% for post in site.posts %}
      <li class="postlist__item">
        <a class="postlist__title" href="{{ post.url | relative_url }}">{{ post.title }}</a>
        <div class="postlist__meta">{{ post.date | date: "%B %d, %Y" }}</div>
        {% if post.excerpt %}<div class="postlist__excerpt">{{ post.excerpt | strip_html | strip_newlines }}</div>{% endif %}
      </li>
      {% endfor %}
    </ul>
  {% endif %}
</div>

<div class="card" style="margin-top:1rem;">
  <p style="margin:0;" class="muted">Subscribe via <a href="{{ "/atom.xml" | relative_url }}">Atom</a>.</p>
</div>
