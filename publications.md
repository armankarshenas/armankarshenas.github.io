---
layout: page
title: Publications
permalink: /publications/
---

## Journal Articles

{% for publication in site.data.publications %}
  <div class="publication-entry">
    <p>
      <strong>{{ publication.authors }}</strong> ({{ publication.year }}). 
      <strong><i>{{ publication.title }}.</i></strong> <i>{{ publication.journal }}</i>{% if publication.doi %}, <a href="({{ publication.doi }})">[doi: {{ publication.doi }}]</a>{% endif %}{% if publication.url %}, [Link]({{ publication.url }}){% endif %}
    </p>
  </div>
{% endfor %}

## Conference Papers

<!-- You can add similar loops for conference papers if they are also included in your publications.yml -->
{% for conference in site.data.conference_papers %}
  <div class="publication-entry">
    <p>
      <strong>{{ conference.authors }}</strong> ({{ conference.year }}). 
      "{{ conference.title }}." *{{ conference.conference_name }}*{% if conference.doi %}, [DOI: {{ conference.doi }}](https://doi.org/{{ conference.doi }}){% endif %}{% if conference.url %}, [Link]({{ conference.url }}){% endif %}
    </p>
  </div>
{% endfor %}

## Book Chapters

<!-- Similarly, add a loop for book chapters if needed -->
{% for chapter in site.data.book_chapters %}
  <div class="publication-entry">
    <p>
      <strong>{{ chapter.authors }}</strong> ({{ chapter.year }}). 
      "{{ chapter.title }}." *{{ chapter.book_title }}*{% if chapter.doi %}, [DOI: {{ chapter.doi }}](https://doi.org/{{ chapter.doi }}){% endif %}{% if chapter.url %}, [Link]({{ chapter.url }}){% endif %}
    </p>
  </div>
{% endfor %}
