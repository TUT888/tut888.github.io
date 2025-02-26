---
layout: default
permalink: /project/mobile
---

[Back to project](/project)

{% for pj in site.data.project-type %}
{% if pj.url == page.permalink %}
  {% assign project = pj %}
  {% break %}
{% endif %}
{% endfor %}

# {{ project.heading }} projects
{% include project/project-summary.html project-field=project.code detail-url=project.url %}
