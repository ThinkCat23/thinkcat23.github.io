---
layout: default
title: Home
---

<h1>My Notes</h1>


<ul>
{% for category in site.categories %}
  <h1 style = "font-size: 150%; color: black"><a name="{{ category | first }}">{{ category | first }}</a></h1>
    <ul>
    {% for post in category.last %}
    <b><a href="{{ post.url }}">{{ post.title }}</a></b>
    {% endfor %}
    </ul>
{% endfor %}
</ul>
