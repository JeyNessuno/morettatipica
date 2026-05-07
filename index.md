---
layout: default
title: Home
---

# Welcome

## Posts

<ul>
{% raw %}{% for post in site.posts %}{% endraw %}
  <li>
    <a href="{{ post.url }}">
      {{ post.title }}
    </a>
  </li>
{% raw %}{% endfor %}{% endraw %}
</ul>