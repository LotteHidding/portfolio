---
layout: base.njk
---

## Onderwijskrabbels

{% for post in collections.posts%}
<a href="{{ post.url }}">

  <article>
      <header>
        <h3>{{ post.data.title }}</h3>
        <time>{{ post.data.date | date: "%d-%m-%Y" }}</time>
      </header>
      <p>{{ post.data.description }}</p>
  </article>
</a>
{% endfor %}
