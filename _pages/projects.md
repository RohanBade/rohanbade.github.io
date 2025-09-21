---
title: Projects
layout: default
permalink: "/projects/"
---

# Projects

{% for project in site.projects reversed %}

<div class="ap-project">
    <a class="ap-project-title" href="{{project.url}}" target="_blank">{{project.title}}</a>
    <p class="ap-project-year">{{project.year}}</p>
    <p class="ap-project-excerpt">{{project.excerpt}}</p>
    <p class="ap-project-tags">
        {% for tag in project.tags %}
        <span class="ap-project-chip">{{tag}}</span>
        {% endfor %}
    </p>
</div>
{% endfor %}
