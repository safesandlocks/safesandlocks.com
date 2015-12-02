---
layout: inner
title: Brands
description: 'Please find below an overview of our most popular brands.'
permalink: /brands/
---

<div class="row brands">
    {% for brand in site.data.brands %}
    <div class="col-xs-12 col-md-3 brand">
        <div class="thumbnail-container">
            {% if brand.url %}
                <a class="thumbnail" href="{{ brand.url }}"><img src="{{ brand.image }}" alt="{{ brand.name }} - {{ brand.description }}"></a>
            {% else %}
                <img class="thumbnail" src="{{ brand.image }}" alt="{{ brand.name }} - {{ brand.description }}">
            {% endif %}
        </div>
    </div>
    <div class="clear"></div>
    {% endfor %}
</div>