---
layout: inner
title: Brands
description: 'Please find below an overview of our most popular brands.'
permalink: /brands/
---

{% for brand in site.data.brands %}
<div class="brand">
    {% if brand.url %}
        <a href="{{ brand.url }}"><img src="{{ brand.image }}" alt="{{ brand.name }} - {{ brand.description }}"></a>
    {% else %}
        <img src="{{ brand.image }}" alt="{{ brand.name }} - {{ brand.description }}">
    {% endif %}
</div>
{% endfor %}
