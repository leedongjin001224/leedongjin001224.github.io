---
layout: page
permalink: /teaching/
title: teaching
description: List of my teaching experiences.
nav: true
nav_order: 4
---

{% assign sorted_courses = site.courses | sort: "num" | reverse %}
<div class="projects">
  <div class="row justify-content-center">
    {% for course in sorted_courses %}
      {% if course.short %}
        {% include courses_short.liquid%}
      {% else %}
        {% include courses.liquid %}
      {% endif %}
    {% endfor %}
  </div>
</div>
