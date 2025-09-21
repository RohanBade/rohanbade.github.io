---
title: Education
layout: default
permalink: "/education/"
---

{% for education in site.education %}

<div class="ap-education">
    <p class="ap-education-degree">{{education.degree}}</p>
    <p class="ap-education-institute">{{education.institute}}</p>
    <p class="ap-education-year">{{education.duration}}</p>
    <p class="ap-education-excerpt">{{education.excerpt}}</p>
</div>
{% endfor %}
