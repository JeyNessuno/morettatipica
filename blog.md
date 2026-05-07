---
layout: default
title: Blog
permalink: /blog/
---

# Il blog della Ciliegia Moretta di Vignola

Storie di campo, ricette tradizionali e aggiornamenti dal presidio: leggi gli articoli pubblicati dai produttori.

---

{% if site.posts.size > 0 %}
  {% for post in site.posts %}
    <div style="margin-bottom: 40px; padding: 20px; border: 1px solid #ddd; border-radius: 8px;">
      <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
      <p style="font-size: 0.9rem; color: #666;">
        <span style="font-weight: bold;">📅 {{ post.date | date: "%d %B %Y" }}</span>
      </p>
      <p>{{ post.excerpt | strip_html | truncatewords: 50 }}</p>
      <p><a href="{{ post.url }}">Leggi l'articolo completo →</a></p>
    </div>
  {% endfor %}
{% else %}
  <p>Nessun articolo pubblicato ancora. Torna a trovarci presto!</p>
{% endif %}
