---
title: Employment
layout: page
icon: fa-solid fa-briefcase
order: 4
---

{% for employment in site.employment %}
  <b>{{employment.position}} - {{employment.org}}, {{employment.loc}}</b> <br>
  {{employment.startdt}} - {{employment.enddt}} <br>
  <ul>
  {% for bullet in employment.bullets %}
    <li>{{bullet}}</li>
  {% endfor %}
  <li><a href="{{employment.url}}" style="color:  #2e765e; text-decoration: none;">more details...</a></li>
  </ul>
{% endfor %}

