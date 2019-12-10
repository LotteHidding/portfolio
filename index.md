---
layout: base.njk
---

## Onderwijskrabbels

{% for post in collections.posts %}

<article>
  <header>
    <h3><a href="{{ post.url }}">{{ post.data.title }}</a></h2>
    <time>{{ post.date | date: "%Y-%m-%d" }}</time>
  </header>
  <p>{{ post.data.teaser }}</p>

</article>
{% endfor %}
