---
layout: default
permalink: /news/
---

<h1>News</h1>

<div>
{% for post in site.posts %}
    {% if post.type != "news" %}
        {% continue %}
    {% endif %}
    {% include post.html post=post %}
{% endfor %}
</div>
