---
layout: page
show_meta: false
title: "Research"
subheadline: "Ongoing and past research projects"
header:
   image_fullwidth: "header_unsplash_5.jpg"
permalink: "/research/"
---

Research projects are listed in chronological order (newest first). Currently, projects are displayed by a link only, it is planned to arrange them in a grid with tiles showing a short teaser.

<ul>
    {% for post in site.categories.research %}
    <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>
