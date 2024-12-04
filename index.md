---
layout: home
title: Arman Karshenas, Ph.D.
---

<div style="display: flex; align-items: center; width: 100%;">
    <img src="{{ site.baseurl }}/assets/images/headshot.jpg" alt="Dr. Arman Karshenas" class="profile-photo" style="width: 170px; height: 170px; border-radius: 50%; margin-right: 20px;">
    <div>
        <h1>Welcome to my Personal Webpage!</h1>
        <p>
            I am a researcher, data scientist, and entrepreneur with expertise in applying machine learning to biological data, particularly in genomics, biophysics, and life sciences. I have a strong academic background, having completed an MPhil from the University of Cambridge and a BA from the University of Oxford. I am currently finishing my PhD at UC Berkeley, where I work on understanding enhancer functions in fruit flies and exploring how generative AI models can map enhancer sequences to spatial gene expression patterns.
        </p>
    </div>
</div>

## Recent Publications
Here are the most recent publications I have authored:

{% for publication in site.data.publications limit:3 %}
- **{{ publication.title }}**  
  *{{ publication.authors }}*  
  *Published in {{ publication.journal }}*  
  [Link to publication]({{ publication.url }})
{% endfor %}

## Recent Courses
Below are the courses I have recently taught:

{% for course in site.data.courses limit:3 %}
- **{{ course.title }}**  
  *{{ course.institution }}*  
  *{{ course.semester }}*
{% endfor %}

## Contact

Feel free to reach out for collaborations or inquiries:

- Email: **karshenas(at)berkeley(dot)edu**
- [LinkedIn Profile](https://www.linkedin.com/in/arman-karshenas-ph-d-283a3990/)
- [Google Scholar](https://scholar.google.co.uk/citations?user=viit6XUAAAAJ&hl=en)

---
Thank you for visiting my page!
