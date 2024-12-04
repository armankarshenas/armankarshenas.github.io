---
layout: page
title: Publications
permalink: /publications/
---

## Journal Articles

{% for publication in site.data.publications %}
  <ul>
    <li class="publication-entry">
      <p>
        <strong>{{ publication.authors }}</strong> ({{ publication.year }}). 
        <em>{{ publication.title }}</em>. <i>{{ publication.journal }}</i>
        {% if publication.doi %}, <a href="https://doi.org/{{ publication.doi }}">doi: {{ publication.doi }}</a>{% endif %}
        {% if publication.url %}, <a href="{{ publication.url }}">Link</a>{% endif %}
      </p>
    </li>
  </ul>
{% endfor %}

## Conference Papers

{% for conference in site.data.conference_papers %}
  <ul>
    <li class="publication-entry">
      <p>
        <strong>{{ conference.authors }}</strong> ({{ conference.year }}). 
        "<em>{{ conference.title }}</em>." <i>{{ conference.conference_name }}</i>
        {% if conference.doi %}, <a href="https://doi.org/{{ conference.doi }}"> doi: {{ conference.doi }}</a>{% endif %}
        {% if conference.url %}, <a href="{{ conference.url }}">Link</a>{% endif %}
      </p>
    </li>
  </ul>
{% endfor %}

## Book Chapters

{% for chapter in site.data.book_chapters %}
  <ul>
    <li class="publication-entry">
      <p>
        <strong>{{ chapter.authors }}</strong> ({{ chapter.year }}). 
        "<em>{{ chapter.title }}</em>." <i>{{ chapter.book_title }}</i>
        {% if chapter.doi %}, <a href="https://doi.org/{{ chapter.doi }}">doi: {{ chapter.doi }}</a>{% endif %}
        {% if chapter.url %}, <a href="{{ chapter.url }}">Link</a>{% endif %}
      </p>
    </li>
  </ul>
{% endfor %}
