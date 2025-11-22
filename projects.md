---
title: Projects
layout: projects
---

# Projects

List of projects (from github):

<ul>
    {% for project in site.projects %}
        <li>
            <a href="{{ project.url }}">
                {{ project.title }}
            </a>
        </li>
    {% endfor %}
</ul>