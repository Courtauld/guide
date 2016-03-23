---
title: Navigation
---


{% for document in site.navigation %}
<article>
<h1>
<a href="{{ document.url | prepend: site.baseurl | prepend: site.url }}">{{ document.title }}</a>
</h1>
    <div id="{{ document.title | slugify }}" class="test">
        {{ document.content }}
    </div>
</article>
{% endfor %}