---
title: Navigation
---


{% for document in site.navigation %}
<article>
<h1>{{ document.title }}</h1>
<p>{{ document.excerpt }}</p>
<a href="{{ document.url }}">Link</a>
</article>
{% endfor %}