---
layout: page
permalink: /teaching/
title: teaching
description: List of my teaching experiences.
nav: true
nav_order: 4
---

{% assign sorted_courses = site.courses | sort: "importance" %}
<div class="projects">
  <div class="row justify-content-center">
    {% for course in sorted_courses %}
      {% include courses.liquid %}
    {% endfor %}
  </div>
</div>
