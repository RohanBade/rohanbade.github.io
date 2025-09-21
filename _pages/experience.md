---
title: Experience
layout: default
permalink: "/experience/"
---

{% for experience in site.experience %}

<div class="ap-experience">
    <p class="ap-experience-title">{{experience.title}}, <a href="{{experience.institute-url}}">{{experience.institute}}</a></p>
    <p class="ap-experience-year">{{experience.duration}}</p>
    <p class="ap-experience-excerpt">{{experience.excerpt}}</p>
    <p class="ap-experience-tags">
        {% for tag in experience.tags %}
        <span class="ap-experience-chip">{{tag}}</span>
        {% endfor %}
    </p>
</div>
{% endfor %}
