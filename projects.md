---
title: Projects
layout: projects
---

# Projects

List of github projects:

<ul>
    {% assign sorted = site.projects | sort: "project-id" %}
    {% for project in site.projects %}
    {% unless project.hidden %}
        <li>
            <a href="{{ project.url }}">
                {{ project.title }}
            </a>
        </li>
    {% endunless %}
    {% endfor %}
</ul>