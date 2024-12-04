---
layout: home
title: Arman Karshenas, Ph.D.
---

# Welcome to my Personal Webpage!

I am a researcher, data scientist, and entrepreneur with expertise in applying machine learning to biological data, particularly in genomics, biophysics, and life sciences. I have a strong academic background, having completed an MPhil from the University of Cambridge and a BA from the University of Oxford. I am currently finishing my PhD at UC Berkeley, where I work on understanding enhancer functions in fruit flies and exploring how generative AI models can map enhancer sequences to spatial gene expression patterns.

## Education

- **PhD in Biophysics** - UC Berkeley  
- **MPhil in Biophysics** - University of Cambridge  
- **BA in Biophysics** - University of Oxford  


## Research Interests

My research spans a range of topics within **biophysics**, **machine learning**, **data science**, and **life sciences**. Some of my key areas of focus include:

- **Computational biology and genomics**: Developing AI and machine learning models to analyze and predict biological outcomes, such as enhancer functions and transcription factor binding.
- **Biophysics and molecular dynamics**: Applying computational techniques to understand DNA-protein interactions, regulatory mechanisms, and gene expression.
- **Machine learning for life sciences**: Leveraging machine learning models, such as convolutional neural networks (CNNs), to predict gene expression and regulatory activity from sequence data.
- **Life sciences consulting**: Utilizing data science and machine learning to support M&A, drug development, and clinical trials.

## Recent Publications

{% for publication in site.data.publications limit:3 %}
1. {{ publication.authors }} ({{ publication.year }}). "{{ publication.title }}." *{{ publication.journal }}*{% if publication.doi %}, [DOI: {{ publication.doi }}](https://doi.org/{{ publication.doi }}){% endif %}{% if publication.url %}, [Link]({{ publication.url }}){% endif %}
{% endfor %}

[View all publications](/publications)

## Recent Courses

{% for course in site.data.courses limit:3 %}
- {{ course.code }}: {{ course.name }} - {{ course.semester }}
{% endfor %}

[More about my teaching](/teaching)
## Recent Blog Posts

{% for post in site.posts limit:3 %}
  <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
  <p>{{ post.excerpt | strip_html | truncatewords:50 }}</p>
{% endfor %}

[View all posts](/blog)
  
## Contact

Feel free to reach out for collaborations or inquiries:

- Email: **karshenas(at)berkeley(dot)edu**
- [LinkedIn Profile](https://www.linkedin.com/in/arman-karshenas-ph-d-283a3990/)
- [Google Scholar](https://scholar.google.co.uk/citations?user=viit6XUAAAAJ&hl=en)

---
Thank you for visiting my page!
