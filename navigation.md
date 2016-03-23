---
title: Navigation
layout: default
---

<nav class="document-nav">
<ul>
{% for document in site.navigation %}
<li ><a href="#{{ document.title | slugify }}">{{ document.title }}</a>
</li>
{% endfor %}
</ul>
</nav>
<div class="document-wrap">
{% for document in site.navigation %}
<article id="{{ document.title | slugify }}" class="test">
    <span>{{ collection.label }} &#8593;</span><h1>{{ document.title }}</h1>
    {{ document.content }}
</article>
{% endfor %}
</div>