---
layout: base.njk
---

## Onderwijskrabbels van Lotte

{% for post in collections.posts %}
<a href="{{ post.url }}">

  <article>
      <header>
        <h3>{{ post.data.title }}</h3>
        <time>{{ post.date | date: "%d-%m-%Y" }}</time>
      </header>
      <p>{{ post.data.teaser }}</p>
  </article>
</a>
{% endfor %}
