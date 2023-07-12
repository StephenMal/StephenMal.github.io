---
title: Education
layout: page
icon: fa-solid fa-briefcase
order: 2
---

{% for education in site.education %}
  <div>
  <h3>{{education.school}}, {{education.city}}, {{education.state}}<br>
  {{education.title}} - {{education.year}}</h3>
  <ul>
  {% for bullet in education.bullets %}
    <li>{{bullet}}</li>
  {% endfor %}
  <li><a href="{{education.url}}" style="color:  #2e765e; text-decoration: none;">more details...</a></li>
  </ul>
</div>
{% endfor %}