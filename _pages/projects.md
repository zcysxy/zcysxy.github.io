---
layout: archive
title: "Open Source Projects [<a href='(https://github.com/{{ site.author.github }})'>GitHub</a>]"
permalink: /projects/
author_profile: false
---

<br style="margin-bottom: 1.5em;" />

{% include base_path %}


{% for post in site.projects %}
  {% include archive-single.html %}
{% endfor %}

