---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---
{% if page.author and site.data.authors[page.author] %}
  {% assign author = site.data.authors[page.author] %}{% else %}{% assign author = site.author %}
{% endif %}


{% if author.googlescholar %}
  You can also find my articles on <u><a href="https://scholar.google.com/citations?user=fLWv-VgAAAAJ&hl=en&oi=ao">My Google Scholar</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
