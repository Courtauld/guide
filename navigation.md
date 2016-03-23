---
title: Navigation
---

<nav class="document-nav">
<ul>
{% for document in site.navigation %}
<li><a href="#{{ document.title | slugify }}">{{ document.title }}</a>
</li>
{% endfor %}
</ul>
</nav>
<div class="document-wrap">
{% for document in site.navigation %}
<article id="{{ document.title | slugify }}" class="test">
        {{ document.content }}
</article>
{% endfor %}
</div>