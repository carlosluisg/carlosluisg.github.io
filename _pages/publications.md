---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include base_path %}

{% if page.author and site.data.authors[page.author] %}
  {% assign author = site.data.authors[page.author] %}{% else %}{% assign author = site.author %}
{% endif %}

{% if author.googlescholar %}
  You can find a list of all my articles on [my Google Scholar profile]( {{ author.googlescholar }}) 
{% endif %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
