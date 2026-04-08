---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include base_path %}

{% assign pubs_journal = site.publications | where: 'type', 'journal' | reverse %}

<h2>Journal articles</h2>
{% for post in pubs_journal%}
  {% include archive-single-publication.html %}
{% endfor %}

{% assign pubs_article-volume = site.publications | where: 'type', 'article-volume' | reverse %}

<h2>Articles in edited volumes</h2>
{% for post in pubs_article-volume %}
  {% include archive-single-publication.html %}
{% endfor %}

{% assign pubs_monograph = site.publications | where: 'type', 'monograph' | reverse%}

<h2>Monographs</h2>
{% for post in pubs_monograph%}
  {% include archive-single-publication.html %}
{% endfor %}

{% assign pubs_edited-book = site.publications | where: 'type', 'edited-book' | reverse %}

<h2>(Co-)edited books</h2>
{% for post in pubs_edited-book%}
  {% include archive-single-publication.html %}
{% endfor %}

