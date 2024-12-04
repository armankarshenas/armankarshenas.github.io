---
layout: page
title: Teaching
permalink: /teaching/
---

## Courses
{% for course in site.data.courses %}
  <details>
    <summary>
      <strong>{{ course.name }}</strong> --- <i>{{ course.institution }}</i> ({{ course.semester }})
    </summary>
    <p>{{ course.description }}</p>
    <ul>
      {% for pdf in course.pdfs %}
        <li><a href="{{ '/assets/courses/' | append: course.name | append: '/' | append: pdf }}" target="_blank">{{ pdf }}</a></li>
      {% endfor %}
    </ul>
  </details>
{% endfor %}
