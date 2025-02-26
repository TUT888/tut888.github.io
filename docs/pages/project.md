---
layout: default
permalink: /project
---

# My Project

Over the course of my academic journey, I have had the opportunity to work on a variety of projects across three key fields: Artificial Intelligence and Machine Learning, Web Development and Mobile Development. 

Each project has allowed me to not only apply theoretical concepts but also to gain practical, hands-on experience in creating innovative solutions. From developing intelligent systems with AI/ML techniques to building functional web and mobile applications, I have cultivated a well-rounded skill set and a deep understanding of the diverse technologies that drive today’s digital world.

{% for project in site.data.project-type %}

## {{ project.heading }}
***

{% include project/project-summary.html project-field=project.code detail-url=project.url %}

{% endfor %}
