---
title: Navigation
---


{% for document in site.navigation %}
<h1>
<a href="#{{ document.title | slugify }}">{{ document.title }}</a>
</h1>
{% endfor %}

{% for document in site.navigation %}
<article id="{{ document.title | slugify }}" class="test">
        {{ document.content }}
</article>
{% endfor %}