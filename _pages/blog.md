---
layout: inner
title: Blog
permalink: /blog/
---

{% for post in paginator.posts %}
    {% include post-preview.html %}
{% endfor %}

{% include pagination.html %}
