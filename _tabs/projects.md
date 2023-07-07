---
title: Projects
layout: page
icon: fa-solid fa-code
order: 2
---


{% for project in site.projects %}
  <div>
  <h1>{{project.title}}</h1>
  <p style="margin-left: 25px;">
  {{project.shortdesc}}<br><a href="{{project.url}}" style="color:  #2e765e; text-decoration: none;">more...</a></p>
  </div>
  
{% endfor %}
