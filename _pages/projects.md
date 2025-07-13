---
layout: single
permalink: /projects/
title: "Projects"
author_profile: true
---

Here are some of the projects I've worked on:

{% if site.data.projects %}
{% for project in site.data.projects %}
{% if project.featured %}

## {{ project.title }}

{% else %}

## {{ project.title }}

{% endif %}

{{ project.description }}

**Technologies:** {{ project.technologies | join: ', ' }}  
 **Status:** {{ project.status | capitalize }}

{% if project.github_url %}
[🔗 GitHub]({{ project.github_url }}){: .btn .btn--primary}
{% endif %}

---

{% endfor %}
{% else %}
_Projects will be displayed here once you add them to `_data/projects.yml`_
{% endif %}

## Want to see more?

Check out my [GitHub profile](https://github.com/hanjihun2000) for all my repositories and contributions!
