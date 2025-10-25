---
layout: simple
title: Michael Nath
permalink: /
subtitle: hacking science for the everyday person
---

My life's work involves collaborating with brilliant people everyday, building incredible technologies that propel humanity to wonderful, unimaginable realms. Everything I do plays a part in advancing this chief interest in our world.

I am currently an AI engineer & researcher at <span class="gold-bold">Jump Trading</span>, based out of my hometown of New York City. If you'd like to grab a coffee, please reach out!

### Quick Facts

- Proud <span class="gold-bold">Stuyvesant</span> & <span class="gold-bold">Stanford</span> alum
- Concentrated in systems (BS) & artificial intelligence (MS).
- Avid table tennis player (can find me practicing @ PingPod)
- Love the cold (favorite place I've been to is <span class="frost-text">Lofoten, Norway</span>)

## Writings

<ul class="writing-list">
  {% if site.posts and site.posts != empty %}
    {% for post in site.posts %}
      <li>
        <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        <span class="date">{{ post.date | date: "%B %Y" }}</span>
      </li>
    {% endfor %}
  {% else %}
    <li>No writings yet. Check back soon.</li>
  {% endif %}
</ul>
